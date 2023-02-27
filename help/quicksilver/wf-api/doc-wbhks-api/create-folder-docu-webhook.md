---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Een map maken met documentwebkoppelingen
description: Een map maken met documentwebkoppelingen
author: Becky
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 1%

---


# Een map maken met documentwebkoppelingen

Maakt een map in een bepaalde map.

## URL

POST /createFolder

## Zoekparameters

| **Naam** | **Beschrijving** |
|---|---|
| parentId  | De map-id waarin de map moet worden gemaakt |
| name  | De naam van de nieuwe map |




**Antwoord**

De meta-gegevens voor de pas gecreëerde omslag, zoals die door het /metadata eindpunt wordt bepaald.

## Voorbeeld

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

retourneert

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
