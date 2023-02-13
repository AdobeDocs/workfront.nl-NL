---
navigation-topic: financials
title: Factureringsrecords maken
description: Naast het opzetten van inkomsten en het volgen van uitgaven, kunt u het facturerings verslagen over een project voor informatie tot stand brengen die in rekening moet worden gebracht.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 0%

---

# Factureringsrecords maken

Naast het opzetten van inkomsten en het volgen van uitgaven, kunt u het facturerings verslagen over een project voor informatie tot stand brengen die in rekening moet worden gebracht.

U kunt geen factureringsverslagen voor taken tot stand brengen. U kunt alleen factureringsrecords voor projecten maken.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor het project beheren met beheerdersmachtigingen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overzicht van factureringsrecords

Factureringsverslagen worden gecreeerd als gehechtheid aan een project en bevatten financiële gegevens van het project evenals wat financiële informatie voor de taken in een project.

Overweeg het volgende wanneer u factureringsrecords wilt gebruiken:

* U maakt een factureringsrecord wanneer u een bedrag dat betrekking heeft op het project, wilt factureren aan een externe leverancier of partner. Naast het factureren van een vast bedrag aan een externe bron, zijn er tijden wanneer u het bedrag van het werk aan het project (van geregistreerde uren) aan een externe contractant moet factureren, evenals de gemaakte kosten of het bedrag van vaste inkomsten. U kunt al deze gegevens in hetzelfde factureringsrecord opnemen.
* Als een factureringsrecord eenmaal is ingesteld op Met factuur, kan het niet worden bewerkt.

   >[!IMPORTANT]
   >
   >Dit is belangrijk wanneer uw tarieven variëren en u de opbrengst en de uitgaveninformatie over uw project wilt sluiten. Als u deze aan een factureringsrecord toevoegt en als factureringsrecord markeert, wordt de record niet bijgewerkt wanneer de tarieven in uw systeem worden bijgewerkt.

* Een project met factureringsverslagen die zijn gemarkeerd als Met factuur kan niet worden verwijderd.

## Een factureringsrecord maken

1. Navigeer naar een project.
1. Klikken **Factureringsgegevens** in het linkerdeelvenster.

   Deze sectie bevindt zich mogelijk onder **Meer weergeven**.

