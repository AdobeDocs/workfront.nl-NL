---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Documentinhoud ophalen via webhooks
description: Hiermee worden de onbewerkte bytes van een document geretourneerd
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 0%

---

# Documentinhoud ophalen via webhooks

Hiermee worden de onbewerkte bytes van een document geretourneerd

## URL

GET/download

## Zoekparameters

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> De document-id.</td> 
  </tr> 
 </tbody> 
</table>

## Antwoord

De onbewerkte bytes van het document.

**Voorbeeld:**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
