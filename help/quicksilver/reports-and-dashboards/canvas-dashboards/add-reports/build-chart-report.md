---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Een diagramrapport samenstellen
description: Een grafiekrapport dat uw gegevens visualiseert als bar, kolom, lijn, of cirkeldiagram kan aan een Dashboard van het Canvas worden toegevoegd.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: 981d86fa7d54d9d26c0a2b6142db98d5989cbed2
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# Een diagramrapport samenstellen

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Voor meer informatie, zie {de bètainformatie van de Dashboards van het 0} Canvas [.](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)

U kunt een grafiekrapport aan een dashboard van het Canvas bouwen en toevoegen om uw gegevens als bar, kolom, lijn, of cirkeldiagram visualiseren.

![ rapport van de Grafiek ](assets/chart-report-main.png)

+++ Vouw uit om de vereisten voor toegang weer te geven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan</p></td> 
   <td> 
<p>Alle </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td> 
<p>Huidig: Plan </p> 
<p>Nieuw: Standaard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td> 
   <td><p>Toegang tot rapporten, dashboards en kalenders bewerken</p>
  </td> 
  </tr>  
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Vereisten

U moet een dashboard tot stand brengen alvorens u een grafiekrapport kunt bouwen.

## Bouw een grafiekrapport in een dashboard van het Canvas

Er zijn vele configuratieopties beschikbaar voor het bouwen van een grafiekrapport. In deze sectie doorlopen we het algemene proces voor het maken van een sectie.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**

1. Klik **creëren**.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Grafiek**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. (Facultatief) volg de stappen hieronder om de **sectie van Details** te vormen:

   1. Ga een rapport **Naam** in.

   1. Ga een rapport **Beschrijving** in.

   1. Indien gewenst, uncheck **extra reeksen als &quot;Andere&quot;** doos tonen.

      >[!NOTE]
      >
      >Er is een maximumaantal reeksen dat in een grafiek kan worden getoond. Wanneer deze doos wordt gecontroleerd, worden om het even welke reeksen boven de grens geconsolideerd in a **Andere** groepering in de grafiek.

