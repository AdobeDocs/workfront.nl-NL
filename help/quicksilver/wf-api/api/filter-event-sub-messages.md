---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Abonnementsberichten voor gebeurtenissen filteren
description: Abonnementsberichten voor gebeurtenissen filteren
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Abonnementsberichten voor gebeurtenissen filteren

U kunt intermediaire verwerkingscomponenten bouwen die u kunnen helpen slechts de berichten van het gebeurtenisabonnement filtreren en verwerken die uw zaken vereist.

Zie voor meer informatie over gebeurtenisabonnementen [Event Subscription API](../../wf-api/general/event-subs-api.md).

## Gebeurtenisberichten filteren

Deze sectie bevat codefragmenten van het filtreren die u kunt uitvoeren om de lading van de berichten van het gebeurtenisabonnement te verminderen.  Deze fragmenten illustreren dezelfde set filters die in de volgende talen zijn geschreven, zodat u de verschillen in de syntaxis van de verschillende talen kunt zien:

U kunt voorbeelden bekijken van filteren bij [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), waar u de verschillen in syntaxis voor elke taal en de middelen van interactie met de SDK van AWS kunt zien.Deze voorbeelden worden geschreven als AWS Lambdas, die een gemeenschappelijke methode voor het toepassen van intermediaire filtreren en verwerkingscomponenten is.

De volgende codefragmenten zijn dichtbij plaatsing-klaar en kunnen als uitgangspunt worden gebruikt om u te helpen uw eigen, complexere, filters en verwerkingscomponenten schrijven.

### Java

