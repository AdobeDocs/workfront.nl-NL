---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Een eenmalig te gebruiken tijdspagina maken
description: U kunt manueel tot een enig-gebruik timesheet leiden als u een timesheet wilt die niet terugkeert. Wanneer de einddatum van timesheet wordt bereikt en u meer timesheets nodig hebt, moet u nieuwe degenen creëren.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 0%

---

# Een timesheet voor eenmalig gebruik maken

<!--Audited: 6/2025-->

U kunt manueel tot een enig-gebruik timesheet leiden als u een timesheet wilt die niet terugkeert. Wanneer de einddatum van timesheet wordt bereikt en u meer timesheets nodig hebt, moet u nieuwe degenen creëren.

Voor informatie over het creëren van een timesheet profiel dat terugkomende timesheets voor uw gebruikers zonder enige verdere interventie van u (geadviseerd) produceert, [ creeert, uitgeeft, en toewijst timesheet profielen ](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Voor informatie over manueel het produceren van timesheets voor alle gebruikers in het systeem die met een timesheet profiel worden geassocieerd, zie [ manueel timesheets ](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md) produceren.

>[!NOTE]
>
>* Tijdschema&#39;s voor eenmalig gebruik kunnen niet worden gemaakt voor groepen.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Wanneer het creëren van enig-gebruik timesheet, kunt u geen specifieke algemene uurtypes selecteren om in uw timesheet te omvatten. Alle typen van algemene uren die in uw systeem worden geactiveerd, worden in handmatig gemaakte tijdbladen weergegeven.
>
>  Als u slechts bepaalde algemene uurtypes aan vertoning in uw timesheets wilt selecteren, gebruik een timesheet profiel. Voor meer informatie over timesheet profielen, zie [ creëren, uitgeven, en toewijzen timesheet profielen ](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard </p>
   <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>U moet administratieve toegang tot Chronologie hebben. </p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een timesheet voor eenmalig gebruik maken

{{step1-to-timesheets}}

Het **Al** filter wordt geselecteerd door gebrek. Alle tijdbladen die u kunt bekijken, worden dan weergegeven.

![ lijst van Tijdopnemers met één geselecteerd timesheet ](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optioneel) Voer een van de volgende handelingen uit om het filter in de lijst met tijdbladen bij te werken:

   * Selecteer **Mijn Goedkeuringen van het Chronologie** in de hoger-juiste hoek van de pagina om slechts timesheets te bekijken die u goedkeurt

     of

     Selecteer **Mijn Chronologie** om slechts uw timesheets te bekijken.

     Dit past Mijn Goedkeuringen Timesheet of de Mijn filters Timesheet op de lijst van timesheets toe.

     ![ Mijn timesheets filterknopen op de de lijstpagina van Tijdopnemers ](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klik het **pictogram van de Filter** pictogram ![ van de Filter ](assets/filter-nwepng.png) om een verschillende filter toe te passen, of nieuwe tot stand te brengen. Voor informatie over het creëren van of het bijwerken van filters, zie [ filters in Adobe Workfront ](../../reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.

   >[!NOTE]
   >
   >De Mijn Goedkeuringen Timesheet en Mijn opties Timesheets tonen niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn Goedkeuringen Timesheet en de Mijn filters van Timesheets van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde. Zie de volgende artikelen voor meer informatie:
   > 
   >   * [ pas Filters, Weergaven, en Groepen aan gebruikend een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facultatief) klik het **pictogram van het Onderzoek ![ pictogram van het Onderzoek ](assets/search-icon.png) om een sleutelwoord te typen en naar specifieke timesheet te zoeken.** U kunt bijvoorbeeld zoeken naar een tijdlijntijdframe met de naam van de eigenaar.

1. (Facultatief) klik de **pictogrammen van de Mening** ![ Mening ](assets/view-icon.png) of **Groepering** ![ het pictogram van de Groepering ](assets/grouping.png) om een verschillende mening of groepering toe te passen of nieuwe te creëren.

   Zie de volgende artikelen voor informatie over het maken van filters, weergaven of groepen:

   * [ creeer of geef filters in Adobe Workfront uit ](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [ creeer of geef meningen in Adobe Workfront uit ](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Groepen maken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klik **Nieuwe Chronologie** bij de bovenkant van de lijst van timesheets.

   Geef de volgende informatie op:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong> creeer timesheet voor </strong> </td> 
      <td>Begin ingaand de naam van de gebruiker, een baanrol, of een team voor wie u timesheet creeert, en klik hen wanneer zij in de lijst tonen.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong> Datum van het Begin </strong> </td> 
      <td>Dit is de begindatum van het tijdspad.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong> Datum van het Eind </strong> </td> 
      <td> Dit is de einddatum van het tijdschema.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong> Approvers </strong> </td> 
      <td>Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. Alleen gebruikers met beheerdersrechten voor tijdschriften kunnen worden ingesteld als fiatteurs. Voor meer informatie over timesheet administratieve rechten, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.<br> Begin ingaand de namen van timesheet fiatteurs en klik hen wanneer zij in de lijst verschijnen.<br> u kunt veelvoudige fiatteurs op een timesheet hebben. In dit geval, nadat één van de fiatteurs timesheet goedkeurt, wordt timesheet duidelijk als <strong> Gesloten </strong> en het verdwijnt van de lijst van timesheet goedkeuringen van alle resterende fiatteurs.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong> kan tijd </strong> uitgeven </td>

   <td> <p>Selecteer deze optie als fiatteurs de uren op het tijdblad mogen bewerken.</p>

   Deze optie werkt samen met **beperkt timesheet het uitgeven aan eigenaars en beheert** plaatsen in de Opstelling > de Tijdopmaak &amp; het gebied van de Uren > van de Voorkeur. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md"> timesheet en uurvoorkeur </a> vormen.

   De volgende scenario&#39;s bestaan:

   <ul>
      <li>Wanneer <b> timesheet het uitgeven aan eigenaars en beheert </b> optie wordt toegelaten:</li>
   <ul><li>De fiatteurs kunnen timesheet slechts goedkeuren en verwerpen, ongeacht of <b> tijd </b> kan uitgeven of niet wordt toegelaten. </li>
   <li>De managers van timesheet-eigenaars kunnen alleen de tijdbladen van hun directe rapporten bekijken.</li></ul>
   <li>Wanneer <b> timesheet het uitgeven aan eigenaars en beheert </b> optie wordt onbruikbaar gemaakt:</li>
   <ul><li>Wanneer <b> tijd </b> kan uitgeven wordt toegelaten, kunnen de fiatteurs voorleggen, opnieuw openen of sluiten timesheet en kunnen de tijd uitgeven.</li>
   <li>Wanneer <b> tijd </b> kan uitgeven wordt onbruikbaar gemaakt, kunnen de fiatteurs niet voorleggen, heropenen of sluiten timesheet en kunnen niet de tijd uitgeven. De fiatteurs kunnen timesheet slechts goedkeuren of verwerpen. </li>
   <li>De managers van de eigenaars van de chronologie van chronologie kunnen voorleggen, terugroepen, heropenen en hun directe rapporten uitgeven.</li></ul>
   </ul>

   <p><b>OPMERKING</b>

   Nadat u een tijdspad ter goedkeuring hebt verzonden, kunt u de uren niet meer bewerken. Om een voorgelegde timesheet aan een editable staat terug te keren, wijs timesheet terug of hebben fiatteur de timesheet verwerpen. Voor meer informatie, zie <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md"> een timesheet voor goedkeuring </a> voorleggen en <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md"> goedkeuren timesheet </a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;"> Overtime </span> </td> 
      <td>U kunt ervoor kiezen om het vak Overuren op het tijdblad te verbergen. Deze optie is standaard uitgeschakeld.</td> 
      </tr> 
      </tbody> 
   </table>

1. Klik **creëren timesheet**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Wanneer taken en problemen worden weergegeven op de tijdpagina&#39;s van de gebruiker

Een taak of een kwestie die aan een gebruiker wordt toegewezen verschijnt automatisch op timesheet van een gebruiker als de taak of de kwestie aan om het even welke volgende criteria voldoet:

* De gebruiker heeft uren op de taak of de kwestie het programma geopend
* De geplande datum van de taak of afgifte valt binnen het tijdschema
* De taak of kwestie heeft een Ware Datum van het Begin (de taak of de uitgiftestatus is lopend)
* De taak of kwestie wordt vastgezet aan timesheet
* De geplande datum van voltooiing valt binnen het datumbereik van het tijdschema en de status is bezig

Als **pre-bevolkt timesheets met ...** voorkeur (die in de voorkeur van Timesheets &amp; van het Uur wordt gevestigd) wordt geschrapt, toont timesheet kwesties en taken die een status van Bezig hebben. Voor meer informatie over de Voorkeur van Timesheets &amp; van het Uur, zie [ timesheet en uurvoorkeur ](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.
