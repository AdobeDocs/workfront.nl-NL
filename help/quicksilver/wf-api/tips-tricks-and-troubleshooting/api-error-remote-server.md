---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API-foutbericht 400 Ongeldig verzoek
description: API-foutbericht 400 Ongeldig verzoek
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# API-fout: &quot;De externe server heeft een fout geretourneerd (400): onjuiste aanvraag&quot;

## Probleem

De volgende fout treedt op wanneer u probeert de API te gebruiken om een aangepast veld te importeren naar een uitgave:

`The remote server returned an error: (400) Bad Request`

## Oorzaak

Deze fout treedt op wanneer u via de API een aangepast veld probeert te importeren uit een project waaraan geen aangepast formulier is gekoppeld met een rijonderwerp.

## Oplossing

Voeg de correcte douanevorm aan het Onderwerp van de Rij toe.

Meer over de Onderwerpen van de Rij leren, zie [ de Onderwerpen van de Rij ](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.
