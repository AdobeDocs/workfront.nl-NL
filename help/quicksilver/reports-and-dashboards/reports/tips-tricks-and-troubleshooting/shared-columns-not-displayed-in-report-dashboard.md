---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Gegevens uit gedeelde kolommen worden niet weergegeven in dashboardrapporten
description: De gegevens van gedeelde kolommen tonen niet wanneer het rapport in een veelvoudige kolomdashboardlay-out wordt geplaatst, maar het toont op één enkele kolomlay-out. Regeleinden worden ook overschreven.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Gegevens uit gedeelde kolommen worden niet weergegeven in dashboardrapporten

## Probleem

De gegevens van gedeelde kolommen tonen niet wanneer het rapport in een veelvoudige kolomdashboardlay-out wordt geplaatst, maar het toont op één enkele kolomlay-out. Regeleinden worden ook overschreven.

## Oorzaak

Alleen kolommen gemarkeerd als

```
shortview=true
```

worden opgenomen in de dashboardweergave van het rapport wanneer de indeling van het dashboard de splitsing naar links/rechts of de splitsingsinstelling naar links/midden/rechts bevat.

## Oplossing

Open de weergave die wordt gebruikt in het rapport en open tekstmodus. (Voor meer informatie, zie [ een mening uitgeven gebruikend tekstwijze ](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Label alle kolommen in het rapport, inclusief de kolommen die worden gebruikt in een gedeelde/samengevoegde kolom, met

```
shortview=true
```

. De rapportkolommen zullen dan behoorlijk in het dashboard tonen.
