---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Maestro-modules
description: Met de [!DNL Adobe Maestro] modules, kunt u beginnen [!DNL Adobe Workfront Fusion] scenario gebaseerd op gebeurtenissen in uw [!DNL Adobe] Maestro-account, overeenkomsten en andere records maken, lezen of bijwerken, naar records zoeken aan de hand van criteria die u instelt en documenten uploaden.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# [!DNL Adobe Maestro] modules

Met de [!DNL Adobe Maestro] -modules kunt u een scenario activeren wanneer gebeurtenissen in Maestro optreden. U kunt ook records maken, lezen, bijwerken en verwijderen of een aangepaste API-aanroep naar uw [!DNL Adobe Maestro] account.

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
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinding maken met [!DNL Adobe Maestro]

U kunt een verbinding maken met uw [!DNL Maestro] rechtstreeks vanuit een [!DNL Workfront Fusion] -module.

1. In alle [!DNL Maestro] app-module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] doos.
1. Voer een naam in voor deze verbinding.
1. Selecteer of u met een productiemilieu, of een niet productiemilieu wilt verbinden.
1. Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.
1. Klikken **[!UICONTROL SAML log in]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Adobe Maestro] modules en hun velden

### Gebeurtenissen bekijken

Deze triggermodule start een scenario wanneer een record, recordtype of werkruimte wordt gemaakt, bijgewerkt of verwijderd in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Selecteer de webhaak die u wilt gebruiken of klik op Toevoegen om een nieuwe te maken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>Selecteer of u records, recordtypen of werkruimten wilt bekijken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objects to watch]</td>
      <td>Selecteer of u op nieuw wilt letten. bijgewerkte, nieuwe en bijgewerkte of verwijderde records.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Exclude updates made by this connection]</p>
      </td>
      <td>Schakel deze optie in om te voorkomen dat het scenario wordt geactiveerd wanneer een wijziging wordt aangebracht door de verbinding die door deze module wordt gebruikt. Hierdoor wordt voorkomen dat een andere instantie van het scenario wordt geactiveerd wanneer dit scenario een activerende actie uitvoert.</td> 
      </tr>
  </tbody>
</table>

### Een recordtype verwijderen

Deze actiemodule schrapt één enkel verslagtype in Maestro door zijn identiteitskaart

>[!WARNING]
>
>Als u een recordtype in Maestro verwijdert, worden ook alle records in de tabel met recordtypen verwijderd.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Voer de id in van het veld dat u wilt verwijderen of wijs deze toe.</td> 
      </tr>
  </tbody>
</table>

### Een aangepaste API-aanroep maken

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Voer een pad in dat is gebaseerd op https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
      </td>
      <td>
        <p>Selecteer de gewenste API-versie. Als u geen versie selecteert, wordt standaard de meest recente versie gebruikt.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API Path override]</p>
      </td>
      <td>
        <p>Voer een pad in dat is gebaseerd op https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Voor elk sleutel/waardepaar dat u aan het vraagkoord wilt toevoegen, klik <b>Item toevoegen</b> en voert u de sleutel en waarde in.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Een record maken

Met deze handeling maakt u één record in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Voer het type record in dat u wilt maken of wijs dit toe. Beschikbare recordtypen zijn gebaseerd op uw Maestro-account.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Overige velden</p>
      </td>
      <td>Deze velden zijn gebaseerd op het geselecteerde recordtype.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Een record verwijderen

Deze actiemodule verwijdert de opgegeven record in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Voer de id in van de record die u wilt verwijderen of wijs deze toe.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Een record ophalen

Deze actiemodule haalt één record op uit [!DNL Adobe Maestro], opgegeven door de id ervan.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Voer de id in of wijs deze toe aan de record die u wilt ophalen.</td>
    </tr>
  </tbody>
</table>

### Records ophalen op recordtype

Deze actiemodule wint alle verslagen van het gespecificeerde type terug.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Selecteer of wijs de werkruimte toe die de verslagen bevat u wilt terugwinnen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Selecteer het type record dat u wilt ophalen.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td> 
  </tbody>
</table>

### Recordtypen ophalen

Deze actiemodule wint een lijst van verslagtypes in terug [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
  </tbody>
</table>

### Record bijwerken

Deze handeling werkt één record bij in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Maestro], zie <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Verbinding maken met [!DNL Adobe Maestro]</a> in dit artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Typ of wijs het type record toe dat u wilt bijwerken. Beschikbare recordtypen zijn gebaseerd op uw Maestro-account.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Overige velden</p>
      </td>
      <td>Deze velden zijn gebaseerd op het geselecteerde recordtype.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Zoeken in records

Deze actiemodule wint een lijst van verslagen terug die op criteria worden gebaseerd u specificeert.

>[!NOTE]
>
>Deze module is in aanbouw.

