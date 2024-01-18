---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Workfront Fusion release activity: Week 7 november 2022"
description: Deze pagina beschrijft alle verbeteringen die in Adobe Workfront Fusion in de week van 7 november 2022 zijn aangebracht.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Workfront Fusion release activity: Week 7 november 2022

**Optimalisatie webshwachtrij**

De wachtrij van Fusion voor webhaken is geoptimaliseerd met deze release. De service die webhooks accepteert, staat nu los van wachtrijen en andere processen. Door deze wijziging kan Fusion webhaakwachtrijen sneller en consistenter verwerken.

Tijdens de implementatie van deze verandering, konden wij verwachte logboekverwerkingstijd beter voor een rij gevormde webhaakgebeurtenissen begrijpen. De webhaakviewerpagina van Fusion is naar verwachting niet ouder dan 1 minuut.

Navigeer naar Webhooks in linkernavigatie om webhaakgebeurtenissen in de wachtrij weer te geven. De pictogrammen van de vrachtwagen met een aantal in de teller wijzen op rijgebeurtenissen voor die webhaak. Klik op het vrachtwagenpictogram om de gebeurtenissen in de wachtrij te zien.

![](assets/fusion-webhook-queue-1866x567.png)


**Ongebruikte webhaken worden nu gedeactiveerd of verwijderd**

We hebben een aantal wijzigingen aangebracht in de manier waarop Workfront Fusion ongebruikte webhaken verwerkt. Webhooks worden nu automatisch gedeactiveerd als een van de volgende twee van toepassing is:

* De webhaak is langer dan vijf dagen niet verbonden met een scenario.
* De webhaak wordt alleen gebruikt in inactieve scenario&#39;s, die al meer dan 30 dagen inactief zijn.

gedeactiveerde webhaken worden automatisch verwijderd en niet geregistreerd als ze niet zijn aangesloten op scenario&#39;s en meer dan 30 dagen in de gedeactiveerde status zijn geweest.
