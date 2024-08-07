---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 2-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 2-release van 2018.2. De functionaliteit is op 5 april 2018 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in juni 2018 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 2018.2 Beta 2-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 2-release van 2018.2. De functionaliteit is op 5 april 2018 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in juni 2018 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2018.2 zijn aangebracht, raadpleegt u  [ 2018.2 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

De Beta 2-release van 2018.2 bevat de volgende verbeteringen:

* [ geef Gebieden direct van het Gebied van het Huis ](#edit-fields-directly-from-the-home-area) uit
* [ Tijd van het Logboek in Dagen ](#log-time-in-days)
* [ de Verhoudingen van de Predecessor van de Mening Cross-Project op de Grafiek van Gantt in een Lijst van Projecten ](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [ Begrotende Kosten van het Gebruik in Portfolio Optimizer om de Financiën van de Portfolio te berekenen ](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [ het Rapport van het Gebruik: Bevolkt de Beoogde Uren van het Nieuwe Bewegende Gebied van het Middel ](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (Voorproef slechts)

* [ het Rapport van het Gebruik: Mening Beoogde Uren door Gebruiker op een Project ](#utilization-report-view-budgeted-hours-by-user-on-a-project) (Voorproef slechts)

* [ Voortgang van het Bewijs van de Lijst van het Document Beschikbaar aan Niet-Proofing Gebruikers ](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Mobiele verbeteringen](#mobile-improvements)

## Velden rechtstreeks vanuit het begingebied bewerken {#edit-fields-directly-from-the-home-area}

Wanneer u nu een object selecteert in het gebied Home, kunt u de velden die aan dat object zijn gekoppeld rechtstreeks vanuit het rechterdeelvenster van het gebied Home bewerken. 

Vóór deze wijziging kon de informatie alleen worden weergegeven in het gebied Home, niet worden bewerkt.

Voor meer informatie, zie [ Update of geef een het werkpunt op het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) in het artikel uit  [ werk of geef een het werkpunt in het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) bij.

## Logtijd in dagen {#log-time-in-days}

Workfront-beheerders kunnen nu configureren of gebruikers in hun organisatie zich in dagen of uren aanmelden. Gebruikers met een Planner-licentie kunnen deze instelling voor zichzelf configureren.

Vóór deze wijziging konden gebruikers zich slechts in uren aanmelden.

U kunt deze instelling configureren door het gebruikersprofiel te bewerken. Voor meer informatie, zie [ vormen of de tijd uren of dagen ](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md) het programma wordt geopend.

Voor informatie over hoe de gebruikers tijd in dagen kunnen registreren nadat dit plaatsen is bijgewerkt, zie [ tijd van het Logboek ](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## De Verhoudingen van de Predecessor van het dwars-Project van de mening op de Grafiek van Gantt in een Lijst van Projecten {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

U kunt nu de relaties van voorgaande projecten voor meerdere projecten bekijken in het Gantt-diagram in de volgende lijsten met projecten:

* Het tabblad Projecten in een portfolio of programma
* In een projectrapport

Voorafgaand aan deze verandering, kon u cross-project voorgangersverhoudingen slechts voor individuele taken op het projectniveau bekijken.

Voor meer informatie, zie [ vormen hoe de informatievertoningen op de Grafiek van Gantt ](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## De Begrotende Kosten van het gebruik in Portfolio Optimizer om de Financiën van Portfolio&#39;s te berekenen {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

De nieuwe Optimizer van het Portfolio gebruikt nu de Begrotende Kosten van het nieuwe gebied van de Begroting van het Middel van het BedrijfsGeval of van de Planner van het Middel om de volgende gebieden te berekenen:

* Nettowaarde
* Rendement van investeringen (ROI)
* Kosten

Eerder gebruikte zowel het nieuwe als het oudere Portfolio Optimizer de verouderde budgettaire kosten. De Verouderde Optimizer van het Portfolio gebruikt nog de Verouderde Begrotende Kosten om Netto Waarde, Rendement op Investering, en Kosten te berekenen.

We hebben ook twee nieuwe velden toegevoegd aan het Portfolio Financial Fields: verouderde ROI en verouderde Net Value om de nieuwe waarden van de nieuwe hulpmiddelen voor resourcebeheer vast te leggen.

Voor meer informatie, zie [ Portfolio Optimizer overzicht ](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) in het artikel  [ Portfolio Optimizer overzicht ](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Gebruiksrapport: Bevolken begrote uren uren uit nieuw gebied voor de begroting van bronnen {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Deze functionaliteit wordt niet meegeleverd bij de officiële release naar de voorvertoningsomgeving met de release van 2018.2. Deze wordt opnieuw geïntroduceerd tijdens de bètaperiode voor de release van 2018.3 en wordt met de release van 2018.3 in de productieomgeving geïntroduceerd. 

De begrote Uren in het Rapport van het Gebruik zijn nu bevolkt van informatie beschikbaar in het nieuwe gebied van de Begroting van het Middel van de BedrijfsGeval.

Vóór deze verandering, werd de informatie van het gebied van de Schattingen van het erfenisMiddel gebruikt.

Voor meer informatie, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in het artikel  [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Gebruiksrapport: Beoogde uren per gebruiker weergeven voor een project {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Deze functionaliteit wordt niet meegeleverd bij de officiële release naar de voorvertoningsomgeving met de release van 2018.2. Deze wordt opnieuw geïntroduceerd tijdens de bètaperiode voor de release van 2018.3 en wordt met de release van 2018.3 in de productieomgeving geïntroduceerd. 

Het rapport van het Gebruik over een project toont nu Beoogde Uren door Gebruiker.

Voorafgaand aan deze verandering, toonde het rapport van het Gebruik begrotingsuren slechts door baanrol. 

Voor meer informatie, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in het artikel [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Voortgang proefdrukken vanuit de documentlijst beschikbaar voor gebruikers zonder proefdrukken {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Proefvoortgangsindicatoren (Verzonden, Geopend, Opmerkingen gemaakt en Besluit) worden nu voor alle gebruikers weergegeven wanneer ze de documentlijst bekijken. Dit geldt ook voor gebruikers die geen proefdrukken kunnen genereren (zie sectie voor meer informatie over het mogelijk maken van proefdrukken voor gebruikers).

Voorafgaand aan deze wijziging waren indicatoren voor de voortgang van het proefproject alleen beschikbaar voor gebruikers die proefdrukken konden maken.

Voor meer informatie, zie [ vooruitgang van het Bewijs en statusoverzicht ](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Mobiele verbeteringen {#mobile-improvements}

De mobiele app bevat de volgende verbeteringen:

* Koppelingen die met u worden gedeeld in andere mobiele toepassingen, worden nu geopend in de mobiele Workfront-app.

  Zie voor meer informatie over het delen van koppelingen.

  Deze update is nu beschikbaar op iOS en Android.

* We hebben onze supportvereisten voor het iOS-platform bijgewerkt om iPhone X te ondersteunen.

  Zie de . 
