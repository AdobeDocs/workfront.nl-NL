---
content-type: api
navigation-topic: general-api
title: Basisprincipes van API's
description: Basisprincipes van API's
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '4396'
ht-degree: 0%

---


# Basisprincipes van API&#39;s

Het doel voor de Adobe Workfront API is het vereenvoudigen van de integratie van gebouwen met Workfront door de introductie van een REST-ful architectuur die werkt via HTTP. In dit document wordt ervan uitgegaan dat u bekend bent met REST- en JSON-reacties en wordt de aanpak beschreven die door de Workfront API wordt gevolgd.

Een vertrouwdheid met het schema van Workfront zal u helpen bij het begrijpen van de gegevensbestandverhoudingen die kunnen worden gebruikt om gegevens uit Workfront voor integratiedoeleinden te trekken.

## Grenswaarden en richtsnoeren

Voor consistente Workfront-systeemprestaties op aanvraag beperkt de Workfront API gelijktijdige API-threads. Deze handleiding voorkomt systeemproblemen die worden veroorzaakt door foutieve API-aanroepen. De Sandbox-omgeving heeft dezelfde gelijktijdige limiet voor de API-thread, waardoor klanten en partners API-aanroepen nauwkeurig kunnen testen voordat code wordt vrijgegeven voor productie.

Voor productie, voorproef, en testaandrijvingsmilieu&#39;s hebben de eindgebruikersverzoeken een maximumlengte van URI van 8892 bytes omdat zij door Workfront CDN (Akamai) worden verpletterd. Deze limiet geldt alleen voor URI&#39;s die worden gerouteerd via de CDN.

### Disclaimer

Elk gebruik van de API moet in de bètaomgeving van Workfront worden getest voordat het in de productieomgeving wordt uitgevoerd. Als een klant de API gebruikt voor een proces dat Workfront redelijkerwijs als belastend voor de software op aanvraag beschouwt (d.w.z. het proces veroorzaakt een wezenlijk negatief effect op de prestaties van de software voor andere klanten), behoudt Workfront zich het recht voor te vragen dat de klant dat proces beëindigt. Als de klant niet voldoet en het probleem zich blijft voordoen, behoudt Workfront zich het recht voor het proces te beëindigen.

## Workfront API-URL

