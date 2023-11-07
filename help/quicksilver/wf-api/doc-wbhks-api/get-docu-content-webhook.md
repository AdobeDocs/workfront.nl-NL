---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Documentinhoud ophalen via webhooks
description: Hiermee worden de onbewerkte bytes van een document geretourneerd
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '43'
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

The raw bytes of the document.

**Voorbeeld**:  `https://www.acme.com/api/download?id=123456`
