---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdlijngegevens bewerken
description: Als gebruiker met administratieve toegang tot Timesheets, kunt u informatie over bestaande timesheets in Adobe Workfront uitgeven. U kunt bijvoorbeeld de eigenaar, de fiatteurs of het tijdframe van de tijdpagina bewerken.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Tijdlijngegevens bewerken

Als gebruiker met administratieve toegang tot Timesheets, kunt u informatie over bestaande timesheets in Adobe Workfront uitgeven. U kunt bijvoorbeeld de eigenaar, de fiatteurs of het tijdframe van de tijdpagina bewerken.

U kunt informatie op één enkel timesheet uitgeven, of u kunt veelvoudige timesheets in bulk uitgeven.

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet administratieve toegang tot Timesheets hebben. </p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Tijdschema&#39;s bewerken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Timesheets**.

   De **Alles** Het filter wordt standaard geselecteerd, zodat alle tijdbladen worden weergegeven die u kunt bekijken.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optioneel) Klik op de knop **zoeken** pictogram ![](assets/search-icon.png) en typ een trefwoord en zoek naar een specifieke tijdlijn. U kunt bijvoorbeeld zoeken naar een tijdlijnframe of de naam van de eigenaar.

1. (Optioneel) Voer een van de volgende handelingen uit om het filter in de lijst met tijdbladen bij te werken:

   * Selecteren **Goedkeuringen van mijn tijdsplaat** in de rechterbovenhoek van de pagina om alleen de door u goedgekeurde tijdbladen weer te geven

      of

      Selecteren **Mijn tijdbladen** om alleen uw tijdbladen weer te geven.

      Dit past Mijn Goedkeuringen Timesheet of de Mijn filters Timesheet op de lijst van timesheets toe.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klik op het pictogram Filter ![](assets/filter-nwepng.png) om een ander filter toe te passen, of creeer nieuwe. Voor informatie over het maken of bijwerken van filters raadpleegt u [Filters maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >De Mijn Goedkeuringen Timesheet en Mijn opties Timesheets tonen niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn Goedkeuringen Timesheet en de Mijn filters van Timesheets van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde. Zie de volgende artikelen voor meer informatie:
   * [Filters, weergaven en groepen aanpassen met een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optioneel) Klik op de knop **Weergave** ![](assets/view-icon.png) of **Groepering** ![](assets/grouping.png) pictogrammen om een andere weergave of groep toe te passen of om een nieuwe weergave of groep te maken.

   Zie de volgende artikelen voor informatie over het maken van filters, weergaven of groepen:

   * [Filters maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Weergaven maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Groepen maken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecteer een of meerdere tijdbladen en klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) boven aan de lijst met tijdlijnen.
1. Geef de volgende informatie weer of geef deze op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Eigenaar</strong> </td> 
      <td> <p>Dit is de naam van de gebruiker waarvoor timesheet werd gecreeerd. U kunt dit veld niet bewerken. </p> <p>Het veld wordt niet weergegeven wanneer u meerdere tijdbladen selecteert. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Begindatum</strong> </td> 
      <td>Dit is de begindatum van het tijdspad.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Einddatum</strong> </td> 
      <td> Dit is de einddatum van het tijdschema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fiatteurs</strong> </td> 
      <td> <p>Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. Alleen gebruikers met beheerdersrechten voor tijdbladen kunnen als fiatteurs worden ingesteld. </p> <p>Voor meer informatie over administratieve rechten op tijdspagina raadpleegt u <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p>Voer de namen van de fiatteurs van de tijdpagina in en selecteer deze wanneer ze in de lijst worden weergegeven.</p> <p>U kunt veelvoudige fiatteurs op een timesheet hebben. In dat geval wordt het tijdspad, nadat een van de fiatteurs het tijdsplaat heeft goedgekeurd, als volgt gemarkeerd <strong>Gesloten</strong> en verdwijnt uit de lijst van goedkeuringen volgens het tijdschema van alle resterende fiatteurs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kan tijd bewerken</strong> </td> 
      <td> <p>Selecteer deze optie als fiatteurs de uren op het tijdblad mogen bewerken.</p> <p>Deze optie is niet beschikbaar wanneer u meerdere tijdbladen selecteert. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Overwerk</span> </td> 
      <td> <p>U kunt ervoor kiezen om het vak Overuren op het tijdblad te verbergen.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op Opslaan.
