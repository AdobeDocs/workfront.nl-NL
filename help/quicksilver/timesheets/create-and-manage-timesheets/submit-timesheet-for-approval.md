---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Een tijdschema ter goedkeuring indienen
description: Door uw tijdspagina ter goedkeuring in te dienen, krijgt uw manager inzicht in uw werkuren. De fiatteurs kunnen verifiëren dat alle geregistreerde tijd in de juiste gebieden is toegewezen en dat er gedurende de periode een voldoende aantal uren is geregistreerd.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Een tijdschema ter goedkeuring indienen

<!--Audited: 8/2024-->

Door uw tijdspagina ter goedkeuring in te dienen, krijgt uw manager inzicht in uw werkuren. De fiatteurs kunnen verifiëren dat alle geregistreerde tijd in de juiste gebieden is toegewezen en dat er gedurende de periode een voldoende aantal uren is geregistreerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td> <p>Licht of hoger </p>
   <p>Controleren of hoger </p>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en problemen weergeven of vergroten </p> </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan timesheet</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een tijdschema ter goedkeuring indienen

* [&#x200B; voorlegt een timesheet voor goedkeuring &#x200B;](#submit-a-timesheet-for-approval)
* [De status van een verzonden tijdsplaat weergeven](#view-the-status-of-a-submitted-timesheet)

### Een tijdschema ter goedkeuring indienen

Nadat een timesheet fiatteur wordt geplaatst (zoals die in de sectie [&#x200B; wordt beschreven wijs timesheet goedkeurt &#x200B;](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) in het artikel [&#x200B; een timesheet &#x200B;](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md) goed), **dicht** knoop bij de bodem van de timesheet verandert in a **voorleggen voor goedkeuring** knoop.

Een tijdschema ter goedkeuring indienen:

1. Ga naar een timesheet dat is gevormd om een fiatteur te hebben.
1. De tijd van het logboek, zoals die in [&#x200B; wordt beschreven tijd van het Logboek &#x200B;](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Klik **voorleggen voor goedkeuring** om het proces van de timesheet goedkeuring te lanceren.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   **voorlegt voor goedkeuring** knoop wordt vervangen door **goedkeuren**, **Afwijzen**, en **Recall** knopen. Het statuut van timesheet verandert in **Voorgelegd**.

   Wanneer uw timesheet voor goedkeuring wordt voorgelegd, ziet de fiatteur timesheet dat in **wordt vermeld Mijn goedkeurt** widget in het **3&rbrace; gebied van het Huis.** De volgende dingen kunnen zich voordoen:

   * Als zij het goedkeuren, verandert de **Herinnerde** knoop in **heropenen** en de updates van de timesheet status aan **Open**.
   * Als zij het verwerpen, **voorlegt voor goedkeuring** knoop vervangt de **Recall** knoop en de updates van de timesheet status aan **Verworpen**.

1. (Facultatief) klik **Herinneren** als u timesheet moet heropenen en uw tijd bijwerken. Voor informatie, zie [&#x200B; Rappel een timesheet &#x200B;](#recall-a-timesheet) sectie in dit artikel.

### De status van een verzonden tijdsplaat weergeven {#view-the-status-of-a-submitted-timesheet}

U kunt de status van een tijdblad bekijken nadat u het hebt verzonden.

Als de beheerder van Workfront de Goedkeuring van de Tijdopmaak aan Gebruiker en de Afwijzing van de Chronologie aan de gebeurtenismanagers van de Gebruiker heeft toegelaten, wordt u op de hoogte gebracht nadat timesheet wordt goedgekeurd of verworpen. Voor informatie over het toelaten van gebeurtenisberichten, zie [&#x200B; de berichttypes van de Gebeurtenis &#x200B;](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Zonder deze berichten, kunt u over de status van uw voorgelegde chronologie in het gebied van de Chronologie van Workfront leren.

U kunt als volgt de status van een tijdblad weergeven:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.
1. Klik **Tijdopnemers**. Het **Al** filter wordt geselecteerd door gebrek.

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
   >De Mijn Goedkeuringen Timesheet en Mijn opties Timesheets tonen niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn Goedkeuringen Timesheet en de Mijn filters van Timesheets van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde. Zie de volgende artikelen voor meer informatie:
   >
   >   
   >   
   >   * [&#x200B; pas Filters, Weergaven, en Groepen aan gebruikend een lay-outmalplaatje &#x200B;](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Voorwaardelijk) als u **Mijn Tijdopnemers** selecteerde, zorg ervoor dat de **Standaard** mening wordt toegepast en merk de **Status** kolom op.

   Timesheets kunnen de volgende statussen hebben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Openen</td> 
      <td> <p>Uw timesheet is momenteel open en u kunt tijd registreren. </p> <p>Er wordt een teruggeroepen tijdlijnvenster weergegeven met de status Open. Voor informatie, zie <a href="#recall-a-timesheet" class="MCXref xref"> Rappel een timesheet </a> sectie in dit artikel. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verzonden</td> 
      <td>U hebt uw tijdschema ter goedkeuring ingediend, maar het is nog niet goedgekeurd. U kunt een voorgelegde tijdkaart herinneren om het verder uit te geven. Voor informatie, zie <a href="#recall-a-timesheet" class="MCXref xref"> Rappel een timesheet </a> sectie in dit artikel. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gesloten</td> 
      <td> <p>De volgende scenario's bestaan:</p> 
       <ul> 
        <li> <p>Als de tijdpagina geen fiatteur heeft, hebt u de tijd opgeslagen en gesloten.</p> </li> 
        <li> <p>Als het tijdschema een fiatteur heeft, hebt u het ter goedkeuring ingediend en is het goedgekeurd.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geweigerd</td> 
      <td>U hebt het tijdschema ter goedkeuring ingediend en de fiatteur heeft het afgewezen.</td> 
     </tr> 
    </tbody> 
   </table>

## Een tijdblad terugdraaien {#recall-a-timesheet}

U kunt zich een overzicht herinneren dat reeds ter goedkeuring is voorgelegd. Alleen timesheets die niet zijn goedgekeurd, kunnen worden teruggeroepen.

U kunt als volgt een tijdschema weergeven:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Tijdopnemers**.
1. Klik **Mijn Tijdopnemers** in de hoger-juiste hoek van het scherm of selecteer **Mijn Tijdopnemers** van het **Filter** ![](assets/filter-nwepng.png) drop-down menu.
1. Klik het tijdkader voor een timesheet met een status van **voorgelegde**.
1. Klik **Herinneren**.

   Tijdschema wordt editable opnieuw en zijn statusveranderingen in **Open**.
