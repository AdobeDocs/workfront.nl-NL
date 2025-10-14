---
product-area: reporting
navigation-topic: reporting-elements
title: 'Elementen rapporteren: filters, weergaven en groepen'
description: De belangrijkste elementen die elke lijst en het rapport in Workfront moeten hebben zijn een filter, een mening, en een groepering. Elk element verstrekt verschillende informatie binnen om het even welk rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
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

  Voor informatie over het verlenen van toegang tot filters, meningen, en groeperingen, zie [&#x200B; toegang van de Verlening tot filters, meningen, en groeperingen &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Uw beheerder van Workfront moet u toegang tot rapporten, dashboards, en kalenders in uw toegangsniveau verlenen om rapporten te kunnen bekijken of uitgeven.

  Voor informatie over het verlenen van toegang tot rapporten, dashboards, en kalenders, zie [&#x200B; de toegang van de Verlening tot rapporten, dashboards, en kalenders &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Als u een filter, weergave of groepering voor een rapport of lijst selecteert, behoudt Workfront deze selectie voor de lijsten van dat object zelfs nadat u zich hebt afgemeld of de browser hebt gesloten. Als u bijvoorbeeld een specifieke weergave voor een taakrapport selecteert, wordt die selectie weergegeven voor andere takenlijsten, zoals de takenlijst van een project.

## Filters

Het filter controleert de resultaten die in een rapport verschijnen, typisch versmalend resultaten van algemeen aan specifiek. Het werkt als een zeef die slechts de informatie graaft die u nodig hebt en die informatie terugbrengt naar uw rapport.

Bijvoorbeeld, als u slechts taken wilt zien die aan de het programma geopende gebruiker worden toegewezen, kunt u een filter tot stand brengen getiteld &quot;Mijn Taken,&quot;bepaalt de criteria die voor de filter moeten worden vervuld en het rapport in werking stellen om slechts taken te bekijken die aan de het programma geopende gebruiker worden toegewezen.

Enkele kenmerken van filters zijn:

* Workfront biedt standaard een aantal filters voor verschillende objecten.
* U kunt filters aanpassen die u bezit of beheert.

  Voor meer informatie over filters, zie het artikel [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Weergaven

Door de mening van een rapport te bepalen, bepaalt u welke informatie u in het rapport omvat. Net als alle rapportelementen zijn weergaven gebaseerd op één objecttype.

Een weergave voor een taakrapport kan bijvoorbeeld de vervaldatum weergeven, belangrijke financiële details zoals Kosten bevatten of worden gebruikt om de details van de toewijzingen en de leveringsdatum weer te geven. De meningen kunnen worden gebruikt om een verscheidenheid van details over de gegevens in het rapport te leveren.

Enkele weergavekenmerken zijn:

* U kunt een standaard Workfront-weergave gebruiken of uw eigen weergave maken.
* U kunt extra meningen van het drop-down gebied van de Mening toepassen na het runnen van een rapport.
* De extra meningen vervangen tijdelijk de mening die wanneer het creëren van het rapport wordt bepaald; nochtans, wordt de standaardmening getoond de volgende tijd u aan het rapport terugkeert.

  Voor meer informatie over meningen, zie het artikel [&#x200B; overzicht van Meningen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Groepen

Een groepering bepaalt hoe u gegevens ordent, waardoor het makkelijker wordt om te lezen en te begrijpen. Groepen leiden tot horizontale bars door een rapport dat resultaten toont die samen door gemeenschappelijke attributen worden vermeld. U bepaalt de criteria voor hoe u de resultaten van uw rapport wilt groeperen wanneer het creëren van de groepering.

Bijvoorbeeld, organiseert het groeperen van een lijst van taken die veelvoudige projecten door hun projectnaam overspannen alle respectieve taken die tot één enkel project onder die naam behoren.

Enkele kenmerken van groepen zijn:

* Groepen zijn een verplicht rapporteringselement als u een grafiek aan uw rapport wilt later toevoegen.
* Groepen geven een geaggregeerde waarde in de resultaten weer. &#x200B;
* Groepen bepalen de as in grafieken.
* Groepen bepalen de headeridentificatie in matrixrapporten.\
  Voor meer informatie over matrixrapporten, zie het artikel [&#x200B; een matrixrapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md) creëren.

* De hulp van groeperingen bouwt de Samenvatting tabel van een rapport, die de samengevoegde waarden van het rapport verstrekt.
* Workfront biedt standaard een aantal groepen voor verschillende objecten.
* U kunt groepen aanpassen die u hebt of beheert.

  Voor meer informatie over groeperingen, zie [&#x200B; Overzicht van Groepen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Overige rapporteringselementen

Naast filters, meningen, en groeperingen, kon u de volgende elementen aan een rapport ook toevoegen:

* **Herinnering**: Een open filter dat kan worden aangepast en verschillend worden toegepast telkens als u een rapport in werking stelt.\
  Voor meer informatie over herinneringen, zie het artikel [&#x200B; een herinnering aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

* **Grafiek**: U kunt uw rapporten verbeteren door een grafiek aan hen toe te voegen en de informatie op een visuele manier te tonen.\
  Voor meer informatie over grafieken in rapporten, zie het artikel [&#x200B; een grafiek aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.
