---
content-type: release-notes
title: 'Eerste kwartaal van 2026: releaseactiviteit voor Adobe Workfront Planning'
description: Dit is de versieactiviteit voor het product van de Planning van Adobe Workfront voor het Eerste Kwartaal 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: fdfb1ecb61fd85fa927fc7c3443c2a7f23409873
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Eerste kwartaal van 2026: releaseactiviteit voor Adobe Workfront Planning

In dit artikel worden de functies beschreven die tijdens de release Eerste kwartaal van 2026 beschikbaar zijn voor Workfront Planning.

<!--keep the sentence below for all future quarterly release pages-->

Voor een lijst van alle eigenschappen die voor de Planning van Adobe Workfront worden vrijgegeven, zie [ de versieactiviteit van de Planning van Adobe Workfront: artikelindex ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Algemene recordtypen en de mogelijkheid om deze als bestaande recordtypen toe te voegen aan andere werkruimten

>[!NOTE]
>
>Voorbeeld: 16 oktober 2025
>>Snelle productie: 13 november 2025
>>Productie voor iedereen: 15 januari 2026

Wanneer het uitvoeren van de Planning van Workfront voor een multi-teamorganisatie met gemeenschappelijke werkschema&#39;s, zou u een samenhangende structuur en meta-gegevens voor zeer belangrijke verslagtypes (zoals Campagnes of Deliverables) kunnen moeten bepalen die aan de werkruimten van elk team kunnen worden toegevoegd om hun werk te vangen en te beheren.

Ook, zou u het werk van elk team kunnen nodig hebben om tot een centraal niveau te rollen.

In zulk een werkschema, kunt u ervoor zorgen dat de teams hun werk constant vangen terwijl het ontgrendelen van dwars-teamzicht, zonder de behoefte om iedereen in de organisatie aan elke werkruimte toe te voegen. Hiervoor kunt u algemene recordtypen gebruiken.

U kunt nu een recordtype toewijzen dat globaal moet zijn en het gebruiken in meerdere werkruimten. Gebruikers kunnen dezelfde veldstructuur en verbindingen gebruiken die al in een centrale werkruimte zijn geconfigureerd.

Raadpleeg de volgende artikelen voor meer informatie:

* [ het type van het werkruimterecord overzicht ](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [ vorm verslagtype dwars-werkruimtemogelijkheden ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Bestaande recordtypen uit een andere werkruimte toevoegen](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Nieuwe limiet voor verbindingsvelden voor één recordtype

>[!NOTE]
>
>Voorbeeld: 16 oktober 2025
>>Snelle productie: 13 november 2025
>>Productie voor iedereen: 15 januari 2026

Voor elk recordtype is een limiet van 30 verbindingsvelden ingesteld.

NOTA: Als uw organisatie momenteel meer dan 30 verbindingsgebieden voor één verslagtype heeft, kunt u de extra gebieden houden die de grens van 30 overschrijden. U kunt echter geen verbindingsvelden toevoegen aan recordtypen die de limiet overschrijden. In de toekomst wordt de nieuwe limiet van 30 verbindingsvelden gehandhaafd.

Voor meer informatie, zie [ Verbonden overzicht van de Types van Verslag ](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Gebruikersvriendelijke waarden instellen voor keuzen in selectievelden

>[!NOTE]
>
>Voorbeeld: 16 oktober 2025
>>Snelle productie: 13 november 2025
>>Productie voor iedereen: 15 januari 2026

Wanneer u veldopties toevoegt aan een veld met één of meerdere selecties, wijst Workfront nu unieke gebruikersvriendelijke waarden toe aan elke keuze. Vóór deze verbetering, produceerde Workfront een alpha-numerieke identiteitskaart die moeilijk te begrijpen en in API vraag en andere integraties was te gebruiken.

Overweeg het volgende met deze verbetering:

* De nieuwe waarden worden toegevoegd aan nieuwe veldopties. Bestaande veldopties behouden hun alfanumerieke id&#39;s.

* De gekozen waarden zijn uniek voor één veld, maar kunnen tussen verschillende velden worden herhaald.

* Als u de naam van een keuze wijzigt, wordt de oorspronkelijke waarde niet bijgewerkt.

* De gekozen waarden worden weergegeven in kleine letters en worden gescheiden door onderstrepingstekens in het geval van keuzen voor meerdere woorden. Als u een label gebruikt dat al is gebruikt als een andere keuzenaam voor hetzelfde veld, voegt Workfront een volgnummer aan de waarde toe.

Voor informatie, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.