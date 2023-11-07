---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Bestand uploaden via documentwebhoos
description: Bestand uploaden via documentwebhoos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# Bestand uploaden via documentwebhoos

Het uploaden van een bestand naar een leverancier van documentopslag is een proces in twee stappen waarvoor twee afzonderlijke API-eindpunten nodig zijn. Adobe Workfront begint het uploadproces door /uploadInit te roepen. Dit eindpunt keert een document identiteitskaart terug die dan tot /upload wordt overgegaan wanneer het uploaden van de documentbytes. Afhankelijk van het onderliggende documentopslagsysteem kan het nodig zijn om een document met een lengte van nul te maken en de inhoud van het document later bij te werken.

De document-id en de document-versie-id zijn toegevoegd aan versie 1.1 van deze specificatie en kunnen worden gebruikt om extra informatie van Workfront op te halen.

**Voorbeeld:** Als het documentbeheersysteem extra informatie over het document wil, kan de webhimplementatiecode de document-id gebruiken om die informatie op te halen met de Workfront RESTful-API. Als goede praktijk, kon deze informatie uit de gebieden van douanegegevens op het document komen en het bevat taak, kwestie, of project.

## Methode POST

**URL**

POST /uploadInit

### Zoekparameters

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
   <td>parentId </td> 
   <td>De bovenliggende map-id, waarnaar wordt verwezen door de websiteprovider.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>De naam van het document</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>De Workfront-document-id (toegevoegd in versie 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>De Workfront-document versie-id (toegevoegd in versie 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## Antwoord

De meta-gegevens voor het dossier, zoals die door het /metadata eindpunt wordt bepaald. Hieronder valt de document-id die door de provider wordt gebruikt.

**Voorbeeld:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Methode PUT

Hiermee uploadt u de bytes van een document naar de websiteprovider.

**URL**

PUT /upload

## Zoekparameters

| Naam  | Beschrijving |
|---|---|
| id  |  De document-id, die zojuist is gemaakt. |


**Indieningsinstantie**

De onbewerkte inhoudbytes voor het document.

**Antwoord**

```
{
result: "success"
}
```

of

```
{
result: "fail"
}
```

**Voorbeeld**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

reactie

```
{
result:"success"
}
```
