---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Naam wijzigen van document of map (nog niet geïmplementeerd)
description: De naam van een document of map wijzigen
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# Naam wijzigen van document of map (nog niet geïmplementeerd)

Hiermee wijzigt u de naam van een document of map met de opgegeven id in het externe systeem.

**URL**

PUT /naam wijzigen

## Zoekparameters

| Naam  | Beschrijving |
|---|---|
| id | De naam van het document of de map moet worden gewijzigd |
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
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
