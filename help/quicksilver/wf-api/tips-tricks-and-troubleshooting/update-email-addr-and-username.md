---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Bijwerken naar e-mailadres werkt de gebruikersnaam niet bij
description: Bijwerken naar e-mailadres werkt de gebruikersnaam niet bij
author: Becky
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Bijwerken naar e-mailadres werkt de gebruikersnaam niet bij

## Probleem

Normaal gesproken `emailAddr` en `username` zijn hetzelfde kenmerk. Daarom als u een gebruiker verandert `emailAddr` kenmerk, de `username` kenmerk wordt automatisch bijgewerkt.

Wanneer de `username` komt niet overeen met de `emailAddr`, een update van de `emailAddr` werkt de `username` automatisch. Dit geldt voor beide `emailAddr` wijzigingen door de gebruikersinterface en via de API.

## Oorzaak

Het verschil kan op verschillende manieren worden gemaakt:

* De gebruikers die vóór de synchronisatieregel werden gecreeerd bestonden. Zeer oude gebruikersaccounts hebben deze kenmerken mogelijk niet synchroon.

* Gebruikers die via SSO zijn gemaakt op een moment dat het e-mailadres in Workfront hoofdlettergevoelig was. De auto-leveringsoptie SSO zou een case-sensitive controle voor gebruikers in werking stellen die op de attributen van de gebruiker van de identiteitsleverancier wordt gebaseerd. Wanneer een nauwkeurige gelijke niet bestond, zouden de auto-leveringsdiensten tot een nieuwe gebruiker leiden. Als een gebruiker al bestond, was er een potentieel dat de gebruikersnaam en `emailAddr` niet dezelfde behuizing zou hebben.

* Gebruikers die de `username` kenmerken die rechtstreeks via de API zijn bijgewerkt, en hun `emailAddr` is niet bijgewerkt. De `username` en `emailAddr` komt mogelijk niet overeen.

## Oplossing

Gebruik de API om de `username` kenmerk moet hetzelfde zijn als het kenmerk `emailAddr`. Na het synchroniseren van de kenmerken, om het even welke update aan `emailAddr` zal ook de `username` overeenkomen (wanneer het veld gebruikersnaam niet is opgenomen in de update).
