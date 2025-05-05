---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta Slotrelease
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta Final release van 2018.1. De functionaliteit is op 31 januari 2018 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in maart 2018 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 2018.1 Beta Slotrelease

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta Final release van 2018.1. De functionaliteit is op 31 januari 2018 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in maart 2018 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2018.1 zijn aangebracht, raadpleegt u  [ 2018.1 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

De slotversie van Beta van 2018.1 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders**

* [Vorm de Beschikbaarheid van het Middel en de Toewijzingen van de Gebruiker om Gebaseerd op het Programma van de Gebruiker te berekenen](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**voor Alle Gebruikers**

* [ Mobiele Verbeteringen ](#mobile-enhancements)
* [ Integratie Jira ](#jira-integration)
* [ Update aan het proefdrukken van kijkernamen ](#update-to-proofing-viewer-names)
* [ Verandering in de Koorden van de Synchronisatie wanneer het Synchroniseren van het Milieu van de Productie van het Proofing aan Voorproef ](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Het waarschuwingsbericht wordt weergegeven wanneer de limiet van 2.000 items wordt bereikt in de bronnenplanner](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Verbeteringen voor mobiele apparaten {#mobile-enhancements}

De volgende functionaliteit wordt begin maart 2018 in de Mobile App-winkels geïntroduceerd:

* Nieuwe navigatie: de startpagina van onze mobiele apps is opnieuw ontworpen.
* Home op Mobile: onze nieuwe thuisfunctionaliteit is nu ook bijgewerkt voor onze mobiele apps.

De nieuwe functionaliteit wordt ondersteund voor zowel de iOS- als de Android-platforms.

## Jira Integration {#jira-integration}

U kunt Jira-problemen nu koppelen aan Workfront-taken of -problemen door de invoegtoepassing Workfront voor Jira te installeren en configureren. Met deze integratie kunnen uw projectmanagers blijven werken in Workfront, terwijl uw ontwikkelingsingenieurs kunnen blijven werken in Jira, terwijl hun individuele punten door de integratie van Workfront met Jira worden verbonden.

U kunt het volgende door deze integratie vormen:

* Stel triggers in voor Workfront-toewijzingen om automatisch Jira-problemen te maken wanneer deze zich voordoen.
* Koppel Jira-problemen handmatig aan Workfront-taken of -problemen die eerder zijn gemaakt.
* Geef velden op die moeten worden gesynchroniseerd op de gekoppelde items zodra een van de items in een van de toepassingen is bijgewerkt.

De invoegtoepassing Workfront is beschikbaar voor zowel de On-Premise- als On-Demand-versies van Jira. De add-on is gratis en kan begin maart 2018 worden gedownload op de Atlassiaanse markt.

Voor meer informatie over Workfront toe:voegen-on voor Jira, met inbegrip van een verbinding om het te downloaden, zie [ Gebruikend Workfront met Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Bijwerken naar proofing van viewernamen {#update-to-proofing-viewer-names}

De namen van de op HTML5 gebaseerde testviewer en de op Flash gebaseerde testviewers zijn in het hele Workfront-systeem hernoemd. De vorige en bijgewerkte namen zijn als volgt: 

| **Vorige Naam** | **bijgewerkte Naam** |
|---|---|
| HTML5-proefviewer | Nieuwe proefdrukviewer |
| Viewer voor Flash-proefdrukken | Verouderde proefdrukviewer |

{style="table-layout:auto"}

 Voor meer informatie over het gebruiken van de nieuwe het proefKijker, zie [ het Reviseren Proofs in de het proefKijker.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Vorm de Beschikbaarheid van het Middel en de Toewijzingen van de Gebruiker om Gebaseerd op het Programma van de Gebruiker te berekenen {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [ Overzicht van de Balancer van de Werkbelasting ](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

De Workfront-beheerder kan nu bepalen hoe Workfront de beschikbaarheid van bronnen en de gebruikerstoewijzing op systeemniveau berekent (rekening houdend met uren en beschikbaarheid van FTE). De beheerder van Workfront kan middelbeschikbaarheid en gebruikerstoewijzing vormen die of gebruikend het standaardprogramma of het programma van de gebruiker worden berekend.

Deze instelling beïnvloedt de beschikbaarheid van gebruikers in de volgende omstandigheden bij het plannen van resources:

* Wanneer Workfront automatisch bronnen mag toewijzen, zoals wordt beschreven in &quot;Niet-toegewezen taken en uitgaven handmatig toewijzen in de planningsgebieden&quot;.

* Bij het weergeven van toewijzingsindicatoren, zoals beschreven in &quot;Gebruikerstoewijzingen beheren in de planningsgebieden&quot;.

Voor meer informatie, zie &quot;vormen hoe Workfront middeluur en VTE beschikbaarheid voor het Plannende gebied berekent&quot;.

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [ Overzicht van de Balancer van de Werkbelasting ](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Wijzigen in Synchronisatie-kring bij synchroniseren van de Proofingproductieomgeving naar Voorvertoning {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Deze wijziging wordt van kracht op 11 februari 2018.

Gegevens uit de Workfront Proof Production-omgeving worden nu elke week gesynchroniseerd met de Workfront Proof Preview-omgeving.

Vóór deze wijziging werden de gegevens maandelijks gesynchroniseerd van de Workfront Proof Production-omgeving naar de Preview-omgeving, terwijl de gegevens van de Workfront Production-omgeving wekelijks werden gesynchroniseerd met de Workfront Preview-omgeving. Deze discrepantie veroorzaakte enkele synchronisatiefouten bij het gebruik van Proofing-functionaliteit in de Workfront Preview-omgeving. 

Voor meer informatie, zie [ het Testen van Sandbox van de Voorproef Milieu - Workfront Proof ](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## Het waarschuwingsbericht wordt weergegeven wanneer de limiet van 2.000 items wordt bereikt in de bronnenplanner {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Aangezien wij momenteel aan een meer permanente oplossing werken om prestaties in de Planner van het Middel te verbeteren, hebben wij een grens van 2.000 punten voor elke mening geïntroduceerd u op de Planner van het Middel kunt toepassen:

* In de gebruikersweergave worden slechts 2000 toewijzingen weergegeven
* De mening van het Project toont slechts 2.000 projecten
* In de weergave Rol worden slechts 2000 rollen weergegeven

Wanneer de Planner van het Middel probeert om meer dan 2.000 punten te laden, toont een berichtvertoningen alarmerend u dat slechts 2.000 punten kunnen worden getoond.

Voor meer informatie over deze grenzen en hoe zij de Planner van het Middel beïnvloeden, zie {de vertoningsbeperkingen van de Banner van 0} Middel [&#128279;](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
