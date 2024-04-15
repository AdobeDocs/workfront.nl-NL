---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Een kaart van een kaart verwijderen of archiveren
description: Wanneer u een kaart van een bord schrapt, wordt het permanent geschrapt en kan niet worden hersteld. Als u een kaart archiveert, wordt deze naar het archief verzonden en kunt u deze later terugzetten op het bord.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Een kaart van een kaart verwijderen of archiveren

Wanneer u een ad-hockaart van een kaart verwijdert, wordt deze permanent verwijderd en kan deze niet worden hersteld. Aangesloten kaarten kunnen handmatig weer aan een kaart worden toegevoegd nadat ze zijn verwijderd.

Als u een aangesloten kaart van een dynamische raad schrapt, zal het opnieuw verschijnen wanneer u de raad verfrist omdat dit bordtype alle taken en kwesties van een specifiek project vult. Als u de kaart wilt verwijderen, moet u de verbonden taak of uitgave uit het Workfront-project verwijderen.

Wanneer u een aangesloten kaart van een ander bordtype schrapt dat een inputkolom heeft, zal de kaart opnieuw in de inputkolom verschijnen wanneer u de raad verfrist als de verbonden taak of de kwestie nog niet duidelijk volledig is. Zie voor meer informatie over inlaatkolommen [Een inlaatkolom aan een bord toevoegen](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Als u een kaart archiveert, wordt deze naar het archief verzonden en kunt u deze later terugzetten op het bord.

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
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een kaart van de kaart verwijderen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Boards]**.
1. Toegang tot een bord. Zie voor meer informatie [Een board maken of bewerken](../../agile/get-started-with-boards/create-edit-board.md).
1. Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Delete]**.
1. Klikken **[!UICONTROL Delete]** in het bevestigingsbericht.

## Een kaart archiveren van een kaart

1. Toegang tot het bord.
1. Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Archive]**.

   Gearchiveerde kaarten worden verborgen van het bord, tenzij u een filter toepast om ze weer te geven. Zie voor meer informatie [Een kaart filteren om gearchiveerde kaarten weer te geven](#filter-a-board-to-show-archived-cards) in dit artikel.

   An [!UICONTROL Archive] pictogram ![Archief](assets/archive-icon-spectrum-25x20.png) wordt weergegeven op gearchiveerde kaarten. U kunt een gearchiveerde kaart niet bewerken, maar u kunt de kaart wel verwijderen of naar een andere kolom verplaatsen.

1. Om een gearchiveerde kaart te herstellen, klik **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Restore]**.

## Een kaart filteren om gearchiveerde kaarten weer te geven {#filter-a-board-to-show-archived-cards}

Standaard worden alleen actieve kaarten op een bord weergegeven. U kunt het bord filteren om ook gearchiveerde kaarten weer te geven.

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Configureren**] rechts van de board om het Configure paneel te openen.
1. Uitbreiden [!UICONTROL **Kaarten**].
1. Inschakelen [!UICONTROL **Gearchiveerde kaarten op de kaart weergeven**].
1. Klikken [!UICONTROL **Filter**], breid de [!UICONTROL Archived Cards] en selecteert u **[!UICONTROL Archived cards]** gearchiveerde kaarten weergeven.

   Het filter geeft het aantal gearchiveerde kaarten weer.

   ![Gearchiveerde kaarten filteren](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >De [!UICONTROL Archived Cards] is niet beschikbaar in het filter als u de configuratie-instelling niet hebt ingeschakeld om gearchiveerde kaarten weer te geven. Zie voor meer informatie [Aanpassen welke velden worden weergegeven op een kaart](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Selecteren **[!UICONTROL Archived cards]** om de optie te wissen en alleen actieve kaarten weer te geven.
