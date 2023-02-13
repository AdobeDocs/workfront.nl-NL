---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Afbeeldingsmodules
description: Met de Adobe Workfront Fusion Image-modules kunt u informatie ophalen over een bepaalde afbeelding (afmetingen, type, enzovoort), een afbeelding omzetten in een andere bestandsindeling en de grootte van de afbeelding rechtstreeks wijzigen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Afbeeldingsmodules

[!DNL Adobe Workfront Fusion] [!UICONTROL Image] kunt u informatie ophalen over een bepaalde afbeelding (afmetingen, type, enzovoort), een afbeelding omzetten in een andere bestandsindeling en de grootte van de afbeelding rechtstreeks wijzigen.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Image] modules en hun velden

Als u deze module configureert, worden de volgende velden weergegeven. Een bolde titel in een module wijst op een vereist gebied.

* [[!UICONTROL Resize]](#resize)
* [[!UICONTROL Convert a format]](#convert-a-format)
* [[!UICONTROL Extract metadata]](#extract-metadata)

### [!UICONTROL Resize]

Deze transformatormodule wijzigt de hoogte en breedte van een afbeelding op basis van criteria die u opgeeft.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer de bron van de afbeelding die u wilt omzetten. U kunt uitvoer uit een vorige module selecteren of het gegevensbestand en de bestandsnaam toewijzen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Wijs het bestand toe dat u wilt converteren. Dit veld is beschikbaar als u [!UICONTROL Map] in de [!UICONTROL Source file] veld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Voer een naam in voor het omgezette bestand. Dit veld is beschikbaar als u [!UICONTROL Map] in de [!UICONTROL Source file] veld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to]</td> 
   <td>Selecteer of u de hoogte-breedteverhouding wilt behouden of de afmetingen wilt wijzigen in een opgegeven hoogte en breedte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL According to]</td> 
   <td> <p>Selecteer hoe de module de nieuwe grootte van de afbeelding moet bepalen. Dit veld wordt weergegeven als u de verhouding tussen hoogte en breedte in het veld I wilt behouden. Andere velden worden weergegeven op basis van de selectie in dit veld.</p> 
    <ul> 
     <li> <p>[!UICONTROL Maximum width]</p> <p>Hiermee verkleint u een afbeelding tot een door u opgegeven breedte. De hoogte wordt automatisch berekend.</p> </li> 
     <li> <p>[!UICONTROL Maximum height]</p> <p>Hiermee verkleint u een afbeelding tot een door u opgegeven hoogte. De breedte wordt automatisch berekend.</p> </li> 
     <li> <p>[!UICONTROL Maximum height or width]</p> <p>Hiermee verkleint u een afbeelding zodanig dat de hoogte en breedte ervan de opgegeven waarden niet overschrijden. Omdat bij deze optie de hoogte-breedteverhouding behouden blijft, kan een van de afmetingen kleiner zijn dan opgegeven. Als hoogte en breedte bijvoorbeeld beide zijn opgegeven als 40, wordt een afbeelding van 400 x 300 verkleind tot 40 x 30.</p> </li> 
     <li> <p>[!UICONTROL Minimum width]</p> <p>Hiermee vergroot u een afbeelding tot een door u opgegeven breedte. De hoogte wordt automatisch berekend.</p> </li> 
     <li> <p>[!UICONTROL Minimum height]</p> <p>Hiermee vergroot u een afbeelding tot een door u opgegeven hoogte. De breedte wordt automatisch berekend.</p> </li> 
     <li> <p>[!UICONTROL Minimum height or width]</p> <p>Hiermee vergroot u een afbeelding zodanig dat de hoogte en breedte niet kleiner zijn dan de waarden die u opgeeft. Omdat bij deze optie de hoogte-breedteverhouding behouden blijft, kan een van de afmetingen groter zijn dan opgegeven. Als hoogte en breedte bijvoorbeeld beide zijn opgegeven als 300, wordt een afbeelding van 40 x 30 vergroot tot 400 x 300.</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>Hiermee wijzigt u de afbeeldingsgrootte met een percentage op basis van de waarde die u opgeeft. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>Voer de gewenste breedte van de gewijzigde afbeelding in pixels in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>Voer de gewenste hoogte van de gewijzigde afbeelding in pixels in of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert a format]

Deze transformatormodule wijzigt de indeling van een afbeeldingsbestand. Deze module is compatibel met de volgende indelingen:

* PNG
* JPG
* GIF
* BMP

Zowel het bronbestand als de uitvoer moeten een van deze indelingen hebben. De [!UICONTROL Image] >[!UICONTROL Convert a format] kan een PNG-bestand omzetten in een BMP-bestand of een BMP-bestand in een JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer de bron van de afbeelding die u wilt omzetten. U kunt uitvoer uit een vorige module selecteren of het gegevensbestand en de bestandsnaam toewijzen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Wijs het bestand toe dat u wilt converteren. Dit veld is beschikbaar als u [!UICONTROL Map] in de [!UICONTROL Source file] veld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Voer een naam in voor het omgezette bestand. Dit veld is beschikbaar als u [!UICONTROL Map] in de [!UICONTROL Source file] veld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output format]</td> 
   <td>Selecteer de indeling waarin de module het bronbestand moet omzetten. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extract metadata]

Deze transformatormodule keert basisinformatie over een module terug.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer de bron van de afbeelding die u wilt omzetten. U kunt uitvoer uit een vorige module selecteren of het gegevensbestand en de bestandsnaam toewijzen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Wijs het bestand toe dat u wilt converteren. Dit veld is beschikbaar als u Kaart hebt geselecteerd in het dialoogvenster [!UICONTROL Source file] veld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Voer een naam in voor het omgezette bestand. Dit veld is beschikbaar als u Kaart hebt geselecteerd in het dialoogvenster [!UICONTROL Source file] veld.</td> 
  </tr> 
 </tbody> 
</table>

## Mogelijke problemen

### Handeling beëindigd met een fout

Er zijn drie gevallen waarin een handeling kan worden beëindigd met een fout:

* De ontvangen gegevens hebben niet de indeling JPG/GIF/PNG/BMP
* De maximale breedte/hoogte is overschreden bij het wijzigen van de afmetingen van de afbeelding. De afbeelding mag niet groter zijn dan 3840 px breedte en 2160 px hoogte
* De maximaal toegestane grootte van een afbeelding is overschreden tijdens het wijzigen van de afmetingen of de indeling van de afbeelding.
