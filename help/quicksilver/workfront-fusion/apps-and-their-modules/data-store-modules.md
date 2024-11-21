---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules voor gegevensopslag
description: Een  [!DNL Adobe Workfront Fusion]  gegevensopslag, gelijkend op een gegevensbestand of een eenvoudige lijst, kan gegevens van scenario's opslaan, makend het mogelijk om gegevens tussen individuele scenario's of scenario looppas over te brengen. U kunt een gegevensopslag gebruiken om nieuwe gegevens van diverse systemen tijdens synchronisatie op te slaan.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# [!UICONTROL Data store] modules

Een [!DNL Adobe Workfront Fusion] gegevensopslag, gelijkend op een gegevensbestand of een eenvoudige lijst, kan gegevens van scenario&#39;s opslaan, die het mogelijk maken om gegevens tussen individuele scenario&#39;s of scenario looppas over te brengen. U kunt een gegevensopslag gebruiken om nieuwe gegevens van diverse systemen tijdens synchronisatie op te slaan.

Met de gegevensopslagmodules kunt u records toevoegen, vervangen, bijwerken, ophalen, verwijderen, zoeken of tellen in de [!DNL Adobe Workfront Fusion] -gegevensopslag.

Voor informatie bij het creëren van, het uitgeven van, en het oplossen van problemengegevensopslag, zie [ Opslag van Gegevens in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Ga voor een video-introductie over gegevensopslag in Workfront Fusion naar:

* [ de Opslag van Gegevens ](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
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

Als u [!UICONTROL Data Store] -modules wilt gebruiken, moet u eerst een gegevensopslag maken.

Voor informatie bij het creëren van gegevensopslag, zie [ de Opslag van Gegevens in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Data Store] modules en hun velden

Wanneer u de modules van de Opslag van Gegevens vormt, [!DNL Workfront Fusion] toont de hieronder vermelde gebieden. Naast deze opties worden mogelijk extra gegevensopslagvelden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Alle [!UICONTROL Data Store] -modules zijn ActionScript-modules.

* [Een record toevoegen/vervangen](#addreplace-a-record)
* [Een record bijwerken](#update-a-record)
* [Een record ophalen](#get-a-record)
* [Controleren of een record bestaat](#check-the-existence-of-a-record)
* [Een record verwijderen](#delete-a-record)
* [Alle records verwijderen](#delete-all-records)
* [Zoeken in records](#search-records)
* [Telrecords](#count-records)

### [!UICONTROL Add/Replace a Record]

Met deze actiemodule kunt u een record toevoegen of vervangen.

U geeft de gegevensopslag en de sleutel van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

>[!NOTE]
>
>De module genereert een fout wanneer u de record probeert toe te voegen die zich al onder dezelfde naam in de gegevensopslag bevindt en de optie [!UICONTROL Overwrite an existing record] is uitgeschakeld.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecteer of voeg de gegevensopslag toe waar u een verslag wilt creëren. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Voer de unieke sleutel in van de record die de module moet toevoegen of vervangen. De sleutel kan later worden gebruikt om het verslag terug te winnen. Als u dit veld leeg laat, wordt automatisch een sleutel gegenereerd.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing record] </td> 
   <td> <p>Schakel deze optie in om de record te overschrijven. De record die u wilt overschrijven, moet worden opgegeven in het veld Sleutel hierboven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>Voer de gewenste waarden in voor de velden van de record.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a Record]

Deze actiemodule werkt een record bij.

U geeft de gegevensopslag en de sleutel van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecteer of voeg de gegevensopslag toe waar u een verslag wilt creëren. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Voer de unieke sleutel in van de record die de module moet bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert missing record] </td> 
   <td> <p>Schakel deze optie in om een nieuwe record te maken als de record met de opgegeven sleutel nog niet bestaat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> Voer de gewenste waarden in voor de velden van de record die u wilt bijwerken.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a Record]

Deze actiemodule haalt een record op.

U geeft de gegevensopslag en de sleutel van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecteer de gegevensopslagruimte waarvan u een record wilt ophalen</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Voer de unieke sleutel in van de record die de module moet ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Check the Existence of a Record]

In deze actiemodule wordt opgegeven of een bepaalde record bestaat.

U geeft de gegevensopslag en de sleutel van de record op.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecteer de gegevensopslagruimte die u wilt controleren op het bestaan van de record.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Voer de unieke sleutel in van de record die de module moet controleren op het bestaan.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a Record]

Met deze actiemodule verwijdert u een record.

U geeft de gegevensopslag en de sleutel van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecteer de gegevensopslagruimte die u wilt controleren op het bestaan van de record.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Voer de unieke sleutel in van de record die de module moet verwijderen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete All Records]

Deze actiemodule schrapt alle verslagen van een bepaalde gegevensopslag.

U geeft de gegevensopslag op.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecteer de gegevensopslagruimte waaruit u alle records wilt verwijderen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search Records]

Deze zoekmodule zoekt naar records in een object in de gegevensopslag dat overeenkomt met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecteer de gegevensopslagruimte die u wilt doorzoeken.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Stel het filter voor de zoekopdracht in.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">Vul voor elk veld waarop u wilt sorteren de volgende velden in:</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Selecteer de kolomnaam waarop u de resultaten wilt sorteren.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Selecteer of u de resultaten in oplopende of aflopende volgorde wilt sorteren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Stel het maximale aantal zoekresultaten in dat [!DNL Workfront Fusion] retourneert tijdens één uitvoeringscyclus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p> Indien toegelaten, de route die deze module deel van verdere verwerking uitmaakt zelfs als deze module geen resultaten terugkeert.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Count Records]

Deze actiemodule nummert de verslagen in een gegevensopslag.

U geeft de gegevensopslag op.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecteer de gegevensopslagruimte die de records bevat die u wilt tellen.</p> </td> 
  </tr> 
 </tbody> 
</table>
