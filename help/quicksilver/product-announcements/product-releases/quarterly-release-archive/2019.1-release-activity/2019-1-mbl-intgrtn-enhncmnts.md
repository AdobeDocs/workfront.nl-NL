---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Verbeteringen op het gebied van mobiele en integratie
description: Deze pagina beschrijft alle verbeteringen in het beheer van bronnen die zijn opgenomen in de release van 2019.1. De functionaliteit is nu beschikbaar in de productieomgeving.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 6b86ba0d-977a-4c89-8832-e81bf28d9dad
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# 2019.1 Verbeteringen op het gebied van mobiele en integratie

Deze pagina beschrijft alle verbeteringen in het beheer van bronnen die zijn opgenomen in de release van 2019.1. De functionaliteit is nu beschikbaar in de productieomgeving.

Voor een lijst van alle veranderingen die in 2019.1 worden aangebracht, zie [&#x200B; 2019.1 overzicht van de versieactiviteit &#x200B;](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Bijgewerkt standaardfilter in de bronnenplanner

Het standaardfilter in de Planner van het Middel filtert niet meer door de Groep van het Project.

Wanneer het bekijken van de Planner van het Middel, ziet u nu slechts de projecten die huidig en datum-gevoelig door gebrek zijn. De informatie van de volgende projecten is standaard inbegrepen:

* Met een geplande Voltooiingsdatum die na de eerste datum van de maand van vandaag voorkomt.
* Met een Geplande Datum van het Begin die vóór de laatste datum van de vierde maand van vandaag voorkomt.
* Met een status van Actief of Planning.

Eerder, zou het standaardfilter de informatie van de volgende extra projecten terugwinnen:

* Met een geplande Voltooiingsdatum die na de eerste datum van de maand van vandaag voorkomt.
* Met een Geplande Datum van het Begin die vóór de laatste datum van de vierde maand van vandaag voorkomt.
* Met een status van Actief of Planning.
* Met een Groep die de Groep van het Huis van de gebruiker aanpast die het programma wordt geopend.

Voor informatie over het toepassen van filters op de Planner van het Middel, zie [&#x200B; informatie van de Filter in de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Het gebruiken van Kaders voor de Filters van de Planner van het Middel

U kunt vervangingen nu gebruiken wanneer het bouwen van filters in de Planner van het Middel. U kunt bijvoorbeeld $$USER.ID gebruiken om te filteren voor informatie over de gebruiker die is aangemeld, of $$USER.companyID om informatie te filteren over alle gebruikers die tot hetzelfde bedrijf behoren als de gebruiker die is aangemeld. Voor een volledige lijst van op gebruiker-gebaseerde variabelen, zie de [&#x200B; Op gebruiker-gebaseerde de variabelen van de vervangingsfilter &#x200B;](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) sectie in [&#x200B; de filtervariabelen van de Verjaring &#x200B;](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Eerder waren jokertekens niet beschikbaar voor de filters Bronnen.

Voor informatie over het filtreren in de Planner van het Middel, zie [&#x200B; informatie van de Filter in de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)

VIDEO

## Ondersteuning voor op datum gebaseerde jokertekenfiltervariabelen in de functie voor middelenplanner

U kunt nu elke versie van de $$TODAY-jokertekenfiltervariabele gebruiken wanneer u een filter maakt in de Resource Planner.

Voorafgaand aan deze verbetering, kon u slechts op gebruiker-gebaseerde variabelen van de vervangingsfilter gebruiken.

Voor informatie over het filtreren in de Planner van het Middel, zie [&#x200B; informatie van de Filter in de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Voor informatie over de variabelen van de vervangingsfilter, zie [&#x200B; de filtervariabelen van de Vervanging &#x200B;](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

VIDEO

## Exportopties voor de weergave Rol in de bronnenplanner

U kunt nu selecteren welke informatieniveaus u wilt exporteren vanuit de functie voor middelenplanner in de weergave Rol.

U kunt het volgende exporteren:

* Alleen rollen
* Rollen en projecten
* Rollen, projecten en gebruikers

Vóór deze verbetering, werden alle niveaus van informatie uitgevoerd in de mening van de Rol. Deze opties zijn geïntroduceerd in de projectweergaven en gebruikersweergaven in een vorige release.

Voor informatie over het uitvoeren van informatie van de Planner van het Middel, zie [&#x200B; informatie van de Uitvoer van de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDEO

## Opties voor gegevensopmaak voor het exporteren van de bronnenplanner

U kunt nu selecteren hoe u informatie in het dossier van Excel wanneer uitgevoerd van de Planner van het Middel wilt tonen.

U kunt de beschikbaarheid en de toewijzing van informatie tonen die uit de Planner van het Middel op de volgende manieren wordt uitgevoerd:

* Degroepeerd door de naam van de objecten waartoe het behoort. In dit geval worden de namen van de objecten waartoe het behoort op elke gegevensrij weergegeven. (dit is de standaardoptie)
* Gegroepeerd door de naam van de objecten waartoe het behoort. In dit geval wordt de informatie in het geëxporteerde bestand weergegeven zoals deze wordt weergegeven in Workfront.

Vóór deze verbetering werd de informatie in het geëxporteerde bestand weergegeven zoals deze in Workfront wordt weergegeven.

Voor informatie over het uitvoeren van informatie van de Planner van het Middel, zie [&#x200B; informatie van de Uitvoer van de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDEO

## Tijdlijn voor continue planning

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [&#x200B; Overzicht van de Balancer van de Werkbelasting &#x200B;](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Door tijdlijnen te plannen blijft nu het tijdframe dat u hebt geselecteerd wanneer u de tijdlijn vernieuwt of bij de pagina vandaan navigeert.

Voorafgaand aan deze verbetering, kwamen de het plannen chronologie aan standaardtimeframe terug wanneer u verfrist of weg van de pagina navigeerde.

Deze verbetering is beschikbaar op de volgende gebieden:

* Tabblad Plannen in het gebied Personen
* Team werkt aan tabblad
* Subtab plannen op het tabblad Werkruimte van een project

Voor informatie over het werken met de chronologie in het Middel dat gebieden plant, zie &quot;begonnen worden met het Plannen van het Middel&quot;.

VIDEO

## Nieuwe exportopties in de bronnenplanner

U kunt nu selecteren welke informatieniveaus u wilt exporteren vanuit de functie voor middelenplanning.

In de projectweergave kunt u een van de volgende handelingen exporteren:

* Alleen projecten
* Projecten en rollen
* Projecten, rollen en gebruikers

In de gebruikersweergave kunt u een van de volgende handelingen exporteren:

* Alleen gebruikers
* Gebruikers en projecten
* Gebruikers, Projecten, Rollen, Taken, en Kwesties

Voorafgaand aan deze verbetering, werden alle niveaus van informatie uitgevoerd in alle meningen van de Planner van het Middel door gebrek.

Voor informatie over het uitvoeren van informatie van de Planner van het Middel, zie [&#x200B; informatie van de Uitvoer van de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDEO

## Update aan de Mening van de Gebruiker in de Planner van het Middel

Alle gebruikers in het systeem tonen nu in de Mening van de Gebruiker van de Planner van het Middel, maar slechts tonen de gebruikers verbonden aan de gefiltreerde projecten ook uurinformatie.

Voorafgaand aan deze update, slechts hebben de gebruikers aan het werkpunten op de projecten toegewezen u voor getoond in de Mening van de Gebruiker van de Planner van het Middel filtert.

U kunt op gebruiker-gebaseerde filters gebruiken om het aantal gebruikers te verminderen dat in de Mening van de Gebruiker wordt getoond aan slechts die die aan de projecten worden toegewezen u wilt tonen.

Voor informatie over filters in de Planner van het Middel, zie [&#x200B; informatie van de Filter in de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