Voor informatie over URL die u zult gebruiken om Workfront API te roepen, zie [&#x200B; formaat van het Domein voor Adobe Workfront API vraag &#x200B;](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Basisbeginselen van REST

In deze sectie wordt op hoog niveau uitgelegd hoe u kunt communiceren met de Workfront REST API voor de volgende REST-beginselen:

### Object-URI

Elk object in het systeem krijgt een unieke URI die bestaat uit het objecttype en de id. In het volgende voorbeeld ziet u URI&#39;s die drie unieke objecten beschrijven:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Het objecttype is niet hoofdlettergevoelig en kan de afgekorte ObjCode (zoals proj) of de alternatieve objectnaam (project) zijn.

Zie voor een lijst met objecten, geldige ObjCodes en objectvelden  [&#x200B; API Ontdekkingsreiziger &#x200B;](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>In de context van de Workfront API is een aangepast formulier een `Category` -object en een aangepast veld is een `Parameter` -object.

### Bewerkingen

Objecten worden gemanipuleerd door een HTTP-aanvraag naar hun unieke URI te verzenden. De uit te voeren bewerking wordt opgegeven door de HTTP-methode.

De standaard HTTP-methoden komen overeen met de volgende bewerkingen:

* **GET** - wint een voorwerp door identiteitskaart terug, zoekt naar alle voorwerpen door een vraag, looppas rapporten, of voert genoemde vragen uit
* **POST** - neemt een nieuw voorwerp op
* **PUT** - geeft een bestaand voorwerp uit
* **DELETE** - schrapt een voorwerp

Om rond cliëntgebreken of protocollengtegrenzen te werken, kan de methodeparameter worden gebruikt om het gedrag van HTTP met voeten te treden. Een GET-bewerking kan bijvoorbeeld worden geïmplementeerd door de volgende URI te posten:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get <br> GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Antwoord

Elk verzoek krijgt een antwoord in JSON-indeling. De reactie heeft een gegevenskenmerk als de aanvraag succesvol was of een foutkenmerk als er een probleem was. De aanvraag

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

retourneert een JSON-respons die vergelijkbaar is met het volgende:


<pre><br>    "data": [<br>        <br>            "percentComplete": 0, <br>            "status": "CUR", <br>            "priority": 2, <br>            "name": "Brand New Project", <br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        &rbrace; <br>    ] <br></pre>

>[!NOTE]
>
>Wanneer het uitvoeren van een GET verzoek door uw browser adresbar, is het niet noodzakelijk om sessionID als deel van het verzoek te omvatten.

Er is speciale beveiliging toegevoegd rondom PUT-, POST- en DELETE-verzoeken. Om het even welk verzoek dat in het schrijven aan of het schrappen van het gegevensbestand resulteert kan slechts worden uitgevoerd als **sessionID=abc123** inbegrepen in URI is. In de volgende voorbeelden wordt getoond hoe dit op een DELETE-verzoek lijkt:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123 <br> GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc1 23</pre>

### Verificatie

De API verifieert elke aanvraag om ervoor te zorgen dat de client toegang heeft om een aangevraagd object te bekijken of te wijzigen.

Verificatie wordt uitgevoerd door een sessie-id door te geven die kan worden gegeven met een van de volgende methoden:

#### Koptekstverificatie aanvragen

De aangewezen methode van authentificatie is een verzoekkopbal over te gaan genoemd SessionID die het zittingsteken bevat. Dit heeft het voordeel om tegen [&#x200B; Cross-site van het Verzoek Smederij (CSRF) &#x200B;](https://en.wikipedia.org/wiki/Cross-site_request_forgery) aanvallen veilig te zijn en zich niet met URI voor caching doeleinden te mengen.

Hieronder ziet u een voorbeeld van een aanvraagkoptekst:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Verificatie op basis van cookie

De API gebruikt de zelfde op koekje-gebaseerde authentificatie die door Web UI aan het systeem wordt gebruikt. Als een client zich aanmeldt bij Workfront via de webinterface, wordt voor alle AJAX-aanroepen die vanuit dezelfde browser worden uitgevoerd, dezelfde verificatie gebruikt.

>[!NOTE]
>
>Ter bescherming tegen de mogelijkheid van aanvallen CSRF (Cross-Site Request Svervalsing), is deze methode van authentificatie slechts beschikbaar voor read-only verrichtingen.

## Aanmelden

>[!IMPORTANT]
>
>Workfront raadt niet langer het gebruik van de `/login` eindpunt- of API-toetsen aan. Gebruik in plaats daarvan een van de volgende verificatiemethoden:
>
>* Serververificatie met JWT
>* Gebruikersverificatie met OAuth2
>
>Voor instructies bij vestiging deze authentificatiemethodes, zie [&#x200B; tot toepassingen OAuth2 voor de integratie van Workfront leiden &#x200B;](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Voor instructies bij het gebruiken van serverauthentificatie in Workfront, zie [&#x200B; vormen en gebruiken de douaneOAuth 2 van uw organisatie toepassingen gebruikend stroom JWT &#x200B;](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Voor instructies bij het gebruiken van gebruikersauthentificatie in Workfront, zie [&#x200B; vormen en gebruiken de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van de vergunningscode &#x200B;](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>De in dit gedeelte beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord zijn gegaan bij het Adobe Business Platform. Aanmelden bij Workfront via de Workfront API is niet beschikbaar als uw organisatie is aangemeld bij het Adobe Business Platform.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan het Van Bedrijfs Adobe Platform is genegeerd, zie [&#x200B; Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) &#x200B;](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Met een geldige gebruikersnaam en wachtwoord kunt u de volgende aanvraag gebruiken om een sessie-id op te halen:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Dit plaatst een koekje om toekomstige verzoeken voor authentiek te verklaren evenals een reactie JSON met onlangs gecreeerde sessionID, de userID van de aangemelde gebruiker, en andere zittingsattributen terug te keren.

>[!NOTE]
>
>Als u een aangewezen API-gebruiker hebt die ook beheerder is, wordt u door Workfront sterk aangeraden zich aan te melden met behulp van een API-sleutel.

**producerend een Sleutel van API**

U kunt een API-sleutel genereren wanneer u zich als die gebruiker bij het systeem aanmeldt, zoals in het volgende voorbeeld wordt getoond:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**het terugwinnen van een eerder-Gegenereerde API Sleutel**

U kunt ook een API-sleutel ophalen die eerder voor een bepaalde gebruiker is gegenereerd door getApiKey uit te voeren:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Vervolgens kunt u dit resultaat gebruiken om elke API-aanroep te verifiëren door &quot;apiKey&quot; als een parameter request met deze waarde toe te voegen in plaats van een sessionID of gebruikersnaam en wachtwoord. Dit is uit veiligheidsoogpunt gunstig.

Het volgende verzoek is een voorbeeld van het ophalen van gegevens van een project met behulp van apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Het ongeldig maken van een API Sleutel**

Als de apiKey-waarde is gecompromitteerd, kunt u &quot;clearApiKey&quot; uitvoeren, waarmee de huidige API-sleutel ongeldig wordt gemaakt, zoals in het volgende voorbeeld wordt getoond:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Als de API is gewist, kunt u getApiKey opnieuw uitvoeren om een nieuwe API-sleutel te genereren.

### Afmelden

Wanneer een zitting volledig is, kunt u het volgende verzoek gebruiken om de gebruiker uit te loggen, verhinderend om het even welke verdere toegang met sessionID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

De sessionID die moet worden geregistreerd kan of als koekje, verzoekkopbal, of verzoekparameter worden gespecificeerd.

Een gebruiker afmelden:

1. Navigeer naar het aanmeldingsscherm, maar meld u niet aan.
1. Wijzig de URL in /attask/api/v15.0/project/search.\
   De pagina kan niet worden gevonden.
1. Vervang het woord *onderzoek* met login?username=admin&amp;password=user, substituerend uw gebruikersbenaming en wachtwoord voor *admin* en *user\
   *Deze sessie wordt in de browser opgeslagen als een cookie en hoeft niet in elke volgende GET-aanvraag te worden aangepast.

1. Wijzig de URL weer in **/attask/api/v15.0/project/search** .
1. Bericht het verstrekte antwoord.

U moet de sessionID altijd omvatten die na login wordt verstrekt wanneer het uitvoeren van PUT, POST, en DELETE verzoeken.

## GET-gedrag

Met de HTTP GET-methode kunt u een of meerdere objecten ophalen en rapporten uitvoeren.

### Objecten ophalen

U kunt een zoekopdracht naar objecten verbeteren met wijzigingstoetsen en filters.

#### Een object ophalen met de object-id

Als u de id van een object kent, kunt u het object ophalen door de unieke URI van het object te openen. De aanvraag

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

retourneert een reactie die lijkt op het volgende:

<pre><br>    "percentComplete": 0, <br>    "status": "CUR", <br>    "priority": 2, <br>    "name": "Brand New Project", <br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br></pre>


U kunt veelvoudige voorwerpen in het zelfde verzoek terugwinnen door de parameter van het identiteitskaart- verzoek te specificeren en een komma-gescheiden lijst van identiteitskaart&#39;s te geven, zoals aangetoond in het volgende voorbeeld:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Let op: de aanvraag /attask/api/v15.0/project?id=... is gelijk aan de aanvraag `/attask/api/v15.0/project/...` .

#### Een object ophalen met de URI

Als u een object wilt ophalen op andere criteria dan de id, kunt u zoeken naar de URI.

U kunt bijvoorbeeld het volgende verzoek gebruiken om een lijst met alle projecten in het systeem te retourneren:

```
GET /attask/api/v15.0/project/search
```

U kunt filters specificeren gebruikend de verzoekparameters als naam-waardeparen. In het volgende voorbeeld wordt bijvoorbeeld een aanvraag getoond waarin alle huidige projecten worden gevonden:

```
GET /attask/api/v15.0/project/search?status=CUR
```

Het volgende verzoek vindt alle taken die nog niet volledig zijn en die aan een gebruiker genoemd John worden toegewezen.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Zoekopties gebruiken

De volgende tabel bevat een aantal opties die u kunt gebruiken met de Workfront API.

| **Modifier** | **Beschrijving** | **Voorbeeld** |
| --- | --- | --- |
| eq | retourneert resultaten die de status van gesloten hebben | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | retourneert resultaten die niet de status van closed hebben | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gist | retourneert resultaten met een percentage voltooid groter dan of gelijk aan 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | retourneert resultaten die een percentage voltooid hebben van minder dan of gelijk aan 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | retourneert resultaten als de beschrijving Null is | <pre>...description_Mod=is null...</pre> |
| notnull | retourneert resultaten als de beschrijving niet null is | <pre>...description_Mod=notnull...</pre> |
| contains | retourneert resultaten als de naam &quot;Workfront&quot; bevat | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| Tussen | retourneert resultaten die de laatste 7 dagen een ingangsdatum hebben | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Zoekverzoeken zijn hoofdlettergevoelig. Als er een fout optreedt, controleert u of  **_Mod** en **_Range** hebben de correcte kapitalisatie.

#### OR-instructies gebruiken

U kunt een zoekopdracht verfraaien door een parameter toe te voegen die &quot;OR&quot; bevat, en een getal om het niveau van een filter of reeks filters aan te geven.

Een OF verklaring keert slechts verslagen in de API vraag terug die aan de OF verklaring het filtreren criteria voldoen. Filters worden niet geïmpliceerd over OR verklaringsniveaus.

Als u bijvoorbeeld wilt filteren op

* Taken die een naam hebben die &quot;Planning&quot;OF bevatten
* Taken in een portfolio met de naam &quot;FixedAssets&quot; EN toegewezen aan iemand met de naam &quot;Steve&quot; OR
* Taken die een oudertaak hebben genoemd &quot;Definitieve Taak&quot;

Gebruik vervolgens de volgende API-aanroep met de verschillende OR-instructies:
<pre>GET /attask/api/v15.0/task/search?name=Planning <br>&amp;name_Mod=contains <br> &amp;OR :1: portefeuille:name=FixedAssets <br> &amp; OF :1: portefeuille:name_Mod=eq <br>&amp;OR :1: toegewezenAan:name=Steve <br> &amp; OF :1: toegewezenAan:name_Mod=icontains <br> &amp;OF :2: ouder:name=Final Taak <br> &amp;OF :2: ouder:name_Mod=eq
</pre>

#### Filterparameters gebruiken

Een mogelijk probleem bij het gebruik van URL-parameters voor zoekfilters is dat Workfront bepaalde parameters parseert voordat er op verschillende verificatiemethoden wordt gecontroleerd (bijvoorbeeld gebruikersnaam, wachtwoord, apiKey, cookie). Wanneer dit gebeurt worden de parameters niet gebruikt als filters in de vraag. 

U voorkomt dit probleem door deze waarden in filterparameters met JSON-opmaak te plaatsen. Als u bijvoorbeeld wilt filteren op de gebruiker van de gebruikersnaam in plaats van deze te gebruiken 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>Geef de URL-parameter door in een filter, zoals in het volgende voorbeeld wordt getoond:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### De parameter Kaartverzoek gebruiken

Standaard zijn de gegevens die door een zoekopdracht worden geretourneerd, een JSON-array. Afhankelijk van uw gebruikscase kan het efficiënter zijn om het resultaat op te halen als een JSON-object dat met ID wordt geïndexeerd. Dit kan worden gedaan door de parameter van het kaartverzoek te gebruiken. De aanvraag 
<pre>/attask/api/v15.0/task/search?map=true</pre>retourneert een reactie geïndexeerd door ID, vergelijkbaar met het volgende:
<pre><br>    "data": <br>        "4c9a97db000000f13ee4446b9aead9b": <br>            "percentComplete": 0, <br>            "status": "NEW", <br>            "name": "first task",<br>            "ID": "4c9a97db000000f13ee4446b9aead9b", <br>            "taskNumber": 1 <br>        &rbrace;,<br>        "4ca28ba60002024cd49e75bd43cf601": <br>            "percentComplete": 0, <br>            "status": "INP:A", <br>            "name": "second task", <br>            "ID": "4ca28ba60002024cd49e75bd43cf601", <br>            "taskNumber": 2 <br>        &rbrace; <br>    &rbrace; <br></pre>

#### De veldverzoekparameter gebruiken

Als u een object ophaalt, wordt standaard alleen de meest gebruikte subset met velden geretourneerd.

U kunt de parameter van het gebiedsverzoek gebruiken om een komma-gescheiden lijst van specifieke gebieden te specificeren is teruggekeerd. De aanvraag
<pre>/attask/api/v15.0/task/search?fields=scheduledStartDate,priority</pre>retourneert een reactie die lijkt op het volgende:
<pre><br>    "priority": 2, <br>    "name": "first task", <br>    "ID": "4c7c08fa000002ff924e298ee148df4", <br>    "SchedulStartDate": "2010-08-30T09 :00: 00:000-0600" <br></pre>

>[!NOTE]
>
>Deze veldnamen zijn hoofdlettergevoelig.

Voor een lijst met mogelijke veldverwijzingen raadpleegt u de  [&#x200B; API Ontdekkingsreiziger &#x200B;](../../wf-api/general/api-explorer.md)

#### Zoeken naar geneste objecten

U kunt zoeken naar geneste objecten. Standaard worden geneste objecten alleen met de naam en id geretourneerd. Als u bijvoorbeeld alle problemen samen met de eigenaar wilt ophalen, gebruikt u de volgende aanvraag:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Als u meer informatie nodig hebt, kunt u een genest veld aanvragen met de syntaxis van een dubbele punt. Met de volgende aanvraag wordt bijvoorbeeld naar alle problemen gezocht, samen met de naam, id, titel en telefoonnummer van de eigenaar
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>en retourneert het volgende: 
<pre><br>    "name": "an major issue", <br>    "ID": "4c78285f00000908ea8cfd66e084939f", <br>    "owner": <br>        "title": "Operations Specialist", <br>        "phoneNumber": "555-1234", <br>        "name": "Admin User", <br>        "ID": "4c76ed7a000054c172b2c2d9f7f81c3" <br>    &rbrace; <br></pre>

#### Geneste verzamelingen ophalen

U kunt geneste verzamelingen van objecten ophalen. Als u bijvoorbeeld een project wilt ophalen met alle bijbehorende taken, gebruikt u de volgende aanvraag:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>De volgende aanvraag krijgt taaktoewijzingen:
<pre>/attask/api/v15.0/task/search?fields=toewijzingen</pre>

#### Zoeken naar meerdere geneste velden

Standaard worden alleen de naam en de id van elke taak geretourneerd, maar u kunt aanvullende geneste velden opgeven met een dubbele puntnotatie. Als u alle beschikbare velden voor een verwant object of verzameling wilt weergeven, voegt u gewoon een dubbele punt en sterretje toe aan de verwijzing naar object of verzameling.
<pre>/attask/api/v15.0/task/search?fields=astaken:*</pre>

#### Aangepaste gegevens ophalen

U kunt aangepaste gegevensvelden ophalen met het voorvoegsel &quot;DE:&quot;. Als u bijvoorbeeld een project wilt aanvragen met de parameter &quot;CustomText&quot;, gebruikt u de volgende aanvraag:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>die worden geretourneerd
<pre><br>    "name": "custom data project", <br>    "ID": "4c9a954f000001afad0687d7b1b4e43", <br>    "DE:CustomText": "task b" <br></pre>U kunt ook alle aangepaste gegevens voor een object ophalen door het veld parameterValues aan te vragen. Bijvoorbeeld: 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>retourneert vergelijkbare gegevens naar het volgende:
<pre><br>    "name": "custom data project", <br>    "ID": "4c9a954f000001afad0687d7b1b4e43", <br>    parameterValues: <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBox": ["first", "second", "third"] <br>    &rbrace; <br></pre>

#### Benoemde query&#39;s gebruiken

Sommige objecttypen hebben benoemde zoekopdrachten die doorgaans worden uitgevoerd en die beschikbaar zijn door de naam van de query aan het einde van het objecttype URI toe te voegen. Met de volgende aanvraag worden bijvoorbeeld de werkitems (taken en problemen) opgehaald waaraan de gebruiker momenteel is toegewezen:
<pre>/attask/api/v15.0/work/myWork</pre>Benoemde query's ondersteunen het aanvragen van de parameter fields om extra velden op te halen. Sommige benoemde query's accepteren ook extra filters. Zie het tabblad Handeling voor het object in het dialoogvenster  [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### `Count` gebruiken

Met `count` kunt u het aantal resultaten retourneren dat overeenkomt met uw query. Dit kan handig zijn wanneer u de gegevens in de resultaten niet nodig hebt. Door alleen het aantal te retourneren, kan de server de aanvraag sneller verwerken en bandbreedte opslaan. De aanvraag
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>retourneert het aantal resultaten in de volgende indeling:
<pre><br>    "count": 3 <br></pre>Het retourneren van een telling is een veel kleinere gegevensoverdracht dan wanneer alle objecten worden geretourneerd. De syntaxis is identiek aan de zoekopdracht.

### Een rapport aanvragen

U kunt een rapportverzoek uitvoeren, waar slechts het totaal van één of ander gebied met één of meerdere groeperingen wordt gewenst. Zoals in het volgende voorbeeld wordt getoond, is de rapportsyntaxis gelijk aan de syntaxis voor de SOAP API:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>dat het volgende resultaat retourneert
<pre><br>    "First Project": <br>        "sum_hours": 15 <br>    &rbrace;, <br>     "Second Project": <br>        "sum_hours": 30 <br>    &rbrace; <br></pre>Wanneer u de parameter $$ROLLUP=true toevoegt, wordt op elk groeperingsniveau een totaal opgenomen:
<pre><br>    "First Project": <br>        "sum_hours": 15 <br>    &rbrace;, <br>    "Second Project": <br>        "sum_hours": 30 <br>    &rbrace;, <br>    "$$ROLLUP": <br>        "sum_hours": 45 <br>    &rbrace; <br></pre>

### Zoekresultaten sorteren in de API

U kunt de resultaten op elk veld sorteren als u het volgende aan uw API-aanroep toevoegt:

&amp;entryDate_Sort=asc

Als u bijvoorbeeld wilt sorteren op geplande begindatum van taak, verwijdert u entryDate en vervangt u deze door scheduledCompletionDate.

Dit werkt voor de meeste velden in Workfront.

### Zoekbeperkingen overwegen

Bij het opvragen van een object moet speciale aandacht worden besteed aan de relatie tussen verwante objecten en zoekbeperkingen. Bijvoorbeeld, zoals aangetoond in de volgende lijst, kan een vraag voor projecten niet meer dan 2.000 projecten terugkeren. Deze 2000 projecten worden beschouwd als &quot;primaire objecten&quot;. Als u voor het gebied van Taken op de projecten vraagt, wordt het gebied van Taken, dat een inzameling is, een secundair voorwerp aan het primaire objectenProject. Een vraag voor het gebied van Taken kan duizenden taken op projecten omvatten. In totaal kan het gecombineerde aantal geretourneerde objecten (projecten en taken) het maximum van 50.000 niet overschrijden.

Om optimale prestaties te verzekeren, toont de volgende lijst de beperkingen die op onderzoeksverzoeken worden geplaatst. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zoekresultaat</th> 
   <th>Beperking</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Standaardaantal resultaten</td> 
   <td>100</td> 
   <td> Als er geen limiet is opgegeven in het queryfilter (d.w.z. $$LIMIT), mag het resultaat niet meer dan 100 primaire objecten bevatten. <br> zie <a href="#using-paginated-responses" class="MCXref xref"> Gebruikend Gepagineerde Reacties </a> voor instructies op hoe te om deze beperking met voeten te treden. </td> 
  </tr> 
  <tr> 
   <td>Max. aantal resultaten</td> 
   <td>2.000</td> 
   <td>Het queryfilter (d.w.z. $$LIMIT) kan maximaal 2000 resultaten retourneren. Zie "Gepagineerde reacties" voor meer informatie.</td> 
  </tr> 
  <tr> 
   <td>Maximale velddiepte</td> 
   <td>4</td> 
   <td>Bij het identificeren van de velden die u wilt weergeven, kunt u niet meer dan vier niveaus van het object dat wordt gevraagd, weggaan.</td> 
  </tr> 
  <tr> 
   <td>Max. aantal objecten</td> 
   <td>50.000</td> 
   <td>De resultaatset mag geen 50000 primaire en secundaire objecten bevatten.</td> 
  </tr> 
  <tr> 
   <td>Max. aantal velden</td> 
   <td nowrap>1.000.000</td> 
   <td>Als de resultaatset minder dan 50000 objecten is, kunnen de resultaten maximaal 1000.000 velden bevatten.</td> 
  </tr> 
  <tr> 
   <td>Max. aantal batch-inhoud maakt/werkt bij</td> 
   <td>100</td> 
   <td>De maximale limiet voor het maken of bijwerken van batch is 100.</td> 
  </tr> 
 </tbody> 
</table>

### Gepagineerde reacties gebruiken {#using-paginated-responses}

Als u de standaardlimiet voor zoekopdrachten met betrekking tot het aantal resultaten wilt overschrijven en 200 resultaten wilt toestaan, kunt u het filter `$$LIMIT=200` in de query opnemen, zoals in het volgende voorbeeld wordt getoond:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Om betrouwbaarheid en prestaties voor andere huurders in het systeem te verzekeren, is de maximum toegestane resultaatgrens per vraag 2000 voorwerpen. Als u probeert een grotere limiet op te geven, wordt een `IllegalArgumentException` -foutbericht weergegeven. 

Daarom adviseren wij u het gebruiken van gepagineerde reacties voor grote datasets overweegt. Voeg het filter `$$FIRST` toe om het eerste resultaat op te geven dat moet worden geretourneerd. Bijvoorbeeld, keert het volgende verzoek resultaten 201-250 voor een vraag terug:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

In het bovenstaande voorbeeld retourneert `$$FIRST=200` het 201e resultaat. `$$FIRST=0` retourneert het eerste resultaat. Het kan helpen om van de waarde $$FIRST als aantal resultaten te denken u wilt overslaan alvorens resultaten terug te keren.

Gebruik een sorteerparameter om ervoor te zorgen dat de resultaten correct worden gepagineerd. Hierdoor kunnen de resultaten in dezelfde volgorde worden geretourneerd, zodat de paginering de resultaten niet herhaalt of overslaat. Als u bijvoorbeeld wilt sorteren met de object-id, gebruikt u `ID_Sort=asc` .

### Toegangsregels maken

U kunt een toegangsregel maken om te bepalen wie toegang heeft tot een object. Hieronder volgen voorbeelden van toegangsregels die u kunt instellen:

Om een project te plaatsen zodat wordt het gedeeld slechts met een gebruiker met identiteitskaart &quot;abc123&quot;gebruik het volgende verzoek:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxx?method=put updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Alternatief, om slechts met een nieuwe persoon te delen en bestaande toestemmingen intact te houden:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Om de bestaande toegangsregels terug te winnen:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST-gedrag

POST voegt een nieuw object in. De syntaxis is identiek aan PUT, maar met een paar uitzonderingen. Omdat het nieuwe object nog niet bestaat, heeft het geen id. Daarom bevat de URI de id niet.

### Een object maken

Hieronder ziet u een voorbeeld van een aanvraag om een nieuw project te maken:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>De reactie omvat het nieuwe project samen met zijn nieuwe identiteitskaart en om het even welke andere gespecificeerde gebieden.

### Een object kopiëren

Sommige objecten ondersteunen kopiëren. Voor deze objecttypen is het mogelijk om nieuwe objecten te maken door te posten met een copySourceID-parameter. Met de volgende aanvraag wordt bijvoorbeeld het opgegeven project gekopieerd en krijgt het een nieuwe naam:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Documenten uploaden

U kunt documenten uploaden via de volgende API-URL:
<pre>POST /attask/api/v15.0/upload</pre>De API verwacht dat het inhoudstype multipart/form-data is. De parameternaam voor het bestand moet uploadedFile zijn. De server retourneert de volgende JSON-gegevens:
<pre><br>    "handle": "4c7c08fa000002ff924e298ee148df4"<br></pre>U kunt de greep en de post naar de volgende URL gebruiken wanneer u een Workfront-document maakt:
<pre>POST /attask/api/v15.0/document?updates=&lbrace;<br>    name: aFileName,<br>    handle: abc...123, (handle from the file upload) <br>    docObjCode: PROJ, (of TASK, OPTASK, enz.) <br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br></pre>

## PUT-gedrag

PUT wordt gebruikt om een bestaand object bij te werken.

De reactie voor een PUT is identiek aan die van een GET. In beide gevallen retourneert de server de nieuwe status van het object na de update. Alle regels die worden gebruikt om een reactie op een GET-verzoek te wijzigen, werken ook met PUT, zoals het opgeven van extra velden die moeten worden geretourneerd, aangepaste gegevens enzovoort.

### Objecten bewerken

Objecten worden altijd bijgewerkt door de id met behulp van de unieke URI van het object. Velden die moeten worden bijgewerkt, worden opgegeven als aanvraagparameters. Als u bijvoorbeeld de naam van een project wilt wijzigen, kunt u een aanvraag verzenden die vergelijkbaar is met het volgende:
<pre>PUT /attask/api/v15.0/project/4c7...?name=New de Naam van het Project <br> PUT /attask/api/v15.0/project?id=4c7..&amp;name=New de Naam van het Project</pre>Aangezien voor de update een id is vereist, mislukt deze bewerking (zonder invoeging) als het object niet op de server bestaat.

### JSON-bewerkingen opgeven

Zoals in het volgende voorbeeld wordt getoond, kunt u de parameter van het updateverzoek gebruiken om de gebieden te specificeren die moeten worden bijgewerkt gebruikend syntaxis JSON:
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>&lbrace;<br>     name: "New Project Name", <br>     status: "CUR", <br>     ... <br></pre>

### Geneste updates maken

Sommige objecten hebben privéverzamelingen die kunnen worden bijgewerkt. In het volgende voorbeeld ziet u hoe u de bestaande toewijzingen voor een bepaalde taak overschrijft:
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>{<br>    toewijzingen: [ <br>        <br>            assignedToID: "2222...54d0, <br>            assignPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br></pre>

>[!NOTE]
>
>Terwijl de updates aan het hoogste niveau worden gemaakt klein zijn, vervangen de updates aan een inzameling of een genesteld voorwerp volledig de bestaande inzameling. Als u één toewijzing op een taak wilt bewerken zonder de objecten te beïnvloeden, gebruikt u PUT op de toewijzing in plaats van op de taak.

In het volgende voorbeeld wordt van een project een wachtrij voor een openbare helpdesk gemaakt. De bestaande wachtrijeigenschappen worden vervangen.
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>&lbrace; <br>    queueDef: { <br>        isPublic: 1 <br>    } <br></pre>

### De parameter Handelingverzoek gebruiken

Sommige objecten ondersteunen aanvullende acties die naast eenvoudige bewerkingen kunnen worden uitgevoerd. U kunt deze handelingen opgeven met de parameter voor actiedracht. In het volgende verzoek wordt bijvoorbeeld de tijdlijn voor een bepaald project opnieuw berekend:
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline <br><br> of <br><br> PUT /attask/api/v15.0/project/4c7../calculateTimeline </pre>

### Objecten verplaatsen

In het volgende voorbeeld ziet u de syntaxis voor het verplaatsen van een taak van het ene project naar het andere:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8...</pre>Hier ziet u een voorbeeld voor elk handelingstype: (??)
<pre>PUT /attask/api/v15.0/project/1234/acceptApproval <br><br> PUT /attask/api/v15.0/project/1234/calculateFinance <br><br> PUT /attask/api/v15.0/project/1234/calculateTimeline <br><br> de aanvaller van PUT/api/v15.0/project/1234/calculateDataExtension <br><br> PUT /attask/api/v15.0/project/1234/retrieveApproval <br><br> PUT /attask/api/v15.0/project/1234/rejectApproval <br><br> PUT /attask/api i/v15.0/task/1234/move <br><br> PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Alleen voor de verplaatsingsactie zijn aanvullende kenmerken vereist om het project op te geven waar het werkitem moet worden verplaatst.

Hieronder ziet u een voorbeeld van elk actietype: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Objecten delen

In het volgende voorbeeld ziet u de syntaxis voor het delen van een project met een team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Wanneer u een object bewerkt, kunt u alle toegangsregels voor een object vervangen door een PUT uit te voeren en updates te verzenden die vergelijkbaar zijn met het volgende voorbeeld:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates=&lbrace;accessRules:&lbrack;{accessorID:'123abcxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',xxxxcore:'VIEW'}</pre>In het volgende voorbeeld ziet u de syntaxis voor het verplaatsen van een taak van het ene project naar het andere:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8...</pre>

## DELETE-gedrag

DELETE verwijdert een object. In elk geval, kan URI de parameter force=true omvatten om de server te veroorzaken om de gespecificeerde gegevens en zijn afhankelijke personen te verwijderen. In het volgende voorbeeld wordt een taak verwijderd door de HTTP DELETE-methode uit te voeren op een URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0 <br> DELETE /attask/api/v15.0/task?id=4c7821c 0000d6fa8d5e52f07a1d54d0 <br> DELETE /attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d?force=true <br> DELETE /attask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0?force=true</pre>

## Bulkupdates

Met een bulkupdateinstructie worden meerdere objecten tegelijkertijd bijgewerkt binnen één API-aanroep. Een bulk creeert API vraag wordt gebouwd gelijkaardig aan een normale updatevraag, zoals aangetoond in de volgende voorbeelden:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-xxxxxxxxxxxx</pre>of <pre>PUSH /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-xxxxxxxxxxxxxx</pre>wat resulteert in een rendement dat vergelijkbaar is met het volgende:
<pre>gegevens: [<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3", <br>    name: "Test_Project_1", <br>    objCode: "PROJ", <br>    percentComplete: 0, <br>    scheduledCompletionDate: "2014-08-28T11 :00: 00:000-0400", <br>    SchedulStartDate: "2014-08-28T11 :00: 00:000-0400", <br>    prioriteit: 0, <br>    projectedCompletionDate: "2014-08-28T16 :12: 00:000-0400", <br>    status: "CUR"<br>, <br> &lbrace;<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10", <br>    name: "Test_Project_2", <br>    objCode: "PROJ", <br>    percentComplete: 0usi,<br>    scheduledCompletionDate: "2014-08-28T11 :00: 00:000-0400", <br>    scheduledStartDate: "2014-08-28T11 :00: 00:000-0400", <br>    priority: 0, <br>    projectedCompletionDate: "2014-08-28T16 :12: 00:000-0400", <br>    status: "CUR"<br>]</pre>U kunt ook een bulkupdate uitvoeren die vergelijkbaar is met het volgende:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx", "name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxx</pre>wat resulteert in een rendement dat vergelijkbaar is met het volgende:
<pre>gegevens: [<br>     ID: "53ff8e15003b461d4560f7f65a440078", <br>     name: "Test_Project_1_Edit", <br>     objCode: "PROJ", <br>     percentComplete: 0, <br>     scheduledCompletionDate: "2014-08-28T11 :00: 00:000-0400", <br>     SchedulStartDate: "2014-08-28T11 :00: 00:000-0400", <br>     prioriteit: 0, <br>     projectedCompletionDate: "2014-08-28T16 :16: 00:000-0400", <br>     status: "CUR"<br>, <br> &lbrace;<br>    ID: "53ff8e19003b46238a58d303608de502", <br>    name: "Test_Project_2_Edit", <br>    objCode: "PROJ", <br>    percentComplete: 0, <br>    scheduledCompletionDate: "2014-08-28T11 :00: 00:000-0400", <br>    scheduledStartDate: "2014-08-28T11 :00: 00:000-0400", <br>    priority: 0, <br>    projectedCompletionDate: "2014-08-28T16 :16: 00:000-0400", <br>    status: "CUR"<br>]</pre>Als u alle bewerkingen in dezelfde transactie wilt uitvoeren, voegt u "atomic=true" toe aan uw batch-API-aanroep als een aanvraagparameter. Op deze manier worden alle bewerkingen teruggedraaid als een van de bewerkingen mislukt.

>[!NOTE]
>
>Atoombatchbewerkingen kunnen alleen &#39;success: true&#39; of een fout retourneren.

