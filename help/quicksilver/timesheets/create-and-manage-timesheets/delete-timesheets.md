---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdschema's in Adobe Workfront verwijderen
description: De wijzigingen die u aanbrengt in een tijdlijnprofiel, zijn niet onmiddellijk van kracht voor de momenteel bestaande tijdbladen, zoals uitgelegd in Create, geef, en wijs timesheet profielen uit. Als u de wijzigingen zichtbaar wilt maken op bestaande tijdbladen, moet u de tijdbladen verwijderen die zijn gegenereerd en nieuwe tijdbladen genereren. Dit is alleen van toepassing op tijdbladen die zijn gegenereerd door tijdbladprofielen aan gebruikers te koppelen.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Tijdschema&#39;s in Adobe Workfront verwijderen

De wijzigingen die u aanbrengt in een tijdlijnprofiel, zijn niet onmiddellijk van kracht voor de huidige bestaande tijdbladen, zoals wordt uitgelegd in [Werkbladprofielen maken, bewerken en toewijzen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Als u de wijzigingen zichtbaar wilt maken op bestaande tijdbladen, moet u de tijdbladen verwijderen die zijn gegenereerd en nieuwe tijdbladen genereren. Dit is alleen van toepassing op tijdbladen die zijn gegenereerd door tijdbladprofielen aan gebruikers te koppelen.

>[!NOTE]
>
>De chronologiebladen die manueel zijn gecreeerd kunnen niet worden opnieuw gemaakt door timesheets te regenereren, tenzij de gebruikers met een timesheet profiel zijn geassocieerd aangezien timesheet manueel werd gecreeerd. Als u een handmatig gemaakt tijdblad verwijdert, kunnen er gegevens verloren gaan. Voor informatie over het creëren van één enkele timesheets, zie [Een timesheet voor eenmalig gebruik maken](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Adobe Workfront-beheerders of groepsbeheerders kunnen tijdbladen voor iedereen in het systeem genereren. Voor meer informatie over manueel het produceren van timesheets, zie:

* [Tijdbladen handmatig genereren](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [De profielen van een groep maken en beheren](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* U kunt een verwijderde tijdpagina niet herstellen.
>* Wij adviseren dat u voorbij timesheets niet schrapt omdat zij niet automatisch gebaseerd op timesheet profielen worden geproduceerd. U kunt de huidige en toekomstige tijdbladen verwijderen en hen manueel produceren als u de veranderingen in uw timesheet profielen onmiddellijk zichtbaar in nieuwe chronologie wilt zijn.
>* Wanneer u timesheets schrapt, worden de uren tegen taken, kwesties, en projecten worden geregistreerd niet geschrapt. Alleen de algemene uren worden met de tijdpagina verwijderd. In een afzonderlijke tekstredacteur, schrijf welke Algemene Uren met timesheet worden geassocieerd. Nadat timesheet wordt geschrapt, kunt u hen in nieuwe timesheet dan registreren.
>


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
   <td> <p>U moet administratieve toegang tot Timesheets hebben. </p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Tijdschema&#39;s in een lijst verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Timesheets**. De **Alles** is standaard geselecteerd en worden alle tijdbladen weergegeven die u kunt bekijken.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optioneel) Voer een van de volgende handelingen uit om het filter in de lijst met tijdbladen bij te werken:

   * Selecteren **Goedkeuringen van mijn tijdsplaat** in de rechterbovenhoek van de pagina om alleen de door u goedgekeurde tijdbladen weer te geven

      of

      Selecteren **Mijn tijdbladen** om alleen uw tijdbladen weer te geven.

      Dit past Mijn Goedkeuringen Timesheet of de Mijn filters Timesheet op de lijst van timesheets toe.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klik op het pictogram Filter ![](assets/filter-nwepng.png) om een ander filter toe te passen, of creeer nieuwe. Voor informatie over het maken of bijwerken van filters raadpleegt u [Filters maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   De Mijn Goedkeuringen Timesheet en Mijn opties Timesheets tonen niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn Goedkeuringen Timesheet en de Mijn filters van Timesheets van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde. Zie de volgende artikelen voor meer informatie:
   * [Filters, weergaven en groepen aanpassen met een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optioneel) Klik op de knop **Weergave** ![](assets/view-icon.png) of **Groepering** ![](assets/grouping.png) pictogrammen om een andere weergave of groep toe te passen of om een nieuwe weergave of groep te maken.

   Zie de volgende artikelen voor informatie over het maken van filters, weergaven of groepen:

   * [Filters maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Weergaven maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Groepen maken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecteer een of meerdere tijdbladen die u wilt verwijderen en klik op de knop **Verwijderen**  ![](assets/delete.png) boven aan de lijst met tijdbladen.

1. Klikken **Verwijderen**.

   De geselecteerde tijdbladen worden verwijderd en kunnen niet worden hersteld.

   Om nieuwe timesheets te produceren, zorg ervoor dat de gebruikers met een timesheet profiel worden geassocieerd en vraag de beheerder van Workfront of een groepsbeheerder om nieuwe timesheets te produceren.

   Raadpleeg de volgende secties voor meer informatie:

   * [Werkbladprofielen maken, bewerken en toewijzen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Tijdbladen handmatig genereren](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [De profielen van een groep maken en beheren](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Een timesheet verwijderen uit de pagina met tijdlijnen

1. Klik op de knop [!UICONTROL **Hoofdmenu**] pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.
1. Klik op de tijdpagina die u wilt verwijderen om deze te openen.
1. Klik op de knop [!UICONTROL **Meer**] pictogram ![](assets/more-icon.png) rechts van de naam van de tijdpagina klikt u op **Verwijderen**.

   ![Tijdschema verwijderen uit pagina met tijdlijnen](assets/delete-timesheet-from-timesheet-page.png)
1. Klikken [!UICONTROL **Verwijderen**] ter bevestiging.

   Het tijdschema wordt verwijderd en kan niet worden hersteld.
