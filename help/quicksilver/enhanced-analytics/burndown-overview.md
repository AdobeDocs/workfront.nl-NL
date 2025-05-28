---
title: Bekijk de Burndown-visualisatie in de uitgebreide analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De burndown visualisatie toont de onderbreking van een specifiek project in tijd en helpt u het verband tussen projectvoorwaarde, snelheid, en het blijven uren-of dagen begrijpen.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Bekijk de Burndown-visualisatie in de uitgebreide analyse

>[!IMPORTANT]
>
>Enhanced Analytics is op 27 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2} gids van de Afleiding van Analytics {voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


<!-- Audited: 12/2023 -->

De burndown visualisatie toont de onderbreking van een specifiek project in tijd en helpt u het verband tussen projectvoorwaarde, snelheid, en het blijven uren-of dagen begrijpen.

![ Verbeterd analytics burndown voorbeeld ](assets/burndown120623.png)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>
      <p>Nieuw: alle</p>
      <p>of</p>
      <p>Huidig: Zakelijk of hoger</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
      <p>Nieuw: Licht of hoger</p>
      <p>of</p>
      <p>Huidig: Controleren of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Weergave</p> </td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie de &quot;sectie van Eerste vereisten&quot;in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de Burndown visualisatie

De effen blauwe lijn toont de geplande snelheid vanaf de begindatum tot de geplande einddatum. Deze lijn past zich aan aangezien het werk wordt toegevoegd, verwijderd of bijgewerkt, en het verandert in een onderbroken verticale lijn wanneer het project de geplande voltooiingsdatum bereikt.

![ Geplande snelheid ](assets/burndown-planned-line.png)

De daadwerkelijke lijn toont het aantal uren-of dagen-besteed aan het project in tijd. De kleur van deze lijn wijst op de voorwaarde van het project elke dag:

* **Groen**: Het project is op doel.

  ![ op doel ](assets/burndown-green.png)

* **Oranje**: Het project is in gevaar.

  ![ Op risico ](assets/burndown-orange.png)

* **Rood**: Het project is in probleem.

  ![ In probleem ](assets/burndown-red.png)

Voor meer informatie over deze projectvoorwaarden, zie [ Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project ](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Wanneer de daadwerkelijke lijn verticaal omhoog beweegt, is het werk toegevoegd aan het project. Wanneer de lijn verticaal naar beneden beweegt, is het werk verwijderd of voor het project voltooid.

Onder de x as van de visualisatie, kunt u meer informatie over zien hoe de taken en uren-of dagen-veranderd op een bepaalde dag (de toegevoegde hoeveelheid, de voltooide hoeveelheid, en het verschil tussen twee).

Door al deze informatie te bekijken in de Burndown-visualisatie kunt u beter bepalen:

* De gezondheid van het afzonderlijke project in de loop van de tijd
* De invloed van problemen die zich voordoen (of ongeplande werkzaamheden) op de geplande werkzaamheden
* Welke gebeurtenissen uw project voorbij de originele voltooiingsdatum verlengden

Leren hoe te om de beste gegevens voor deze visualisatie te krijgen, zie [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## De Burndown-visualisatie weergeven

{{step1-to-analytics}}

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![ Uitgezochte data ](assets/filters-select-date-range-350x344.png)

   Voor informatie bij het gebruiken van de filter van de datumwaaier, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie bij het toevoegen van filters in Verbeterde analyses, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u het punt naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt automatisch een tijdframefilter gemaakt.

   ![ filter Tijdframe ](assets/timeframe-filter-350x220.png)

1. Voor het Vluchtplan of de visualisatie van de treemap van het Project, klik een project om meer informatie te bekijken.

   De Burndown- en Taken in vluchtvisualisaties worden weergegeven.

   >[!NOTE]
   >
   >Zie voor meer informatie over deze andere visualisaties:
   >
   >   * [ Mening de visualisatie van het Plan van de Vlucht in Verbeterde analyses ](../enhanced-analytics/flight-plan-overview.md)
   >   * [ Mening de boomtopvisualisatie van het Project in Verbeterde analyses ](../enhanced-analytics/project-treemap-overview.md)
   >   * [ Mening de Taken in vluchtvisualisatie in Verbeterde analyses ](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Facultatief) verander de mening van geplande uren in **duur**.

   Geplande uren zijn standaard geselecteerd.

   >[!NOTE]
   >
   >Het selecteren van **duur** verandert alle ureninformatie in dagen.\
   >![ de begraving van de Duur ](assets/duration-burndown-350x112.png)\
   >Voor meer informatie over duur in het Verbeterde analysegebied, zie de &quot;mening van de Duur&quot;sectie in [ Verbeterde analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Klik op een punt in de lijngrafiek.

   De nauwkeurige datumvertoningen en verdere informatie over taken en uren-of dagen-voor de geselecteerde dag toont onder de grafiek.

   ![ details van de Burndown ](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Als de daadwerkelijke snelheid een vlakke lijn is die langs de x as (gealigneerd met 0 uren of 0 dagen) van visualisatie loopt, betekent dit dat geen geplande uren-of dagen-werden toegevoegd aan het project.\
   >Als de werkelijke snelheid een vlakke lijn boven de x-as is (in lijn met een aantal uren of dagen) die nooit omlaag gaat, betekent dit dat er geen taken zijn uitgevoerd binnen de gefilterde tijdsperiode.

1. (Facultatief) om de visualisatiegegevens uit te voeren, klik het **pictogram van de Uitvoer ![ pictogram van de Uitvoer ](assets/export.png) in de hoogste juiste hoek van de visualisatie, en selecteer het uitvoerformaat:**

   * Diagram (PNG)
   * Gegevenstabel (XSLX)

1. (Optioneel) Als u meer informatie wilt over de voortgang van taken in het geselecteerde project, bekijkt u de taken in de visualisatie van de vlucht die onder de Burndown-visualisatie wordt weergegeven. Voor meer informatie, zie [ Mening de Taken in vluchtvisualisatie in Verbeterde analyses ](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
