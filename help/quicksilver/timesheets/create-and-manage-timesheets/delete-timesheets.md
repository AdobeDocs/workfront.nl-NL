---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdschema's in Adobe Workfront verwijderen
description: De wijzigingen die u aanbrengt in een tijdlijnprofiel, zijn niet onmiddellijk van kracht voor de momenteel bestaande tijdbladen, zoals uitgelegd in Create, geef, en wijs timesheet profielen uit. Als u de wijzigingen zichtbaar wilt maken op bestaande tijdbladen, moet u de tijdbladen verwijderen die zijn gegenereerd en nieuwe tijdbladen genereren. Dit is alleen van toepassing op tijdbladen die zijn gegenereerd door tijdbladprofielen aan gebruikers te koppelen.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Tijdschema&#39;s in Adobe Workfront verwijderen

De veranderingen u aan een timesheet profiel aanbrengt zijn niet onmiddellijk voor de momenteel bestaande timesheets, zoals die in [&#x200B; worden verklaard creeer, geef uit, en wijs timesheet profielen &#x200B;](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe. Als u de wijzigingen zichtbaar wilt maken op bestaande tijdbladen, moet u de tijdbladen verwijderen die zijn gegenereerd en nieuwe tijdbladen genereren. Dit is alleen van toepassing op tijdbladen die zijn gegenereerd door tijdbladprofielen aan gebruikers te koppelen.

>[!NOTE]
>
>De chronologiebladen die manueel zijn gecreeerd kunnen niet worden opnieuw gemaakt door timesheets te regenereren, tenzij de gebruikers met een timesheet profiel zijn geassocieerd aangezien timesheet manueel werd gecreeerd. Als u een handmatig gemaakt tijdblad verwijdert, kunnen er gegevens verloren gaan. Voor informatie over het creëren van één enkele timesheets, zie [&#x200B; een enig-gebruik timesheet &#x200B;](../../timesheets/create-and-manage-timesheets/create-tmshts.md) creëren.

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

## Tijdschema&#39;s in een lijst verwijderen

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Tijdopnemers**. Het **Al** filter wordt geselecteerd door gebrek en het toont alle timesheets die u toegang tot mening hebt.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

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

1. Selecteer één of verscheidene timesheets die u wilt schrappen en het **pictogram van de Schrapping** ![](assets/delete.png) bij de bovenkant van de lijst van timesheets klikken.

1. Klik **Schrapping**.

   De geselecteerde tijdbladen worden verwijderd en kunnen niet worden hersteld.

   Om nieuwe timesheets te produceren, zorg ervoor dat de gebruikers met een timesheet profiel worden geassocieerd en vraag de beheerder van Workfront of een groepsbeheerder om nieuwe timesheets te produceren.

   Raadpleeg de volgende secties voor meer informatie:

   * [&#x200B; creeer, geef uit, en wijs timesheet profielen &#x200B;](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe
   * [&#x200B; produceert manueel timesheets &#x200B;](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [De profielen van een groep maken en beheren](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Een timesheet verwijderen uit de pagina met tijdlijnen

1. Klik het [!UICONTROL **Belangrijkste pictogram van het Menu**] ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.
1. Klik op de tijdpagina die u wilt verwijderen om deze te openen.
1. Klik [!UICONTROL **Meer**] pictogram ![](assets/more-icon.png) aan het recht van de timesheet naam, dan klik **Schrapping**.

   ![&#x200B; Schrap timesheet van timesheet pagina &#x200B;](assets/delete-timesheet-from-timesheet-page.png)
1. Klik [!UICONTROL **Schrapping**] om te bevestigen.

   Het tijdschema wordt verwijderd en kan niet worden hersteld.
