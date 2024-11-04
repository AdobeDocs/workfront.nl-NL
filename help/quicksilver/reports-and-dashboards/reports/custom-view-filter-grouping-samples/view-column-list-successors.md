---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: een lijst met taakopvolgers toevoegen in een kolom'
description: U kunt een kolom aan een taakmening toevoegen om een lijst van de opvolgers van de taken te tonen. De kolom Opvolgers van de Taak omvat het aantal van de opvolger evenals de naam.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Weergave: voeg een lijst met taakopvolgers toe in een kolom

<!--Audited: 11/2024-->

U kunt een kolom aan een taakmening toevoegen om een lijst van de opvolgers van de taken te tonen. De **kolom van de Opvolgers van de Taak** omvat het aantal van de opvolger evenals de naam.

![ task_view_with_a_list_of_succesors_.png ](assets/task-view-with-a-list-of-successors--350x118.png)

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


## Een lijst met taakopvolgers toevoegen in een kolom

Deze kolom toevoegen aan een taakweergave:

1. Ga naar een takenlijst.
1. Vouw het **drop-down menu van de Mening** uit, en klik **Nieuwe Mening**.
1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**, dan klik **uitgeven de Wijze van de Tekst**.
1. Verwijder alle tekst in **uitgeeft de Wijze van de Tekst** vakje, en vervang het met de volgende code:

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. Klik **Gedaan**, dan **sparen Mening**.
