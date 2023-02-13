---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Geplande loonkosten berekenen
description: Terwijl u het werk aan uw projecten plant, berekent Adobe Workfront de geplande arbeidskosten voor de rollen en gebruikers die aan dit werk zijn toegewezen op basis van hun kosten per uur-waarden.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Geplande loonkosten berekenen

Terwijl u het werk aan uw projecten plant, berekent Adobe Workfront de geplande arbeidskosten voor de rollen en gebruikers die aan dit werk zijn toegewezen op basis van hun kosten per uur-waarden.

De geplande arbeidskosten van een project is een berekening tussen de kosten verbonden aan de baanrollen of de gebruikers die worden toegewezen om het werk aan het project te voltooien en de hoeveelheid geplande uren (Geplande Uren) die elke rol of gebruiker zou kunnen nemen om dat werk te voltooien.

## Overzicht van de geplande loonkosten

De **Geplande loonkosten** van een project wordt berekend door alle geplande arbeidskosten van alle taken van het project op te tellen.

>[!TIP]
>
>Er zijn geen geplande arbeidskosten verbonden aan kwesties of met het project zelf.

Workfront berekent de geplande loonkosten van een project met behulp van de volgende formule:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

De geplande loonkosten van de Taak worden berekend op basis van het volgende:

* Het aantal middelen voor de taak en de individuele toewijzing ervan aan de taak
* Het kostentype van taak.

De taak Geplande Kosten van de Arbeid wordt berekend gebruikend de volgende formule:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Voor meer informatie over hoe Workfront Geplande Arbeidskosten voor taken berekent, afhankelijk van taaktaken en het Type van Kosten, zie de &quot;wijzig de Types van Kosten voor individuele taken&quot;sectie in het artikel [Trackkosten](../../../manage-work/projects/project-finances/track-costs.md).

## Zoek de geplande arbeidskosten

U kunt de geplande arbeidskosten van een project in de volgende gebieden van Workfront vinden:

* Een projectrapport
* Een lijst van projecten
* Een rapport van de Basislijn waar u het in tijd kunt volgen
* Via de API

Raadpleeg de volgende artikelen voor informatie over het maken van rapporten en het gebruik van de Workfront API:

* [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Basisbeginselen van API](../../../wf-api/general/api-basics.md)
