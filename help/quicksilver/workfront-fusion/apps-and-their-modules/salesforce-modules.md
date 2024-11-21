---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Salesforce-modules
description: In een Adobe Workfront Fusion-scenario kunt u workflows automatiseren die gebruikmaken van Salesforce, en deze koppelen aan meerdere toepassingen en services van derden.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 0%

---

# [!DNL Salesforce] modules

In een Adobe Workfront Fusion-scenario kunt u workflows automatiseren die [!DNL Salesforce] gebruiken en er verbinding mee maken met meerdere toepassingen en services van derden.

Ga voor een video-introductie over de Salesforce-connector naar:

* [ Salesforce ](https://video.tv.adobe.com/v/3427027/){target=_blank}

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Niet alle versies van [!DNL Salesforce] hebben API-toegang. Zie voor meer informatie de informatie over [!DNL Salesforce] -edities met API-toegang op de [!DNL Salesforce] -communitysite.
>* Zie de API-documenten van [!DNL Salesforce] voor informatie over specifieke fouten die door de [!DNL Salesforce] API worden geretourneerd. U kunt ook de status van de [!DNL Salesforce] API controleren op mogelijke uitval van de service.
>

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
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het abonnement [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Als u [!DNL Salesforce] -modules wilt gebruiken, moet u een [!DNL Salesforce] -account hebben.

## Salesforce API-informatie

De Salesforce-connector gebruikt het volgende:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> {{connection.instanceUrl}</td>
  </tr> 
  <tr> 
   <td role="rowheader">API-versie</td> 
   <td> v46,0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-tag</td> 
   <td>v1.15.14</td> 
  </tr>
 </tbody> 
 </table>

## Informatie over zoeken naar [!DNL Salesforce] -objecten

Bij het zoeken naar objecten kunt u afzonderlijke zoekwoorden invoeren of een complexere query maken met behulp van jokertekens en operatoren:

* Gebruik de asterisk wild card (\*) als vervanging voor nul of meer tekens. Als u bijvoorbeeld zoekt naar CA\*, worden items gevonden die met CA beginnen
* Wilde kaart met vraagteken gebruiken (?) als vervanging van één teken. Bijvoorbeeld, vindt een onderzoek naar Jo?n punten met de term John of Joan maar niet Jon
* Gebruik de operator voor aanhalingstekens (&quot; &quot;) om een exacte woordovereenkomst te zoeken. Bijvoorbeeld: &quot;Maandvergadering&quot;

Zie de [!DNL Salesforce] documentatie voor ontwikkelaars over SOQL en SOSL voor meer informatie over zoekmogelijkheden.

## [!DNL Salesforce] modules en hun velden

* [ Trekkers ](#triggers)
* [ Acties ](#actions)
* [Zoekopdrachten](#searches)

### Triggers

* [[!UICONTROL Watch for Records]](#watch-for-records)
* [[!UICONTROL Watch Outbound Messages]](#watch-outbound-messages)
* [[!UICONTROL Watch a field]](#watch-a-field)

#### [!UICONTROL Watch for Records]

Deze triggermodule voert een scenario uit wanneer een record in een object wordt gemaakt of bijgewerkt. De module retourneert alle standaardvelden die zijn gekoppeld aan de record of records, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Selecteer het type [!DNL Salesforce] record dat u in de module wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Fields]</td> 
   <td>Selecteer de velden die u in de module wilt bekijken. Beschikbare velden zijn afhankelijk van het type record.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Bepaal of u het scenario alleen nieuwe records van het geselecteerde type wilt bekijken, of nieuwe records van het geselecteerde type en alle andere wijzigingen in records van dat type.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Outbound Messages]

Deze trekkermodule voert een scenario uit wanneer iemand een bericht verzendt. De module retourneert alle standaardvelden die zijn gekoppeld aan de record of records, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Voor deze module is extra installatie vereist:

1. Ga naar de instellingspagina van [!DNL Salesforce] .

   Ga naar de knop met het label &quot; [!UICONTROL Setup]&quot; in de rechterbovenhoek van het [!DNL Salesforce] -account en klik op deze knop om de instellingspagina te openen. Van de [!DNL Salesforce] opstellingspagina, bepaal de plaats van de &quot;[!UICONTROL Quick Find / Search]&quot;bar op de linkerkant. Zoek naar &quot;[!UICONTROL Workflow Rules].&quot;

1. Klik op **[!UICONTROL Workflow Rules]**.
1. Voor de [!UICONTROL Workflow Rules] pagina die verschijnt, klik **[!UICONTROL New Rule]** en selecteer het objecten type de regel zal van toepassing zijn (zoals &quot; [!UICONTROL Opportunity]&quot;als u updates aan verslagen van de Opportunity controleert).
1. Klik op **[!UICONTROL Next]**.
1. Stel een regelnaam, evaluatiecriteria en regelcriteria in en klik op **[!UICONTROL Save]** en **[!UICONTROL Next]** .

1. Klik op **[!UICONTROL Done]**.
1. Klik op **[!UICONTROL Edit]**..
1. Selecteer in de vervolgkeuzelijst **[!UICONTROL Add Workflow Action]** de optie **[!UICONTROL New Outbound Message]**.

1. Geef een naam, beschrijving, URL van eindpunt en velden op die u in het nieuwe uitgaande bericht wilt opnemen en klik op **[!UICONTROL Save]** .

   Het veld **[!UICONTROL Endpoint URL]** bevat de URL die wordt opgegeven in de lus [!DNL Salesforce] [!UICONTROL Outbound Message] in [!DNL Workfront Fusion] .

1. Configureer een scenario dat begint met de gebeurtenis [!UICONTROL Outbound Message] .

1. Klik **&lt;/>** pictogram in het bodemrecht en kopieer verstrekte URL.
1. Ga terug naar de pagina **[!UICONTROL Workflow Rules]** , zoek de nieuwe regel en klik op **[!UICONTROL Activate]** .

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Selecteer de webhaak die u wilt gebruiken om uitgaande berichten te bekijken. Als u een webhaak wilt toevoegen, klikt u op <strong>[!UICONTROL Add]</strong> en voert u de naam en de verbinding van de webhaak in.</p> <p>Voor instructies over het aansluiten van uw [!DNL Salesforce] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!UICONTROL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Selecteer het type [!DNL Salesforce] record dat de module moet controleren voor uitgaande berichten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Selecteer de gebieden die u de module voor uitgaande berichten wilt letten. Beschikbare velden zijn afhankelijk van het type record.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Watch a field]*

Deze triggermodule start een scenario wanneer een veld wordt bijgewerkt in [!DNL Salesforce] .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Selecteer het type record dat het veld bevat waarop de module moet letten. Kies een recordtype waarvoor [!UICONTROL Field History] is ingeschakeld in [!DNL Salesforce] . Voor meer informatie, zie <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5"> het Volgen van de Geschiedenis van het Gebied </a> in de [!DNL Salesforce] documentatie. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Selecteer de gebieden die u de module voor veranderingen wilt controleren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal gebieden in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Create a Record]](#create-a-record)
* [[!UICONTROL Read a Record]](#read-a-record)
* [[!UICONTROL Delete a Record]](#delete-a-record)
* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Upload Attachment/Document]](#upload-attachmentdocument)
* [[!UICONTROL Download Attachment/Document]](#download-attachmentdocument)

#### [!UICONTROL Create a Record]

Deze actiemodule maakt een nieuwe record in een object.

In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module. Dit vermindert het aantal gebieden u door moet scrollen wanneer vestiging de module.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Selecteer het type [!DNL Salesforce] record dat u met de module wilt maken. Velden worden beschikbaar op basis van het type record dat is geselecteerd in het veld [!UICONTROL Record Type] . Deze velden zijn gebaseerd op de API van [!DNL Salesforce] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Selecteer de gebieden die u de module wilt vormen wanneer het creëren van het nieuwe verslag. De vereiste velden staan boven aan de lijst. </p> <p>De velden die u selecteert, worden geopend onder dit veld. U kunt nu waarden invoeren in deze velden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a Record]

Deze actiemodule leest gegevens van één object in [!DNL Salesforce] .

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Selecteer het type [!DNL Salesforce] record dat de module [action].read moet gebruiken.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Record Fields]</td>
    <td>Selecteer de velden die u in de module wilt lezen. U moet ten minste één veld selecteren.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Voer de unieke [!DNL Salesforce] -id in of wijs deze toe aan de record die u wilt lezen in de module.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Salesforce] in uw browser en kopieert u de tekst aan het einde van de URL na de laatste schuine streep (/). Bijvoorbeeld: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Record]

Deze actiemodule verwijdert een bestaande record in een object.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Selecteer het type [!DNL Salesforce] -record dat u wilt verwijderen door de module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Voer de unieke [!DNL Salesforce] -id in of wijs deze toe aan de record die u wilt verwijderen door de module.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Salesforce] in uw browser en kopieert u de tekst aan het einde van de URL na de laatste schuine streep (/). Bijvoorbeeld: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Custom API Call]

Met deze actiemodule kunt u een aangepaste, geverifieerde aanroep van de [!DNL Salesforce] API maken. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de andere [!DNL Salesforce] -modules kan worden uitgevoerd.

De module retourneert het volgende:

* **[!UICONTROL Status Code]** (nummer): Dit geeft aan of uw HTTP-aanvraag is geslaagd of mislukt. Dit zijn standaardcodes die u kunt opzoeken op internet.
* **[!UICONTROL Headers]** (object): een gedetailleerdere context voor de respons-/statuscode die geen betrekking heeft op de hoofdtekst van de uitvoer. Niet alle kopteksten in een antwoordkoptekst zijn reactiekoppen. Sommige koppen zijn daarom niet altijd even handig.

  De antwoordheaders zijn afhankelijk van de HTTP-aanvraag die u hebt gekozen bij het configureren van de module.

* **[!UICONTROL Body]** (object): afhankelijk van de HTTP-aanvraag die u hebt gekozen bij het configureren van de module, ontvangt u mogelijk gegevens terug. Die gegevens, zoals de gegevens van een [!UICONTROL GET] aanvraag, bevinden zich in dit object.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Ga een weg met betrekking tot <code> &lt;Instance URL&gt;/services/data/v46.0/</code> in.</p> <p>Voor de lijst van beschikbare eindpunten, verwijs naar de <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm"> Gids van de Ontwikkelaar van de REST API van Salesforce </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld <code>{"Content-type":"application/json"}</code> . Workfront Fusion voegt de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** de volgende API vraag keert de lijst van alle gebruikers in uw [!DNL Salesforce] rekening terug:
>
>* **URL**: `query`
>
>* **Methode**: [!UICONTROL GET]
>
>* **Koord van de Vraag**:
>
>* **Sleutel**: `q`
>
>* **Waarde**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Overeenkomsten met de zoekopdracht vindt u in de sectie Uitvoer van de module onder **[!UICONTROL Bundle]> [!UICONTROL Body] >[!UICONTROL records]** .
>
>In ons voorbeeld werden 6 gebruikers geretourneerd:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Upload Attachment/Document]

Deze actiemodule uploadt een bestand en koppelt het aan een record die u opgeeft, of uploadt een document.

De module retourneert de id van de bijlage of het document en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type of Upload]</td> 
   <td>Selecteer of u een bijlage of een document wilt uploaden in de module.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Voer de id in of wijs de id toe van het object waarnaar u een bijlage wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Selecteer de map met het bestand dat u wilt uploaden in de module. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source File]</td> 
   <td>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download Attachment/Document]

