---
title: Toewijzingen in een verwijderd object worden onverwacht weergegeven in toewijzingsrapporten
description: Toewijzingen in een verwijderd object worden onverwacht weergegeven in toewijzingsrapporten
author: Courtney
draft: Probably
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Toewijzingen in een verwijderd object worden onverwacht weergegeven in toewijzingsrapporten

## Probleem

Nadat u een object met een toewijzing hebt verwijderd, worden zowel het object als de toewijzing verwijderd. Maar de opdracht komt misschien nog wel voor in sommige verslagen.

Als u bijvoorbeeld een taak verwijdert die aan een gebruiker is toegewezen, wordt de toewijzing aan de gebruiker ook verwijderd. Nochtans, als u later een taakrapport in werking stelt dat door toegewezen, met die gespecificeerde gebruiker wordt gefiltreerd, maakt het rapport nog een lijst van de geschrapte taak als de taak nog in de Bak van de Recycling is.

## Oorzaak

Dit komt door architecturale beperkingen van de prullenbak. Op dit moment zijn er geen plannen in de routekaart om dit probleem aan te pakken vanwege de omvang van het architectonisch herontwerp dat nodig zou zijn.
