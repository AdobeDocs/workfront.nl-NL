---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: items in een lijst verwijderen door twee velden te vergelijken'
description: U kunt items uit een lijst filteren door twee van de velden te vergelijken. U kunt bijvoorbeeld alleen taken weergeven als de datum van feitelijke voltooiing van de taak groter is dan de geplande voltooiingsdatum.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 4532e08bddf993426e9d4eed6f7f8bd638663188
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Filter: items in een lijst verwijderen door twee velden te vergelijken

<!--Audited: 10/2024-->

U kunt items uit een lijst filteren door twee van de velden te vergelijken. U kunt bijvoorbeeld alleen taken weergeven als de datum van feitelijke voltooiing van de taak groter is dan de geplande voltooiingsdatum.

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

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Items filteren door twee velden te vergelijken

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. Voeg een filter voor **Taak toe:De Ware Datum van de Voltooiing** > **Groter dan** > **selecteer een datum**.

   >[!TIP]
   >
   >Kies de filteroptie die u voor het geselecteerde veld wilt gebruiken, indien beschikbaar.

1. Klik **wijze van de Tekst**.
1. Voeg de volgende code toe in het weergegeven gebied:

   `actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt`

1. Klik **toepassen** > **sparen als nieuw**.
