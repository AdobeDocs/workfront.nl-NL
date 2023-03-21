---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Een inlaatkolom aan een bord toevoegen
description: U kunt desgewenst een inlaatkolom toevoegen aan uw board die taken en problemen automatisch ophaalt als verbonden kaarten wanneer deze worden toegevoegd in Workfront, op basis van filters die u definieert.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 0bcd7cbe43a03216dddabb173aa5888b97cffd23
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Een inlaatkolom aan een bord toevoegen

U kunt desgewenst een inlaatkolom aan uw board toevoegen die taken en problemen automatisch ophaalt als verbonden kaarten wanneer deze worden toegevoegd [!DNL Workfront], op basis van filters die u definieert. De innamekolom kan als backlogkolom voor een team Kanban, een innamelocatie voor een steunteam dienen om kwesties te zien aangezien zij aan een verzoekrij, of een ander doel worden toegevoegd u wenst.

Er is slechts één inlaatkolom toegestaan op een bord en deze wordt altijd weergegeven als de meest linkse kolom.

De inlaatkolom is beperkt tot 300 taken en 300 problemen. Ze worden gesorteerd op de prioriteit die op de items is gedefinieerd. Voor informatie over prioriteit raadpleegt u [Taak-prioriteit bijwerken](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) en [Probleemprioriteit bijwerken](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

Voor meer informatie over kolommen raadpleegt u [Bordkolommen beheren](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Voor informatie over verbonden kaarten raadpleegt u [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!DNL Request] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een inlaatkolom maken

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Boards]**.
1. Toegang tot een bord. Zie voor meer informatie [Een board maken of bewerken](../../agile/get-started-with-boards/create-edit-board.md).
1. Klikken **[!UICONTROL Configure]** rechts van de board om het Configure paneel te openen.
1. Uitbreiden **[!UICONTROL Board]**.
1. Inschakelen **[!UICONTROL Dynamically intake items to board]**.

   ![Invoerkolom maken](assets/create-intake-column2.png)

   De inlaatkolom wordt links van het bord toegevoegd. Deze blijft leeg totdat u er filters op toepast.

1. Klikken **[!UICONTROL Filter sources]** en selecteert u **[!UICONTROL Tasks]** of **[!UICONTROL Issues]**.

   >[!NOTE]
   >
   >U kunt de inlaatkolom filteren om zowel taken als problemen op te nemen, maar u moet de filters voor elk objecttype afzonderlijk instellen.
   >
   >Opgeslagen filters en standaardfilters van het systeem kunnen ook worden geselecteerd.

1. Klik in het filterdeelvenster op **[!UICONTROL New filter]** om aan de slag te gaan.

   ![Klik op Nieuw filter](assets/intake-filter-dialog5.png)

1. Stel uw filter samen en klik op **[!UICONTROL Save as new]**.

   ![Filter builder](assets/intake-filter-dialog6.png)

   Dit voorbeeld toont een filter voor taken van een specifiek project die in de status van [!UICONTROL New] of [!UICONTROL In Progress]en worden aan mij toegewezen.

   Zie de sectie &quot;Een filter maken of bewerken in de bètabuilder&quot; in het artikel voor meer informatie over het maken van een filter [Filters maken of bewerken in [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Geef het filter een naam en klik op **[!UICONTROL Save]**.

   ![Typ een naam voor het filter](assets/intake-filter-dialog7.png)

   Als u het filter een unieke naam geeft, kunt u er later naar zoeken.

1. Het filter wordt weergegeven in de lijst met opgeslagen filters en wordt automatisch toegepast op de inlaatkolom. Klik op de X boven aan het filterdeelvenster om het te sluiten.

   ![Opgeslagen filter](assets/intake-filter-dialog8.png)

1. (Optioneel) Als u het filter met anderen wilt delen, houdt u de muisaanwijzer boven het opgeslagen filter en klikt u op de knop **[!UICONTROL More]** menu ![Meer menupictogram](assets/more-icon-spectrum.png)en selecteert u **[!UICONTROL Share]**. Kies de gebruikers of teams waarmee u wilt delen in het vak Filter delen. Zie voor meer informatie [Een filter, weergave of groep delen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Optioneel) Klik op **[!UICONTROL Filter sources]** en selecteer het andere object om een ander filter te maken.
1. Wanneer u klaar bent met het toevoegen van filters, bekijkt u de inlaatkolom om te controleren of de juiste taken en problemen worden weergegeven.

   ![Kolom opnemen](assets/intake-column-added3.png)

   Kaarten in de inlaatkolom kunnen pas worden bewerkt als u ze naar andere boardkolommen verplaatst. U kunt op de kaart klikken om deze te openen in een alleen-lezen weergave of op ![Taak of probleem openen](assets/boards-launch-icon.png) om de taak of uitgave te openen in een nieuw browsertabblad.

   >[!NOTE]
   >
   >De alleen-lezen weergave voor kaarten in de innamekolom is alleen beschikbaar via de vroege functieaanmelding voor [!DNL Workfront] [!UICONTROL Boards].

   U kunt de volgorde van de items in de inlaatkolom handmatig wijzigen.

   De pictogrammen op de bovenkant recht van de inlaatkolom tonen u hoeveel kaarten momenteel in de kolom zijn, en hoeveel filters worden toegepast.

   >[!NOTE]
   >
   >U kunt de filters op elk ogenblik bijwerken door het Configure paneel te openen, klikken **[!UICONTROL Filter sources]** en selecteert u **[!UICONTROL Tasks]** of **[!UICONTROL Issues]**.

1. (Optioneel) Als u wilt zoeken naar een item in de kolom Opname, klikt u op ![Zoekpictogram](assets/search-icon.png) in de kolom.
1. (Optioneel) Als u een kaart van de inlaatkolom naar een andere kolom wilt verplaatsen, sleept u de kaart naar de gewenste positie.

   of

   Klik op de knop **[!UICONTROL More]** menu ![Meer menupictogram](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Move]**. Dan, op **[!UICONTROL Move Item]** een andere kolom kiezen en **[!UICONTROL Move]**.

1. (Optioneel) Als u de opnamekolom wilt verwijderen, klikt u op de knop **[!UICONTROL More]** menu ![Meer menupictogram](assets/more-icon-spectrum.png) en selecteert u **[!UICONTROL Delete]**.
