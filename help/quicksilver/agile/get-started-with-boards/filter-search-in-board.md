---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filteren en zoeken in een kaart
description: U kunt een bord filteren om alleen bepaalde kaarten weer te geven.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '668'
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

Wanneer de filters worden toegepast, wordt een indicator getoond op de raad ![ die Filter op raad ](assets/boards-filterapplied-30x30.png) wordt toegepast. Klik op **[!UICONTROL Clear All]** om alle filters van het bord te verwijderen en klik op het pictogram Samenvouwen om het filterdeelvenster te sluiten.

![ het paneel van de Filter ](assets/boards-all-filters-collapsed-0823.png)

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

## Een bord filteren op toewijzing

{{step1-to-boards}}

1. Toegang tot een bord. Voor informatie, zie [ creeer of geef een raad ](../../agile/get-started-with-boards/create-edit-board.md) uit.
1. Klik [!UICONTROL **Filter**], breid de [!UICONTROL Members] sectie uit, en selecteer de persoon of de mensen waarvan kaarten u wilt zien. U kunt ook niet-toegewezen kaarten weergeven.

   ![ Filter door lid ](assets/boards-filter-by-assignees-0822.png)

## Een board filteren op tags

1. Toegang tot het bord.
1. Klik [!UICONTROL **Filter**], breid de [!UICONTROL Tags] sectie uit, en selecteer de markeringen u wilt zien.

   ![ Filter door markering ](assets/boards-filter-by-tags-0822.png)

## Een bord filteren op status

1. Toegang tot het bord.
1. Klik [!UICONTROL **Filter**], breid de [!UICONTROL Statuses] sectie uit, en selecteer de statustypes u wilt zien.

   U kunt ook voltooide kaarten verbergen.

   ![ Filter door status ](assets/boards-filter-by-status-0822.png)

## Een board filteren op de datum van de datum

1. Toegang tot het bord.
1. Klik [!UICONTROL **Filter**], breid de [!UICONTROL Due Date] sectie uit, en selecteer de datumopties u wilt zien.

   Alleen kaarten in de geselecteerde datumbereiken worden weergegeven.

   ![ Filter door te zijn datum ](assets/boards-filter-by-due-date-0822.png)

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

## Een bord filteren op verbinding

1. Toegang tot het bord.
1. Klik [!UICONTROL **Filter**], breid de [!UICONTROL Connection] sectie uit, en selecteer de [!DNL Workfront] projecten voor de verbonden kaarten u wilt zien.

   U kunt ook kaarten weergeven die niet zijn verbonden met een project.

   ![ Filter door verbinding ](assets/boards-filter-by-connection.png)

## Sorteren op een board

Wanneer u een optie selecteert om op te sorteren, worden alle kolommen gesorteerd. U kunt geen enkele kolom sorteren en de kolom voor het aantal kolommen of de kolom voor het aantal kolommen wordt niet gesorteerd.

1. Toegang tot het bord.
1. Klik [!UICONTROL **Soort door**] en selecteer [!UICONTROL **Naam**], [!UICONTROL **Verdachte datum**], [!UICONTROL **Schatting**], [!UICONTROL **Status**], of [!UICONTROL **Verbinding**].

   De verbinding (projectnaam) is slechts op verbonden kaarten van toepassing, en de andere opties zullen zowel verbonden als ad hoc kaarten in de kolommen sorteren.

   Met de optie &quot;Gebruikersvolgorde&quot; worden de kaarten geretourneerd in de volgorde waarin ze handmatig zijn ingesteld, voordat er andere sorteeropties zijn toegepast. Dit is de standaardsortering voor de kolommen.

1. Selecteer [!UICONTROL **omgekeerde orde**] om de kolommen in omgekeerde orde van de soortoptie te sorteren.

   De pijl op het sorteerpictogram geeft aan of de kolommen in oplopende of aflopende volgorde worden gesorteerd.

   Wanneer een soort buiten het gebrek wordt toegepast, wordt een indicator getoond op het soortpictogram ![ toegepaste Soort ](assets/sort-applied-boards.png).

   ![ Soort door kolommen op een raad ](assets/sort-by-columns-in-board.png)

## Zoeken in een board

1. Toegang tot het bord.
1. Klik [!UICONTROL **Onderzoek**] en typ een onderzoekstermijn. Druk vervolgens op Enter.

   Alle kaarten die de zoekterm bevatten, worden weergegeven.

   Klik op de X om de zoekopdracht te wissen.

   ![ Onderzoek naar kaarten in een raad ](assets/boards-searchbox.png)
