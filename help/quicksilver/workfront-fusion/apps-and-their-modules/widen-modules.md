---
title: Breidingsmodules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!UICONTROL Widen]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 1%

---

# [!DNL Widen] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!UICONTROL Widen]en deze verbinding maken met meerdere toepassingen en services van derden.

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
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!UICONTROL Widen] modules, moet u een [!UICONTROL Widen] account.

## Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

U kunt een verbinding maken met uw [!DNL Widen] rechtstreeks vanuit een [!DNL Widen] module.

1. In alle [!DNL Widen] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Selecteer [!DNL Widen] domein waarmee u verbinding wilt maken.
1. Voer het token voor uw [!DNL Widen] account. Zie voor instructies over het zoeken naar deze token de [[!DNL Widen] API Veelgestelde vragen](https://community.widen.com/collective/s/article/API-FAQs).
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Widen] modules en hun velden

Wanneer u [!DNL Widen] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Widen] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggermodules](#trigger-modules)
* [Modules voor handelingen](#action-modules)
* [Zoekmodules](#search-modules)

### Triggermodules

#### [!UICONTROL Watch assets]

Deze triggermodule start een scenario wanneer een element wordt gemaakt of bijgewerkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p>Selecteer of u nieuwe elementen of bijgewerkte elementen wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Selecteer de eigenschappen die u in de moduleuitvoer naast de activagebieden wilt omvatten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt opnemen in de uitvoer van de module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal activa in u de module wilt werken met tijdens elke cyclus van de scenariouitvoering.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules voor handelingen

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Read asset info]](#read-asset-info)
* [[!UICONTROL Add assets to collections]](#add-assets-to-collections)
* [[!UICONTROL Remove assets from collection]](#remove-assets-from-collection)
* [[!UICONTROL Update asset metadata]](#update-asset-metadata)
* [[!UICONTROL Download File]](#download-file)
* [[!UICONTROL Upload] een bestand](#upload-a-file)

#### [!UICONTROL Custom API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Widen] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Widen] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Selecteer of u de recentste versie van wilt gebruiken [!DNL Widen] API, of versie 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ga of kaart URL voor uw API vraag in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
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

#### [!UICONTROL Read asset info]

Deze actiemodule wint een individueel middel door zijn unieke identiteitskaart terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Voer de id in van het element waarvoor u informatie wilt lezen of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Selecteer de eigenschappen die u in de moduleuitvoer naast de activagebieden wilt omvatten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt opnemen in de uitvoer van de module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add assets to collections]

Deze actiemodule voegt een of meer elementen toe aan verzamelingen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>Voor elke verzameling waaraan u de elementen wilt toevoegen:</p> 
    <ol> 
     <li value="1"> <p> Klik op <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Voer de [!UICONTROL Collection ID].</p> </li> 
     <li value="3"> <p>Klik op <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>Voor elk element dat u aan een verzameling wilt toevoegen:</p> 
    <ol> 
     <li value="1"> <p> Klik op <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Voer de id van het element in of wijs deze toe.</p> </li> 
     <li value="3"> <p>Klik op <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal activa in u de module wilt werken met tijdens elke cyclus van de scenariouitvoering.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove assets from collection]

Deze actiemodule verwijdert een of meer elementen uit verzamelingen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>Voor elke verzameling waarvan u de elementen wilt verwijderen:</p> 
    <ol> 
     <li value="1"> <p> Klik op <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Ga of kaart identiteitskaart van de Inzameling in.</p> </li> 
     <li value="3"> <p>Klik op <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Element-id</td> 
   <td> <p>Voor elk element dat u uit een verzameling wilt verwijderen:</p> 
    <ol> 
     <li value="1"> <p> Klik op <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Voer de id van het element in of wijs deze toe.</p> </li> 
     <li value="3"> <p>Klik op <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal activa in u de module wilt werken met tijdens elke cyclus van de scenariouitvoering.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update asset metadata]

In deze actiemodule worden de metagegevensvelden van een element bijgewerkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Voer de id van het element in of wijs deze toe aan de locatie waar u de metagegevens wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata type]</td> 
   <td> <p>Selecteer het type metagegevens voor de metagegevens die u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Selecteer de metagegevensvelden die u wilt bijwerken. Voer voor elk veld de nieuwe waarde voor het veld in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal activa in u de module wilt werken met tijdens elke cyclus van de scenariouitvoering.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download File]

Deze actiemodule downloadt een middel uit uw [!DNL Widen] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Voer de id in van het element dat u wilt downloaden of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a file]

Deze actiemodule uploadt een bestand naar uw [!DNL Widen] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Profile]</td> 
   <td> <p>Selecteer het uploadprofiel dat de module moet gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>Selecteer hoe u het bestand wilt uploaden.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>Selecteer of wijs het brondossier van een vorige module toe.</p> </li> 
     <li> <p><strong>[!UICONTROL By URL]</strong> </p> <p>Voer de URL in van het bestand dat u wilt uploaden of wijs deze toe.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Voer een naam voor het geüploade bestand in of wijs een naam toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata Type]</td> 
   <td>Selecteer het type metagegevens voor het bestand dat u wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Selecteer de metagegevensvelden die u wilt opnemen in de bestandsupload. Voer voor elk veld de [!UICONTROL value] voor het veld.</td> 
  </tr> 
 </tbody> 
</table>

### Zoekmodules

* [[!UICONTROL Read collection assets]](#read-collection-assets)
* [[!UICONTROL Search assets]](#search-assets)

#### [!UICONTROL Read collection assets]

Deze actiemodule wint een lijst van activa binnen een inzameling terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Voer de id in van de verzameling die de elementen bevat die u wilt lezen of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Voer het nummer in of wijs het nummer toe van het eerste item dat u wilt aanbieden. Dit is een manier om de records te pagineren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>Selecteer de eigenschap waarmee u de elementen wilt sorteren. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Selecteer of u elementen in oplopende of aflopende volgorde wilt sorteren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt opnemen in de uitvoer van de module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search assets]

Deze zoekmodule haalt een lijst op met elementen die voldoen aan de specifieke zoekcriteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Widen] account aan [!DNL Workfront Fusion], zie <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search query]</td> 
   <td> <p>Voer de criteria in waarmee u elementen wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>Selecteer hoe u de elementen wilt sorteren. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Selecteer of u elementen in oplopende of aflopende volgorde wilt sorteren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include deleted]</td> 
   <td>Schakel deze optie in om verwijderde elementen op te nemen in de zoekopdracht.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>Schakel deze optie in om gearchiveerde elementen op te nemen in de zoekopdracht.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search document text]</td> 
   <td>Schakel deze optie in om documenttekst in de zoekopdracht op te nemen, of false om alleen elementen op te nemen waarvoor de titel overeenkomt met de zoekcriteria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Ga of kaart het aantal van het eerste punt in u details voor wilt terugwinnen. Dit is een manier om de records te pagineren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>Schakel deze optie in als u schuiven wilt toestaan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Selecteer de eigenschappen die u in de moduleuitvoer naast de activagebieden wilt omvatten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de velden die u wilt opnemen in de uitvoer van de module.</td> 
  </tr> 
 </tbody> 
</table>