Het volgende voorbeeld in Java toont hoe te om projectlading te filtreren die op identiteitskaart van de Groep van het project wordt gebaseerd, zoals gedaan in [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Bepaal de groep-id die u zoekt en maak deze als een statische constante.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   In dit voorbeeld, neemt de handleRequest methode, die een standaardmethodenaam van AWS Lambda is, een type van Kaart als zijn eerste parameter, die de inhoud van het gebeurtenisabonnementbericht is.\
   De tweede parameter het neemt is de context van het huidige Lambda verzoek van de Volmacht.\
   Het voorwerp van de Context wordt gebruikt om een Logger te verkrijgen Lambda, die wordt gebruikt om een bericht aan CloudWatchLogs te schrijven.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Op aanroeping van de methode handleRequest, verkrijg het &quot;newState&quot;attribuut van het bericht van het gebeurtenisabonnement, dat de bijgewerkte staat van het middel vertegenwoordigt.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Ga voor meer informatie over de nieuweState-indeling naar [Uitgaande berichtindeling voor gebeurtenisabonnementen](../../wf-api/api/message-format-event-subs.md).

3. Na het ontleden van de Kaart &quot;newState&quot;van het bericht, zorg ervoor de de groepsidentiteitskaart van objecten de groepsidentiteitskaart aanpast u in Stap 1 identificeerde.

4. (Voorwaardelijk) Als de id&#39;s **niet** laten aflopen, het bericht neerzetten, zodat een lege reactie wordt geretourneerd.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >Terugsturen van een leeg, succesvol antwoord is cruciaal. Alles behalve een 200-niveau reactie wordt beschouwd als een mislukte levering.

5. Verwerk het bericht.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK wordt gebruikt om een andere Lambda aan te halen, die voor het leveren van het gefiltreerde bericht aan ons gewenste eindpunt verantwoordelijk is.

   Het doel van het overdragen van de verantwoordelijkheid om het bericht aan een andere Lambda te leveren is een onderbreking van het leveringsverzoek te vermijden die van de dienst van het Abonnement van de Gebeurtenis komt. Momenteel, wordt de toegestane onderbreking voor levering geplaatst aan vijf seconden. Als het filter langer duurt dan toegestaan door het plaatsen, kunt u het verzoek verwerken, maar de dienst van het Abonnement van de Gebeurtenis zal uit en in een hertry lijn vallen tot het een 200 niveaureactie binnen de onderbrekingsperiode ontvangt.

   Voor meer informatie over het beheren van berichtlevering, zie [Berichtlevering verbeteren tijdens het aanpassen van time-outs](#improving-message-delivery-while-accommodating-timeouts).

### Python

Het belangrijkste verschil tussen de Java- en Python-voorbeelden is dat in het Java-voorbeeld het abonnementsbericht voor een gebeurtenis als eerste parameter wordt ontvangen. In het Python-voorbeeld is de eerste parameter een Lambda-proxygebeurtenis, die het abonnementsbericht voor een gebeurtenis bevat, samen met informatie over het proxyverzoek van AWS Lambda.

Het volgende voorbeeld in Python toont hoe te om projectlading te filtreren die op identiteitskaart van de Groep van het project wordt gebaseerd, zoals gedaan in  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Bepaal de groep-id die u zoekt en maak deze als een statische constante.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   De eerste parameter is de &quot;gebeurtenis van de volmacht Lambda,&quot;die het bericht van het gebeurtenisabonnement en wat extra informatie bevat die uit moet worden ontleed.\
   De tweede parameter is de context van het huidige Lambda- verzoek van de Volmacht.\
   In dit voorbeeld, wordt het voorwerp van de Context gebruikt om een Logger te verkrijgen Lambda, die wordt gebruikt om een bericht aan CloudWatchLogs te schrijven.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Parseer het bericht uit de gebeurtenis.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Verkrijg het &quot;newState&quot;attribuut van het bericht van het gebeurtenisabonnement.\
   Het kenmerk newState vertegenwoordigt de bijgewerkte status van de bron.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Ga voor meer informatie over de nieuweState-indeling naar [Uitgaande berichtindeling voor gebeurtenisabonnementen](../../wf-api/api/message-format-event-subs.md).

1. Na het ontleden van de Kaart &quot;newState&quot;van het bericht, zorg ervoor de de groepsidentiteitskaart van objecten de groepsidentiteitskaart aanpast u in Stap 1 identificeerde.

1. (Voorwaardelijk) Als de id&#39;s niet overeenkomen, zet het bericht neer, zodat een leeg antwoord wordt geretourneerd.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >Terugsturen van een leeg, succesvol antwoord is cruciaal. Alles behalve een 200-niveau reactie wordt beschouwd als een mislukte levering.

1. Verwerk het bericht.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK wordt gebruikt om een andere Lambda aan te halen, die voor het leveren van het gefiltreerde bericht aan ons gewenste eindpunt verantwoordelijk is.

   Het doel van het overdragen van de verantwoordelijkheid om het bericht aan een andere Lambda te leveren is een onderbreking van het leveringsverzoek te vermijden die van de dienst van het Abonnement van de Gebeurtenis komt. Momenteel is de time-out voor levering ingesteld op vijf seconden. Als het filter langer duurt dan toegestaan door het plaatsen, kunt u het verzoek verwerken, maar de dienst van het Abonnement van de Gebeurtenis zal uit en in een hertry lijn vallen tot het een 200 niveaureactie binnen de onderbrekingsperiode ontvangt.


### Node.js

Het voorbeeld Node.js van het filtreren van identiteitskaart van de projectgroep leest gelijkaardig aan Java en de voorbeelden van Python. Net als bij het Python-voorbeeld is de eerste parameter een Lambda-proxygebeurtenis en de tweede parameter de Lambda-context.

Het volgende voorbeeld in Node.js toont hoe te om projectladingen te filtreren die op identiteitskaart van de Groep van het project worden gebaseerd, zoals binnen gedaan  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Bepaal de groep-id die u zoekt en maak deze als een statische constante.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   De eerste parameter is de &quot;gebeurtenis van de volmacht Lambda,&quot;die het bericht van het gebeurtenisabonnement en wat extra informatie bevat die uit moet worden ontleed.\
   De tweede parameter is de context van het huidige Lambda- verzoek van de Volmacht.\
   In dit voorbeeld, wordt het voorwerp van de Context gebruikt om een Logger te verkrijgen Lambda, die wordt gebruikt om een bericht aan CloudWatchLogs te schrijven.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Parseer het bericht uit de gebeurtenis.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Haal het projectGroupIDfrom het &quot;newState&quot;attribuut van het bericht van het gebeurtenisabonnement op, dan pas het met groepsidentiteitskaart van de groep aan u in Stap 1 identificeerde.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Ga voor meer informatie over de nieuweState-indeling naar [Uitgaande berichtindeling voor gebeurtenisabonnementen](../../wf-api/api/message-format-event-subs.md).

4. (Voorwaardelijk) Als de id&#39;s niet overeenkomen, zet het bericht neer, zodat een leeg antwoord wordt geretourneerd.\
   In het volgende voorbeeld worden overeenkomende groep-id&#39;s weergegeven:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >Terugsturen van een leeg, succesvol antwoord is cruciaal. Alles behalve een 200-niveau reactie wordt beschouwd als een mislukte levering.

5. Verwerk het bericht.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK wordt gebruikt om een andere Lambda aan te halen, die voor het leveren van het gefiltreerde bericht aan ons gewenste eindpunt verantwoordelijk is.\
   Het doel van het overdragen van de verantwoordelijkheid om het bericht aan een andere Lambda te leveren is een onderbreking van het leveringsverzoek te vermijden die van de dienst van het Abonnement van de Gebeurtenis komt. Momenteel is de time-out voor levering ingesteld op vijf seconden. Als het filter langer duurt dan toegestaan door het plaatsen, kunt u het verzoek verwerken, maar de dienst van het Abonnement van de Gebeurtenis zal uit en in een hertry lijn vallen tot het een 200 niveaureactie binnen de onderbrekingsperiode ontvangt.\
   Om over het beheren van berichtlevering te leren, zie [Berichtlevering verbeteren tijdens het aanpassen van time-outs](#improving-message-delivery-while-accommodating-timeouts).

## Berichtlevering verbeteren tijdens het aanpassen van time-outs

De dienst van het Abonnement van de Gebeurtenis heeft een strikte onderbreking van **vijf seconden** voor alle leveringsverzoeken. Als de levering van een bericht de toegestane tijd overschrijdt, begint de dienst van het Abonnement van de Gebeurtenis een herprobeer cyclus voor dat bericht.

Bijvoorbeeld, bouwt u een filter van identiteitskaart van de projectgroep gelijkend op één van de voorbeelden die in worden gevonden [Gebeurtenisberichten filteren](#filtering-event-messages) en u omvat een gegevensbestandraadpleging om te bepalen of het bericht nodig is. Het is mogelijk dat de gegevensbestandraadpleging samen met de tijd nodig voor vereiste verwerking en voor Lambda aan kou-start meer dan vijf seconden kon vergen, die de dienst van het Abonnement van de Gebeurtenis ertoe brengen om het leveren van het bericht opnieuw te proberen.

U kunt een herpoging voorkomen door de tijdrovende delen van het proces te scheiden van de logica die verantwoordelijk is voor het bepalen of het bericht één is u wilt verwerken en leveren. Door dit te doen, kunt u het bericht goedkeuren en een 200-vlakke reactie op de dienst van het Abonnement van de Gebeurtenis terugsturen, terwijl het asynchroon voortzetten om het bericht op de achtergrond te verwerken of te filtreren (zie Stap 5 in [Java](#java) bijvoorbeeld).


Zelfs als uw verwerking of het filtreren niet de vijf-tweede onderbreking overschrijdt, is het nog steeds voordelig om het eerste aanraakpunt van berichtfiltratie of verwerking van de andere verwerking of leveringsstappen op de cliëntkant te scheiden. Zo heeft de overdracht van het bericht aan de bestemming van de dienst van het Abonnement van de Gebeurtenis minimale tijd en prestatiesinvloed aan beide partijen.

Ga voor meer informatie over het mechanisme voor opnieuw proberen naar [Abonnementspogingen voor gebeurtenissen opnieuw proberen](../../wf-api/api/event-sub-retries.md).

## Gehoste filters implementeren in cloudloze architectuur

Als u geen cloudarchitectuur kunt gebruiken voor het filteren van abonnementen op gebeurtenissen, kunt u de voorbeelden in [Gebeurtenisberichten filteren](#filtering-event-messages) als roadmaps van hoe te om uw eigen ontvangen filters of verwerkingscomponenten uit te voeren.

### Het aanpassen van Filtrerende Voorbeelden voor Zelfstandige Diensten

Ga als volgt te werk voordat u de filtervoorbeelden gebruikt in een cloudloze omgeving:

* Laat de Lambda-specifieke stukken van de voorbeelden, zoals de parameter van de Context weg.

* Wijzig de aanroepen van andere Lambdas in de voorbeelden in aanvullende asynchrone HTTP-aanvragen voor andere filters of verwerkingscomponenten die u host.

* Als u verwijst naar de voorbeelden Python en Node.js, vervangt u de eerste gebeurtenisparameter door de eerste parameter voor laadbewerking die in het Java-voorbeeld wordt getoond. Zie Stap 1 in [Java](#java).

* De filters of processors implementeren met een webgebaseerde API.

### Abonnementsberichten voor gemiste gebeurtenissen voorkomen

Soms, in een cloudless architectuur, kunnen de diensten verantwoordelijk voor het ontvangen van de berichten van het gebeurtenisabonnement onbereikbaar zijn. In een dergelijke gebeurtenis, zouden de berichten de retry grens kunnen overschrijden en worden verloren, zonder manier om de informatie binnen de berichten terug te winnen.

Wij adviseren dat tijdens het opstarten van uw dienst u een vraag uitvoert die om de meest recente staat van alle middelen vraagt die in de gemiste berichten zouden kunnen zijn omvat. Zoals aangetoond in het volgende voorbeeld, kunt u de filtercriteria gebruiken om voor middelen te vragen die die criteria aanpassen en dan hun huidige staat verwerken.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v9.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

Door middelen te vragen, zorgt u ervoor dat uw integrerende systemen de recentste versie van middelen hebben.

### Het uitvoeren van Asynchrone Verwerking in het leveren van Berichten

Alle voorbeelden in het dialoogvenster [Gebeurtenisberichten filteren](#filtering-event-messages) de verantwoordelijkheid voor het afleveren van gefilterde berichten aan een andere AWS Lambda. Dit wordt gedaan vermijden overschrijdend de vijf-tweede onderbreking in het leveringsverzoek, die door de dienst van het Abonnement van de Gebeurtenis wordt afgedwongen die het verzoek uitgeeft.

In een cloudloze architectuur, zou u een asynchroon verwerkingsmechanisme kunnen moeten uitvoeren gelijkend op hoe SDK van AWS voor asynchrone vraag aan andere Lambdas van AWS toestaat. De meeste moderne programmeertalen beschikken over bibliotheken van derden of kernbibliotheken die asynchrone verwerking afhandelen, zodat u de asynchrone verwerkingsstijl die in onze voorbeelden is geïmplementeerd, kunt benutten.
