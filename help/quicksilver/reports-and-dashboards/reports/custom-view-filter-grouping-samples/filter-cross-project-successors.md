---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: onvolledige opvolgers voor meerdere projecten weergeven'
description: Deze taakfilter keert onvolledige dwars-projectopvolgers terug.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---

# Filter: onvolledige opvolgers voor meerdere projecten weergeven

Deze taakfilter keert onvolledige dwars-projectopvolgers terug.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Opvolgers voor meerdere projecten filteren

Dit filter toepassen:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. Klik **wijze van de Tekst**.
1. Plak de volgende code in het weergegeven gebied:
   <pre>percentComplete=100 <br> percentComplete_Mod=ne <br> opvolgersMM:projectID=FIELD:projectID <br> opvolgersMM:projectID_Mod=ne</pre>

1. Klik **toepassen** > **sparen als nieuw**.
