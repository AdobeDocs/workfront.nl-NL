---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: ServiceNow-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL ServiceNow]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 0%

---

# [!DNL ServiceNow] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL ServiceNow]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!DNL ServiceNow] modules, moet u een [!DNL ServiceNow] account.

## Verbinden [!DNL ServiceNow] tot [!DNL Workfront Fusion]

Als u een verbinding wilt maken voor uw [!DNL ServiceNow] modules:

1. Klikken **[!UICONTROL Add]** naast de [!UICONTROL Connection] vakje wanneer u begint vormend eerste [!DNL ServiceNow] module.
1. Voer het volgende in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Voer een naam in voor de nieuwe [!DNL ServiceNow] verbinding</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>Voer uw [!DNL ServiceNow] gebruikersnaam.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>Voer uw wachtwoord voor ServiceNow in.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p>Voer het adres in van uw [!DNL ServiceNow] account zonder <code>https://</code> (gewoonlijk <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] modules en hun velden

Wanneer u [!DNL ServiceNow] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL ServiceNow] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Als een aangepast record is geselecteerd in een &quot;[!UICONTROL Record type]&quot;, kan het enige tijd duren om de aangepaste velden te laden.
>
>Als er geen aangepaste records zijn, is de vervolgkeuzelijst leeg.

* [[!UICONTROL Watch records]](#watch-records)
* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Deactivate a User]](#deactivate-a-user)
* [[!UICONTROL Download an attachment]](#download-an-attachment)
* [[!UICONTROL Upload an attachment]](#upload-an-attachment)
* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Update a record]](#update-a-record)
* [[!UICONTROL Delete a record]](#delete-a-record)
* [[!UICONTROL Search for records]](#search-for-records)

### [!UICONTROL Watch records]

Deze triggermodule activeert een scenario wanneer een record wordt gemaakt of bijgewerkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Selecteer of de tabel die u wilt bekijken, een aangepaste tabel of een standaardtabel is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>Selecteer het type record dat u wilt bekijken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selecteer het type waarden dat u wilt weergeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt uitvoeren in de module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Selecteer of u nieuwe records of bijgewerkte records wilt bekijken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Custom API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL ServiceNow] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL ServiceNow] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>Typ het adres op de webserver waarmee de module moet communiceren.</p> <p>U kunt een relatieve URL typen, wat betekent dat u het protocol (zoals <code>http://</code>) aan het begin. Dit suggereert aan de Webserver dat de interactie op de server voorkomt.</p> <p>Bijvoorbeeld: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Read a record]

Deze actiemodule leest een [!DNL ServiceNow] opnemen met de systeem-id.

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL ServiceNow] Id van de record die de module moet lezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Selecteer of de record die u wilt lezen zich in een aangepaste tabel of in een standaardtabel bevindt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type van [!DNL ServiceNow] record dat de module moet lezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selecteer het type waarden dat u wilt weergeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt uitvoeren in de module.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Deactivate a User]

In deze actiemodule wordt een gebruiker gedeactiveerd in [!DNL ServiceNow] door de systeem-id te gebruiken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> De unieke sleutel invoeren of toewijzen [!DNL ServiceNow] Id van de gebruiker die de module moet deactiveren.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Download an attachment]

Deze actiemodule downloadt een bijlage in een [!DNL ServiceNow] opnemen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment System ID]</td> 
   <td> De unieke sleutel invoeren of toewijzen [!DNL ServiceNow] Id van de bijlage die u wilt downloaden.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Upload an attachment]

Deze actiemodule uploadt een bijlage naar een [!DNL ServiceNow] opnemen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table name]</td> 
   <td>Typ of wijs de naam van de tabel toe waar u de bijlage wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL ServiceNow] Id van het systeem waar u de bijlage wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Een naam voor de bijlage invoeren of toewijzen</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File content]</td> 
   <td>Voer het bestand in of wijs het toe waarnaar u wilt uploaden [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create a record]

Deze actiemodule maakt een nieuwe [!DNL ServiceNow] opnemen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Selecteer of u een record wilt maken in een aangepaste tabel of een standaardtabel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type van [!DNL ServiceNow] record die u met de module wilt maken. Vervolgens kunt u de beschikbare velden voor dit recordtype invullen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a record]

Deze actiemodule maakt een nieuwe [!DNL ServiceNow] opnemen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL ServiceNow] Id van de record die de module moet bijwerken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Selecteer of de record die u wilt bijwerken zich in een aangepaste tabel of een standaardtabel bevindt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type van [!DNL ServiceNow] record dat de module moet worden bijgewerkt. Vervolgens kunt u de beschikbare velden voor dit recordtype invullen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a record]

Met deze actiemodule verwijdert u een incident of een gebruiker.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer of u een incident of een gebruiker wilt schrappen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL ServiceNow] Id van de record die u wilt verwijderen uit de module.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search for records]

Deze module zoekt naar records aan de hand van criteria die u selecteert.

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het verbinden van uw account ServiceNow met [!DNL Workfront Fusion], zie <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Selecteer of de tabel die u wilt doorzoeken, een aangepaste tabel of een standaardtabel is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>Selecteer het type record waarnaar u wilt zoeken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Selecteer of u wilt dat de module alle records retourneert die aan de criteria voldoen, of alleen de eerste record die aan deze criteria voldoet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search type]</td> 
   <td> <p>Selecteer welk type zoekopdracht u wilt uitvoeren door de module</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Advanced query]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Query]</p> <p>Voer de aangepaste zoekquery in. Voor informatie over [!DNL ServiceNow] aangepaste zoekopdrachten, raadpleegt u de <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow-querydocumentatie</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Criteria]</p> <p>Voer de criteria in waarmee u de module wilt zoeken. Ga voor meer informatie over het instellen van zoekfilters naar <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Een filter toevoegen aan een scenario in Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Sort by]</p> <p>Geef aan op welk veld de module de resultaten moet sorteren en of ze oplopend of aflopend moeten worden gesorteerd.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selecteer het type waarden dat u wilt weergeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt uitvoeren in de module.</td> 
  </tr> 
 </tbody> 
</table>
