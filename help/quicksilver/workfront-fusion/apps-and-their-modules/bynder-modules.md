---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Byndermodules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Bynder]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# [!DNL Bynder] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Bynder]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Te gebruiken [!DNL Bynder] modules, moet u een [!DNL Bynder] account.

## Verbinden [!DNL Bynder] naar Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Verbinding maken met [!DNL Bynder] van [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Een [!UICONTROL Client ID] en [!UICONTROL Client Secret] in [!DNL Bynder] (Optioneel)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Verbinding maken met [!DNL Bynder] van [!DNL Workfront Fusion]

U kunt een verbinding maken op basis van [!DNL Workfront Fusion] aan uw [!DNL Bynder] rechtstreeks vanuit een [!DNL Bynder] module.

1. In alle [!DNL Bynder] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Selecteer [!DNL Bynder] domein waarmee u verbinding wilt maken.
1. (Optioneel) Klik op **[!UICONTROL Advanced settings]** en voer vervolgens uw [!UICONTROL Client ID] en [!UICONTROL Client Secret].

   Voor instructies voor het genereren van de client-id en het clientgeheim raadpleegt u [Client-id en clientgeheim genereren in [!DNL Bynder] (Optioneel)](#generate-a-client-id-and-client-secret-in-bynder-optional) in dit artikel.

1. In de [!UICONTROL login] voert u uw gebruikersnaam (e-mailadres) en wachtwoord in.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

### Een [!UICONTROL Client ID] en [!UICONTROL Client Secret] in [!DNL Bynder] (Optioneel)

Als u een verbinding wilt tot stand brengen gebruikend identiteitskaart van de Cliënt en Geheim van de Cliënt, kunt u hen van uw produceren [!DNL Bynder] account. De client-id en het clientgeheim worden gegenereerd wanneer u een app maakt in [!DNL Bynder].

Voor instructies voor het maken van een app in [!DNL Bynder], zie [2.0-apps voor Oauth](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) in de [!DNL Bynder] documentatie.

>[!NOTE]
>
>Wanneer u de app maakt in [!DNL Bynder]Voer het volgende in als de `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] modules en hun velden

Wanneer u [!DNL Bynder] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Bynder] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handelingen](#actions)
* [Zoekopdrachten](#searches)
* [Triggers](#triggers)

### Handelingen

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Read asset metadata]](#read-asset-metadata)
* [[!UICONTROL Update asset metadata]](#update-asset-metadata)
* [[!UICONTROL Add assets to a collection]](#add-assets-to-a-collection)
* [[!UICONTROL Remove assets from collection]](#remove-assets-from-collection)
* [[!UICONTROL Add a tag to assets]](#add-a-tag-to-assets)
* [[!UICONTROL Remove a tag] uit activa](#remove-a-tag-from-assets)
* [[!UICONTROL Download asset]](#download-asset)
* [[!UICONTROL Upload asset]](#upload-asset)

#### [!UICONTROL Custom API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Bynder] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Bynder] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

De module keert een statuscode, samen met de kopballen en het lichaam van de API vraag terug.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Een pad invoeren ten opzichte van <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion voegt de machtigingsheaders voor u toe.</p> </td> 
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

#### [!UICONTROL Read asset metadata]

In deze actiemodule worden de metagegevens van een element gelezen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Voer de id in van het element waarvoor u metagegevens wilt ophalen of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update asset metadata]

In deze actiemodule worden de metagegevens van een bestaand element bijgewerkt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Voer de id in van het element waarvoor u metagegevens wilt bijwerken of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Selecteer de velden waarvoor u informatie wilt invoeren, en voer vervolgens de gegevens in of wijs de gegevens toe waarmee u de metagegevens wilt bijwerken naar die velden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>Selecteer de opties die u wilt bijwerken en voer de informatie in of wijs deze toe aan die eigenschappen. Metaeigenschappen zijn informatie over het element die geen specifieke velden in het element vertegenwoordigen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add assets to a collection]

Deze actiemodule voegt een of meer elementen toe aan een verzameling.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Ga of kaart identiteitskaart van de inzameling in waar u activa wilt toevoegen.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Voor elk element dat u aan de verzameling wilt toevoegen, klikt u op <strong>[!UICONTROL Add item]</strong>Voer vervolgens de element-id in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove assets from collection]

Deze actiemodule verwijdert een of meer elementen uit een verzameling.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Voer de id van de verzameling in of wijs deze toe op de plaats waar u elementen wilt verwijderen.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Voor elk element dat u uit de verzameling wilt verwijderen, klikt u op <strong>[!UICONTROL Add item]</strong>Voer vervolgens de element-id in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a tag to assets]

Een tag toevoegen aan een of meer elementen

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>Voer de id in van de tag die u aan elementen wilt toevoegen of wijs deze toe.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Voor elk element waarop u een tag wilt toepassen, klikt u op <strong>[!UICONTROL Add item]</strong>Voer vervolgens de element-id in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove a tag from assets]

Een tag verwijderen uit een of meer elementen

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>Voer de id in van de tag die u uit de elementen wilt verwijderen of wijs deze toe.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Voor elk element waarvan u een tag wilt verwijderen, klikt u op <strong>[!UICONTROL Add item]</strong>Voer vervolgens de element-id in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download asset]

Deze actiemodule downloadt één element.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Voer de id in van het element dat u wilt downloaden of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset version]</td> 
   <td> <p>Voer de versie in van het element dat u wilt downloaden of wijs deze versie toe. Laat het veld leeg als u de meest recente versie van het element wilt downloaden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload asset]

Deze actiemodule uploadt één element.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save as]</td> 
   <td> <p>Selecteer hoe u het bestand dat u uploadt wilt opslaan.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL New asset]</strong> </p> <p>Selecteer de velden en metaeigenschappen waarvoor u informatie wilt invoeren en voer de informatie in die velden in.</p> <p>Voer de id in van het merk dat u voor het geüploade element wilt gebruiken of wijs deze toe.</p> </li> 
     <li> <p><strong>[!UICONTROL New asset version]</strong> </p> <p>Voer de id in van het element waarvoor u een nieuwe versie uploadt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

* [[!UICONTROL List record]](#list-record)
* [[!UICONTROL Search for assets]](#search-for-assets)

#### [!UICONTROL List record]

Deze zoekmodule haalt alle items van een bepaald type op.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record dat u wilt weergeven.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Read all collections]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Read information about all tags]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Read all assets of a collection]</strong> </p> <p>Voer de id in van de verzameling waarvan u de elementen wilt weergeven of wijs deze toe.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer van de module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal activa in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search for assets]

Deze zoekmodule zoekt naar elementen op basis van criteria die u opgeeft.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteria]</td> 
   <td> <p>Voer de zoekcriteria in. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Selecteer het veld dat u in de zoekopdracht wilt gebruiken</p> </li> 
     <li> <p><strong>[!UICONTROL Logical Operator]</strong> </p> <p>Selecteer de operator die u in de zoekopdracht wilt gebruiken.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Voer de waarde in die u in het geselecteerde veld wilt zoeken of wijs deze toe. Het waardetype moet hetzelfde zijn als het gegevenstype van het geselecteerde veld. </p> <p>Voor meer informatie over gegevenstypen raadpleegt u <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Gegevenstypen item in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Selecteer of u het eerste overeenkomende element of alle overeenkomende elementen wilt retourneren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Selecteer het veld waarop u wilt sorteren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort Direction]</td> 
   <td> <p>Selecteer of u oplopend of aflopend wilt sorteren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer van de module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal activa in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Triggers

#### [!UICONTROL Watch assets]

Deze triggermodule start een scenario wanneer een element wordt gemaakt of bijgewerkt.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Bynder] account aan [!DNL Workfront Fusion], zie <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Collections]</td>
   <td> <p>Selecteer de verzameling die u wilt controleren voor nieuwe elementen. Als u alle verzamelingen wilt bekijken, laat u dit veld leeg.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Ga het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>
