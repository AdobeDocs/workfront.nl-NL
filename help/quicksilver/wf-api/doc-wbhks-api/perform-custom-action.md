---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Een aangepaste handeling uitvoeren
description: Een aangepaste handeling uitvoeren
author: John
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Een aangepaste handeling uitvoeren (nog niet geïmplementeerd)

Dit eindpunt staat een gebruiker van Adobe Workfront (of een geautomatiseerde werkschemagebeurtenis) toe om een actie in het externe systeem uit te voeren. Het /customAction eindpunt keurt een &quot;naam&quot;parameter goed, die de websiteleverancier toestaat om veelvoudige douaneverrichtingen uit te voeren.

De websiteleverancier registreert douaneacties met Workfront door de acties in de /serviceInfo reactie onder customActions te omvatten. Workfront laadt deze lijst bij het instellen of vernieuwen van de websiteprovider onder Instellen > Documenten > Aangepaste integratie.

Gebruikers kunnen de aangepaste handeling activeren door de sectie onder &quot;Documenthandelingen&quot; te selecteren

**URL**

GET /customAction

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
   <td> <p>name</p> </td> 
   <td> <p>De id die het type handeling aangeeft dat moet worden uitgevoerd. Deze waarde beantwoordt aan één van de waarden customAction die door het /serviceInfo eindpunt zijn teruggekeerd.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>De werkfront document-id waarvoor de handeling wordt uitgevoerd.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> De werkfront document versie-id waarvoor de handeling wordt uitgevoerd.</td> 
  </tr> 
 </tbody> 
</table>

 

## Antwoord

Een JSON-tekenreeks die aangeeft of de functie is gelukt of mislukt, zoals is opgegeven in de sectie Foutafhandeling hieronder. Bij een fout (d.w.z. status = &quot;mislukking&quot;) geeft Workfront het aangeboden foutbericht aan de gebruiker weer.

**Voorbeeld:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

reactie

```
{
status: “success”
}
```
