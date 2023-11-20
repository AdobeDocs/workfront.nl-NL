---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filteren en zoeken in een board
description: U kunt een bord filteren om alleen bepaalde kaarten weer te geven.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: b6a824ac6248c86043f7f21866c8a14a6c97602f
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Filteren en zoeken in een board

U kunt een board filteren om weer te geven:

* Kaarten aan bepaalde personen
* Kaarten met bepaalde labels
* Kaarten met een specifieke status
* Kaarten die in een bepaald tijdsbestek verschuldigd zijn
* Gearchiveerde kaarten
* Kaarten verbonden met een specifiek project

Als u het bord sorteert, worden alle kaarten in de kolommen gesorteerd. U kunt geen enkele kolom sorteren en de kolom voor het aantal kolommen of de kolom voor het aantal kolommen wordt niet gesorteerd.

Door te zoeken kunt u ook een bepaalde kaart op het bord vinden.

Wanneer filters worden toegepast, wordt een indicator weergegeven op het bord ![Filter toegepast op board](assets/boards-filterapplied-30x30.png). Klikken **[!UICONTROL Clear All]** om alle filters van de raad te verwijderen, en het samenvouwpictogram te klikken om het filterpaneel te sluiten.

![Deelvenster Filter](assets/boards-all-filters-collapsed-0823.png)

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

## Een bord filteren op toewijzing

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Boards]**.
1. Toegang tot een bord. Zie voor meer informatie [Een board maken of bewerken](../../agile/get-started-with-boards/create-edit-board.md).
1. Klikken [!UICONTROL **Filter**], breid de [!UICONTROL Members] en selecteert u de persoon of personen van wie u de kaarten wilt zien. U kunt ook niet-toegewezen kaarten weergeven.

   ![Filteren op lid](assets/boards-filter-by-assignees-0822.png)

## Een board filteren op tags

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Filter**], breid de [!UICONTROL Tags] en selecteert u de tags die u wilt zien.

   ![Filteren op tag](assets/boards-filter-by-tags-0822.png)

## Een bord filteren op status

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Filter**], breid de [!UICONTROL Statuses] en selecteert u de statustypen die u wilt zien.

   U kunt ook voltooide kaarten verbergen.

   ![Filteren op status](assets/boards-filter-by-status-0822.png)

## Een board filteren op de datum van de datum

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Filter**], breid de [!UICONTROL Due Date] en selecteert u de datumopties die u wilt zien.

   Alleen kaarten in de geselecteerde datumbereiken worden weergegeven.

   ![Filteren op vervaldatum](assets/boards-filter-by-due-date-0822.png)

## Een kaart filteren om gearchiveerde kaarten weer te geven

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

## Een bord filteren op verbinding

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Filter**], breid de [!UICONTROL Connection] en selecteert u de [!DNL Workfront] projecten voor de verbonden kaarten u wilt zien.

   U kunt ook kaarten weergeven die niet zijn verbonden met een project.

   ![Filteren op verbinding](assets/boards-filter-by-connection.png)

## Sorteren op een board

Wanneer u een optie selecteert om op te sorteren, worden alle kolommen gesorteerd. U kunt geen enkele kolom sorteren en de kolom voor het aantal kolommen of de kolom voor het aantal kolommen wordt niet gesorteerd.

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Sorteren op**] en selecteert u [!UICONTROL **Naam**], [!UICONTROL **Vervaldatum**], [!UICONTROL **Schatting**], [!UICONTROL **Status**], of [!UICONTROL **Verbinding**].

   De verbinding (projectnaam) is slechts op verbonden kaarten van toepassing, en de andere opties zullen zowel verbonden als ad hoc kaarten in de kolommen sorteren.

   Met de optie &quot;Gebruikersvolgorde&quot; worden de kaarten geretourneerd in de volgorde waarin ze handmatig zijn ingesteld, voordat er andere sorteeropties zijn toegepast. Dit is de standaardsortering voor de kolommen.

1. Selecteren [!UICONTROL **Omgekeerde volgorde**] om de kolommen in omgekeerde volgorde van de sorteeroptie te sorteren.

   De pijl op het sorteerpictogram geeft aan of de kolommen in oplopende of aflopende volgorde worden gesorteerd.

   Wanneer een andere sortering dan de standaardinstelling wordt toegepast, wordt een indicator weergegeven op het sorteerpictogram ![Sorteren toegepast](assets/sort-applied-boards.png).

   ![Sorteren op kolommen aan boord](assets/sort-by-columns-in-board.png)

## Zoeken in een board

1. Toegang tot het bord.
1. Klikken [!UICONTROL **Zoeken**] en typ een zoekterm. Druk vervolgens op Enter.

   Alle kaarten die de zoekterm bevatten, worden weergegeven.

   Klik op de X om de zoekopdracht te wissen.

   ![Kaarten in een kaart zoeken](assets/boards-searchbox.png)
