---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Een document of map verwijderen
description: Een document of map verwijderen
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 0%

---


# Een document of map verwijderen (nog niet geïmplementeerd)

Hiermee verwijdert u een document of map met de opgegeven id in het externe systeem. Als u een map verwijdert, wordt ook de inhoud van de map verwijderd.

## URL

PUT /delete

## Zoekparameters

| Naam  | Beschrijving |
|---|---|
| documentId  | Te verwijderen document-id |
| folderId  |  De te verwijderen map-id |



## Antwoord

Een JSON-tekenreeks die aangeeft of de functie is gelukt of mislukt, zoals is opgegeven in de sectie Foutafhandeling hieronder.

### Voorbeeld

PUT https://www.example.com/api/deleteid=1234
* retourneert `status: "success"`

* retourneert `status: "failure", error: "File not found"`