1. Met **Gegevens factureringsrecord** geselecteerd in het linkerpaneel, klik **Nieuwe factureringsrecord**.
1. In de **Nieuwe factureringsrecord** Geef de volgende informatie op in het vak dat wordt weergegeven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Dit is een verplicht veld. Geef een beschrijving voor de factureringsrecord op om het doel of de intentie van deze record te weerspiegelen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Factureringsstatus</td> 
      <td> <p>Selecteren <strong>Niet gefactureerd</strong>, als deze record nog niet is gefactureerd.</p> <p>Selecteren <strong>Gefactureerd</strong> wanneer de factureringsrecord wordt gefactureerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Factureringsdatum</td> 
      <td>Selecteer de datum waarop deze factureringsrecord wordt gefactureerd door op het kalenderpictogram te klikken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inkoopordernummer</td> 
      <td>Als er een Inkoopordernummer is dat aan dit factureringsrecord is gekoppeld, geeft u deze informatie op in dit veld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Factuur-id</td> 
      <td>Als er een factuur is gekoppeld aan dit factureringsrecord, geeft u deze informatie in dit veld op.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Extra bedrag</td> 
      <td>Voer de vaste hoeveelheid factureringsrecord in. Dit is het bedrag u van plan bent om een externe klant, een aannemer of een partner voor dit project in rekening te brengen. Dit bedrag kan niet worden gewijzigd nadat de status van de factureringsrecord is gewijzigd in Facturering.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Onder **Aangepaste Forms**, selecteert u een aangepast formulier voor factureringsrecords dat u aan de factureringsrecord wilt toevoegen.

   U (of een andere gebruiker met toegang tot aangepaste formulieren) moet een aangepaste factureringsrecord maken voordat u deze hier kunt selecteren. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Voor informatie over het maken van aangepaste formulieren raadpleegt u [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   U kunt deze stap herhalen om andere aangepaste formulieren toe te voegen die u nodig hebt voor de factureringsrecord.

1. Klikken **Opslaan.**

   De factureringsrecord wordt gemaakt. Volg de stappen in de volgende subsectie om Billable Hours, Expenses and Fixed Revenues op te nemen in het factureringsdossier.

## Opnemen van factureerbare uren, kosten en vaste inkomsten in een factureringsbestand

* [Billable Hours opnemen in een factureringsrecord](#include-billable-hours-in-a-billing-record)
* [Facultatieve uitgaven opnemen in een factureringsrecord](#include-billable-expenses-in-a-billing-record)
* [Vaste inkomsten opnemen in een factureringsbestand](#include-fixed-revenues-in-a-billing-record)

### Billable Hours opnemen in een factureringsrecord {#include-billable-hours-in-a-billing-record}

U kunt uren omvatten die het programma geopend taken, kwesties, of het project in uw het facturerings verslagen zijn.\
Als de gebruiker die de uren of hun Primaire Rol van de Taak registreert met het Factureren per Tarief van het Uur wordt geassocieerd, wordt de opbrengst van deze uren toegevoegd aan het factureringsverslag.

* [Welke uren kunnen aan een factureringsverslag worden toegevoegd](#what-hours-can-be-added-to-a-billing-record)
* [Uren toevoegen aan een factureringsrecord](#add-hours-to-a-billing-record)

#### Welke uren kunnen aan een factureringsverslag worden toegevoegd {#what-hours-can-be-added-to-a-billing-record}

U kunt uren aan een factureringsverslag toevoegen wanneer aan de volgende voorwaarden wordt voldaan:

* De taken, de kwesties, of het project hebben het programma geopende uren.
* Het type uur van de geregistreerde uren is duidelijk als Telling als Ontvangsten.

   Raadpleeg het artikel voor meer informatie over het type uren [Uurtypen beheren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Alle uren die voor kwesties of voor het project worden geregistreerd kunnen aan een het facturerings verslag worden toegevoegd als de gebruiker die de tijd registreert een Facturering per het uurtarief verbonden aan hen of hun Primaire Rol van de Baan heeft.
* Als de uren op een taak worden geregistreerd, moet de taak het volgende Type van Ontvangsten hebben:

   * Het type van Inkomsten kan niet worden geplaatst aan Niet Facultatief.
   * Als het Type van Inkomsten aan Uur van de Gebruiker wordt geplaatst, moet de gebruiker die de tijd registreert een Facturering per Tarief hebben die in hun profiel wordt geplaatst.
   * Als het type van Inkomsten aan Rol Hourly wordt geplaatst, moet de Primaire Rol van de gebruiker die de tijd registreert een Facturering per Uuretarief hebben.

      >[!NOTE]
      >
      >U kunt factureringstarieven voor baanrollen op het projectniveau met voeten treden.\
      >Voor meer informatie over het met voeten treden van de tarieven van het het factureren van de baanrol, zie de sectie &quot;het Overschrijven van de Facturering van de Rol van de Baan op het Niveau van het Project&quot;in het artikel [Overzicht van het overschrijven van de Billing Rates van de Rol en het berekenen van Inkomsten op een project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Indien **Voor dit project goed te keuren tijd vereisen** wordt gecontroleerd onder de Montages van het Project, dan moet de Eigenaar van het Project de geregistreerde uren goedkeuren.\
   Raadpleeg het artikel voor meer informatie over het vereisen van goedkeuring over projecturen [Tijd vereisen om te worden goedgekeurd voor een project](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Uren toevoegen aan een factureringsrecord {#add-hours-to-a-billing-record}

U voegt als volgt factureerbare uren toe aan een factureringsrecord:

1. Ga naar het project met de factureringsverslagen.
1. Klikken **Factureringsgegevens** in het linkerdeelvenster.

   Deze sectie bevindt zich mogelijk onder **Meer weergeven**.

1. Klik op de knop **Beschrijving** van een factureringsrecord om de **Gegevens factureringsrecord** tab.

1. Klikken **Billable Hours** in het linkerdeelvenster.
1. Als er uren zijn die in een factureringsrecord kunnen worden opgenomen, klikt u op **Uren toevoegen**.\
   De **Billable Hours toevoegen** wordt geopend.

   >[!NOTE]
   >
   >Als er geen uren worden geregistreerd of als de geregistreerde uren niet aan de voorwaarden voldoen die aan een factureringsverslag moeten worden toegevoegd, **Uren toevoegen** wordt niet weergegeven. Zie de sectie voor meer informatie over de uren die kunnen worden geregistreerd bij een factureringsrecord [Welke uren kunnen aan een factureringsverslag worden toegevoegd](#what-hours-can-be-added-to-a-billing-record) in dit artikel.

1. Selecteer de uren die u in de factureringsrecord wilt opnemen en klik op **Uren toevoegen**.\
   De werkelijke kosten van de uren worden toegevoegd als de **Billable Hours** bedrag aan **Totaal factureringsrecord**.

1. (Optioneel) Klik op **Factuurgegevens** om de **Billable Hours** en **Totaal factureringsrecord** bedragen. U kunt het totaal van het factureringsverslag in de kopbal van het het facturerings verslag ook zien.

### Facultatieve uitgaven opnemen in een factureringsrecord {#include-billable-expenses-in-a-billing-record}

Als u Billable Uitgaven aan het het facturerings verslag toevoegt, zorg de uitgaven op de taken ervoor en het project zijn duidelijk als Billable. Uitgaven die niet als Billable worden gemerkt zijn niet beschikbaar om in een factureringsverslag toe te voegen. Raadpleeg het artikel voor meer informatie over het toevoegen van kosten [Projectkosten beheren](../../../manage-work/projects/project-finances/manage-project-expenses.md).

U kunt als volgt factureringskosten aan een factureringsrecord toevoegen:

1. Ga naar het project met de factureringsverslagen.
1. Klikken **Factureringsgegevens** in het linkerdeelvenster.

   Mogelijk moet u op **Meer weergeven** vervolgens **Factureringsgegevens**.

1. Klik op de knop **Beschrijving** van een factureringsrecord om de **Gegevens factureringsrecord** tab.

1. Klikken **Facultatieve kosten** in het linkerdeelvenster.
1. (Voorwaardelijk) als u uitgaven aan uw taken of het project hebt toegevoegd en hen als Billable hebt gemerkt, klik **Uitgaven toevoegen**.

   >[!NOTE]
   >
   >Als u kosten hebt maar niet als Billable worden gemerkt, **Uitgaven toevoegen** wordt niet weergegeven. Alleen factureerbare uitgaven met een werkelijk bedrag groter dan nul komen in aanmerking om in een factureringsrecord te worden opgenomen.

1. Selecteer de factuurelatiekosten die beschikbaar zijn om aan het factureringsverslag toe te voegen, dan klik **Uitgaven toevoegen**.\
   Het werkelijke bedrag van de kosten wordt toegevoegd als de **Facultatieve kosten** bedrag aan **Totaal factureringsrecord**.

1. (Optioneel) Klik op **Factuurgegevens** om de **Facultatieve kosten** en **Totaal factureringsrecord** bedragen. U kunt het totaal van het factureringsverslag in de kopbal van het het facturerings verslag ook zien.

### Vaste inkomsten opnemen in een factureringsbestand {#include-fixed-revenues-in-a-billing-record}

U kunt vaste inkomsten toevoegen aan uw factureringsgegevens als u taken hebt waarvoor vaste inkomsten beschikbaar zijn. Er zijn geen andere typen taken of projectinkomsten beschikbaar die in een factureringsrecord kunnen worden toegevoegd. Voor meer informatie over opbrengsttypes, zie [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) sectie in [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Om vaste opbrengsten aan een factureringsverslag toe te voegen:

1. Ga naar het project met de factureringsverslagen.
1. Klikken **Factureringsgegevens** in het linkerdeelvenster.

   Mogelijk moet u op **Meer weergeven** vervolgens **Factureringsgegevens**.

1. Klik op de knop **Beschrijving** van een factureringsrecord om de **Gegevens factureringsrecord** tab.

1. Selecteer **Vaste inkomsten** tab.
1. Als u vaste inkomsten hebt toegevoegd aan uw taken, klikt u op **Vaste inkomsten toevoegen**.

   >[!NOTE]
   >
   >Als u inkomstenbedragen voor taken hebt maar niet als &quot;Vast&quot;gemerkt, **Vaste inkomsten toevoegen** wordt niet weergegeven.

1. Selecteer de taken waarvan u de vaste inkomsten in de factureringsrecord wilt opnemen en klik vervolgens op **Taken toevoegen**.\
   De **Vaste inkomsten** het aantal taken dat als de **Facultatieve inkomsten** bedrag aan **Totaal factureringsrecord**.

1. (Optioneel) Klik op **Factuurgegevens** om de **Facultatieve inkomsten** en **Totaal factureringsrecord** bedragen. U kunt het totaal van het factureringsverslag in de kopbal van het het facturerings verslag ook zien.

## Een factureringsrecord bewerken

Nadat u een factureringsrecord hebt gemaakt en uren, uitgaven en inkomsten in de factureringsrecord hebt opgenomen, kunt u bepaalde gegevens in de bestaande record bewerken voordat deze als factureringsgegevens worden gemarkeerd.

1. Ga naar de factureringsrecord.
1. Met **Gegevens factureringsrecord** in het linkerdeelvenster geselecteerd, gegevens bewerken in alle beschikbare velden

   of

   Klik op de knop **Pictogram Bewerken** ![](assets/edit-icon.png) in de rechterbovenhoek, dan geef informatie in om het even welke beschikbare gebieden uit.

   Werk het volgende bij:

   * **Beschrijving**
   * **Factureringsstatus**

      >[!TIP]
      >
      >Als u **Gefactureerd** Voor de Factureringsstatus, kan het het facturerings verslag niet worden uitgegeven, nadat u uw veranderingen bewaart.

   * **Factureringsdatum**
   * **Inkoopordernummer**
   * **Factuur-id**
   * **Extra bedrag**

   De volgende velden kunnen niet worden bewerkt:

   * **Billable Hours:** Het totaal van de werkelijke inkomsten van de uren die in de factureringsgegevens zijn opgenomen. Zie de sectie voor meer informatie over het opnemen van uren in een factureringsrecord [Billable Hours opnemen in een factureringsrecord](#include-billable-hours-in-a-billing-record) in dit artikel.

   * **Facultatieve kosten**: Het totaal van het werkelijke bedrag van de in de factureringsstaat opgenomen factureringskosten. Zie de sectie voor meer informatie over het opnemen van factureerbare kosten in een factureringsrecord [Facultatieve uitgaven opnemen in een factureringsrecord](#include-billable-expenses-in-a-billing-record) in dit artikel.

   * **Facultatieve inkomsten**: The total of the Fixed Revenue of the tasks included in the facilling record. Zie de sectie voor meer informatie over het opnemen van vaste inkomsten in een factureringsrecord [Vaste inkomsten opnemen in een factureringsbestand](#include-fixed-revenues-in-a-billing-record) in dit artikel.

   * **Totaal factureringsrecord**: Het totaal van alle factureerbare bedragen. Dit wordt berekend aan de hand van de volgende formule:

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. Klikken **Opslaan***Wijzigingen**.
