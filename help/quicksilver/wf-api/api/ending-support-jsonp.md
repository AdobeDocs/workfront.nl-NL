---
content-type: api
navigation-topic: api-navigation-topic
title: Aflopende ondersteuning voor JSONP
description: Aflopende ondersteuning voor JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Aflopende ondersteuning voor JSONP

Omdat JSONP (Javascript met het Opvullen) een oude norm met bekende veiligheidskwetsbaarheid is, zal Adobe Workfront JSONP niet meer steunen vanaf November 2018. Dit besluit steunt ons grotere initiatief om het Workfront-platform te moderniseren.

JSONP is een norm waardoor de dwars-oorsprong of intersite verzoeken kunnen worden uitgevoerd. Vele klanten en partners van Workfront gebruiken JSONP om tot Workfront van een systeem op hun eigen domein als deel van een integratie toegang te hebben. JSONP staat voor verzoeken van niet-Workfront domeinen toe om door de toepassing van Workfront worden verwerkt.

Als u JSONP als deel van om het even welk van uw integratie van Workfront gebruikt, moet u uw integratie bijwerken om de norm van CORS (het Delen van Middelen van het Middel van de Cross-Origin) te gebruiken. Voor deze update moet u het volgende doen:

1. Verzend een verzoek bij het ondersteuningsteam van Workfront om om het even welke domeinen te hebben die worden gebruikt om verzoeken van de dwars-oorsprong aan onze lijst van gewenste personen te maken.

   Als u uw domeinen wilt toevoegen aan de lijst van gewenste personen voor CORS, neemt u contact op met de klantenondersteuning van Workfront op 844-306-HELP(4357) of door een ondersteuningsticket online in te dienen.

   >[!NOTE]
   >
   >Het toevoegen van domeinen aan de lijst van gewenste personen voor CORS wordt gesteund slechts voor klanten die JSONP voorafgaand aan 1 Augustus, 2018 gebruikten.


1. Breng wijzigingen aan in uw integratiecode om CORS te gebruiken.
