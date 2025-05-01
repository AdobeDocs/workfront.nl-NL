---
title: Derde kwartaal 2025 — Rapportverbeteringen
description: Verbeteringen van projecten in het derde kwartaal van 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Derde kwartaal 2025 — Rapportverbeteringen

Op deze pagina worden alle rapportverbeteringen beschreven die zijn aangebracht met de release Derde kwartaal 2025 voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving, zoals vermeld.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Derde Kwartaal 2025 versiecyclus, zie [ Derde Kwartaal 2025 releaseoverzicht ](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## De vervangingsresultaten van de gebruiker niet meer met een ongeldige waarde wanneer het filtreren

>[!NOTE]
>
>* Voorbeeld: 30 april 2025
>* Snelle productie: 15 mei 2025
>* Productie voor alle afnemers: 17 juli 2025

Wij hebben het gedrag van de gebruikersvervanging bijgewerkt om ongeldige waarde uit te sluiten wanneer het filtreren van een rapport. Deze verandering helpt de filter nauwkeurigere resultaten produceren, eerder dan het terugkeren van resultaten die een gebruiker hebben correct gevormd (een ongeldig resultaat).

Eerder, wanneer een gebruikersvervanging een ongeldige waarde produceerde, zou een rapport alle verslagen tonen die ook een ongeldige waarde hebben.

Deze wijziging is van toepassing op de volgende jokertekenfilters:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

