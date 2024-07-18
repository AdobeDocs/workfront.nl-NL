---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: De uitvoering van het scenario, cycli, en fasen in  [!DNL Adobe Workfront Fusion]
description: Dit artikel beschrijft gebeurtenissen die voorkomen terwijl een  [!DNL Adobe Workfront Fusion]  scenario, zoals initialisering, verrichtingen, begaat, en terugdraaiversies loopt.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Uitvoering, cycli en fasen van scenario [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] is een transactiesysteem, vergelijkbaar met relationele databases. Elke uitvoering van het scenario begint met de initialisatiefase, gaat verder met minstens één cyclus die uit de verrichtings en verbind/terugschroeven van prijzen fasen wordt samengesteld, en eindigt met de finalisatiefase:

>[!INFO]
>
>**Voorbeeld**
>
>Initialisatie
>
>Cyclus 1
>
>Bewerking (lezen of schrijven)
>
>Vastleggen of terugdraaien
>
>Cyclus 2
>
>Bewerking (lezen of schrijven)
>
>Vastleggen of terugdraaien
>
>...
>
>Cyclus #N
>
>Bewerking (lezen of schrijven)
>
>Vastleggen of terugdraaien
>
>Voltooiing

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
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
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
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

## Initialisatie

Tijdens de initialisatiefase worden alle benodigde verbindingen (verbinding met een database, e-mailservice enzovoort) gemaakt. Ze worden ook gecontroleerd of elke module in staat is de beoogde bewerkingen uit te voeren.

## Cycli

Elke cyclus vertegenwoordigt een niet-scheidbare werkeenheid die bestaat uit een reeks bewerkingen. Het maximum aantal cycli kan worden ingesteld in het deelvenster [!UICONTROL scenario settings] . Het standaardnummer is 1.

Voor meer informatie, zie [ het paneel van scenario montages in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Bewerking

Tijdens de bewerkingsfase wordt het lezen en/of schrijven uitgevoerd:

* De lezingsverrichting bestaat uit het verkrijgen van gegevens van de dienst die dan door andere modules volgens een vooraf bepaald scenario wordt verwerkt. De module [!UICONTROL Dropbox] > [!UICONTROL Watch files] retourneert bijvoorbeeld nieuwe bundels (bestanden) die zijn gemaakt sinds de laatste uitvoering van het scenario.
* De schrijfbewerking bestaat uit het verzenden van gegevens naar een bepaalde dienst voor verdere verwerking. De module [!DNL Dropbox] > [!UICONTROL Upload a file] uploadt bijvoorbeeld een bestand naar een map [!DNL Dropbox] .

## Vastleggen

Als de verrichtingsfase voor alle modules succesvol is, begaat fase waarin alle die verrichtingen door de modules worden uitgevoerd worden begaan. Dit betekent dat [!DNL Workfront Fusion] informatie over het succes van de bewerkingsfase naar alle services stuurt die bij de bewerkingsfase zijn betrokken.

## Terugdraaien

Als een fout tijdens de verrichting voorkomt of fase op om het even welke module begaan, wordt de fase geaborteerd en de terugdraaiingsfase is begonnen, makend alle verrichtingen tijdens de bepaalde cyclusleegte. Sommige modules ondersteunen geen terugdraaiacties en bewerkingen die door deze modules worden uitgevoerd, kunnen niet worden teruggenomen. Voor meer informatie zie de [ ACID modules ](#acid-modules) sectie.

## Voltooiing

Tijdens de afwerkingsfase worden open verbindingen (bijvoorbeeld FTP-verbindingen, databaseverbindingen, enzovoort) gesloten en wordt het scenario voltooid.

## ACID-modules

Alle [!DNL Workfront Fusion] -modules die rollback (ook wel transactie genoemd) ondersteunen, worden gemarkeerd met de ACID-tag.

![](assets/acid-modules-350x189.png)

Modules die niet met deze tag zijn gemarkeerd, kunnen niet worden teruggezet naar de oorspronkelijke status wanneer er fouten optreden in andere modules. Een typisch voorbeeld van een niet-ACID module is de [!UICONTROL Email] > [!UICONTROL Send an Email] actie. Nadat het e-mailbericht is verzonden, kunt u het verzenden niet meer ongedaan maken.
