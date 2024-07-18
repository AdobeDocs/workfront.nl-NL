---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Bijwerken naar e-mailadres werkt de gebruikersnaam niet bij
description: Bijwerken naar e-mailadres werkt de gebruikersnaam niet bij
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Bijwerken naar e-mailadres werkt de gebruikersnaam niet bij

## Probleem

Normaal gesproken zijn `emailAddr` en `username` hetzelfde kenmerk. Als u daarom het kenmerk `emailAddr` van een gebruiker wijzigt, wordt het kenmerk `username` automatisch overeenkomstig bijgewerkt.

Als de `username` niet overeenkomt met de `emailAddr` , wordt de `username` niet automatisch bijgewerkt wanneer de `emailAddr` wordt bijgewerkt. Dit geldt voor zowel `emailAddr` -wijzigingen via de gebruikersinterface als via de API.

## Oorzaak

Het verschil kan op verschillende manieren worden gemaakt:

* De gebruikers die vóór de synchronisatieregel werden gecreeerd bestonden. Zeer oude gebruikersaccounts hebben deze kenmerken mogelijk niet synchroon.

* Gebruikers die via SSO zijn gemaakt op een moment dat het e-mailadres in Workfront hoofdlettergevoelig was. De auto-leveringsoptie SSO zou een case-sensitive controle voor gebruikers in werking stellen die op de attributen van de gebruiker van de identiteitsleverancier wordt gebaseerd. Wanneer een nauwkeurige gelijke niet bestond, zouden de auto-leveringsdiensten tot een nieuwe gebruiker leiden. Als een gebruiker al bestond, konden de gebruikersnaam en `emailAddr` niet dezelfde behuizing hebben.

* Gebruikers waarvan het kenmerk `username` rechtstreeks via de API is bijgewerkt, en waarvan het kenmerk `emailAddr` niet is bijgewerkt. De tekens `username` en `emailAddr` komen mogelijk niet overeen.

## Oplossing

Gebruik de API om het kenmerk `username` op dezelfde manier in te stellen als het kenmerk `emailAddr` . Na het synchroniseren van de kenmerken wordt bij elke update naar `emailAddr` ook de `username` bijgewerkt zodat deze overeenkomt (wanneer het veld gebruikersnaam niet is opgenomen in de update).
