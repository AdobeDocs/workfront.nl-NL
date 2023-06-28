---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: SharePoint-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die SharePoint gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2240'
ht-degree: 0%

---

# [!DNL SharePoint] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL SharePoint]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Te gebruiken [!DNL SharePoint] modules, moet u een [!DNL SharePoint] account.

## Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion] met een [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion] geavanceerde instellingen gebruiken](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion] met een [!DNL Microsoft] account

U kunt uw [!DNL Microsoft] account om verbinding te maken met [!DNL SharePoint]. Voor instructies over het aansluiten van uw [!DNL Sharepoint] account aan [!DNL Workfront Fusion], zie [Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion] geavanceerde instellingen gebruiken

Verbinding maken [!DNL SharePoint] tot [!DNL Workfront Fusion] zonder [!DNL Microsoft] account, hebt u een client-id, clientgeheim en huurnummer-id nodig.

1. Klikken **[!UICONTROL Add]** aan de bovenkant van de **[!DNL SharePoint]** om de **[!UICONTROL Create a connection]** doos.

1. (Optioneel) Wijzig de standaardinstelling **[!UICONTROL Connection name]**.
1. Klik op **[!UICONTROL Show advanced settings]**.
1. Voer de [!DNL SharePoint] **[!UICONTROL Client ID]** en **[!UICONTROL Client Secret]**.

1. Klik op **[!UICONTROL Continue]**.
1. Voer in het aanmeldingsvenster dat wordt weergegeven uw aanmeldingsgegevens in om u aan te melden bij de app als u dat nog niet hebt gedaan.
1. (Voorwaardelijk) Als een **[!UICONTROL Allow]** klikt u op de knop om de app te verbinden met [!DNL Workfront Fusion].

## [!DNL SharePoint] modules en hun velden

