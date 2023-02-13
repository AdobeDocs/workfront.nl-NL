---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Gereedschappen
description: De [!DNL Adobe Workfront Fusion Tools] de sectie omvat verscheidene nuttige modules die uw scenario kunnen verbeteren.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1943'
ht-degree: 0%

---

# [!UICONTROL Tools]

De [!DNL Adobe Workfront Fusion Tools] de sectie omvat verscheidene nuttige modules die uw scenario kunnen verbeteren.

[!UICONTROL Tools] zijn beschikbaar in de lijst met toepassingen of vanuit de [!UICONTROL Tools] pictogram ![](assets/tools-icon-small.png) onder aan het scherm.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr>
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Tools] en hun velden

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Samenvoegapparatuur](#aggregators)
* [Transformatoren](#transformers)

### Triggers

#### [!UICONTROL Basic trigger]

In deze module kunt u een aangepaste trigger maken en de bijbehorende invoerbundels definiëren.

U kunt deze module bijvoorbeeld gebruiken voor contactpersonen of een andere lijst die volgens planning naar een opgegeven e-mailadres moet worden verzonden (zoals [!UICONTROL Email] >[!UICONTROL Send an Email], of [!DNL Gmail] >[!UICONTROL Send an Email] (modules) of als een eenvoudige herinnering die op elk gewenst moment moet worden geactiveerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Aangepaste bundels maken door arrayitems toe te voegen. De array bestaat uit naam-waardeparen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Get Multiple Variables]](#get-multiple-variables)
* [[!UICONTROL Get Variable]](#get-variable)
* [[!UICONTROL Increment function]](#increment-function)
* [[!UICONTROL Set Multiple Variables]](#set-multiple-variables)
* [[!UICONTROL Set Variable]](#set-variable)
* [[!UICONTROL Sleep]](#sleep)

#### [!UICONTROL Get Multiple Variables]

Deze module wint waarden terug die eerder door werden gecreeerd [!UICONTROL Set Variable] of [!UICONTROL Set Multiple Variables] module.

Deze module kan variabelen lezen die overal in het scenario werden geplaatst, zelfs als de variabele in een verschillende route werd geplaatst dan waar [!UICONTROL Get Multiple Variables] is gevonden. De enige vereiste is dat de [!UICONTROL Tools] > [!UICONTROL Set Variable] of [!UICONTROL Tools] > [!UICONTROL Set Multiple Variable] module wordt uitgevoerd vóór de [!UICONTROL Tools] > [!UICONTROL Get Multiple Variables] module. Voor meer informatie over de orde waarin de modules worden uitgevoerd, zie [Router module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Voeg de variabelen toe die u de module wilt krijgen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variable name]</td>
        <td>Wijs voor elke variabele die u toevoegt de naam toe van de variabele die u wilt ophalen.</td>
    </tr>
</table>

>[!INFO]
>
>**Voorbeelden:**  Het volgende is mogelijk gebruik te maken van de [!UICONTROL Set]/[!UICONTROL Get (multiple) variable(s)] modules:
>
>* Een berekende waarde opslaan voor later gebruik, zelfs in een verschillende route. Dit is handig wanneer de waarde in meerdere modules wordt gebruikt en de formule voor het berekenen van de waarde te complex is.
>* Fouten opsporen in een formule. Als een in een module gebruikte formule ogenschijnlijk geen correct resultaat oplevert, kopieert u de formule en plakt u deze in een [!UICONTROL Set Variable] die u vóór de relevante module invoegt. Koppel de module(s) los na de [!UICONTROL Set Variable] en voert het scenario uit. Controleer de [!UICONTROL Set Variable] de output van de module, past of vereenvoudigt de formule, voert opnieuw het scenario uit, en blijft dit doen tot de kwestie is opgelost.



#### [!UICONTROL Get Variable]

Deze module wint een waarde terug die eerder door [!UICONTROL Set Variable] of [!UICONTROL Set Multiple Variables] module.

Deze module kan variabelen lezen die overal in het scenario werden geplaatst, zelfs als de variabele in een verschillende route werd geplaatst dan waar [!UICONTROL Get Variable] is gevonden. De enige vereiste is dat de [!UICONTROL Tools] > [!UICONTROL Set Variable] of [!UICONTROL Tools] > [!UICONTROL Set Multiple Variables] module wordt uitgevoerd vóór de [!UICONTROL Tools] > [!UICONTROL Get Variable] module. Voor meer informatie over de orde waarin de modules worden uitgevoerd, zie [Router module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable name]</td> 
   <td> <p>Wijs de naam van de variabele toe die u de module wilt krijgen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Increment function]

Deze module keert een waarde terug die door 1 na de verrichting van elke module wordt verhoogd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reset a value]</td> 
   <td> <p>Selecteer wanneer u de module de waarde wilt verhogen. </p> 
    <ul> 
     <li>[!UICONTROL After one cycle]</li> 
     <li>[!UICONTROL After one scenario run]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:**
>
>Een van de toepassingen van de module is het implementeren van een &#39;round robin&#39;-toewijzing van taken, leads, e-mails, enzovoort, aan gebruikers in een groep. Het algoritme kiest de toewijzen van een groep in een rationele volgorde, meestal van boven naar beneden in een lijst. Wanneer het algoritme het eind van de lijst bereikt, zou het dan de volgende taak aan de gebruiker bij de bovenkant van de lijst geven en blijven taken onderaan de lijst maken.
>
>Het volgende scenario verzendt een e-mail naar de eerste ontvanger na elk oneven genummerd scenario in werking gesteld, en naar de tweede ontvanger na elk even genummerd scenario in werking gesteld.
>
>![](assets/example-email-350x246.gif)
>
>1. Dit scenario maken:
>1. De modules instellen **[!UICONTROL Reset a value]** veld naar Nooit.
>1. Stel de route in voor oneven waarden. Plaats de filter voor deze route gebruikend de modulus mathfunctie die evenaart `1`:

>
>   ![](assets/odd-350x459.png)
>
>  **Opmerking**: Vergeet niet de [!UICONTROL Equal to] van de standaardoperator [!UICONTROL Text] aan de [!UICONTROL Numeric] operator.
>
>1. Plaats de route voor zelfs waarden gebruikend de modulus wiskundige functie die evenaart `0`:
>
>De verhogingsfunctie voegt één toe telkens als het scenario loopt. De filters controleren de verhoging en handelen op zijn waarde, die ervoor zorgt dat de e-mails gelijkelijk worden verdeeld.

#### [!UICONTROL Set Multiple Variables]

Deze module leidt tot variabelen die door andere modules in de route kunnen worden in kaart gebracht. De variabele kan ook worden toegewezen aan de [!UICONTROL Get Variable] of [!UICONTROL Get Multiple Variables] modules voor om het even welke route in het scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Voeg de variabelen toe die u de module wilt plaatsen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Voer voor elke variabele de naam van de variabele in. Deze naam zal worden getoond wanneer het in kaart brengen van de variabele in andere modules. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Voer voor elke variabele de waarde voor de variabele in. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>Selecteer hoe lang de variabelen geldig moeten blijven (dezelfde waarde behouden).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: De variabele is geldig voor één cyclus. Nuttig wanneer meerdere webhaken in één scenario worden ontvangen (meer webhooks = meer cycli). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: De variabele is geldig voor één scenario uitvoering. Een uitvoering kan een of meer cycli bevatten.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Set Variable]

Deze module leidt tot een variabele die door andere modules in de route kan worden in kaart gebracht. De variabele kan ook worden toegewezen aan de [!UICONTROL Get Variable] of [!UICONTROL Get Multiple Variables] modules voor om het even welke route in het scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Voer de variabelenaam in. Deze naam zal worden getoond wanneer het in kaart brengen van de variabele in andere modules. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>Selecteer hoe lang de variabelen geldig moeten blijven (dezelfde waarde behouden).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: De variabele is geldig voor één cyclus. Nuttig wanneer meerdere webhaken in één scenario worden ontvangen (meer webhooks = meer cycli). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: De variabele is geldig voor één scenario uitvoering. Een uitvoering kan een of meer cycli bevatten.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Voer de waarde voor de variabele in of wijs deze toe. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sleep]

Deze module staat u toe om de scenariostroom tot 300 seconden (5 minuten) te vertragen.

Deze functie kan bijvoorbeeld nuttig zijn als u de [!DNL target] laden van serviceserver of om menselijk gedrag na te bootsen bij het verzenden van sms- of e-mailberichten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>Voer het aantal seconden in waarvoor het scenario wordt gepauzeerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Als u de stroom voor langere periodes wilt pauzeren, adviseren wij om uw scenario in twee scenario&#39;s te verdelen:
>
>* Het eerste scenario zou het deel vóór de pauze bevatten.
>* Het tweede scenario zou het deel na het bevatten.
>
>In het eerste scenario worden alle benodigde gegevens samen met de huidige tijdstempel opgeslagen in een gegevensopslagruimte. Het tweede scenario zou de gegevensopslag periodiek controleren op verslagen met een timestamp ouder dan de voorgenomen vertraging, de verslagen terugwinnen, de verwerking van de gegevens voltooien en de verslagen uit de gegevensopslag verwijderen.
>
>Voor meer informatie over gegevensopslag, zie [Gegevensopslag in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Voor meer informatie over specifieke modules van de gegevensopslag, zie [[!UICONTROL Data store] modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Samenvoegapparatuur

* [[!UICONTROL Numeric aggregator]](#numeric-aggregator)
* [[!UICONTROL Table aggregator]](#table-aggregator)
* [[!UICONTROL Text aggregator]](#text-aggregator)

#### [!UICONTROL Numeric aggregator]

Met deze module kunt u numerieke waarden ophalen en vervolgens een van de geselecteerde functies (SUM, AVG, COUNT, MAX, MIN) toepassen en het resultaat in één bundel retourneren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Selecteer de module waarvan u velden wilt samenvoegen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>Selecteer de functie die u wilt gebruiken om de waarden samen te voegen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Definieer een expressie waarop u de geaggregeerde uitvoer wilt groeperen. Deze expressie kan een of meer toegewezen items bevatten. De geaggregeerde gegevens worden vervolgens in groepen verdeeld op basis van de waarde van deze expressie. Elke groep voert als een afzonderlijke bundel met een sleutel (de geëvalueerde uitdrukking) en een waarde (de bijeengevoegde waarde) uit. U kunt de sleutel als filter in verdere modules gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Schakel deze optie in om het scenario te stoppen als er geen resultaten zijn.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>Voer de waarde in die u wilt samenvoegen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Table aggregator]

In deze module worden waarden uit de geselecteerde velden met ontvangen bundels samengevoegd in één bundel met een opgegeven kolom- en rijscheidingsteken (waarmee u een tabel kunt maken).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Selecteer de module waarvan u velden wilt samenvoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td> <p> Selecteer de velden in de module die hierboven is geselecteerd en de waarden bevatten die u wilt samenvoegen tot één bundel.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Column separator]</p> </td> 
   <td> <p>Selecteer of typ het type scheidingsteken waarmee de kolommen met veldwaarden in de resulterende bundel worden gescheiden. Als u [!UICONTROL Other]voert u het teken in dat u wilt gebruiken om waarden te scheiden in het scheidingsveld.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>Selecteer of typ het type scheidingsteken waarmee de rijen met veldwaarden in de resulterende bundel worden gescheiden. Als u [!UICONTROL Other]voert u het teken in dat u wilt gebruiken om waarden te scheiden in het scheidingsveld.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Definieer een expressie waarop u de geaggregeerde uitvoer wilt groeperen. Deze expressie kan een of meer toegewezen items bevatten. De geaggregeerde gegevens worden vervolgens in groepen verdeeld op basis van de waarde van deze expressie. Elke groep voert als een afzonderlijke bundel met een sleutel (de geëvalueerde uitdrukking) en een waarde (de bijeengevoegde waarde) uit. U kunt de sleutel als filter in verdere modules gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Selecteer deze optie om het scenario te stoppen als er geen resultaten zijn.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Text aggregator]

In deze module worden waarden uit de geselecteerde velden met ontvangen bundels samengevoegd in één bundel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Selecteer de module waarvan u velden wilt samenvoegen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>Selecteer of typ het type scheidingsteken waarmee de rijen met veldwaarden in de resulterende bundel worden gescheiden. Als u [!UICONTROL Other]voert u het teken in dat u wilt gebruiken om waarden te scheiden in het scheidingsveld.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Definieer een expressie die een of meer in kaart gebrachte items bevat. De samengevoegde gegevens worden gescheiden onder Groepen met de waarde van dezelfde expressie. Elke groep voert als afzonderlijke bundel uit die een Sleutel met de geëvalueerde uitdrukking en de samengevoegde tekst bevat. Door dit te doen, kunt u Sleutel als filter in verdere modules gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> Typ of wijs de tekst toe die u in de module wilt samenvoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Selecteer deze optie om het scenario te stoppen als er geen resultaten zijn.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** U kunt de tekstaggregator gebruiken om meer waarden (bijvoorbeeld klantnamen of notities) in één bundel in te voegen en een e-mail te verzenden die alle waarden in de e-mailhoofdtekst of het onderwerp van de e-mail bevat.

### Transformatoren

* [[!UICONTROL Compose a string]](#compose-a-string)
* [[!UICONTROL Convert the encoding of the text]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Switch]](#switch)

#### [!UICONTROL Compose a string]

Zet om het even welke waarde in een type van koordgegevens (tekst) om. Het maakt de afbeelding gemakkelijker wanneer het in kaart brengen, bijvoorbeeld, binaire gegevens.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>Voer de gegevens in die u in de tekst wilt omzetten of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convert the encoding of the text]

Hiermee wordt ingevoerde invoertekst (of binaire gegevens) omgezet in de geselecteerde codering.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input data]</p> </td> 
   <td> <p>Typ of wijs de inhoud toe die u wilt omzetten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>Selecteer het coderingstype van de invoergegevens. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>Selecteer het coderingstype van uw doel- (uitvoer)gegevens.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Switch]

Controleert de invoerwaarde voor een overeenkomst met de opgegeven lijst met waarden. Retourneert uitvoer op basis van het resultaat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Voer de expressie in die u wilt evalueren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use regular expressions to match]</td> 
   <td> <p>Schakel deze optie in als u reguliere expressies wilt gebruiken. De module bepaalt de gevallen die op de regelmatige uitdrukking, eerder dan een nauwkeurige gelijke worden gebaseerd.</p> 
    <div> 
     <p>Een reguliere expressie is een reeks tekens waarin elk teken een metateken is met een speciale betekenis of een regulier teken met een letterlijke betekenis. Met deze teken- en metatekens wordt een patroon geïdentificeerd dat kan worden gebruikt voor het zoeken naar tekst. Als u bijvoorbeeld naar namen wilt zoeken, kunt u een reguliere expressie instellen om te zoeken naar een patroon dat bestaat uit twee opeenvolgende woorden die beginnen met hoofdletters. Reguliere expressies zijn een krachtig gereedschap voor het zoeken en bewerken van tekst.</p> 
     <p>Een discussie over reguliere expressies valt buiten het toepassingsgebied van dit artikel. Wij adviseren de volgende middelen:</p> 
     <ul> 
      <li>Voor de volledige lijst met metatekens raadpleegt u <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Reguliere expressies</a> in MDN-webdocumenten.</li> 
      <li>Voor een zelfstudie over het maken van reguliere expressies raden we aan <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Voor het experimenteren met reguliere expressies raden we de <a href="https://regex101.com/">Gewone uitdrukkingen 101</a> website. Selecteer de ECMAScript-FLAVOR (JavaScript) in het linkerdeelvenster.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cases] </td> 
   <td> <p>Als de invoer een waarde bevat die is ingevoerd voor de [!UICONTROL Pattern] veld, dan de waarde die is ingevoerd voor het [!UICONTROL Output] wordt geretourneerd.</p> <p>Als de invoer niet overeenkomt met een van de waarden die u in een [!UICONTROL Pattern] in het veld wordt een van de volgende handelingen uitgevoerd:</p> 
    <ul> 
     <li>De waarde van de [!UICONTROL Else] field is returned</li> 
     <li>Als er geen waarde in de [!UICONTROL Else] veld, wordt geen uitvoer geretourneerd.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Voer de waarde in die wordt geretourneerd wanneer niet wordt voldaan aan de criteria die in het veld Gevallen zijn ingesteld. </p> </td> 
  </tr> 
 </tbody> 
</table>
