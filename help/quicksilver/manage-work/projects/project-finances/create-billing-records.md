---
navigation-topic: financials
title: Factureringsrecords maken
description: Naast het opzetten van inkomsten en het volgen van uitgaven, kunt u het facturerings verslagen over een project voor informatie tot stand brengen die in rekening moet worden gebracht.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1898'
ht-degree: 0%

---

# Factureringsrecords maken

Naast het opzetten van inkomsten en het volgen van uitgaven, kunt u het facturerings verslagen over een project voor informatie tot stand brengen die in rekening moet worden gebracht.

U kunt geen factureringsverslagen voor taken tot stand brengen. U kunt alleen factureringsrecords voor projecten maken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten en financiële gegevens bewerken</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Machtigingen voor het project beheren met beheerdersmachtigingen</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. Klik **het Factureren Verslagen** in het linkerpaneel.

   Deze sectie zou onder **kunnen worden gevestigd tonen meer**.

1. Met **het Factureren Details van het Verslag** die in het linkerpaneel wordt geselecteerd, klik **Nieuw het Factureren Verslag**.
1. In de **Nieuwe doos van het Verslag van de Facturering** die toont, specificeer de volgende informatie:

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
      <td> <p>Selecteer <strong> niet Gevulde </strong>, als dit verslag nog niet is gefactureerd.</p> <p>Selecteer <strong> Gevulde </strong> wanneer het het facturerings verslag wordt gefactureerd.</p> </td> 
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

1. (Facultatief) onder **Eigen Forms**, selecteer een het factureren verslagen douaneformulier dat u aan het het facturerings verslag wilt toevoegen.

   U (of een andere gebruiker met toegang tot aangepaste formulieren) moet een aangepaste factureringsrecord maken voordat u deze hier kunt selecteren. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Voor informatie over het creëren van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

   U kunt deze stap herhalen om andere aangepaste formulieren toe te voegen die u nodig hebt voor de factureringsrecord.

1. Klik **sparen.**

   De factureringsrecord wordt gemaakt. Volg de stappen in de volgende subsectie om Billable Hours, Expenses and Fixed Revenues op te nemen in het factureringsdossier.

## Opnemen van factureerbare uren, kosten en vaste inkomsten in een factureringsbestand

