---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Geavanceerde fout behandeling in  [!DNL Adobe]  de Fusie van Workfront
description: Geavanceerde technieken voor foutafhandeling zijn onder andere filteren en nesten.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# Geavanceerde foutafhandeling in [!DNL Adobe Workfront Fusion]

Geavanceerde technieken voor foutafhandeling zijn onder andere filteren en nesten.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Filteren

Er zijn twee soorten het filtreren die op een route van de foutenmanager kunnen plaatsvinden.

* [Een filter toevoegen aan de fouthandlerroute](#adding-a-filter-to-the-error-handler-route)
* [Het toevoegen van een Router die door filters aan de route van de foutenmanager wordt gevolgd](#adding-a-router-followed-by-filters-to-the-error-handler)

### Een filter toevoegen aan de fouthandlerroute

U kunt een filter gebruiken om te controleren welke fouten door de route van de foutenmanager worden behandeld. Op deze manier kunt u alleen bepaalde soorten fouten verwerken. Als een fout niet door de filter overgaat, zal het worden behandeld alsof er geen die route van de foutenmanager voor de bepaalde module wordt bepaald is.

>[!INFO]
>
>**Voorbeeld:**
>
>![](assets/filter-error-handling-350x238.png)

### Een [!UICONTROL Router] , gevolgd door filters, toevoegen aan de fouthandler

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>In dit voorbeeld vindt de fout plaats in de module [!UICONTROL Create a folder] (A), die een reguliere route en een fouthandlerroute heeft. Het laatste wordt gevolgd door een router met één route die een filter heeft dat een specifiek type van fout (de Fout van Gegevens neemt) bepaalt, en andere die de standaardroute voor alle andere fouten is. De eerste route beëindigt met de [!UICONTROL Resume] richtlijn die vervangingswaarden voor het scenario bevat om van module A ([!UICONTROL Create a folder]) te hervatten, terwijl de tweede route met de [!UICONTROL Rollback] richtlijn beëindigt die de uitvoering van het scenario onmiddellijk tegenhoudt.

Zie [ verwerking van de Fout in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) voor verdere informatie over diverse foutentypes en over hoe [!DNL Workfront Fusion] hen verwerkt en evalueert.

### Het voorbeeldscenario

U kunt deze voorbeeldscène instellen om te begrijpen hoe deze filters werken voor foutafhandeling.

Een bestaande [!DNL Dropbox] -map gebruiken om een bestand te uploaden in plaats van een nieuw bestand te maken

Als u de module [!UICONTROL Create a folder] in [!DNL Dropbox] gebruikt en er al een map met dezelfde naam bestaat, genereert de module een gegevensfout zoals hieronder wordt weergegeven:

![](assets/dropbox-350x276.png)

Het volledige scenario:

![](assets/dropbox-scenario-350x190.png)

1. De module [!UICONTROL Tools] > [!UICONTROL Set Variable] bevat de mapnaam
1. De module [!UICONTROL HTTP] > [!UICONTROL Get a file] haalt het bestand dat naar de map moet worden geüpload
1. De module [!UICONTROL Dropbox] > [!UICONTROL Create a folder] meldt een fout als er al een map met dezelfde naam bestaat als de map die in de module is toegewezen
1. De route van de foutenmanager (transparante bellen) bevat een router om de fouten te filtreren
1. De eerste route is voor een gespecificeerd type van fout genoemd de Fout van Gegevens zoals wij reeds van het kennen:

   1. Als er een gegevensfout optreedt en de foutdetails door het filter worden doorgegeven, worden in [!UICONTROL Dropbox] > [!UICONTROL List all files/subfolders in a folder module] alle mappen in [!DNL Dropbox] weergegeven
   1. Het volgende filter komt overeen met de mapnamen
   1. De instructie [!UICONTROL Resume] geeft de map-id en het mappad van de bestaande map op en de uitvoering van het scenario wordt hervat vanuit de module [!UICONTROL Dropbox] > [!UICONTROL Create a folder] . In plaats van te proberen een nieuwe map te maken, gebruikt deze keer de waarden van de instructie [!UICONTROL Resume] om naar de volgende module te gaan en het bestand te uploaden in de bestaande map

1. De tweede route is voor alle andere fouten en eindigt met de instructie [!UICONTROL Rollback] die ertoe leidt dat het scenario onmiddellijk wordt gestopt

Hieronder volgt een gedetailleerde uitleg van de vijfde verklaring:

Om de bestaande omslag in uw verdere modules ([!UICONTROL Upload a file] hieronder) te gebruiken, moet u een route van de foutenmanager aan de module toevoegen en de omslagweg halen die in de [!UICONTROL Resume] richtlijnmodule moet worden in kaart gebracht die volgt:

![](assets/add-error-handler-route-350x113.png)

Het filter op de eerste route wordt geplaatst om de bepaalde fout (de Fout van Gegevens) slechts te behandelen die verschijnt wanneer een omslag met de zelfde naam reeds bestaat:

![](assets/condition-350x327.png)

De module [!UICONTROL Dropbox] > [!UICONTROL List all files in a folder] is geconfigureerd om alle mappen in de doelmap te retourneren. Het volgende filter geeft alleen het filter door dat we oorspronkelijk probeerden te maken (de mapnaam wordt opgeslagen in de 33. Mapnaam (item):

![](assets/condition2-350x193.png)

Uiteindelijk levert de aanwijzing [!UICONTROL Resume] het pad Map als uitvoer voor de mislukte module. Merk op dat identiteitskaart van de Omslag leeg is verlaten aangezien het niet door de &quot;[!UICONTROL Upload a file]&quot;module nodig is:

![](assets/flow-control-350x190.png)

## Nesten

Ongeacht waar een module wordt gevestigd, kunnen de routes van de foutenmanager op alle modules, behalve routers worden gecreeerd en worden uitgevoerd. Zo is het mogelijk om een route van de foutenmanager voor een module tot stand te brengen die reeds deel van een bestaande die route van de foutenmanager voor een andere module wordt gecreeerd.

Hier is een voorbeeld van een genestelde route van de foutenmanager:

![](assets/nested-error-handling-route-350x174.png)

In dit scenario, wordt de tweede route van de foutenmanager genest onder de eerste route van de foutenmanager. Dus als [!UICONTROL Dropbox] > [!UICONTROL Create a folder module] een fout ontmoet, beweegt de uitvoering zich aan Route 1, als het [!UICONTROL Data Error Takes Place] filter wordt overgegaan, wordt de volgende module uitgevoerd gevolgd door de [!UICONTROL Resume] richtlijnmodule als een fout niet met [!UICONTROL Dropbox] > [!UICONTROL List all files/subfolders] in een omslagmodule plaatsvindt.

Als er echter een fout optreedt met deze [!DNL Dropbox] -module, gaat de uitvoering naar Error Handler Route 2 en eindigt deze met de [!UICONTROL Ignore] -instructie. De module [!UICONTROL Resume directive] wordt in dit geval niet uitgevoerd.

Dit is een combinatie van fouthandlers voor filteren en nesten.