Deze actiemodule downloadt een document of bijlage uit een record.

U geeft de id van de record op en het gewenste type download.

De module retourneert de id van de bijlage of het document en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Type of Download]</td>
    <td> <p>Geef het type bestand op dat u van Salesforce wilt downloaden.</p> 
     <ul> 
      <li>[!UICONTROL Attachment]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (Dit is een document dat is geüpload naar een bibliotheek in [!DNL Saleforce CRM Content] of [!DNL Salesforce Files] .)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Voer de unieke [!DNL Salesforce] -id in of wijs deze toe aan de record die u wilt downloaden met de module.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Salesforce] in uw browser en kopieert u de tekst aan het einde van de URL na de laatste schuine streep (/). Bijvoorbeeld: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Update a Record]

Deze actiemodule bewerkt een record in een object.

In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module. Dit vermindert het aantal gebieden u door moet scrollen wanneer vestiging de module.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Voer de id in van de record die u wilt bijwerken of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Selecteer het type [!DNL Salesforce] record dat u wilt bijwerken in de module. Velden worden beschikbaar op basis van het type record dat is geselecteerd in het veld Recordtype. Deze velden zijn gebaseerd op de API van [!DNL Salesforce] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Selecteer de gebieden die u de module wilt vormen wanneer het creëren van het nieuwe verslag. De vereiste velden staan boven aan de lijst. </p> <p>De velden die u selecteert, worden geopend onder dit veld. U kunt nu waarden invoeren in deze velden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