* [ omvat Billable Uren in een het facturerings verslag ](#include-billable-hours-in-a-billing-record)
* [ omvat Facultatieve Uitgaven in een factureringsverslag ](#include-billable-expenses-in-a-billing-record)
* [Vaste inkomsten opnemen in een factureringsbestand](#include-fixed-revenues-in-a-billing-record)

### Billable Hours opnemen in een factureringsrecord {#include-billable-hours-in-a-billing-record}

U kunt uren omvatten die het programma geopend taken, kwesties, of het project in uw het facturerings verslagen zijn.\
Als de gebruiker die de uren of hun Primaire Rol van de Taak registreert met het Factureren per Tarief van het Uur wordt geassocieerd, wordt de opbrengst van deze uren toegevoegd aan het factureringsverslag.

* [ welke uren aan een het facturerings verslag kunnen worden toegevoegd ](#what-hours-can-be-added-to-a-billing-record)
* [Uren toevoegen aan een factureringsrecord](#add-hours-to-a-billing-record)

#### Welke uren kunnen aan een factureringsverslag worden toegevoegd {#what-hours-can-be-added-to-a-billing-record}

U kunt uren aan een factureringsverslag toevoegen wanneer aan de volgende voorwaarden wordt voldaan:

* De taken, de kwesties, of het project hebben het programma geopende uren.
* Het type uur van de geregistreerde uren is duidelijk als Telling als Ontvangsten.

  Voor meer informatie over de Types van Uur, zie het artikel [ de types van uren ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) leiden.

* Alle uren die voor kwesties of voor het project worden geregistreerd kunnen aan een het facturerings verslag worden toegevoegd als de gebruiker die de tijd registreert een Facturering per het uurtarief verbonden aan hen of hun Primaire Rol van de Baan heeft.
* Als de uren op een taak worden het programma geopend, moet de taak het volgende Type van Ontvangsten hebben:

   * Het type van Inkomsten kan niet worden geplaatst aan Niet Facultatief.
   * Als het Type van Inkomsten aan Uur van de Gebruiker wordt geplaatst, moet de gebruiker die de tijd registreert een Facturering per Tarief hebben die in hun profiel wordt geplaatst.
   * Als het type van Inkomsten aan Rol Hourly wordt geplaatst, moet de Primaire Rol van de gebruiker die de tijd registreert een Facturering per Uuretarief hebben.

     >[!NOTE]
     >
     >U kunt factureringstarieven voor baanrollen op het projectniveau met voeten treden.\
     >Voor meer informatie over het met voeten treden van de het factureringspercentages van de baanrol, zie de sectie &quot;het Overschrijven van de Rol die Tarieven van de Taak op het Niveau van het Project&quot;in het artikel [ Overzicht van het met voeten treden van de FactureringsRates van de Rol en het berekenen van Inkomsten op een project ](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Als **tijd vereisen om voor dit project** te worden goedgekeurd onder de Montages van het Project wordt gecontroleerd, dan moet de Eigenaar van het Project de geregistreerde uren goedkeuren.\
  Voor meer informatie over het vereisen van goedkeuring op projecturen, zie het artikel [ tijd vereisen om voor een project ](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md) worden goedgekeurd.

#### Uren toevoegen aan een factureringsrecord {#add-hours-to-a-billing-record}

U voegt als volgt factureerbare uren toe aan een factureringsrecord:

1. Ga naar het project met de factureringsverslagen.
1. Klik **het Factureren Verslagen** in het linkerpaneel.

   Deze sectie zou onder **kunnen worden gevestigd tonen meer**.

1. Klik de **Beschrijving** van een het facturerings verslag om **het Factureren Details van het Verslag** tabel te openen.

1. Klik **Billable Uren** in het linkerpaneel.
1. Als er uren zijn die in een het facturerings verslag zouden kunnen worden omvat, klik **voegt Uren** toe.\
   **voegt Billable Uren** doos toe opent.

   >[!NOTE]
   >
   >Als er geen uren het programma worden geopend of als de geregistreerde uren niet aan de voorwaarden voldoen om aan een het facturerings verslag worden toegevoegd, **voegt de** knoop van Uren toe toont niet. Voor meer informatie over welke uren aan een het facturerings verslag kunnen worden geregistreerd, zie de sectie [ Welke uren aan een het facturerings verslag ](#what-hours-can-be-added-to-a-billing-record) in dit artikel kunnen worden toegevoegd.

1. Selecteer de uuringangen u in het facturerings verslag wilt omvatten, en **klikken voegt Uren** toe.\
   De daadwerkelijke Kosten van de uren worden toegevoegd als **Billable Uren** bedrag aan het **Totaal van het Verslag van de Facturering**.

1. (Facultatief) klik **het Factureren Details van Verslagen** om de **Billable Uren** en **het Factureren van het Totaal van het Verslag** te herzien. U kunt het totaal van het factureringsverslag in de kopbal van het het facturerings verslag ook zien.

### Facultatieve uitgaven opnemen in een factureringsrecord {#include-billable-expenses-in-a-billing-record}

Als u Billable Uitgaven aan het het facturerings verslag toevoegt, zorg de uitgaven op de taken ervoor en het project zijn duidelijk als Billable. Uitgaven die niet als Billable worden gemerkt zijn niet beschikbaar om in een factureringsverslag toe te voegen. Voor meer informatie over het toevoegen van uitgaven, zie artikel [ projectuitgaven beheren ](../../../manage-work/projects/project-finances/manage-project-expenses.md).

U kunt als volgt factureringskosten aan een factureringsrecord toevoegen:

1. Ga naar het project met de factureringsverslagen.
1. Klik **het Factureren Verslagen** in het linkerpaneel.

   U zou **kunnen moeten klikken tonen Meer**, dan **het Factureren Verslagen**.

1. Klik de **Beschrijving** van een het facturerings verslag om **het Factureren Details van het Verslag** tabel te openen.

1. Klik **Billable Uitgaven** in het linkerpaneel.
1. (Voorwaardelijk) als u uitgaven aan uw taken of het project hebt toegevoegd en hen als Billable gemerkt, klik **toevoegt Uitgaven**.

   >[!NOTE]
   >
   >Als u uitgaven hebt maar zij niet als Billable duidelijk zijn, **voegt de knoop van Uitgaven** toe toont niet. Alleen factureerbare uitgaven met een werkelijk bedrag groter dan nul komen in aanmerking om in een factureringsrecord te worden opgenomen.

1. Selecteer de factureerbare uitgaven die beschikbaar zijn om aan het het facturerings verslag worden toegevoegd, dan klik **voegt Uitgaven** toe.\
   Het daadwerkelijke Bedrag van de uitgaven wordt toegevoegd als **Billable Uitgaven** bedrag aan het **Totaal van het Verslag van de Facturering**.

1. (Facultatief) klik **de Details van de Verslagen van het Factureren** om de **Billable Uitgaven** en **het Factureren Totale van het Verslag** bedragen te herzien. U kunt het totaal van het factureringsverslag in de kopbal van het het facturerings verslag ook zien.

### Vaste inkomsten opnemen in een factureringsbestand {#include-fixed-revenues-in-a-billing-record}

U kunt vaste inkomsten toevoegen aan uw factureringsgegevens als u taken hebt waarvoor vaste inkomsten beschikbaar zijn. Er zijn geen andere typen taken of projectinkomsten beschikbaar die in een factureringsrecord kunnen worden toegevoegd. Voor meer informatie over opbrengsttypes, zie het [ Overzicht van het Factureren en van de Opbrengst ](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) sectie in [ Overzicht van Facturering en Opbrengsten ](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Om vaste opbrengsten aan een factureringsverslag toe te voegen:

1. Ga naar het project met de factureringsverslagen.
1. Klik **het Factureren Verslagen** in het linkerpaneel.

   U zou **kunnen moeten klikken tonen Meer**, dan **het Factureren Verslagen**.

1. Klik de **Beschrijving** van een het facturerings verslag om **het Factureren Details van het Verslag** tabel te openen.

1. Selecteer **Vaste Ontvangsten** tabel.
1. Als u vaste opbrengsten aan uw taken hebt toegevoegd, klik **voegt Vaste Inkomsten** toe.

   >[!NOTE]
   >
   >Als u opbrengstbedragen op taken hebt maar zij niet als &quot;Vast&quot;worden gemerkt, **voegt Vaste Inkomsten** knoop toe toont niet.

1. Selecteer de taken waarvan vaste opbrengsten u in het facturerings verslag wilt omvatten, dan klik **toevoegt Taken**.\
   De **Vaste Inkomsten** hoeveelheid van de taken wordt toegevoegd als **Billable Inkomsten** bedrag aan **het Totaal van het Verslag van de Facturering**.

1. (Facultatief) klik **de Details van de Verslagen van de Facturering** om **te herzien Billable Inkomsten** en **het Totale van het Facturerings Verslag** bedragen. U kunt het totaal van het factureringsverslag in de kopbal van het het facturerings verslag ook zien.

## Een factureringsrecord bewerken

Nadat u een factureringsrecord hebt gemaakt en uren, uitgaven en inkomsten in de factureringsrecord hebt opgenomen, kunt u bepaalde gegevens in de bestaande record bewerken voordat deze als factureringsgegevens worden gemarkeerd.

1. Ga naar de factureringsrecord.
1. Met **het Factureren Details van het Verslag** die in het linkerpaneel wordt geselecteerd, geef informatie op om het even welke beschikbare gebieden uit

   of

   Klik het **uitgeven pictogram** ![ uitgeven pictogram ](assets/edit-icon.png) in de hoger-juiste hoek, dan geef informatie op om het even welke beschikbare gebieden uit.

   Werk het volgende bij:

   * **Beschrijving**
   * **het Factureren Status**

     >[!TIP]
     >
     >Als u **Gevulde** voor de Status van het Factureren selecteert, kan het het facturerings verslag niet worden uitgegeven, nadat u uw veranderingen opslaat.

   * **FactureringsDatum**
   * **Aantal van PO**
   * **identiteitskaart van de Factuur**
   * **Extra Bedrag**

   De volgende velden kunnen niet worden bewerkt:

   * **Billable Uren:** Het totaal van de Ware Inkomsten van de uren inbegrepen in het factureringsverslag. Voor meer informatie over het omvatten van uren in een het facturerings verslag, zie de sectie [ omvatten Billable Uren in een het facturerings verslag ](#include-billable-hours-in-a-billing-record) in dit artikel.

   * **Billable Uitgaven**: Het totaal van het Ware Bedrag van de factureerbare uitgaven inbegrepen in het factureringsverslag. Voor meer informatie over het omvatten van factureerbare uitgaven in een factureringsverslag, zie de sectie [ omvatten Billable Uitgaven in een factureringsverslag ](#include-billable-expenses-in-a-billing-record) in dit artikel.

   * **Billable Inkomsten**: Het totaal van de Vaste Inkomsten van de taken inbegrepen in het factureringsverslag. Voor meer informatie over het omvatten van vaste opbrengsten in een factureringsverslag, zie de sectie [ Vaste Ontvangsten in een factureringsverslag ](#include-fixed-revenues-in-a-billing-record) in dit artikel omvatten.

   * **het Totaal van het Verslag van de Facturatie**: Het totaal van alle factureerbare bedragen. Dit wordt berekend aan de hand van de volgende formule:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Klik **sparen***Veranderingen**.
