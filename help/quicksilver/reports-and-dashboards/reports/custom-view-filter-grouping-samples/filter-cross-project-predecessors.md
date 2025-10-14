---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: onvolledige voordecessors voor meerdere projecten weergeven'
description: Deze taakfilter retourneert onvolledige voordecessors voor meerdere projecten.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Filter: onvolledige voordecessors voor meerdere projecten weergeven

<!--Audited: 10/2024-->

Deze taakfilter retourneert onvolledige voordecessors voor meerdere projecten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
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

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Predecessors voor meerdere projecten filteren

Dit filter toepassen:

1. Ga naar een lijst met taken of een taakrapport.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. (Voorwaardelijk) klik **wijze van de Tekst** als u de filter van een lijst of **Schakelaar aan de Wijze van de Tekst** opende, als u de filter van een rapport opende.
1. Plak in het nieuwe gebied de volgende code:
   <pre>predecessorsMM:projectID=FIELD:projectID <br> predecessorsMM:projectID_Mod=ne <br> percentComplete=100 <br> percentComplete_Mod=ne</pre>

1. (Voorwaardelijk) klik **sparen Filter** als u tot de filter van een rapport toegang had, of **&#x200B;**&#x200B;van toepassing is, dan **sparen als nieuw** als u tot de filter van een taaklijst toegang had.
