---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: taakinspringingen weergeven in een takenlijst'
description: In deze taakmening, kunt u code aan de kolom van de Naam van de Taak toevoegen om de taken te tonen die volgens de Structuur van de Onderverdeling van het Werk van het project worden ingesprongen.
author: Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Weergeven: taakinspringingen weergeven in een takenlijst

<!--Audited: 11/2024-->

In deze taakmening, kunt u code aan de kolom van de Naam van de Taak toevoegen om de taken te tonen die volgens de Structuur van de Onderverdeling van het Werk van het project worden ingesprongen.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Taken weergeven in een kolom van een takenlijst

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** en beginnen &quot;Naam van de Taak&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Van de nieuwe kolom, klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst die u zoekt op de regel `valuefield=` en vervang deze door de volgende code:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klik **Gedaan**, dan **sparen Mening**.
1. (Facultatief) werk de meningsnaam bij, dan klik **sparen Mening**.
