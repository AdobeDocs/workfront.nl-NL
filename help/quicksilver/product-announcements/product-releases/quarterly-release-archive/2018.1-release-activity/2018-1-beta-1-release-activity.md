---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 1-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 1-release van 2018.1. De functionaliteit op deze pagina is op 1 december 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in maart 2018 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# 2018.1 Beta 1-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 1-release van 2018.1. De functionaliteit op deze pagina is op 1 december 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in maart 2018 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2018.1 zijn aangebracht, raadpleegt u  [&#x200B; 2018.1 overzicht van de versieactiviteit &#x200B;](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

De Beta 1-release van 2018.1 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders**

* [&#x200B; Bijgewerkt Malplaatje van de Lay-out om het Gebied van het Huis &#x200B;](#updated-layout-template-to-support-the-home-area) te steunen
* [&#x200B; maak het Bewijzen E-mailberichten onbruikbaar die van Workfront worden verzonden &#x200B;](#disable-proofing-email-notifications-sent-from-workfront)
* [Nieuwe bronnen toegevoegd aan abonnementen op gebeurtenissen](#new-resources-added-to-event-subscriptions)

**voor Alle Gebruikers**

* [&#x200B; Gebied van het Huis (Bijgewerkt Mijn Gebied van het Werk) &#x200B;](#home-area-updated-my-work-area)
* [&#x200B; Gegevens van de Planner van het Middel van de Vertoning onder het BedrijfsGeval en Bijgewerkte Samenvatting Bedrijfs van het Geval &#x200B;](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [&#x200B; Vertoning het Percentage van Geplande Toewijzing van het Uur in de Planner van het Middel &#x200B;](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [&#x200B; de &quot;Automatische en op Verandering&quot;en &quot;Verandering slechts&quot;Update Types de Trekker van Updates aan de Ouderlijke Voorwerpen tezelfdertijd zoals de Taken worden bijgewerkt &#x200B;](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Tijdlijnopname beschikbaar in de Gantt-grafiek](#timeline-snapshot-available-in-the-gantt-chart)

## Thuisgebied (Mijn werkgebied is bijgewerkt) {#home-area-updated-my-work-area}

Het nieuwe gebied van het Huis verstrekt een afwisselende, verbeterde mening aan de zelfde gegevens die momenteel in het Mijn gebied van het Werk beschikbaar zijn. Het gebied van het Huis verstrekt de volgende voordelen over het Mijn Gebied van het Werk:

* Een meer gestroomlijnde en intuïtieve interface
* Verbeterde prestaties
* Taken en problemen met tekstopmaak bijwerken

## Bijgewerkte lay-outsjabloon ter ondersteuning van het thuisgebied {#updated-layout-template-to-support-the-home-area}

Als beheerder van Workfront, kunt u bepalen of de gebruikers in uw organisatie toegang tot het gebied van het Huis hebben door het lay-outmalplaatje te vormen zij aan worden toegewezen. Gebruikers aan wie geen lay-outsjabloon is toegewezen, hebben altijd toegang tot het gebied Home.

Zie &quot;Lay-outsjablonen maken en beheren&quot; voor meer informatie.

## Proofing-e-mailberichten die vanuit Workfront zijn verzonden uitschakelen {#disable-proofing-email-notifications-sent-from-workfront}

U kunt nu configureren of gebruikers in uw Workfront-exemplaar e-mailberichten van Workfront ontvangen wanneer er een opmerking wordt gemaakt op een proefdruk.

Eerder werden door Workfront altijd e-mails verzonden waarin werd aangetoond dat er opmerkingen waren gemaakt. Als meldingen ook in Workfront Proof waren ingeschakeld, ontvingen gebruikers dubbele meldingen. 

Voor bestaande Workfront-klanten is Workfront standaard geconfigureerd om e-mailberichten te verzenden wanneer er een opmerking wordt gemaakt op een proefdruk.

Zie voor informatie over het uitschakelen van e-mailmeldingen voor proefdrukken in Workfront, zodat e-mails met proef alleen vanuit Workfront Proof worden verzonden.  

## De Gegevens van de Planner van het Middel van de vertoning onder BedrijfsGeval en Bijgewerkt Overzicht Bedrijfs van Gevallen {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

Het gebied van de Begroting van het Middel is nu beschikbaar in het BedrijfsGeval van een project. Op dit gebied kunt u de begrote uren die voor uw middelen in de Planner van het Middel en de begrote arbeidskosten verbonden aan hen worden geschat herzien.

Het gebied van de Schattingen van het Middel van het BedrijfsGeval is anders genoemd aan de Schattingen van het Middel van de Oudheid.

Als deel van deze verandering, omvat de Samenvatting van BedrijfsGeval nu financiële informatie die op zowel de Schattingen van het Middel als het Begrotingen van het Middel wordt gebaseerd.

Voorafgaand aan deze verandering, kon u niet de informatie van de Planner van het Middel over het BedrijfsGeval van het project zien. U kon slechts informatie van de Schattingen van het Middel zien die in de Planner van de Band van de Capaciteit van de Oudere Groepen van Middel wordt gespecificeerd.

Voor meer informatie over het creëren van een BedrijfsGeval, zie [&#x200B; een BedrijfsGeval voor een project &#x200B;](../../../../manage-work/projects/define-a-business-case/create-business-case.md) creëren.

## Het percentage van de geplande uurtoewijzing weergeven in de bronnenplanner {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

De mening van de Gebruiker van de Planner van het Middel omvat nu een nieuwe kolom die u toelaat om de Geplande Toewijzing van het Uur als percentage van de totale Beschikbare Uren voor de gebruiker en de baanrol te bekijken.

Voorafgaand aan deze wijziging kon u het totaal van Geplande en Beschikbare Uren voor gebruikers en baanrollen slechts in afzonderlijke kolommen bekijken.

Voor meer informatie over de Geplande kolom van het Percentage van de Toewijzing van Uren, zie het &quot;Bekijken van het Verschil tussen Beschikbare en Geplande Uren of VTE in de sectie van de Planner van het Middel&quot;in [&#x200B; overzicht van de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## De &quot;Automatische en bij Verandering&quot;en &quot;Verandering slechts&quot;Update typt updates aan de Ouderlijke Voorwerpen tezelfdertijd zoals de Taken worden bijgewerkt {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

We hebben de manier gewijzigd waarop bovenliggende taken en de projectupdate worden uitgevoerd wanneer een object op een lager niveau in een project wordt bijgewerkt. De tijd wanneer een oudervoorwerp bijwerkt wordt bepaald door het gebied van het Type van Update op een project. U kunt een van de volgende updatetypen selecteren:

* Automatisch en bij wijziging
* Alleen wijzigen
* Alleen automatisch
* Alleen handmatig

Nu, wanneer u &quot;Automatisch en bij Verandering&quot;of &quot;Verandering slechts&quot;de Types selecteert van Update, worden de veranderingen u op de individuele taken toepast ook toegepast op de oudertaak en het project onmiddellijk.

Vóór deze wijziging moest u de pagina vernieuwen om ervoor te zorgen dat de bovenliggende objecten en de tijdlijn van het project ook werden bijgewerkt.

Voor meer informatie over het Type van Update van een project, zie [&#x200B; het Type van projectupdate &#x200B;](../../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.

## Tijdlijnopname beschikbaar in de Gantt-grafiek {#timeline-snapshot-available-in-the-gantt-chart}

U kunt nu snel naar een bepaald punt in de levensduur van een project schuiven met de nieuwe tijdlijnmomentopname in het Gantt-diagram.

Wanneer u een korter tijdkader voor de grafiek van Gantt terwijl het bekijken van een taak of een projectlijst selecteert, wordt een horizontale rolbar getoond bij de bodem van de grafiek van Gantt. Als u op de schuifbalk klikt, kunt u de volledige tijdlijn van het project in een momentopname bekijken. U kunt overal binnen de grafiekmomentopname van Gantt klikken om aan een specifiek punt in het leven van het project te navigeren.

Vóór deze wijziging moest u horizontaal schuiven op het hele Gantt-diagram om een bepaald tijdstip te vinden, of u moest uitzoomen uit de korrelweergave.

Voor meer informatie over hoe de informatievertoningen in de grafiek van Gantt, zie [&#x200B; vormen hoe de informatievertoningen op de Grafiek van Gantt &#x200B;](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Nieuwe bronnen toegevoegd aan abonnementen op gebeurtenissen {#new-resources-added-to-event-subscriptions}

Nu kunt u gebeurtenisabonnementen voor de volgende middelen tot stand brengen:

* **Kosten:** deelt u mee wanneer een uitgave wordt toegevoegd of gewijzigd.
* **Taak:** deelt u mee wanneer een taak op een taak of een kwestie voor een gebruiker, een baanrol, of een team wordt toegevoegd of wordt gewijzigd.
* **Chronesheet:** deelt u mee wanneer een timesheet wordt voorgelegd, verworpen, of goedgekeurd.

Meer over gebeurtenisabonnementen leren, zie [&#x200B; Abonnement API van de Gebeurtenis &#x200B;](../../../../wf-api/general/event-subs-api.md).
