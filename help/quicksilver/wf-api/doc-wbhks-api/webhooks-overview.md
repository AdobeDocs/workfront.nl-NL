---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Overzicht van webhooks
description: Overzicht van webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '209'
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

**Implementatie van de Verwijzing**

Workfront geeft voorbeelden van een voorbeeldimplementatie om de ontwikkeling van een nieuwe webhooks-implementatie te versnellen. Deze voorbeelden kunnen in [ https://github.com/Workfront/webhooks-app ](https://github.com/Workfront/webhooks-app) worden gevonden. De voorbeelden zijn gebaseerd op Java en stellen Workfront in staat om documenten te verbinden met een netwerkbestandssysteem. 

>[!NOTE]
>
>De middelen op GitHub zijn slechts voorbeelden, en kunnen geen implementatie uitvoeren.

## Versies

* Versie 1.0 (Releasedatum - mei 2015): initiële specificatie

* Versie 1.1 (Releasedatum - juni 2015). Bijgewerkt /uploadInit - Toegevoegde documentId en documentVersionId

* Versie 1.2 (Releasedatum - oktober 2015): Toegevoegd /createFolder

* Volgende versies (Releasedatum - TBD):

   * Toegevoegd /delete
   * Toegevoegde /naam wijzigen
   * Toegevoegde /serviceInfo
   * Toegevoegde /customAction
   * Paginering en parentId toevoegen aan /search
