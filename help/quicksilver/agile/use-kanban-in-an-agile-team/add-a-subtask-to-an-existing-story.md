---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Een subtaak toevoegen aan een bestaand artikel op het Kanban-bord
description: Lees dit artikel om te leren hoe u subtaken kunt maken voor bestaande artikelen op de Kanban-board.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '327'
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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Contribute] of [!UICONTROL Manage] toegang hebben tot de taak waarop de subtaak is uitgevoerd</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een subtaak toevoegen aan een bestaand artikel op het [!UICONTROL Kanban] -bord

1. Ga naar de [!UICONTROL Kanban] -board die het artikel bevat waar u een subtaak wilt toevoegen.
1. Klik op de naam van de taak in de artikeltegel op het [!UICONTROL Kanban] -bord.
1. Voeg een subtask aan de taak toe zoals u in een andere taaklijst binnen [!DNL Workfront] zou doen, zoals die in [ wordt beschreven creeer subtasks ](../../manage-work/tasks/create-tasks/create-subtasks.md).
