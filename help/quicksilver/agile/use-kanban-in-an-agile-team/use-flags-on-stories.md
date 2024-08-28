---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Vlaggen gebruiken op artikelen op de Kanban Board
description: Op het  [!DNL Kanban]  bord, verstrekken de vlaggen een visuele aanwijzing van wanneer een verhaal aan de volgende status klaar is te bewegen. Hierdoor kunnen Kanban-teams een "pull"-benadering gebruiken in plaats van een "push"-benadering bij het verplaatsen van artikelen over statussen.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Vlaggen gebruiken op artikelen op het [!UICONTROL Kanban] -bord

Op het [!DNL Kanban] -bord geven vlaggen een visuele indicatie van wanneer een artikel gereed is om naar de volgende status te gaan. Hierdoor kunnen [!UICONTROL Kanban] -teams een &#39;pull&#39;-benadering gebruiken in plaats van een &#39;push&#39;-benadering bij het verplaatsen van artikelen over statussen.

**Voorbeeld:** overweeg het volgende voorbeeld van een team gebruikend een &quot;trekkingsbenadering&quot;: Olivia, grafisch ontwerper op het team, voltooit haar werk en plaatst dan de verhaalvlag als &quot;[!UICONTROL Ready to Pull]&quot;. Deze vlag geeft een visuele indicatie aan Tony, de copywriter op het team, dat het verhaal klaar is voor hem om naar de volgende status te gaan. Tony brengt het verhaal dan naar de volgende status wanneer hij klaar is om eraan te gaan werken.

Houd rekening met het volgende wanneer u markeringen in artikelen gebruikt:

* Vlaggen zijn geen status, maar een visuele indicatie dat het verhaal gereed is om door een ander teamlid naar de volgende status te worden verplaatst.
* Vlaggen worden niet weergegeven op artikelkaarten in de kolom [!UICONTROL Backlog] of in de kolom [!UICONTROL Complete] (of in een kolom waarin de status van de kolom gelijk is aan [!UICONTROL Complete] ).

  Voor meer informatie over artikelstatussen, zie {de vlaggen van 0} Gebruik op verhalen op de karton Kanban ](#updating-the-status-of-stories-and-subtasks)[

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
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vlaggen gebruiken op artikelen op het [!UICONTROL Kanban] -bord

Een markering in een artikel wijzigen:

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw [!UICONTROL Kanban] team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Ga naar het [!UICONTROL Kanban] -bord waar u een markering in een artikel wilt wijzigen.
1. Vouw de artikeltegel uit om de markering weer te geven.
De markering is standaard ingesteld op **[!UICONTROL On Track]** voor elk artikel.
   ![ Kanban kaart ](assets/agile-storycard-kanban-2021-350x308.png)

1. Klik op de huidige markering en selecteer een van de volgende markeringsopties:

   * **[!UICONTROL On Track]:** Het artikel heeft de juiste status en op dit moment hoeft niets te worden gedaan.

     Dit is de standaardvlag voor elk verhaal op het Kanban-bord.
     ![ kanban_flag_ontrack.png ](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Is Blocked]:** Het artikel kan niet doorgaan naar de volgende status. Wanneer deze markering is ingesteld op een artikel, telt het artikel niet mee voor de WIP-limiet. (Voor meer informatie over de grenzen van WIP, zie het artikel [ Kanban ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) vormen.)

     ![ kanban_flag_locked.png ](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Ready to Pull]:** Het artikel kan door een ander lid van het team naar de volgende status worden verplaatst.

     ![ kanban_flag_ready.png ](assets/kanban-flag-ready.png)
