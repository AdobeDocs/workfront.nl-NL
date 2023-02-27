---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Overzicht van webhooks
description: Overzicht van webhooks
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Overzicht van webhooks

Adobe Workfront Document Webhooks definieert een set API-eindpunten waarmee Workfront geoorloofde API-aanroepen uitvoert naar een externe documentprovider. Hierdoor kan iedereen een middleware-insteekmodule maken voor elke leverancier van documentopslag.

![](assets/mceclip0-350x262.png)

De gebruikerservaring voor integratie op basis van een webhaak is vergelijkbaar met die van bestaande documentintegratie, zoals Google Drive, Box en Dropbox. Een Workfront-gebruiker kan bijvoorbeeld de volgende handelingen uitvoeren:

* Navigeren door de mapstructuur van de externe documentprovider
* Bestanden zoeken
* Bestanden koppelen naar Workfront
* Bestanden uploaden naar de externe documentprovider
* Een miniatuur voor het document weergeven

**Referentie-implementatie**

Workfront biedt een voorbeeldimplementatie om de ontwikkeling van een nieuwe webhooks-implementatie te versnellen. Code hiervoor is te vinden op [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . Deze implementatie is gebaseerd op Java en maakt het Workfront mogelijk om verbinding te maken met documenten op een netwerkbestandssysteem. 

## Versies

* Versie 1.0 (Releasedatum - mei 2015): Oorspronkelijke specificatie

* Versie 1.1 (Releasedatum - juni 2015). Bijgewerkt /uploadInit - Toegevoegde documentId en documentVersionId

* Versie 1.2 (Releasedatum - oktober 2015): Toegevoegde /createFolder

* Volgende versies (Releasedatum - TBD):

   * Toegevoegd /delete
   * Toegevoegde /naam wijzigen
   * Toegevoegde /serviceInfo
   * Toegevoegde /customAction
   * Paginering en parentId toevoegen aan /search
