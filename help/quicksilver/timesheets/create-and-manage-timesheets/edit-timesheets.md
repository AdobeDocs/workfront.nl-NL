---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdlijngegevens bewerken
description: Als gebruiker met administratieve toegang tot Timesheets, kunt u informatie over bestaande timesheets in Adobe Workfront uitgeven. U kunt bijvoorbeeld de eigenaar, de fiatteurs of het tijdframe van de tijdpagina bewerken.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Tijdlijngegevens bewerken

Als gebruiker met administratieve toegang tot Timesheets, kunt u informatie over bestaande timesheets in Adobe Workfront uitgeven. U kunt bijvoorbeeld de eigenaar, de fiatteurs of het tijdframe van de tijdpagina bewerken.

U kunt informatie op één enkel timesheet uitgeven, of u kunt veelvoudige timesheets in bulk uitgeven.

>[!IMPORTANT]
>
>Als gebruikers zijn gekoppeld aan tijdlijnprofielen en de tijdbladen automatisch worden gegenereerd, weerspiegelen de wijzigingen die u aanbrengt in bestaande tijdbladen niet de tijdbladen die worden gegenereerd voor toekomstige datums. Alle automatisch gegenereerde tijdbladen beschikken over de instellingen die zijn vastgelegd in de tijdlijnprofielen. Voor meer informatie, zie [&#x200B; timesheet profielen &#x200B;](../create-and-manage-timesheets/create-timesheet-profiles.md) creëren

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td><p>Administratieve toegang tot timesheets</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tijdschema&#39;s bewerken

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Tijdopnemers**.

   Het **Al** filter wordt geselecteerd door gebrek dat alle timesheets toont die u toegang tot mening hebt.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatief) klik het **onderzoek** pictogram ![](assets/search-icon.png) en typ een sleutelwoord en onderzoek naar specifieke timesheet. U kunt bijvoorbeeld zoeken naar een tijdlijnframe of de naam van de eigenaar.

1. (Optioneel) Voer een van de volgende handelingen uit om het filter in de lijst met tijdbladen bij te werken:

   * Selecteer **Mijn Goedkeuringen van het Chronologie** in de hoger-juiste hoek van de pagina om slechts timesheets te bekijken die u goedkeurt

     of

     Selecteer **Mijn Chronologie** om slechts uw timesheets te bekijken.

     Dit past Mijn Goedkeuringen Timesheet of de Mijn filters Timesheet op de lijst van timesheets toe.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klik op het pictogram Filter ![](assets/filter-nwepng.png) om een ander filter toe te passen of een nieuw filter te maken. Voor informatie over het creëren van of het bijwerken van filters, zie [&#x200B; filters in Adobe Workfront &#x200B;](../../reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.

   >[!NOTE]
   >
   >De Mijn Goedkeuringen Timesheet en Mijn opties Timesheets tonen niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn Goedkeuringen Timesheet en de Mijn filters van Timesheets van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde. Zie de volgende artikelen voor meer informatie:
   >
   >   
   >   
   >   * [&#x200B; pas Filters, Weergaven, en Groepen aan gebruikend een lay-outmalplaatje &#x200B;](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatief) klik de **Mening** ![](assets/view-icon.png) of **Groepering** ![](assets/grouping.png) pictogrammen om een verschillende mening of groepering toe te passen of nieuwe tot stand te brengen.

   Zie de volgende artikelen voor informatie over het maken van filters, weergaven of groepen:

   * [&#x200B; creeer of geef filters in Adobe Workfront uit &#x200B;](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [&#x200B; creeer of geef meningen in Adobe Workfront uit &#x200B;](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Groepen maken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecteer één of verscheidene timesheets, dan klik **uitgeven** pictogram ![](assets/edit-icon.png) bij de bovenkant van de timesheet lijst.
1. Geef de volgende informatie weer of geef deze op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Eigenaar </strong> </td> 
      <td> <p>Dit is de naam van de gebruiker waarvoor timesheet werd gecreeerd. U kunt dit veld niet bewerken. </p> <p>Het veld wordt niet weergegeven wanneer u meerdere tijdbladen selecteert. </p> </td> 
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
      <td role="rowheader"><strong> Status </strong> </td> 
      <td> Dit is de status van het tijdspad.
      Hieronder vindt u mogelijke statusopties voor tijdschriften: 
      <ul><li><b> Open </b>: De timesheet is open en de uuringangen kunnen worden uitgegeven.</li>
      <li><b> voorgelegd </b>: Tijdschema wordt voorgelegd ter goedkeuring aan de aangewezen fiatteurs.</li>
      <li><b> Verworpen </b>: Tijdschema werd niet goedgekeurd door de fiatteurs en is nu beschikbaar opnieuw voor de gebruiker om de tijdingangen uit te geven.</li>
      <li><b> Gesloten </b>: Tijdschema wordt of gesloten door de gebruiker of goedgekeurd door de fiatteur en dientengevolge, is het nu gesloten. U kunt geen tijd aan een gesloten timesheet toevoegen.</li>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Approvers </strong> </td> 
      <td> <p>Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. Alleen gebruikers met beheerdersrechten voor tijdbladen kunnen als fiatteurs worden ingesteld. </p> <p>Voor meer informatie over timesheet administratieve rechten, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> <p>Voer de namen van de fiatteurs van de tijdpagina in en selecteer deze wanneer ze in de lijst worden weergegeven.</p> <p>U kunt veelvoudige fiatteurs op een timesheet hebben. In dit geval, nadat één van de fiatteurs timesheet goedkeurt, wordt timesheet duidelijk als <strong> Gesloten </strong> en het verdwijnt van de lijst van timesheet goedkeuringen van alle resterende fiatteurs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> kan tijd </strong> uitgeven </td> 
      <td> <p>Selecteer deze optie als fiatteurs de uren op het tijdblad mogen bewerken.</p> <p>Deze optie is niet beschikbaar wanneer u meerdere tijdbladen selecteert. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;"> Overtime </span> </td> 
      <td> <p>U kunt ervoor kiezen om het vak Overuren op het tijdblad te verbergen.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen**.
