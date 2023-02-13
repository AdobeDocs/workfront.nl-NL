---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Een map maken met documentwebkoppelingen
description: Een map maken met documentwebkoppelingen
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
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
