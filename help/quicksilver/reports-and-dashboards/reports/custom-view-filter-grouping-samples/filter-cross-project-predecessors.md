---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: onvolledige voordecessors voor meerdere projecten weergeven'
description: Deze taakfilter retourneert onvolledige voordecessors voor meerdere projecten.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Filter: onvolledige voordecessors voor meerdere projecten weergeven

<!--Audited: 10/2024-->

Deze taakfilter retourneert onvolledige voordecessors voor meerdere projecten.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Predecessors voor meerdere projecten filteren

Dit filter toepassen:

1. Ga naar een lijst met taken of een taakrapport.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. (Voorwaardelijk) klik **wijze van de Tekst** als u de filter van een lijst of **Schakelaar aan de Wijze van de Tekst** opende, als u de filter van een rapport opende.
1. Plak in het nieuwe gebied de volgende code:
   <pre>predecessorsMM:projectID=FIELD:projectID <br> predecessorsMM:projectID_Mod=ne <br> percentComplete=100 <br> percentComplete_Mod=ne</pre>

1. (Voorwaardelijk) klik **sparen Filter** als u tot de filter van een rapport toegang had, of **** van toepassing is, dan **sparen als nieuw** als u tot de filter van een taaklijst toegang had.
