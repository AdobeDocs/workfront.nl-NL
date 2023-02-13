---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hier worden metagegevens voor bestanden of mappen weergegeven
description: Hier worden metagegevens voor bestanden of mappen weergegeven
author: John
feature: Workfront API
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: d89d8cec90678aa3a047d1bfc0f1a8dd1682c58a
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Itemlijst met mapinhoud ophalen

Hier worden metagegevens voor de bestanden en mappen voor een bepaalde map weergegeven.

**URL**

GET/bestanden

## Zoekparameters

| Naam  | Beschrijving |
|---|---|
| parentId  | De map-id. Gebruik de waarde &#39;/&#39; om de metagegevens van de hoofdmap op te halen. |
| max  | Het maximumaantal items dat moet worden geretourneerd. Wordt gebruikt voor paginering. |
| offset  |  De pagina-verschuiving, gebruikt in combinatie met &#39;max&#39;. |


## Antwoord

JSON bevat een lijst met bestanden en mappen. De meta-gegevens voor elk punt zijn het zelfde dat door het /metadata eindpunt is teruggekeerd.

**Voorbeeld:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
