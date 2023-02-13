---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive voor bedrijfsmodules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Microsoft OneDrive for Business]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Microsoft OneDrive for Business]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Te gebruiken [!DNL Microsoft OneDrive for Business] with [!DNL Adobe Workfront Fusion]hebt u een [!DNL Microsoft] account.

Voor instructies over het aansluiten van uw [!DNL OneDrive for Business] account aan [!DNL Workfront Fusion], zie [Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] modules en hun velden

Wanneer u [!DNL Microsoft OneDrive for Business] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Microsoft OneDrive for Business] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)

### Triggers

* [[!UICONTROL Watch files]](#watch-files)
* [[!UICONTROL Watch folders]](#watch-folders)

#### [!UICONTROL Watch files]

Deze triggermodule wordt geactiveerd wanneer een nieuw bestand wordt toegevoegd of bijgewerkt in een map die wordt gecontroleerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Selecteer het station dat u wilt controleren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> Selecteer de map die u wilt controleren. In een scenario kunt u slechts één map controleren.</p> <p>Tip: Als u meerdere mappen wilt bijhouden, maakt u een onafhankelijk scenario voor elk van deze mappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL I want to watch]</p> </td> 
   <td> <p>Selecteer of u nieuwe bestanden en alle wijzigingen wilt bekijken, of alleen nieuwe bestanden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned rows]</td> 
   <td> <p> Stel het maximale aantal resultaten in dat [!DNL Workfront Fusion] werkt met één cyclus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch folders]

Deze triggermodule wordt geactiveerd wanneer een nieuwe map wordt toegevoegd aan de map die wordt gecontroleerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Selecteer het station dat u wilt controleren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> Selecteer de map die u wilt controleren. In een scenario kunt u slechts één map controleren.</p> <p>Tip: Als u meerdere mappen wilt bijhouden, maakt u een onafhankelijk scenario voor elk van deze mappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL I want to watch]</p> </td> 
   <td> <p>Selecteer of u nieuwe mappen en alle wijzigingen wilt bekijken, of alleen nieuwe mappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned rows]</td> 
   <td> <p> Stel het maximale aantal resultaten in dat [!DNL Workfront Fusion] werkt met één cyclus.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Upload a file]](#upload-a-file)
* [[!UICONTROL Delete a file]](#delete-a-file)
* [[!UICONTROL Get a file]](#get-a-file)
* [[!UICONTROL Create a folder]](#create-a-folder)
* [[!UICONTROL Delete a folder]](#delete-a-folder)
* [[!UICONTROL Get a sharing link]](#get-a-sharing-link)

#### [!UICONTROL Upload a file]

Deze actiemodule uploadt een binair of tekstbestand naar een opgegeven map

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Selecteer het station waarnaar u een bestand wilt uploaden.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map in het station.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL If the file with the same name exists]</td> 
   <td> <p> Selecteer wat u wilt doen als een bestand met dezelfde naam als het bestand dat u probeert te uploaden al bestaat.</p> 
    <ul> 
     <li>[!UICONTROL Replace the existing file]</li> 
     <li>[!UICONTROL Rename the new file]</li> 
     <li>[!UICONTROL End with an error]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a file]

Met deze actiemodule wordt het opgegeven bestand naar de prullenbak verplaatst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Selecteer het station waaruit u een bestand wilt verwijderen.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Voer de id in van het bestand dat u wilt verwijderen. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a file]

Deze actiemodule haalt het bestand met de opgegeven id op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Selecteer het station waarvan u een bestand wilt ophalen.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Voer de id in van het bestand dat u wilt ophalen. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a folder]

Maakt een map in de opgegeven bovenliggende map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Drive ID]</strong> </td> 
   <td> <p>Selecteer het station waarop u een nieuwe map wilt maken.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder]</strong> </td> 
   <td> <p>Selecteer de map waarin u een nieuwe map wilt maken.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder name]</strong> </td> 
   <td>Voer een naam voor de nieuwe map in of wijs deze toe.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a folder]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Selecteer het station waaruit u een bestand wilt verwijderen.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td> <p>Voer de id in van de map die u wilt verwijderen of wijs deze toe. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a sharing link]

Deze module wint een verbinding terug die u kunt delen om toegang tot het gespecificeerde dossier te verlenen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Selecteer het station waarnaar u een bestand wilt uploaden.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>Selecteer of u een bestand wilt kiezen met de bestands-id of het bestandspad. Voer de bestands-id of het pad in het veld in dat wordt weergegeven.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permission type]</p> </td> 
   <td> <p>Selecteer of u wilt dat personen die de koppeling ontvangen, lees- en schrijfmachtigingen hebben of alleen-lezen.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope]</td> 
   <td> <p> Selecteer of u het bestand toegankelijk wilt maken voor iedereen die over de koppeling beschikt of alleen toegankelijk wilt zijn voor leden van uw organisatie.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
