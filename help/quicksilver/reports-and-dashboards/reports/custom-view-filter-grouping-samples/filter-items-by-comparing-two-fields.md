---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: items in een lijst verwijderen door twee velden te vergelijken'
description: U kunt items uit een lijst filteren door twee van de velden te vergelijken. U kunt bijvoorbeeld alleen taken weergeven als de datum van feitelijke voltooiing van de taak groter is dan de geplande voltooiingsdatum.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filter: items in een lijst verwijderen door twee velden te vergelijken

<!--Audited: 10/2024-->

U kunt items uit een lijst filteren door twee van de velden te vergelijken. U kunt bijvoorbeeld alleen taken weergeven als de datum van feitelijke voltooiing van de taak groter is dan de geplande voltooiingsdatum.

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

## Items filteren door twee velden te vergelijken

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. Voeg een filter voor **Datum van de Taak :Actual Voltooiing** toe > **Groter dan** > **selecteer een datum**.

   >[!TIP]
   >
   >Kies de filteroptie die u voor het geselecteerde veld wilt gebruiken, indien beschikbaar.

1. Klik **wijze van de Tekst**.
1. Voeg de volgende code toe in het weergegeven gebied:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Klik **toepassen** > **sparen als nieuw**.
