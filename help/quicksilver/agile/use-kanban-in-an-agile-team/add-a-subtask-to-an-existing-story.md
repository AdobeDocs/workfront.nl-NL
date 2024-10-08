---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Een subtaak toevoegen aan een bestaand artikel op het Kanbankenbord
description: Lees dit artikel om te leren hoe u subtaken kunt maken voor bestaande artikelen op de Kanban-board.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Een subtaak toevoegen aan een bestaand artikel op het Kanban-bord

Houd rekening met het volgende wanneer u subtaken maakt voor bestaande artikelen:

**wanneer het [!UICONTROL Summary Completion Mode] plaatsen voor het project aan [!UICONTROL Manual] wordt geplaatst:**

* U kunt een bovenliggend artikel met subtaken verplaatsen naar [!UICONTROL Complete] , waar het bovenliggende artikel wordt bijgewerkt naar 100% en de [!UICONTROL Status] naar [!UICONTROL Complete] . Subtaken worden niet bijgewerkt.
* Als u [!UICONTROL Percent Complete] voor het artikel wilt bijwerken, moet u het bijwerken vanaf de [!UICONTROL Stories] -tab of de [!UICONTROL Details] -pagina van het object.

**wanneer het [!UICONTROL Summary Completion Mode] plaatsen voor het project aan [!UICONTROL Automatic] wordt geplaatst:**

* U kunt het bovenliggende artikel niet over de hele linie verplaatsen. Als u [!UICONTROL Percent Complete] voor het artikel wilt bijwerken, moet u [!UICONTROL Percent Complete] voor alle subtaken bijwerken. De waarde [!UICONTROL Percent Complete] voor het artikel wordt berekend op basis van de waarde [!UICONTROL Percent Complete] van alle subtaken.
* Als u een bovenliggend artikel met subtaken verplaatst naar [!UICONTROL Complete] , wordt het bovenliggende artikel bijgewerkt naar 100% en de [!UICONTROL Status] naar [!UICONTROL Complete] . Subtaken worden ook bijgewerkt naar 100% en [!UICONTROL Status] wordt bijgewerkt naar [!UICONTROL Complete] .

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p> 
   of
   <p>Huidig: [!UICONTROL Work] of hoger</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>[!UICONTROL Contribute] of [!UICONTROL Manage] toegang hebben tot de taak waarop de subtaak is uitgevoerd</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een subtaak toevoegen aan een bestaand artikel op het [!UICONTROL Kanban] -bord

1. Ga naar de [!UICONTROL Kanban] -board die het artikel bevat waar u een subtaak wilt toevoegen.
1. Klik op de naam van de taak in de artikeltegel op het [!UICONTROL Kanban] -bord.
1. Voeg een subtask aan de taak toe zoals u in een andere taaklijst binnen [!DNL Workfront] zou doen, zoals die in [ wordt beschreven creeer subtasks ](../../manage-work/tasks/create-tasks/create-subtasks.md).