Wanneer u [!DNL SharePoint] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL SharePoint] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Drive-item](#drive-item)
* [Item](#item)
* [Lijst](#list)
* [Pagina (bèta)](#page-beta)
* [Site](#site)
* [Overige](#other)

### Drive-item

* [Een bestand maken](#create-a-file)
* [Een map maken](#create-a-folder)
* [Een bestand ophalen](#get-a-file)
* [Mapitems controleren](#watch-folder-items)

#### Wijzigingen ophalen

Deze module retourneert wijzigingen die zijn aangebracht in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Selecteer hoe u de locatie wilt identificeren van de map waarin u de wijzigingen wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Folder ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Selecteer de locatie waar u de wijzigingen wilt ophalen. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Een map maken

Deze actiemodule maakt een nieuwe map in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Selecteer hoe u de locatie wilt identificeren van de map die u wilt maken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Folder ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Selecteer de locatie waar u de map wilt maken. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder name]</td> 
   <td>Voer een naam voor de nieuwe map in of wijs deze toe.</td> 
  </tr>
  </tbody> 
</table>

#### Een bestand ophalen

Deze actiemodule haalt het opgegeven SharePoint-bestand op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Selecteer hoe u de locatie wilt identificeren van het bestand dat u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL File ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Selecteer de locatie van het bestand. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Mapitems controleren

Deze triggermodule start een scenario wanneer een item wordt bijgewerkt in een map die u selecteert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Selecteer hoe u de locatie wilt identificeren van het bestand dat u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL folder ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Selecteer de locatie van de map die u wilt controleren. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Voer het maximum aantal objecten in [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Item

* [[!UICONTROL Copy Item]](#copy-an-item)
* [[!UICONTROL Create an item]](#create-an-item)
* [[!UICONTROL Delete an item]](#delete-an-item)
* [[!UICONTROL Get an Item]](#get-an-item)
* [[!UICONTROL List Items]](#list-items)
* [[!UICONTROL Move Item]](#move-an-item)
* [[!UICONTROL Update an item]](#update-an-item)
* [[!UICONTROL Watch Items] (Gepland)](#watch-items-scheduled)


#### [!UICONTROL Copy Item]

Deze actiemodule kopieert een bestaand item in een SharePoint-lijst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Site-, station- en map-id's invoeren</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt kopiëren.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Item ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from list that you follow]</strong> </p> <p>Selecteer in het veld Itemtype of u een veld of een map verplaatst.  Selecteer de site die het item bevat dat u wilt kopiëren, selecteer vervolgens de lijst en selecteer vervolgens het item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination ID]</td> 
   <td> Voer de id in van de map waarnaar u het item wilt kopiëren of wijs deze toe. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td>Voer een naam in of wijs een naam toe aan de nieuwe kopie van het item. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create an item]

Deze actiemodule maakt een nieuw item in een SharePoint-lijst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Create an Item]</td> 
   <td> <p>Selecteer hoe u de site wilt identificeren en vermeld waar u een item wilt maken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong> en <strong>[!UICONTROL List ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die de lijst bevat waar u een item wilt maken en selecteer vervolgens de lijst. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Voer voor elk veld dat u voor het nieuwe item wilt instellen de sleutel van het veld in (geeft het veld aan) en de waarde die het nieuwe item voor dat veld moet hebben.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an item]

Met deze actiemodule verwijdert u een bestaand item uit een SharePoint-lijst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update an Item]</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt verwijderen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Item ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die het item bevat dat u wilt verwijderen, selecteer vervolgens de lijst en selecteer vervolgens het item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get an Item]

Deze actiemodule retourneert de gegevens van een opgegeven item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get an Item]</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Item ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site met de lijst waarvan u een item wilt ophalen, selecteer vervolgens de lijst en selecteer vervolgens het item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Items]

Deze actiemodule wint een lijst van alle punten in een gespecificeerde lijst terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List Items]</td> 
   <td> <p>Selecteer hoe u de lijst wilt identificeren waarvan u items wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong> en <strong>[!UICONTROL List ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site met de lijst waaruit u items wilt ophalen en selecteer vervolgens de lijst. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal punten in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move an Item]

Deze actiemodule kopieert een bestaand item in een SharePoint-lijst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Site-, station- en map-id's invoeren</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt verplaatsen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Item ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from list that you follow]</strong> </p> <p>Selecteer in het veld Itemtype of u een veld of een map verplaatst. Selecteer de site die het item bevat dat u wilt kopiëren, selecteer vervolgens de lijst en selecteer vervolgens het item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination ID]</td> 
   <td> Voer de id in van de map waarnaar u het item wilt verplaatsen of wijs deze toe. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td>Voer een naam in of wijs een naam toe aan het verplaatste item. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update an item]

Deze actiemodule werkt een bestaand item in een SharePoint-lijst bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update an Item]</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt bijwerken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>, en <strong>[!UICONTROL Item ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die het item bevat dat u wilt bijwerken, selecteer vervolgens de lijst en selecteer vervolgens het item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Voer voor elk veld dat u wilt bijwerken voor het nieuwe item de sleutel van het veld in (geeft het veld aan) en de nieuwe waarde die het item voor dat veld moet hebben.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Items] (Gepland)

Deze triggermodule start een scenario wanneer een item wordt gemaakt of gewijzigd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Lists]</td> 
   <td>Selecteer of u lijsten wilt volgen door aanmaaktijd (nieuwe items) of door wijzigingstijd (bijgewerkte items).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site and List ID]</td> 
   <td> <p>Selecteer hoe u de site wilt identificeren en welke lijst u wilt bekijken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong> en <strong>[!UICONTROL List ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Selecteer de site die u wilt controleren en selecteer vervolgens de lijst. Deze drop-down wint slechts volgende plaatsen terug.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal punten in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lijst

* [[!UICONTROL Create a List]](#create-a-list)
* [[!UICONTROL Get a List]](#get-a-list)
* [[!UICONTROL List Lists]](#list-lists)
* [[!UICONTROL Watch Lists]](#watch-lists)

#### [!UICONTROL Create a List]

Deze actiemodule maakt een nieuwe lijst in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a Site ID]</td> 
   <td> <p>Selecteer hoe u de site wilt identificeren en vermeld waar u een lijst wilt maken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong> waar u een lijst wilt maken.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site waarop u een lijst wilt maken. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display Name]</td> 
   <td>Voer een naam voor de nieuwe lijst in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Voer een beschrijving voor de nieuwe lijst in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Add Columns]</td> 
   <td>Voer voor elke kolom die u voor de nieuwe lijst wilt instellen een <strong>[!UICONTROL Name]</strong> voor het veld en selecteert u de <strong>[!UICONTROL Type]</strong> van waarde die de nieuwe kolom moet hebben.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a List]

Deze actiemodule retourneert de gegevens van een opgegeven lijst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a List]</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong> en <strong>Lijst-id</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die de lijst bevat die u wilt ophalen en selecteer vervolgens de lijst. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Lists]

Deze actiemodule wint een lijst van alle punten in een gespecificeerde lijst terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List Lists]</td> 
   <td> <p>Selecteer hoe u de site wilt identificeren waarvan u lijsten wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die de lijsten bevat die u wilt ophalen. In de vervolgkeuzelijst worden alleen de volgende sites opgehaald.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal lijsten in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Lists]

Deze triggermodule start een scenario wanneer een lijst wordt gemaakt of gewijzigd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Lists]</td> 
   <td>Selecteer of u lijsten wilt volgen door aanmaaktijd (nieuwe items) of door wijzigingstijd (bijgewerkte items).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site and List ID]</td> 
   <td> <p>Selecteer hoe u de site wilt identificeren en welke lijst u wilt bekijken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong> waar de lijst die u wilt controleren zich bevindt.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list that you follow]</strong> </p> <p>Selecteer de site die u wilt bekijken. Met de vervolgkeuzelijst haalt u alleen de volgende site op.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal lijsten in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pagina (bèta)

>[!NOTE]
>
>API&#39;s in de `beta` versie in [!DNL Microsoft Graph] kunnen worden gewijzigd. Het gebruik van deze API&#39;s in productietoepassingen wordt niet ondersteund.

#### [!UICONTROL Get a Page]

Deze actiemodule retourneert de gegevens van een opgegeven pagina.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a Page]</td> 
   <td> <p>Selecteer hoe u de pagina wilt identificeren die u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>en <strong>[!UICONTROL Page ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die de pagina bevat die u wilt ophalen en selecteer vervolgens de pagina.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL Get a Site]](#get-a-site)
* [[!UICONTROL Search Sites]](#search-sites)

#### [!UICONTROL Get a Site]

Deze actiemodule retourneert de gegevens van een opgegeven site.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a Site]</td> 
   <td> <p>Selecteer hoe u de pagina wilt identificeren die u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die u wilt ophalen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search Sites]

