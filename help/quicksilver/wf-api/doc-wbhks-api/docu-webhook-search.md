---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Zoeken via documentwebhaken
description: Zoeken via documentwebhaken
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Zoeken via documentwebhaken

Retourneert metagegevens voor de bestanden en mappen die door een zoekopdracht worden geretourneerd. Dit kan als full-text onderzoek of als regelmatige gegevensbestandvraag worden uitgevoerd. Adobe Workfront roept het /search eindpunt wanneer de gebruiker een onderzoek van externe dossierbrowser uitvoert.

## URL

GET/zoekopdracht

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
   <td>query</td> 
   <td>De zoekterm of uitdrukking.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optioneel) De map-id waaruit de zoekopdracht is uitgevoerd. Opmerking: Dit is een tijdelijke aanduiding voor een toekomstige functie in Workfront. Workfront geeft deze parameter momenteel niet door. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Het maximumaantal items dat moet worden geretourneerd. Wordt gebruikt voor paginering.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> De pagina-verschuiving, gebruikt in combinatie met 'max'.</td> 
  </tr> 
 </tbody> 
</table>

 

## Antwoord

JSON bevat een lijst met metagegevens voor bestanden en mappen die overeenkomen met de query. Wat een &quot;gelijke&quot;is wordt bepaald door de websiteleverancier. In het ideale geval wordt een zoekopdracht in volledige tekst uitgevoerd. Het uitvoeren van een op bestandsnaam gebaseerde zoekopdracht werkt ook.

**Voorbeeld:**

Voorbeeld:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
