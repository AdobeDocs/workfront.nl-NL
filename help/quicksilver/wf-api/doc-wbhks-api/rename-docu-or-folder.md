---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Naam wijzigen van document of map (nog niet geïmplementeerd)
description: De naam van een document of map wijzigen
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 1%

---


# Naam wijzigen van document of map (nog niet geïmplementeerd)

Hiermee wijzigt u de naam van een document of map met de opgegeven id in het externe systeem.

**URL**

PUT /naam wijzigen

## Zoekparameters

| Naam  | Beschrijving |
|---|---|
| id | De document- of map-id waarvan de naam moet worden gewijzigd |
| name  | De nieuwe naam van het document of de map |


## Antwoord

Een JSON-tekenreeks die aangeeft of de functie is gelukt of mislukt, zoals is opgegeven in de sectie Foutafhandeling hieronder.

**Voorbeeld:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

retourneert

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
