---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 2-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 2-release van 2018.3. De functionaliteit is op 1 augustus 2018 beschikbaar in de voorvertoningsomgeving. Proofingverbeteringen die beschikbaar zijn in Beta 2 zijn woensdag 18 juli beschikbaar in de voorvertoningsomgeving. Het zal in november 2018 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 2018.3 Beta 2-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 2-release van 2018.3. De functionaliteit is op 1 augustus 2018 beschikbaar in de voorvertoningsomgeving. Proofingverbeteringen die beschikbaar zijn in Beta 2 zijn woensdag 18 juli beschikbaar in de voorvertoningsomgeving. Het zal in november 2018 beschikbaar worden gesteld in de productieomgeving.

>[!NOTE]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2018.3 zijn aangebracht, raadpleegt u  [ 2018.3 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

De Beta 2-release van 2018.3 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders**

* [Het e-mailadres in het gebruikersprofiel bijwerken als groepsbeheerder](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**voor Alle Gebruikers**

* [ de Goedkeuringen van de Mening aan me in het Gebied van het Huis ](#view-approvals-delegated-to-me-in-the-home-area) worden gedelegeerd
* [ Gegevens van de Uitvoer voor een bepaalde Periode in de Planner van het Middel ](#export-data-for-a-given-period-in-the-resource-planner)
* [ Dagelijkse Totalen nu Vertoning in Rood wanneer de Gebruiker ](#daily-totals-now-display-in-red-when-the-user-is-overallocated) wordt oververdeeld
* [ de Taken en de Kwesties worden verborgen op de Plannende Chronologie wanneer geminimaliseerd ](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [ Commentaren van de Filter en Reacties door Gebruiker in de het proef kijker ](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [ Commentaar op een Waaier van Beeldmateriaal in een Videoproef ](#comment-on-a-range-of-footage-in-a-video-proof)
* [ Nieuw PolylineHulpmiddel voor de Prijsverhoging van de Commentaar in de het proef kijker ](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Flash verwijderen voor rapport, kalender en document delen](#flash-removal-for-report-calendar-and-document-sharing)

## Het e-mailadres in het gebruikersprofiel bijwerken als groepsbeheerder {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

U kunt nu e-mailadressen bijwerken voor gebruikers die behoren tot een groep die u beheert. 

Eerder konden alleen Workfront-beheerders e-mailadressen voor andere gebruikers bijwerken. 

Voor meer informatie, zie [ de beheerders van de Groep ](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Goedkeuringen weergeven die aan mij zijn gedelegeerd in het thuisgebied {#view-approvals-delegated-to-me-in-the-home-area}

U kunt het gebied van het Huis nu gebruiken om project, taak, en geven goedkeuringen te bekijken die aan u zijn gedelegeerd.

Voorafgaand aan deze verandering, kon u gedelegeerde goedkeuringen slechts in Mijn Gebied van het Werk bekijken.

Voor meer informatie, zie [ de goedkeuringsverzoek van de Afgevaardigde ](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Gegevens exporteren voor een bepaalde periode in de bronnenplanner {#export-data-for-a-given-period-in-the-resource-planner}

Er wordt nu een nieuw venster weergegeven wanneer u de informatie exporteert in de functie Bronnen waarmee u een specifiek tijdframe voor het geëxporteerde bestand kunt selecteren.

Voorafgaand aan deze verbetering, kon u slechts de informatie uitvoeren die op het scherm wordt getoond.

Voor meer informatie over het uitvoeren van gegevens van de Planner van het Middel, zie [ het navigatieoverzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) in het artikel [ navigatie overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Dagelijkse totalen worden nu rood weergegeven wanneer de gebruiker teveel is toegewezen {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [ Overzicht van de Balancer van de Werkbelasting ](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Wanneer een gebruiker wordt oververdeeld, worden de dagelijkse totalen voor de dagen waarop de gebruiker wordt oververdeeld nu in rood weergegeven. Deze optie wordt alleen weergegeven wanneer de optie Totalen voor Daily Planned Hours weergeven is ingeschakeld in de tijdlijninstellingen voor planning. Voorafgaand aan deze verbetering, was er een rode bar indicator voor de dagen toen de gebruiker werd oververdeeld, maar de dagelijkse totalen getoond zonder een rood hoogtepunt.

Voor meer informatie over gebruikerstoewijzingen, zie &quot;gebruikerstoewijzingen in de Plannende gebieden beheren&quot;.

## Taken en problemen worden op de geplande tijdlijn verborgen wanneer deze tot pictogram zijn verkleind {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Wanneer u taken en problemen in uw planningtijdlijn minimaliseert, worden ze nu verborgen voor gebruikers en rollen als de optie Totalen van dagelijks geplande uren weergeven is ingeschakeld in uw instellingen. Taken en problemen in het gebied Niet toegewezen worden weergegeven in een gecomprimeerde weergave.

Eerder bij het minimaliseren van taken en kwesties, zouden de taken en de kwesties op de plannende chronologie voor gebruikers en rollen blijven, maar zouden in een samengeperste mening tonen.

Zie voor meer informatie over het minimaliseren van taken en problemen in de tijdlijn van de planning  &quot;Ga aan de slag met Resource Scheduling.&quot;

## Opmerkingen en reacties filteren op gebruiker in de proefdrukviewer {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Nu kunt u reacties opnemen wanneer u opmerkingen filtert die zijn gemaakt door gebruikers die u opgeeft. Dit is nuttig wanneer u zich op al wilt concentreren terugkoppelt die door een belangrijke recensent, zoals een cliënt of een projectmanager wordt gemaakt.

Het filteren op gebruiker was eerder beperkt tot alleen de opmerkingen die zijn gemaakt (gestart) door de revisoren die u opgeeft.

## Opmerking over een bereik beeldmateriaal in een videoproefdruk {#comment-on-a-range-of-footage-in-a-video-proof}

U kunt een opmerking maken voor een reeks beelden in een videoproefdruk. Dit is bijvoorbeeld handig wanneer u moet aangeven dat een segment met beeldmateriaal opnieuw moet worden opgenomen of verwijderd.

Eerder kon u alleen een opmerking maken voor één punt op een videotijdlijn.

## Nieuwe veelhoek voor opmerkingsmarkeringen in de proefdrukviewer {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Nu kunt u opmaakcodes voor meerdere lijnen gebruiken om gesegmenteerde lijnen en vormen te tekenen wanneer u een opmerking toevoegt aan een proefdruk. U kunt een open gesegmenteerde lijn of een gesloten vorm tot stand brengen. Dit gereedschap is vooral handig bij het werken met complexe afbeeldingen, zoals technische of architectonische afbeeldingen.

Wanneer u eerder een proefdruk markeert om een opmerking toe te voegen, kunt u een rechthoek, een rechte lijn, een vrije lijn of vorm of een pijl tekenen.

## Flash verwijderen voor rapport, kalender en document delen {#flash-removal-for-report-calendar-and-document-sharing}

De Flash is verwijderd uit de volgende dialoogvensters voor delen in Workfront:

* Rapporten
* Kalenders
* Documenten

U kunt deze objecten nog steeds delen zoals u dat eerder hebt gedaan, maar nu is de ervaring niet meer afhankelijk van Flash.
