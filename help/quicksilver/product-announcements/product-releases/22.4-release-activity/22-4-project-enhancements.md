---
title: 22.4 Projectverbeteringen
description: 22.4 Projectverbeteringen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# 22.4 Projectverbeteringen

Op deze pagina worden alle projectverbeteringen beschreven die zijn aangebracht met de release 22.4 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de week van 3 oktober 2022.

Voor een lijst van alle veranderingen beschikbaar met versie 22.4, zie [22.4 Overzicht van de release](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Details van voorgaande versies zijn nu beschikbaar

Als u de details van de voorgangers van een taak wilt bekijken, kunt u de muisaanwijzer nu boven het voorganger plaatsen in de kolom Voorgangers. In het detailvak ziet u de vorige taak en het project waarnaar wordt verwezen, de geplande begin- en einddatum voor de voorgangertaak en het aantal voorgangers en opvolgers van de voorgangertaak. U kunt de projectdetails uitbreiden om meer informatie over het project te zien. Aanvullende informatie is opgenomen voor predecessors die voor meerdere projecten werken.

Zie voor meer informatie [Een voorganger-relatie maken in de takenlijst](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Meerdere teams toewijzen aan een taak of uitgave

Om u veel meer flexibiliteit in de manier te geven u taken en kwesties beheert, hebben wij het mogelijk gemaakt om veelvoudige teams aan een taak of een kwestie toe te wijzen. Eerder kon slechts één team worden toegewezen aan een taak of uitgave.

>[!NOTE]
>
>Deze functionaliteit is momenteel niet beschikbaar in Workload Balancer in het gebied Teams.

Zie voor meer informatie [Taken toewijzen](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) en [Problemen toewijzen](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Slimme gebruikersselectie voor projectrollen in Edit en de gebieden van Details

Wij hebben de manier verbeterd de gebruikers tonen wanneer u hen aan de volgende projectgebieden van Edit doos en de sectie van Details van het project toevoegt:

* Projecteigenaar

* Projectsponsor

* Resource Manager

Wanneer u nu een gebruiker aan een van deze velden toevoegt in de gebieden Bewerken of Details, naast de naam en avatar, worden ook de primaire rol en de e-mail weergegeven. Zo kunt u beter onderscheid maken tussen meerdere gebruikers met dezelfde of vergelijkbare namen.

Zie voor meer informatie [Projecten bewerken](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTA: De extra gebruikersgebieden voor projecten, taken, en kwesties zullen met deze functionaliteit in toekomstige versies worden bijgewerkt.

[Bekijk een videodemonstratie van deze functie.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Berekende datumvelden worden altijd opgeslagen op basis van UTC (Coordinated Universal Time)

Nu, kunt u zeker zijn dat alle datumfuncties in berekende gebieden constant werken en het zelfde resultaat voor iedereen produceren, ongeacht hoe een uitdrukking van douanegegevens wordt bijgewerkt, of waar de gebruikers aan het voorwerp over de wereld samenwerken.

Alle berekeningen worden nu berekend en bewaard door één norm - gecoördineerde Universele Tijd (UTC)-niet door de configuraties van de tijdzone die voor de instantie van uw organisatie en uw individueel gebruikersprofiel worden geplaatst. Berekeningen worden echter in een aangepast formulier weergegeven op basis van de afzonderlijke tijdzones van elke gebruiker die in de browser zijn ingesteld.

Eerder veroorzaakten de tijdmontages in berekeningen verwarring wanneer zij in deze situaties veranderden:

* Als iemand een berekende veldexpressie opnieuw heeft berekend met behulp van &quot;Vorige berekeningen bijwerken&quot; in de formulierbuilder, zijn de resultaten van de datumfunctie bepaald door de UTC-tijdzone van uw organisatie.

* Als iemand het object heeft bewerkt en de berekende veldexpressie opnieuw heeft berekend, zijn de resultaten van de datumfunctie bepaald door de lokale tijdzone van de gebruiker. De resultaten van het berekende datumveld in dit scenario worden ook berekend op basis van de UTC.

Zie voor meer informatie [Werken in tijdzones](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Aangepaste formulierverbeteringen: Adobe XD en het snelfilter

Op basis van uw feedback hebben we de volgende verbeteringen geïntroduceerd om uw ervaring bij het beheren van aangepaste formulieren te verbeteren:

* Voeg een Adobe XD-bestand toe om een aangepast formulier visueel en informatief te maken. Wanneer het formulier aan een object is gekoppeld, kunnen gebruikers die met het object werken het XD bestand vanuit het formulier bekijken en ermee werken.

  Zie voor meer informatie [Een afbeelding of andere middelenwidget toevoegen of bewerken in een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Met het snelle filter kunt u gemakkelijk items zoeken in de gemoderniseerde lijst met aangepaste formulieren en velden. Geniet ook van een verbeterde look and feel tijdens het beheren van uw formulieren en velden.

  Zie voor meer informatie over het snelle filter [Het snelle filter toepassen op een lijst](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Bekijk een videodemonstratie van deze functie.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Openbare bètaversie - Nieuwe filterervaring voor projecten, taken en problemen

Het filtreren in project, taak, en de lijst van de kwestie is opnieuw ontworpen om u te helpen filters snel creëren en delen. Functies:

* Een intuïtieve bètabuilder-interface voor het maken van een nieuw filter

* De mogelijkheid om een filter als favoriet te markeren

* Filter stapelen (meerdere opgeslagen filters toepassen)

* Filters dupliceren

* Filters delen

* Filters verwijderen die met u worden gedeeld


De nieuwe filterervaring is ook beschikbaar in timesheet lijsten en de Planner van het Scenario.

De tekstmodus blijft beschikbaar voor geavanceerde filterbewerkingen en systeembeheerders kunnen nog steeds standaardfilters voor alle gebruikers toewijzen via de lay-outsjablonen.

### Waar zal dit beschikbaar zijn?

* Lijst met projecten/taken/problemen

* Scenario Planner

* Timesheets


### We willen je feedback.

Met deze Openbare bètaversie krijgen gebruikers de gelegenheid om feedback rechtstreeks naar het team te verzenden dat aan de filterervaring werkt door op de knop Feedback te klikken. We kijken ernaar uit om van u en uw gebruikers te horen over de nieuwe filterervaring in openbare bèta. Als uw team met product direct zou willen ontmoeten om extra te verstrekken terugkoppelt, voel vrij om een vergadering hier te plannen: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Wat nu?

* Ervaring voor nieuwe groepen en weergaven (ook wel Kolommen genoemd)

  We gaan werken aan de nieuwe ervaring voor groepen en weergaven (ook wel kolommen genoemd). Deze ervaring is dus consistent met de nieuwe filterervaring en bevat enkele van de geweldige functies die de nieuwe filters bieden.

* Nieuwe filters implementeren in andere gebieden van Adobe Workfront

  We zullen samenwerken met teams over het hele product om de nieuwe filterervaring op andere gebieden in Workfront te implementeren.


We willen u hierbij een meerwaarde bieden, zodat we ook in de toekomst resultaten zullen boeken als de nieuwe ervaringen en andere gebieden klaar zijn. Blijf op de hoogte voor spannender updates.

Zie voor meer informatie [Overzicht van filters](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) en [Filters maken of bewerken in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Bekijk een videodemonstratie van deze functie.](https://video.tv.adobe.com/v/3412391/)
