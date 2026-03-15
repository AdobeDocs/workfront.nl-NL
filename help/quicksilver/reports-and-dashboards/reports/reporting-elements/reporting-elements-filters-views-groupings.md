---
product-area: reporting
navigation-topic: reporting-elements
title: 'Elementen rapporteren: filters, weergaven en groepen'
description: De belangrijkste elementen die elke lijst en het rapport in Workfront moeten hebben zijn een filter, een mening, en een groepering. Elk element verstrekt verschillende informatie binnen om het even welk rapport.
author: Courtney
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Elementen rapporteren: filters, weergaven en groepen

<!-- Audited: 11/2024 -->

<!--AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well-->

Er zijn verschillende elementen die een lijst of rapport in Adobe Workfront mogelijk maken. De belangrijkste elementen die elke lijst en het rapport moeten hebben zijn een filter, een mening, en een groepering. Elk element verstrekt verschillende informatie binnen om het even welk rapport.

## Overwegingen bij het rapporteren van elementen

Houd rekening met het volgende wanneer u werkt met filters, weergaven en groepen:

* Elementen rapporteren werkt als de bouwstenen voor rapportage. Zij bepalen het uiterlijk van een rapport of een lijst, evenals de informatie in het rapport of de lijst.
* Rapporten in Workfront zijn specifiek voor één object. U moet uw belangrijkste voorwerp voor een rapport bepalen alvorens u het rapport kunt bouwen. Alle rapportelementen zijn dus objectspecifiek.
* Uw Workfront-beheerder moet u toegang verlenen tot filters, weergaven en groeperingen op uw toegangsniveau om deze in lijsten en rapporten te kunnen weergeven of bewerken.

  Voor informatie over het verlenen van toegang tot filters, meningen, en groeperingen, zie [ toegang van de Verlening tot filters, meningen, en groeperingen ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Your Workfront administrator must grant you access to reports, dashboards, and calendars in your access level to be able to view or edit reports.

  For information about granting access to reports, dashboards, and calendars, see [Grant access to reports, dashboards, and calendars](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* If you select a filter, view, or grouping on a report or list, Workfront retains this selection for that object&#39;s lists even after you log out or close your browser. Als u bijvoorbeeld een specifieke weergave voor een taakrapport selecteert, wordt die selectie weergegeven voor andere takenlijsten, zoals de takenlijst van een project.

## Filters

Het filter controleert de resultaten die in een rapport verschijnen, typisch versmalend resultaten van algemeen aan specifiek. Het werkt als een zeef die slechts de informatie graaft die u nodig hebt en die informatie terugbrengt naar uw rapport.

Bijvoorbeeld, als u slechts taken wilt zien die aan de het programma geopende gebruiker worden toegewezen, kunt u een filter tot stand brengen getiteld &quot;Mijn Taken,&quot;bepaalt de criteria die voor de filter moeten worden vervuld en het rapport in werking stellen om slechts taken te bekijken die aan de het programma geopende gebruiker worden toegewezen.

Enkele kenmerken van filters zijn:

* Workfront biedt standaard een aantal filters voor verschillende objecten.
* U kunt filters aanpassen die u bezit of beheert.

  Voor meer informatie over filters, zie het artikel [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Weergaven

Door de mening van een rapport te bepalen, bepaalt u welke informatie u in het rapport omvat. Net als alle rapportelementen zijn weergaven gebaseerd op één objecttype.

Een weergave voor een taakrapport kan bijvoorbeeld de vervaldatum weergeven, belangrijke financiële details zoals Kosten bevatten of worden gebruikt om de details van de toewijzingen en de leveringsdatum weer te geven. De meningen kunnen worden gebruikt om een verscheidenheid van details over de gegevens in het rapport te leveren.

Enkele weergavekenmerken zijn:

* U kunt een standaard Workfront-weergave gebruiken of uw eigen weergave maken.
* U kunt extra meningen van het drop-down gebied van de Mening toepassen na het runnen van een rapport.
* De extra meningen vervangen tijdelijk de mening die wanneer het creëren van het rapport wordt bepaald; nochtans, wordt de standaardmening getoond de volgende tijd u aan het rapport terugkeert.

  Voor meer informatie over meningen, zie het artikel [ overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Groepen

A grouping controls how you organize data, making it easier to read and understand. Groupings create horizontal bars throughout a report that display results listed together by common attributes. You define the criteria for how you want to group the results of your report when creating the grouping.

For example, grouping a list of tasks that span multiple projects by their project name organizes all respective tasks that belong to a single project under that name.

Some attributes of groupings are:

* Groepen zijn een verplicht rapporteringselement als u een grafiek aan uw rapport wilt later toevoegen.
* Groepen geven een geaggregeerde waarde in de resultaten weer. &#x200B;
* Groepen bepalen de as in grafieken.
* Groepen bepalen de headeridentificatie in matrixrapporten.\
  Voor meer informatie over matrixrapporten, zie het artikel [ een matrixrapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md) creëren.

* De hulp van groeperingen bouwt de Samenvatting tabel van een rapport, die de samengevoegde waarden van het rapport verstrekt.
* Workfront biedt standaard een aantal groepen voor verschillende objecten.
* U kunt groepen aanpassen die u hebt of beheert.

  Voor meer informatie over groeperingen, zie [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Overige rapporteringselementen

Naast filters, meningen, en groeperingen, kon u de volgende elementen aan een rapport ook toevoegen:

* **Herinnering**: Een open filter dat kan worden aangepast en verschillend worden toegepast telkens als u een rapport in werking stelt.\
  Voor meer informatie over herinneringen, zie het artikel [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

* **Grafiek**: U kunt uw rapporten verbeteren door een grafiek aan hen toe te voegen en de informatie op een visuele manier te tonen.\
  For more information about charts in reports, see the article [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
