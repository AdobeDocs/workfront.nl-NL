---
navigation-topic: financials
title: Factureringsrecords maken
description: Naast het opzetten van inkomsten en het volgen van uitgaven, kunt u het facturerings verslagen over een project voor informatie tot stand brengen die in rekening moet worden gebracht.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: fc82ce4b5abb2cd7411d62ac8bb428bc5337386f
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 0%

---

# Factureringsrecords maken

<!-- Audited: 6/2025 -->

Naast het opzetten van inkomsten en het volgen van uitgaven, kunt u het facturerings verslagen over een project voor informatie tot stand brengen die in rekening moet worden gebracht.

U kunt geen factureringsverslagen voor taken tot stand brengen; u kunt het facturerings verslagen voor projecten slechts tot stand brengen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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

Factureringsverslagen worden gecreeerd als gehechtheid aan een project en bevatten financiële gegevens van het project evenals de financiële informatie van de projecttaken.

Overweeg het volgende wanneer u factureringsrecords wilt gebruiken:

* U maakt een factureringsrecord wanneer u een bedrag dat betrekking heeft op het project, wilt factureren aan een externe leverancier of partner. Naast het factureren van een vast bedrag aan een externe bron, zijn er tijden wanneer u het bedrag van het werk aan het project (van geregistreerde uren) aan een externe contractant moet factureren, evenals de gemaakte kosten of het bedrag van vaste inkomsten. U kunt al deze gegevens in hetzelfde factureringsrecord opnemen.
* Als een factureringsrecord eenmaal is ingesteld op Met factuur, kan het niet worden bewerkt.

  >[!IMPORTANT]
  >
  >Dit is belangrijk wanneer uw tarieven variëren en u de opbrengst en de uitgaveninformatie over uw project wilt sluiten. Als u deze aan een factureringsrecord toevoegt en als factureringsrecord markeert, wordt de record niet bijgewerkt wanneer de tarieven in uw systeem worden bijgewerkt.

* Een project met factureringsverslagen die zijn gemarkeerd als Met factuur kan niet worden verwijderd.

## Een factureringsrecord maken

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. Klik **het Factureren Verslagen** in het linkerpaneel.
1. Klik **Nieuw het Factureren Verslag**.
1. In de **Nieuwe doos van het Verslag van de Facturering** die toont, specificeer de volgende informatie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>(Vereist) Voer een beschrijving in voor de factureringsrecord.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Factureringsstatus</td> 
      <td> <p>Selecteer <strong> niet Gevuld </strong> als dit verslag nog niet is gefactureerd.</p> <p>Selecteer <strong> Gevulde </strong> als het het facturerings verslag is gefactureerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Factureringsdatum</td> 
      <td>Selecteer de datum waarop deze factureringsrecord is gefactureerd door op het kalenderpictogram te klikken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inkoopordernummer</td> 
      <td>Voer het inkoopordernummer in dat aan dit factureringsrecord is gekoppeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Factuur-id</td> 
      <td>Voer de Factuur in die aan dit factureringsrecord is gekoppeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Extra bedrag</td> 
      <td>Voer de vaste hoeveelheid factureringsrecord in. Dit is het bedrag u van plan bent om een externe klant, een aannemer, of een partner voor dit project in rekening te brengen. Dit bedrag kan niet worden gewijzigd nadat de status van de factureringsrecord is gewijzigd in Facturering.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatief) onder **Eigen Forms**, selecteer een het factureren verslagen douaneformulier dat u aan het verslag wilt toevoegen.

   Voordat u het hier kunt selecteren, moet u een aangepast formulier voor factureringsrecords maken. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Voor informatie, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Klik **sparen.** De factureringsrecord wordt gemaakt.

## Opnemen van factureerbare uren, kosten en vaste inkomsten in een factureringsbestand

### Billable Hours opnemen in een factureringsrecord {#include-billable-hours-in-a-billing-record}

U kunt uren omvatten die het programma geopend taken, kwesties, of het project in uw het facturerings verslagen zijn.

Als de gebruiker die de uren of hun Primaire Rol van de Taak registreert met het Factureren per Tarief van het Uur wordt geassocieerd, wordt de opbrengst van deze uren toegevoegd aan het factureringsverslag.