#### [!UICONTROL Search with Query]

Deze zoekmodule zoekt naar records in een object in [!DNL Salesforce] dat overeenkomt met de zoekquery die u opgeeft. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search Type]</td> 
   <td> <p>Selecteer het type onderzoek u de module wilt uitvoeren:</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Using SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Als u het eenvoudige zoektype hebt geselecteerd, kiest u het type [!DNL Salesforce] -record waarnaar u in de module wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Voer de query in waarop u wilt zoeken.</p> <p>Voor meer informatie over SOSL, zie <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm"> Taal van het Onderzoek van de Objecten van Salesforce (SOSL) </a> in de [!DNL Salesforce] documentatie.</p> <p>Voor meer informatie over SOQL, zie <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm"> Taal van de Vraag van de Vraag van de Objecten van Salesforce (SOQL) </a> in de [!DNL Salesforce] documentatie.</p> <p>Nota: Gelieve te merken op dat de waarde van de parameter <code>RETURNING </code> de output van de module beïnvloedt. Als u <code>LIMIT</code> gebruikt, negeert [!DNL Fusion] de instellingen in het veld [!UICONTROL Maximal count of records] . Als u geen limiet instelt, voegt Fusion de waarde [!UICONTROL LIMIT = Maximal count of records] in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search]

Deze actiemodule wint alle verslagen terug die aan een bepaalde criteria voldoen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het verbinden van uw [!DNL Salesforce] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL  Adobe Workfront Fusion] - Basisinstructies </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Selecteer het type object waarnaar u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Selecteer het veld waarnaar u wilt zoeken, de operator die u wilt gebruiken in de query en de waarde die u in het veld zoekt. U kunt vragen verbinden door EN of OF te gebruiken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u in de uitvoer van de module wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Selecteer of u de module Alle Overeenkomende Verslagen, of het Eerste Overeenkomende slechts Verslag wilt terugkeren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugwinnen.</td> 
  </tr> 
 </tbody> 
</table>
