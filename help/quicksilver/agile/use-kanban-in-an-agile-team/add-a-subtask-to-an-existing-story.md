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
source-wordcount: '324'
ht-degree: 0%

---

# Een subtaak toevoegen aan een bestaand artikel op het Kanban-bord

Houd rekening met het volgende wanneer u subtaken maakt voor bestaande artikelen:

**Wanneer de [!UICONTROL Summary Completion Mode] instellen voor het project is ingesteld op [!UICONTROL Manual]:**

* U kunt een bovenliggend artikel met subtaken verplaatsen naar [!UICONTROL Complete], waarmee het bovenliggende artikel wordt bijgewerkt naar 100% en de [!UICONTROL Status] tot [!UICONTROL Complete]. Subtaken worden niet bijgewerkt.
* Als u het dialoogvenster [!UICONTROL Percent Complete] voor het artikel moet u het bijwerken vanuit de [!UICONTROL Stories] of van de [!UICONTROL Details] pagina van het object.

**Wanneer de [!UICONTROL Summary Completion Mode] instellen voor het project is ingesteld op [!UICONTROL Automatic]:**

* U kunt het bovenliggende artikel niet over de hele linie verplaatsen. Als u het dialoogvenster [!UICONTROL Percent Complete] voor het artikel moet u de [!UICONTROL Percent Complete] voor alle subtaken. De [!UICONTROL Percent Complete] voor het artikel wordt berekend op basis van de [!UICONTROL Percent Complete] van alle subtaken.
* Een bovenliggend artikel met subtaken verplaatsen naar [!UICONTROL Complete] Hiermee werkt u het bovenliggende artikel bij naar 100% en de [!UICONTROL Status] tot [!UICONTROL Complete]. Subtaken worden ook bijgewerkt naar 100% en de [!UICONTROL Status] wordt bijgewerkt naar [!UICONTROL Complete].

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
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Contribute] of [!UICONTROL Manage] toegang tot de taak subtask is</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een subtaak toevoegen aan een bestaand artikel op het tabblad [!UICONTROL Kanban] board

1. Ga naar de [!UICONTROL Kanban] board dat het artikel bevat waar u een subtaak wilt toevoegen.
1. Klik op de naam van de taak in de artikeltegel op het tabblad [!UICONTROL Kanban] bord.
1. Voeg een subtaak aan de taak toe zoals u in een andere taaklijst binnen [!DNL Workfront], zoals beschreven in [Subtaken maken](../../manage-work/tasks/create-tasks/create-subtasks.md).
