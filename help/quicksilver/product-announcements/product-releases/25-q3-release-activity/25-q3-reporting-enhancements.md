---
title: Derde kwartaal 2025 — Rapportverbeteringen
description: Verbeteringen van projecten in het derde kwartaal van 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Derde kwartaal 2025 — Rapportverbeteringen

Op deze pagina worden alle rapportverbeteringen beschreven die zijn aangebracht met de release Derde kwartaal 2025 voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving, zoals vermeld.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Derde Kwartaal 2025 versiecyclus, zie [&#x200B; Derde Kwartaal 2025 releaseoverzicht &#x200B;](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Uitgebreide beveiliging voor levering van rapporten

* Voorbeeld: 26 juni 2025
* Productie: geleidelijke uitrol van 26 juni 2025 tot 9 juli 2025

We hebben de levering van geplande rapporten verbeterd om ervoor te zorgen dat Workfront-berichten alleen worden verzonden naar e-maildomeinen die zijn goedgekeurd in de lijst van gewenste personen.

Als uw organisatie een beperking had gedefinieerd voor de e-maildomeinen waarvan Workfront-meldingen werden verzonden, zouden we tijdens het toevoegen van e-mails een controle uitvoeren op de lijst van gewenste personen.

Nu voeren we ook een controle uit terwijl het e-mailbericht wordt verzonden om te controleren of het ingevoerde e-mailadres voldoet aan de lijst van gewenste personen voor e-mail. Deze verbeterde controle is van toepassing op e-mailadressen die aan gebruikers zijn gekoppeld en op e-mails ad hoc die aan de lijst met rapportontvangers worden toegevoegd.

Voor meer informatie, zie [&#x200B; Plan een automatische rapportlevering &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


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
