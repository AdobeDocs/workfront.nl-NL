---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Een herhaling in een werkstroom maken
description: Een herhaling is een ingestelde hoeveelheid tijd die is gereserveerd voor het voltooien van het werk. Sommige teams kunnen een herhaling als sprint verwijzen.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 563e0f443ecef9ee99e9f9bfb5a0d579aa50cef4
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Een herhaling in een werkstroom maken

{{highlighted-preview}}

Een herhaling is een ingestelde hoeveelheid tijd die is gereserveerd voor het voltooien van het werk. Sommige teams kunnen een herhaling als sprint verwijzen.

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
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een herhaling in een werkstroom maken

{{step1-to-boards}}

1. Open de werkstroom waar u de herhaling wilt toevoegen. Als u een werkstroom wilt openen, klikt u op [!UICONTROL **Werkstroom weergeven**].
1. Maak een herhaling met een van de volgende methoden:

   * Klik op het tabblad Kaartlijst in de iteratieweergave op [!UICONTROL **Herhaling maken**].
   * Klik op het tabblad Kaartlijst in de lijstweergave op [!UICONTROL **Herhaling maken**].
   * Klik op het tabblad Borden op [!UICONTROL **Tekengebied toevoegen**] en selecteert u [!UICONTROL **Interferatieproces**] als de bordsjabloon. Open vervolgens het herhalingsgebied en klik op [!UICONTROL **Herhalingen configureren**].

1. Voeg de volgende informatie toe in het dialoogvenster Interventiedetails:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Iteration name]</strong></td> 
      <td>De naam van de herhaling, bijvoorbeeld "Afdrukken 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Iteration length]</strong></td> 
      <td>De lengte van de herhaling, in dagen, weken of maanden.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Start date]</strong></td> 
      <td>De datum waarop de herhaling begint. De einddatum wordt automatisch ingevoerd op basis van de herhalingslengte.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken [!UICONTROL **Opslaan**].

   De herhaling wordt nu weergegeven in de herhalingsweergave van de kaartlijst en in het metriekgebied op het iteratiebord.

   Als u kaarten aan een herhaling wilt toevoegen, raadpleegt u [De kaartlijst gebruiken](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Een bestaande herhaling bewerken

1. Als u een werkstroom wilt openen, klikt u op [!UICONTROL **Werkstroom weergeven**].
1. Open de herhaling op een van de volgende manieren:

   * Klik op het tabblad Kaartlijst in de iteratieweergave op de knop [!UICONTROL **Details van herhaling**] pictogram ![Details van herhaling](assets/iteration-details-button.png).
   * Klik in het iterboard op de knop [!UICONTROL **Details van herhaling**] pictogram ![Details van herhaling](assets/iteration-details-button.png) in het metriegebied op de hoogste juiste.

1. In de [!UICONTROL Iteration Configuration] de herhaling naar wens bewerken.
1. Als u de naam van de herhaling wilt wijzigen, vouwt u [!UICONTROL **Details van herhaling**].

   Nadat een herhaling is gestart, kunt u alleen de naam van de herhaling wijzigen en niet de datum- of herhalingslengte.

1. <span class="preview">Om doelstellingen aan de herhaling toe te voegen, breid uit [!UICONTROL **Doelen**].</span>
1. <span class="preview">Klikken [!UICONTROL **Doel toevoegen**] en typ de naam van het doel.</span>

   <span class="preview">Als doelen tijdens de herhaling zijn voltooid, kunt u het selectievakje inschakelen om ze te markeren als voltooid of op de knop **Verwijderen** pictogram ![Pictogram Verwijderen](assets/delete.png) om een doel te verwijderen. Het metriegebied op het hoogste recht van de herhaling toont hoeveel doelstellingen bestaan en hoeveel zijn voltooid.</span>

<!--
<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Een herhaling verwijderen

1. Klik op de knop [!UICONTROL **Kaartlijst**] in de werkstroom en opent u de herhalingsweergave.
1. Klik op de knop **Verwijderen** pictogram ![Pictogram Verwijderen](assets/delete.png) naast de herhaling.
1. Klikken [!UICONTROL **Herhaling verwijderen**] in het bevestigingsbericht.
