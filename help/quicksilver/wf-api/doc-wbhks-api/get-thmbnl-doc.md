---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Een miniatuur voor een document ophalen
description: Een miniatuur voor een document ophalen
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Een miniatuur voor een document ophalen

Retourneert de onbewerkte miniatuurbytes voor een document.

**URL**

GET /miniatuur

## Zoekparameters

| Naam  | Beschrijving |
|---|---|
| id  | De document-id. |
| size  |  De breedte van de miniatuur. |


## Antwoord

De onbewerkte miniatuurbytes.

**Voorbeeld:**: https://www.acme.com/api/thumbnail?id=123456
