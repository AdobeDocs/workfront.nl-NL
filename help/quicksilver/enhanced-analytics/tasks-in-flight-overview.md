---
title: De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De taken in vluchtvisualisatie tonen hoeveel taken (binnen de toegepaste filtercriteria) voor een project, het percentage van het werk dat voor elke taak wordt voltooid, en hoe op programma lopend zijn de taken.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse

>[!IMPORTANT]
>
>Enhanced Analytics is op 27 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2&rbrace; gids van de Afleiding van Analytics &lbrace;voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


De taken in vluchtvisualisatie tonen hoeveel taken (binnen de toegepaste filtercriteria) voor een project, het percentage van het werk dat voor elke taak wordt voltooid, en hoe op programma lopend zijn de taken.

![ Taken in vlucht ](assets/tasks-in-flight-possible-replacement-350x104.png)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank"> plan van Adobe Workfront </a>*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> het vergunningsoverzicht van Adobe Workfront </a>*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>De toegang van de mening tot Taken (om taken bij te werken, hebt u Edit toegang tot Taken nodig.)</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld.<br> voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemming weergeven voor zowel project- als taakobjecten</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie de &quot;sectie van Eerste vereisten&quot;in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de Taken in vlucht visualisatie

De taken in de visualisatie van het vliegplan tonen de volgende taakdetails:

* **Geplande taakduur**: De lengte van een taakbar wijst op de geplande duur, die op de de begindatum en voltooiingsdatum van de taak gebaseerd is.

  ![ Taken in vluchtduur ](assets/tasks-in-flight-duration-350x80.png)

* **voltooide de inspanning van het Werk**: De donkerblauwe kleur binnen een taakbar wijst op de hoeveelheid werk dat voor een taak wordt voltooid. Dit voltooiingspercentage wordt rechts van de taakbalk weergegeven.

  ![ Taken in vlucht donkerblauw ](assets/tasks-in-flight-dark-blue-350x35.png)

* **de inspanning die van het Werk** blijft: De lichtblauwe kleur binnen een taakbar wijst op de hoeveelheid werk die voor een taak moet worden voltooid.

  ![ Taken in lucht lichtblauw ](assets/tasks-in-flight-light-blue-350x35.png)

Aan de hand van deze gegevens kunt u bepalen:

* Waar de inspanningen zijn gericht.
* Welke taken zouden een project in gevaar kunnen brengen.
* Hoe dicht een taak aan voltooiing is.
* Met wie moet u over een specifieke taak spreken?

Leren hoe te om de beste gegevens voor deze visualisatie te krijgen, zie [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## De taken in de vluchtvisualisatie weergeven

1. Klik het Belangrijkste pictogram van het Menu ![ Belangrijkste menupictogram ](assets/main-menu-icon-16x12.png), dan uitgezochte **Analytics**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![ Uitgezochte datumwaaier ](assets/filters-select-date-range-350x344.png)

   Voor informatie bij het gebruiken van de filter van de datumwaaier, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie bij het toevoegen van filters in Verbeterde analyses, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. Voor het Vluchtplan of de visualisatie van de treemap van het Project, klik een project om meer informatie te bekijken.

   De Burndown- en Taken in vluchtvisualisaties worden weergegeven.

   >[!NOTE]
   >
   >Zie voor meer informatie over deze andere visualisaties:
   >
   >   
   >   
   >   * [ Mening de visualisatie van het Plan van de Vlucht in Verbeterde analyses ](../enhanced-analytics/flight-plan-overview.md)
   >   * [ Mening de boomtopvisualisatie van het Project in Verbeterde analyses ](../enhanced-analytics/project-treemap-overview.md)
   >   * [ Mening de Burndown visualisatie in Verbeterde analyses ](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![ filter Tijdframe ](assets/timeframe-filter-350x220.png)

1. (Facultatief) om te veranderen hoe de taken worden gesorteerd, klik de **Soort door** menu, dan selecteer een nieuwe sorteeroptie:

   * **de datum van de Voltooiing**
   * **alfabetisch a-z**
   * **de verdelingsstructuur van het Werk** (Deze optie past de orde aan dat de taken in het project verschijnen.)

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. Controleer de voortgang van de taken in het geselecteerde project en houd de muisaanwijzer boven een specifieke taak om het aantal geplande uren, de geplande vervaldatum en het voltooiingspercentage te zien.

   ![ Taken in vluchtdetails ](assets/tasks-in-flight-task-details-350x242.png)

1. Klik op een taak om de taakdetails aan de rechterkant van het scherm te openen. Hier kunt u meer informatie over de taak zien, updates weergeven of invoeren of wijzigingen in de taak aanbrengen.

   ![ de details van de Taak ](assets/task-details-qs-350x675.png)

1. (Facultatief) om de visualisatiegegevens uit te voeren, klik het **pictogram van de Uitvoer** ![ pictogram van de Uitvoer ](assets/export.png) in de hoogste juiste hoek van de visualisatie, dan selecteer het uitvoerformaat:

   * **Grafiek (PNG)**
   * **Lijst van Gegevens (XSLX)**

