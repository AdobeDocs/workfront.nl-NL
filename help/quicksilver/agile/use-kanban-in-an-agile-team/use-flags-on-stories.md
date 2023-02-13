---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Vlaggen gebruiken op artikelen op het Kanban-bord
description: Op de [!DNL Kanban] vlaggen geven visueel aan wanneer een artikel gereed is om naar de volgende status te gaan. Hierdoor kunnen Kanban-teams een "pull"-benadering gebruiken in plaats van een "push"-benadering bij het verplaatsen van artikelen over statussen.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Markeringen gebruiken voor artikelen op de [!UICONTROL Kanban] board

Op de [!DNL Kanban] vlaggen geven visueel aan wanneer een artikel gereed is om naar de volgende status te gaan. Dit maakt [!UICONTROL Kanban] teams gebruiken een pull-aanpak in plaats van een push-aanpak bij het verplaatsen van artikelen naar andere statussen.

**Voorbeeld:** Bekijk het volgende voorbeeld van een team dat een &quot;trekkingsbenadering&quot;benadering gebruikt: Olivia, de grafisch ontwerper van het team, voltooit haar werk en stelt de artikelvlag in op &quot;[!UICONTROL Ready to Pull].&quot; Deze vlag geeft een visuele indicatie aan Tony, de copywriter op het team, dat het verhaal klaar is voor hem om naar de volgende status te gaan. Tony brengt het verhaal dan naar de volgende status wanneer hij klaar is om eraan te gaan werken.

Houd rekening met het volgende wanneer u markeringen in artikelen gebruikt:

* Vlaggen zijn geen status, maar een visuele indicatie dat het verhaal gereed is om door een ander teamlid naar de volgende status te worden verplaatst.
* Vlaggen worden niet weergegeven op artikelkaarten die zich in de [!UICONTROL Backlog] of in de [!UICONTROL Complete] kolom (of in elke kolom waarin de status van de kolom gelijk is aan [!UICONTROL Complete]).

   Voor meer informatie over artikelstatussen raadpleegt u [Vlaggen gebruiken op artikelen op het Kanban-bord](#updating-the-status-of-stories-and-subtasks)

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
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Markeringen gebruiken voor artikelen op de [!UICONTROL Kanban] board

Een markering in een artikel wijzigen:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuwe [!UICONTROL Kanban] team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Ga naar de [!UICONTROL Kanban] aan boord waar u een vlag in een artikel wilt wijzigen.
1. Vouw de artikeltegel uit om de markering weer te geven.\
   De markering is ingesteld op **[!UICONTROL On Track]** voor elk artikel standaard.\
   ![Kanban-kaart](assets/agile-storycard-kanban-2021-350x308.png)

1. Klik op de huidige markering en selecteer een van de volgende markeringsopties:

   * **[!UICONTROL On Track]:** Het artikel heeft de juiste status en er hoeft op dit moment niets te worden ondernomen.\

      Dit is de standaardvlag voor elk verhaal op het Kanban-bord.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Is Blocked]:** Het artikel kan niet doorgaan naar de volgende status. Wanneer deze markering is ingesteld op een artikel, telt het artikel niet mee voor de WIP-limiet. (Raadpleeg het artikel voor meer informatie over WIP-limieten [Kanban configureren](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_locked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Ready to Pull]:** Het artikel kan door een ander teamlid naar de volgende status worden verplaatst.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
