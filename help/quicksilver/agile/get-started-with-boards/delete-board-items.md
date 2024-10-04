---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Een kaart van een kaart verwijderen of archiveren
description: Wanneer u een kaart van een bord schrapt, wordt het permanent geschrapt en kan niet worden hersteld. Als u een kaart archiveert, wordt deze naar het archief verzonden en kunt u deze later terugzetten op het bord.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 81e87793905fd925db00c7a0ac107150263a1365
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Een kaart van een kaart verwijderen of archiveren

Wanneer u een ad-hockaart van een kaart verwijdert, wordt deze permanent verwijderd en kan deze niet worden hersteld. Aangesloten kaarten kunnen handmatig weer aan een kaart worden toegevoegd nadat ze zijn verwijderd.

Als u een aangesloten kaart van een dynamische raad schrapt, zal het opnieuw verschijnen wanneer u de raad verfrist omdat dit bordtype alle taken en kwesties van een specifiek project vult. Als u de kaart wilt verwijderen, moet u de verbonden taak of uitgave uit het Workfront-project verwijderen.

Wanneer u een aangesloten kaart van een ander bordtype schrapt dat een inputkolom heeft, zal de kaart opnieuw in de inputkolom verschijnen wanneer u de raad verfrist als de verbonden taak of de kwestie nog niet duidelijk volledig is. Voor meer informatie over innamekolommen, zie [ een inlaatkolom aan een raad ](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md) toevoegen.

Als u een kaart archiveert, wordt deze naar het archief verzonden en kunt u deze later terugzetten op het bord.

Gearchiveerde kaarten synchroniseren niet met Workfront-taken en -problemen. Als u een kaart herstelt, wordt deze opnieuw gesynchroniseerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> 
   <p>Nieuw: [!UICONTROL Contributor] of hoger</p> 
   <p>of</p>
   <p>Huidig: [!UICONTROL Request] of hoger</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een kaart van de kaart verwijderen

{{step1-to-boards}}

1. Toegang tot een bord. Voor informatie, zie [ creeer of geef een raad ](../../agile/get-started-with-boards/create-edit-board.md) uit.
1. Klik het **[!UICONTROL More]** menu ![ Meer menu ](assets/more-icon-spectrum.png) op de kaart, en selecteer **[!UICONTROL Delete]**.
1. Klik op **[!UICONTROL Delete]** in het bevestigingsbericht.

## Een kaart archiveren van een kaart

1. Toegang tot het bord.
1. Klik het **[!UICONTROL More]** menu ![ Meer menu ](assets/more-icon-spectrum.png) op de kaart, en selecteer **[!UICONTROL Archive]**.

   Gearchiveerde kaarten worden verborgen van het bord, tenzij u een filter toepast om ze weer te geven. Voor meer informatie, zie [ Filter een raad om gearchiveerde kaarten ](#filter-a-board-to-show-archived-cards) in dit artikel te tonen.

   Een [!UICONTROL Archive] pictogram ![ Archief ](assets/archive-icon-spectrum-25x20.png) verschijnt op gearchiveerde kaarten. U kunt een gearchiveerde kaart niet bewerken, maar u kunt de kaart wel verwijderen of naar een andere kolom verplaatsen.

1. Om een gearchiveerde kaart te herstellen, klik het **[!UICONTROL More]** menu ![ Meer menu ](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Restore]**.

## Een kaart filteren om gearchiveerde kaarten weer te geven

Standaard worden alleen actieve kaarten op een bord weergegeven. U kunt het bord filteren om ook gearchiveerde kaarten weer te geven.

1. Toegang tot het bord.
1. Klik [!UICONTROL **vormen**] op het recht van de raad om het Configure paneel te openen.
1. Breid [!UICONTROL **Kaarten**] uit.
1. Zet [!UICONTROL **gearchiveerde kaarten van de Vertoning op de raad**] aan.
1. Klik [!UICONTROL **Filter**], breid de [!UICONTROL Archived Cards] sectie uit, en selecteer **[!UICONTROL Archived cards]** om het even welke gearchiveerde kaarten te tonen.

   Het filter geeft het aantal gearchiveerde kaarten weer.

   ![ gearchiveerde kaarten van de Filter ](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >De sectie [!UICONTROL Archived Cards] is niet beschikbaar in het filter als u de configuratie-instelling niet hebt ingeschakeld voor het weergeven van gearchiveerde kaarten. Voor meer informatie, zie [ aanpassen welke gebieden op een kaart ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) worden getoond.

1. Selecteer nogmaals **[!UICONTROL Archived cards]** om de optie te wissen en alleen actieve kaarten weer te geven.
