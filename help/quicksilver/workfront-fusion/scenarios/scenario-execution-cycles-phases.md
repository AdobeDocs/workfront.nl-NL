---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Uitvoering van scenario's, cycli en fasen in [!DNL Adobe Workfront Fusion]
description: In dit artikel worden gebeurtenissen beschreven die tijdens een [!DNL Adobe Workfront Fusion] het scenario loopt, zoals initialisatie, verrichtingen, begaat, en terugdraaiversies.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] is een transactioneel systeem, gelijkend op relationele gegevensbanken. Elke uitvoering van het scenario begint met de initialisatiefase, gaat verder met minstens één cyclus die uit de verrichtings en verbind/terugschroeven van prijzen fasen wordt samengesteld, en eindigt met de finalisatiefase:

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Initialisatie

Tijdens de initialisatiefase worden alle benodigde verbindingen (verbinding met een database, e-mailservice enzovoort) gemaakt. Ze worden ook gecontroleerd of elke module in staat is de beoogde bewerkingen uit te voeren.

## Cycli

Elke cyclus vertegenwoordigt een niet-scheidbare werkeenheid die bestaat uit een reeks bewerkingen. Het maximum aantal cycli in de [!UICONTROL scenario settings] deelvenster. Het standaardnummer is 1.

Zie voor meer informatie [Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Bewerking

Tijdens de bewerkingsfase wordt het lezen en/of schrijven uitgevoerd:

* De lezingsverrichting bestaat uit het verkrijgen van gegevens van de dienst die dan door andere modules volgens een vooraf bepaald scenario wordt verwerkt. De [!UICONTROL Dropbox] >[!UICONTROL Watch files] de module keert nieuwe bundels (dossiers) terug die sinds de laatste scenariouitvoering worden gecreeerd.
* De schrijfbewerking bestaat uit het verzenden van gegevens naar een bepaalde dienst voor verdere verwerking. De [!DNL Dropbox] >[!UICONTROL Upload a file] module uploadt een bestand naar een [!DNL Dropbox] map.

## Vastleggen

Als de verrichtingsfase voor alle modules succesvol is, begaat fase waarin alle die verrichtingen door de modules worden uitgevoerd worden begaan. Dit betekent dat [!DNL Workfront Fusion] stuurt informatie over het succes van de exploitatiefase naar alle diensten die bij de exploitatiefase betrokken zijn .

## Terugdraaien

Als een fout tijdens de verrichting voorkomt of fase op om het even welke module begaan, wordt de fase geaborteerd en de terugdraaiingsfase is begonnen, makend alle verrichtingen tijdens de bepaalde cyclusleegte. Sommige modules steunen geen terugdraaiing en de verrichtingen die door deze modules worden uitgevoerd kunnen niet worden teruggenomen. Zie voor meer informatie de [ACID-modules](#acid-modules) sectie.

## Voltooiing

Tijdens de afwerkingsfase worden open verbindingen (bijvoorbeeld FTP-verbindingen, databaseverbindingen, enzovoort) gesloten en wordt het scenario voltooid.

## ACID-modules

Alles [!DNL Workfront Fusion] Modules die terugdraaiacties (ook wel transactie genoemd) ondersteunen, worden gemarkeerd met de ACID-tag.

![](assets/acid-modules-350x189.png)

Modules die niet met deze tag zijn gemarkeerd, kunnen niet worden teruggezet naar de oorspronkelijke status wanneer er fouten optreden in andere modules. Een typisch voorbeeld van een niet-ACID module is [!UICONTROL Email] >[!UICONTROL Send an Email] handeling. Nadat het e-mailbericht is verzonden, kunt u het verzenden niet meer ongedaan maken.
