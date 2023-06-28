---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Team Drive-modules
description: De [!DNL Adobe Workfront Fusion Google Team Drive] met modules kunt u bestanden controleren, uploaden, bijwerken, kopiëren, verwijderen of ophalen en mappen maken in uw [!DNL Google Shared] Station.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# [!DNL Google Team Drive] modules

De [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] met modules kunt u bestanden controleren, uploaden, bijwerken, kopiëren, verwijderen of ophalen en mappen maken in uw [!DNL Google Shared Drive].

Voor gebruik [!DNL Google Team Drive] with [!DNL Adobe Workfront Fusion], is het noodzakelijk [!DNL G Suite] account. Als u er geen hebt, kunt u een [!DNL G Suite] rekening bij [[!DNL G Suite] site aanmelden](https://gsuite.google.com/signup/businessstarter/welcome).

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Google Team Drive]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Te gebruiken [!DNL Google Team Drive] modules, moet u een [!DNL Google Team Drive].

## [!DNL Google Team Drive] modules en hun velden

Wanneer u [!DNL Google Team Drive] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Google Team Drive] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

De velden in het dialoogvenster van de module die worden weergegeven in **vet** (in de [!DNL Workfront Fusion] scenario, **niet** in dit documentatieartikel) zijn verplicht.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Watch Files]

Retourneert de bestandsgegevens wanneer een nieuw bestand wordt toegevoegd en/of gewijzigd in de opgegeven map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecteer het gedeelde station dat u wilt controleren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map in het gedeelde station.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL What files to watch]</td> 
   <td> <p> Selecteer het type bestanden dat u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] bestanden om op te maken] </td> 
   <td> <p>Selecteer de notatie die u voor de controle wilt gebruiken [!DNL Google Documents] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Sheets] bestanden om op te maken] </td> 
   <td> <p>Selecteer de notatie die u voor de controle wilt gebruiken [!DNL Google Sheets] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] bestanden om op te maken] </td> 
   <td> <p>Selecteer de notatie die u voor de controle wilt gebruiken [!DNL Google Slides] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] bestanden om op te maken] </td> 
   <td> <p>Selecteer de notatie die u voor de controle wilt gebruiken [!DNL Google Drawings] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Selecteer of u de map wilt controleren op nieuwe en gewijzigde bestanden of alleen op nieuwe bestanden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of downloaded files]</td> 
   <td> <p> Het maximum aantal bestanden instellen [!DNL Workfront Fusion] wordt tijdens één uitvoeringscyclus geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Upload a File]](#upload-a-file)
* [[!UICONTROL Update a File]](#update-a-file)
* [[!UICONTROL Copy a File]](#copy-a-file)
* [[!UICONTROL Delete a File]](#delete-a-file)
* [[!UICONTROL Move a File to Trash]](#move-a-file-to-trash)
* [[!UICONTROL Get a File]](#get-a-file)
* [[!UICONTROL Get a File List]](#get-a-file-list)
* [[!UICONTROL Create a Folder]](#create-a-folder)

#### [!UICONTROL Upload a File]

Uploadt een bestand naar het opgegeven gedeelde station.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>Selecteer het gedeelde station waarnaar u een bestand wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map in het gedeelde station.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Geef het bestand op dat u naar het gedeelde station wilt uploaden.</p> <p>Wijs het bestand toe dat u uit de vorige module wilt uploaden (bijvoorbeeld [!UICONTROL HTTP] &gt;[!UICONTROL Get a File] of [!UICONTROL Dropbox] &gt;[!UICONTROL Get a file)]of voer de bestandsnaam en de bestandsgegevens handmatig in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> Voer de titel in van het bestand dat in de gedeelde map wordt weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert a File]</td> 
   <td> <p> Schakel deze optie in om het bestand om te zetten in de corresponderende Google-indeling in uw gedeelde map.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a File]

Hiermee kunt u de bestandsnaam en/of bestandsinhoud wijzigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecteer het gedeelde station dat het bestand bevat dat u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map in het gedeelde station.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Voer de id in van het bestand dat u wilt bijwerken (kaart).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Voer de nieuwe titel in voor het bijgewerkte bestand.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert a File]</td> 
   <td> <p> Schakel deze optie in om het bestand om te zetten in de corresponderende [!DNL Google] in uw gedeelde map.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy a File]

Hiermee wordt een opgegeven bestand naar de geselecteerde map gekopieerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecteer het gedeelde station dat het bestand bevat dat u wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de doelmap waarnaar u het bestand wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Voer (kaart) de id in van het bestand dat u wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL The name of the copy file]</p> </td> 
   <td> <p>Voer de nieuwe bestandsnaam in als u deze wilt wijzigen op de doellocatie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a File]

Hiermee wordt een opgegeven bestand verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Voer de id in van het bestand dat u wilt verwijderen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File to Trash]

Hiermee wordt een opgegeven bestand naar de prullenbak verplaatst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Voer de id in van het bestand dat u naar de prullenbak wilt verplaatsen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a File]

Hiermee worden gegevens over het opgegeven bestand opgehaald.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] bestanden om op te maken] </td> 
   <td> <p>Selecteer de gewenste indeling voor de [!DNL Google Documents] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Sheets] bestanden om op te maken] </td> 
   <td> <p>Selecteer de gewenste indeling voor de [!DNL Google Sheets] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] bestanden om op te maken] </td> 
   <td> <p>Selecteer de gewenste indeling voor de [!DNL Google Slides] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] bestanden om op te maken] </td> 
   <td> <p>Selecteer de gewenste indeling voor de [!DNL Google Drawings] bestanden geconverteerd naar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Voer de id in of wijs deze toe aan het bestand dat u wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a File List]

Hiermee haalt u op basis van de zoekterm de gegevens van de bestanden en/of mappen op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecteer het gedeelde station waarvan u bestanden wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map waaruit u bestanden wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Selecteer het type zoekopdracht dat u wilt uitvoeren (zie hieronder).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Query]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Search within file names]</p> <p style="font-weight: normal;">Voer de bestandsnaam (inclusief de bestandsextensie) in wanneer de [!UICONTROL Search for exact term Search] is geselecteerd of voert u het deel van de naam in wanneer de [!UICONTROL Search for names containing the searched term] is geselecteerd.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Fulltext search]</p> <p>Voer de zoekterm in om de bestandsnamen, beschrijvingen en inhoud te doorzoeken.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Custom search query]</p> <p>Voer de [!DNL Google] zoekquery term. Zie voor meer informatie [!DNL Google]s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Documentatie voor zoekopdrachten</a>. Voorbeeld: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td>Selecteer of u bestanden, mappen of beide wilt ophalen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td> <p> Het maximum aantal bestanden of mappen instellen [!DNL Workfront Fusion] wordt tijdens één uitvoeringscyclus geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Folder]

Hiermee maakt u een nieuwe map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Team Drive] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selecteer het gedeelde station waar u een map wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map waarin u een map wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL The name of the new folder]</td> 
   <td> <p> Voer de naam van de nieuwe map in.</p> </td> 
  </tr> 
 </tbody> 
</table>
