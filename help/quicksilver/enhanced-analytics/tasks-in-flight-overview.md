---
title: De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De taken in vluchtvisualisatie tonen hoeveel taken (binnen de toegepaste filtercriteria) voor een project, het percentage van het werk dat voor elke taak wordt voltooid, en hoe op programma lopend zijn de taken.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse

De taken in vluchtvisualisatie tonen hoeveel taken (binnen de toegepaste filtercriteria) voor een project, het percentage van het werk dat voor elke taak wordt voltooid, en hoe op programma lopend zijn de taken.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-plan</a>*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>Toegang tot taken weergeven (als u taken wilt bijwerken, hebt u toegang tot taken bewerken nodig.)</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt.<br>Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemming weergeven voor zowel project- als taakobjecten</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de Taken in vlucht visualisatie

De taken in de visualisatie van het vliegplan tonen de volgende taakdetails:

* **Geplande taakduur**: De lengte van een taakbar wijst op de geplande duur, die op de de begindatum en voltooiingsdatum van de taak gebaseerd is.

   ![](assets/tasks-in-flight-duration-350x80.png)

* **Werkinspanning voltooid**: De donkerblauwe kleur in een taakbalk geeft aan hoeveel werk is voltooid voor een taak. Dit voltooiingspercentage wordt rechts van de taakbalk weergegeven.

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **Resterende arbeidsinspanning**: De lichtblauwe kleur in een taakbalk geeft de hoeveelheid werk aan die voor een taak moet worden voltooid.

   ![](assets/tasks-in-flight-light-blue-350x35.png)

Aan de hand van deze gegevens kunt u bepalen:

* Waar de inspanningen zijn gericht.
* Welke taken zouden een project in gevaar kunnen brengen.
* Hoe dicht een taak aan voltooiing is.
* Met wie moet u over een specifieke taak spreken?

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De taken in de vluchtvisualisatie weergeven

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. Voor het Vluchtplan of de visualisatie van de treemap van het Project, klik een project om meer informatie te bekijken.

   De Burndown- en Taken in vluchtvisualisaties worden weergegeven.

   >[!NOTE]
   >
   >Zie voor meer informatie over deze andere visualisaties:
   >
   >   
   >   
   >   * [Bekijk de visualisatie van het vliegplan in de uitgebreide analyse](../enhanced-analytics/flight-plan-overview.md)
   >   * [Bekijk de visie van de projectreemap in Verbeterde analyse](../enhanced-analytics/project-treemap-overview.md)
   >   * [Bekijk de Burndown-visualisatie in de uitgebreide analyse](../enhanced-analytics/burndown-overview.md)


1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. (Optioneel) Klik op de knop **Sorteren op** selecteert u vervolgens een nieuwe sorteeroptie:

   * **Voltooiingsdatum**
   * **Alfabetisch A-Z**
   * **Structuur voor werkverdeling** (Deze optie komt overeen met de volgorde waarin de taken in het project worden weergegeven.)

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. Controleer de voortgang van de taken in het geselecteerde project en houd de muisaanwijzer boven een specifieke taak om het aantal geplande uren, de geplande vervaldatum en het voltooiingspercentage te zien.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Klik op een taak om de taakdetails aan de rechterkant van het scherm te openen. Hier kunt u meer informatie over de taak zien, updates weergeven of invoeren of wijzigingen in de taak aanbrengen.

   ![](assets/task-details-qs-350x675.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op de knop **Exportpictogram** ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

