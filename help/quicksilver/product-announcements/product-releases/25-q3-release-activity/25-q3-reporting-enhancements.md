---
title: Verbeteringen voor rapportage derde kwartaal 2025
description: Verbeteringen van het project in het derde kwartaal van 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Verbeteringen voor rapportage derde kwartaal 2025

Op deze pagina worden alle rapportverbeteringen beschreven die zijn aangebracht met de release van het derde kwartaal van 2025 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving, zoals aangegeven.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Derde Kwartaal 2025 versiecyclus, zie [ Derde Kwartaal 2025 releaseoverzicht ](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Uitgebreide beveiliging voor levering van rapporten

* Voorbeeld: 26 juni 2025
* Productie: geleidelijke uitrol van 26 juni 2025 tot 9 juli 2025

We hebben de levering van geplande rapporten verbeterd om ervoor te zorgen dat Workfront-meldingen alleen worden verzonden naar e-maildomeinen die zijn goedgekeurd in de bovenstaande lijst.

Als uw organisatie eerder een beperking had gedefinieerd voor welke e-maildomeinen Workfront-meldingen, zouden we tijdens het toevoegen van e-mails een controle uitvoeren op de toegestane lijst.

We voeren nu ook een controle uit terwijl het e-mailbericht wordt verzonden om te controleren of het ingevoerde e-mailadres voldoet aan de lijst met toegestane e-mailadressen. Deze verbeterde controle is van toepassing op e-mailadressen die zijn gekoppeld aan gebruikers en op ad-hoce-mails die zijn toegevoegd aan de lijst met rapportontvangers.

Voor meer informatie, zie [ Plan een automatische rapportlevering ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## jokertekens van gebruikers retourneren niet langer resultaten met een null-waarde bij het filteren

>[!NOTE]
>
>* Voorbeeld: 30 april 2025
>* Snelle productie: 15 mei 2025
>* Productie voor alle afnemers: 17 juli 2025

We hebben het jokertekengedrag van gebruikers bijgewerkt om null-waarde uit te sluiten bij het filteren van een rapport. Deze wijziging helpt het filter nauwkeuriger resultaten te produceren in plaats van resultaten te retourneren waarvoor de gebruiker niet correct is geconfigureerd (een null-resultaat).

Eerder, wanneer een gebruikersparakter een ongeldige waarde produceerde, zou een rapport alle verslagen tonen die ook een ongeldige waarde hebben.

Deze wijziging is van toepassing op de volgende jokertekenfilters:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