* [ welke uren aan een het facturerings verslag kunnen worden toegevoegd ](#what-hours-can-be-added-to-a-billing-record)
* [Uren toevoegen aan een factureringsrecord](#add-hours-to-a-billing-record)

#### Welke uren kunnen aan een factureringsverslag worden toegevoegd {#what-hours-can-be-added-to-a-billing-record}

U kunt uren aan een factureringsverslag toevoegen wanneer aan de volgende voorwaarden wordt voldaan:

* De uren zijn geregistreerd voor de taken, de kwesties, of het project.
* Het type uur van de geregistreerde uren is duidelijk als Telling als Ontvangsten.

  Voor meer informatie, zie het artikel [ de types van uren ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) leiden.

* Alle uren die voor kwesties of het project worden geregistreerd kunnen aan een het facturerings verslag worden toegevoegd als de gebruiker die de tijd registreert een Facturering per het uurtarief verbonden aan hen of hun Primaire Rol van de Baan heeft.
* Als de uren op een taak worden het programma geopend, moet de taak het volgende Type van Ontvangsten hebben:

   * Het type van Inkomsten kan niet worden geplaatst aan niet Billable.
   * Als het Type van Inkomsten aan Uur van de Gebruiker wordt geplaatst, moet de gebruiker die de tijd registreert een Facturering per Tarief hebben die in hun profiel wordt geplaatst.
   * Als het type van Inkomsten aan Rol Hourly wordt geplaatst, moet de Primaire Rol van de gebruiker die de tijd registreert een Facturering per Uuretarief hebben.

     >[!NOTE]
     >
     >U kunt factureringstarieven voor baanrollen op het projectniveau met voeten treden.\
     >Voor meer informatie, zie de sectie met voeten tredende het FactureringsTarieven van de Rol van de Taak op het Niveau van het Project in het artikel [ Overzicht van het met voeten treden van de Factureringstarieven van de Rol van de Taak en het berekenen van Inkomsten op een project ](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Als de Vereiste tijd om voor deze projectoptie worden goedgekeurd onder de Montages van het Project wordt gecontroleerd, dan moet de Eigenaar van het Project de geregistreerde uren goedkeuren.\
  Voor meer informatie, zie [ tijd vereisen om voor een project ](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md) worden goedgekeurd.

#### Uren toevoegen aan een factureringsrecord {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. Klik **het Factureren Verslagen** in het linkerpaneel.
1. Klik het facturerings verslag **Beschrijving** om de **het Factureren Details van het Verslag** tabel te openen.
1. Klik **Billable Uren** in het linkerpaneel.
1. Als er uren zijn die in een het facturerings verslag zouden kunnen worden omvat, klik **voegt Uren** toe. **voegt Billable Uren** doos toe opent.

   >[!NOTE]
   >
   >Als er geen uren het programma worden geopend of als de geregistreerde uren niet aan de voorwaarden voldoen om aan een het facturerings verslag worden toegevoegd, **voegt de** knoop van Uren toe zal niet tonen. Voor meer informatie, zie de volgende sectie in dit artikel: [ Welke uren aan een het facturerings verslag ](#what-hours-can-be-added-to-a-billing-record) kunnen worden toegevoegd.

1. Selecteer de uuringangen u in het facturerings verslag wilt omvatten, dan klik **voegt Uren** toe. De daadwerkelijke Kosten van de uren worden toegevoegd als **Billable Uren** bedrag aan het **Totaal van het Verslag van de Facturering**.

1. (Facultatief) klik **de Details van de Verslagen van het Factureren** om de **Billable Uren** en **het Factureren Totale van het Verslag** bedragen, en het het facturerings verslagtotaal in het facturerings verslagkopbal te herzien.

### Facultatieve uitgaven opnemen in een factureringsrecord {#include-billable-expenses-in-a-billing-record}

Als u Billable Uitgaven aan het het facturerings verslag toevoegt, zorg de uitgaven op de taken ervoor en het project zijn duidelijk als Billable. Uitgaven die niet als Billable worden gemerkt zijn niet beschikbaar om in een factureringsverslag toe te voegen. Voor meer informatie over het toevoegen van uitgaven, zie artikel [ projectuitgaven beheren ](../../../manage-work/projects/project-finances/manage-project-expenses.md).

U kunt als volgt factureringskosten aan een factureringsrecord toevoegen:

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. Klik **het Factureren Verslagen** in het linkerpaneel.
1. Klik het facturerings verslag **Beschrijving** om de **het Factureren Details van het Verslag** tabel te openen.
1. Klik **Billable Uitgaven** in het linkerpaneel.
1. (Voorwaardelijk) als u uitgaven aan uw taken of het project hebt toegevoegd en hen als Billable gemerkt, **toevoegt Uitgaven**.

   >[!NOTE]
   >
   >Als u uitgaven hebt maar zij niet zoals Billable zijn, voegt **de knoop van Uitgaven** toe toont niet. Alleen factureerbare uitgaven met een werkelijk bedrag groter dan nul komen in aanmerking om in een factureringsrecord te worden opgenomen.

1. Selecteer de factureerbare uitgaven die beschikbaar zijn om aan het het facturerings verslag worden toegevoegd, dan klik **voegt Uitgaven** toe.  Het daadwerkelijke Bedrag van de uitgaven wordt toegevoegd als **Billable Uitgaven** bedrag aan het **Totaal van het Verslag van de Facturering**.

1. (Facultatief) klik **de Details van de Verslagen van de Facturering** om de **Billable Uitgaven** en **het Factureren Totale van het Verslag** bedragen, en het het facturerings verslagtotaal in de het registreren kopbal te herzien.

### Vaste inkomsten opnemen in een factureringsbestand {#include-fixed-revenues-in-a-billing-record}

U kunt vaste inkomsten toevoegen aan uw factureringsgegevens als u taken hebt waarvoor vaste inkomsten beschikbaar zijn. Er is geen ander type taak of projectinkomsten beschikbaar die in een factureringsrecord kunnen worden toegevoegd. Voor meer informatie over opbrengsttypes, zie het Overzicht van Facturering en de sectie van de Opbrengst in het artikel [ Overzicht van Facturering en Opbrengsten ](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. Klik **het Factureren Verslagen** in het linkerpaneel.
1. Klik de het factureren van verslag **Beschrijving** om de **het Factureren Details van het Verslag** tabel te openen.
1. Selecteer **Vaste Ontvangsten** tabel.
1. Als u vaste opbrengsten aan uw taken hebt toegevoegd, klik **voegt Vaste Inkomsten** toe.

   >[!NOTE]
   >
   >Als u opbrengstbedragen op taken maar zij niet zoals Vast worden gemerkt, **voegt Vaste Inkomsten** knoop toe zal niet tonen.

1. Selecteer de taken waarvan vaste opbrengsten u in het facturerings verslag wilt omvatten, dan klik **toevoegt Taken**.  De **Vaste Inkomsten** hoeveelheid van de taken wordt toegevoegd als **Billable Inkomsten** bedrag aan **het Totaal van het Verslag van de Facturering**.

1. (Facultatief) klik **de Details van de Verslagen van de Facturering** om de **Billable Inkomsten** en **het Factureren Totale van het Verslag** bedragen, en het het facturerings verslagtotaal in de het registreren kopbal te herzien.

## Een factureringsrecord bewerken

Nadat u een factureringsrecord hebt gemaakt en er uren, kosten en inkomsten aan hebt toegevoegd, kunt u bepaalde informatie over de bestaande record bewerken voordat deze wordt gemarkeerd als Met factuur.

1. Navigeer naar de factureringsrecord.
1. Selecteer **het Factureren Details van het Verslag** in het linkerpaneel.
1. Bewerk de gegevens in alle beschikbare velden.

   of

   Klik **uitgeven** pictogram ![ geeft pictogram ](assets/edit-icon.png) in de hoger-juiste hoek uit, dan geef informatie op om het even welke beschikbare gebieden uit.

   Werk het volgende bij:

   * **Beschrijving**
   * **FactureringsDatum**
   * **het Factureren Status**

     >[!TIP]
     >
     >Als u **Gevulde** voor de Status van het Factureren selecteert, kan het het facturerings verslag niet worden uitgegeven nadat u uw veranderingen opslaat.

   * **identiteitskaart van de Factuur**
   * **Aantal van PO**
   * **Extra Bedrag**

   De volgende velden kunnen niet worden bewerkt:

   * **Billable Uren:** Het totaal van de Ware Inkomsten van de uren inbegrepen in het factureringsverslag. Voor meer informatie, zie de volgende sectie in dit artikel: [ omvat billable Uren in een het facturerings verslag ](#include-billable-hours-in-a-billing-record).

   * **Billable Uitgaven**: Het totaal van het Ware Bedrag van de factureerbare uitgaven inbegrepen in het factureringsverslag. Voor meer informatie, zie de volgende sectie in dit artikel: [ omvat Billable Uitgaven in een het facturerings verslag ](#include-billable-expenses-in-a-billing-record).

   * **Billable Inkomsten**: Het totaal van de Vaste Inkomsten van de taken inbegrepen in het factureringsverslag. Voor meer informatie, zie de volgende sectie in dit artikel: [ omvat Vaste Ontvangsten in een het facturerings verslag ](#include-fixed-revenues-in-a-billing-record).

   * **het Totaal van het Verslag van de Facturatie**: Het totaal van alle factureerbare bedragen. Dit wordt berekend aan de hand van de volgende formule:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Klik **sparen Veranderingen**.