1. Volg hieronder de stappen om **bouwt grafiek** sectie te vormen:

   1. In het linkerpaneel, klik het **bouwt grafiek** ![ het pictogram van de Grafiek ](assets/build-chart-icon.png) bouwen.

   1. In het **type van Grafiek** drop-down, selecteer het type van grafiek u wilt tot stand brengen:

      * **Bar**
      * **Kolom**
      * **Lijn**
      * **Schijf**

   1. In het **type van Kolom** drop-down, selecteer het kolomtype:
      * **Eenvoudig**
      * **Multi-series**
      * **Gestapeld**

   1. Selecteer het **gebied van de Update** knoop in de eerste sectie, bepaal de plaats en selecteer dan van het gebied dat de gegevens bevat die in de grafiek zullen worden samengevat.
   1. In het **type van Samenvoeging** drop-down, selecteer hoe de gegevens omhoog rollen om de grafiekoutput te veroorzaken.

   1. Selecteer het **gebied van de Update** knoop onder de tweede sectie, bepaal de plaats en selecteer dan van het tweede gebied u in de grafiek wilt tonen.

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter**![ van de Filter {](assets/filter-icon.png).
   1. Selecteer **filter uitgeven**.
   1. Klik **toevoegen voorwaarde** en specificeer dan het gebied u tegen en de bepaling wilt filtreren die bepaalt welk soort voorwaarde het gebied moet ontmoeten.
   1. (Facultatief) klik **toevoegen filtergroep** om een andere reeks het filtreren criteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

1. Volg hieronder de stappen om de **sectie van de Montages van de Kolom te vormen 0} Drilldown {:**

   1. In het linkerpaneel, klik het **Drilldown pictogram van Kolommen** ![ Drilldown kolommen ](assets/drilldown-column.png). De velden in het diagram worden automatisch als kolommen weergegeven in de voorbeeldsectie aan de rechterkant.

   1. (Facultatief) om het even welke bestaande kolomconfiguraties bij te werken, selecteer de kolom u in de **Huidige kolommen** sectie wilt bijwerken en dan de gewenste informatie (b.v. etiket, verbonden status, en voorwaarden) bijwerken.

   1. Klik **toevoegen kolom** en selecteer dan het gebied u als kolom in de lijst wilt tonen. Herhaal dit proces voor elke kolom u wilt toevoegen.

1. Volg hieronder de stappen om de **sectie van de Montages van de Groep van de Drilldown** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Montages van de Groep** ![ van de Montages van de Groep ](assets/drilldown-group-icon.png).

   1. Klik **toevoegen groeperend** knoop en dan het gebied selecteren u als groepering wilt tot stand brengen.

1. Klik **sparen** om het rapport tot stand te brengen en het toe te voegen aan het dashboard.

## Een voorbeeld van een diagramrapport maken

In deze sectie, zullen wij over de stappen gaan om een kolomgrafiek tot stand te brengen die achterstallige taken door projecteigenaar toont.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**

1. Klik **creëren**.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Grafiek**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Ga een rapport **Naam** in (b.v. *Verouderde Taken door de Eigenaar van het Project*).

   1. Ga een rapport **Beschrijving** in.

1. Volg hieronder de stappen om **bouwt grafiek** sectie te vormen:

   1. In het linkerpaneel, klik het **bouwt grafiek** pictogram.

   1. In het **type van Grafiek** drop-down, uitgezochte **Kolom**.

   1. In het **type van Kolom** drop-down, uitgezochte **Eenvoudig**.

   1. Selecteer het **gebied van de Update** knoop onder de **bodem (X) as** sectie, dan bepaal de plaats en selecteer van de **Taak** > **Project** > **Eigenaar** > **Naam** gebied.

      ![ gebied van de Update ](assets/bottom-x-axis.png)

   1. Klik het **Uitgezochte gebied** knoop onder de **Linkeras (Y)** sectie, dan bepaal de plaats en selecteer van de **Taak** > **het gebied van de Naam**.

   1. In het **type van Samenvoeging** drop-down, uitgezochte **Telling**.

      ![ het typegebied van de Samenvoeging ](assets/left-y-axis.png)

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter**.

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde**.

   1. Klik op het lege voorwaardengebied, dan selecteren het **Gebied van de Selectie**.

   1. Selecteer het **Volledige** gebied van de Percentage.

   1. In de **drop-down exploitanten**, uitgezocht **minder dan**, dan ga *100* op het evaluatorgebied in.

   1. Klik **toevoegen Voorwaarde**, dan **Gebied van de Selectie**.

   1. Selecteer het **Geplande gebied van de Datum van de Voltooiing**.

   1. In de **drop-down exploitanten**, uitgezochte **minder dan**.

   1. Knevel **Vastgestelde relatieve datum** aan ****.

   1. Ga *$$TODAY* op het evaluatiegebied in.

      ![ het gebied van de Evaluator ](assets/add-condition.png)

1. Volg hieronder de stappen om de **sectie van de Montages van de Kolom te vormen 0} Drilldown {:**

   1. In het linkerpaneel, klik het **Drilldown Kolommen** ![ Drilldown kolommen ](assets/drilldown-column.png) pictogram. De velden in het diagram worden automatisch als kolommen weergegeven in de voorbeeldsectie aan de rechterkant.

   1. Klik **toevoegen kolom**, dan selecteren **Toegewezen aan** > **Naam** gebied.

   1. Klik **toevoegen kolom**, dan selecteren het **Geplande gebied van de Datum van het Begin**.

   1. Klik **toevoegen kolom**, dan selecteren het **Geplande gebied van de Datum van de Voltooiing**.

   1. Klik **toevoegen kolom**, dan selecteren het **Laatste gebied van de Datum van de Update**.

   1. (Facultatief) om de updatetijd te tonen, selecteer de **Laatste optie van de Datum van de Update** op het **Huidige gebied van Kolommen**, dan selecteer een optie van de tijdwaarde in het **formaat van de Datum** drop-down.

1. Volg hieronder de stappen om de **sectie van de Montages van de Groep van de Drilldown** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Montages van de Groep** ![ van de Montages van de Groep ](assets/drilldown-group-icon.png).

   1. Klik **toevoegen groeperend** knoop en selecteer dan het **Project** > **gebied van de Naam**.

1. Klik **sparen** om het rapport tot stand te brengen en het toe te voegen aan het dashboard.