Deze actiemodule zoekt naar sites op basis van een parameter die u opgeeft.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword of Display Name]</td> 
   <td> <p>Voer de zoekterm in of wijs deze toe waarnaar u de sites wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal plaatsen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Overige

#### Wijzigingen ophalen

Deze module haalt toevoegingen, updates, en schrappingen terug die in de omslag van SharePoint worden gemaakt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site, Drive, and Folder IDs]</td> 
   <td> <p>Selecteer hoe u de site en de lijst wilt identificeren die het item bevatten dat u wilt bijwerken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Voer de <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL Drive ID]</strong>, en <strong>[!UICONTROL Folder ID]</strong> in de velden die worden weergegeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de site die het item bevat dat u wilt bijwerken, selecteer vervolgens het station en selecteer vervolgens de map. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> Het teken identificeert vanaf welk punt de module zou moeten beginnen met het terugwinnen van veranderingen.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

In deze module kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL SharePoint] account aan [!DNL Workfront Fusion], zie <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Een pad invoeren ten opzichte van <code>https://graph.microsoft.com</code>. Voorbeeld:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Selecteer het type gegevens dat u in uw API-aanroep wilt verzenden.</td> 
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

#### Gebeurtenissen van Let

Deze instant triggermodule start een scenario wanneer een item in SharePoint wordt toegevoegd, bijgewerkt of verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecteer een bestaande webhaak of klik op Toevoegen om een nieuwe webhaak te maken.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

