---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Informatie ophalen over de service
description: Informatie ophalen over de service
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Informatie ophalen over de service (nog niet geïmplementeerd)

>[!NOTE]
>
>De releasedatum voor deze functie moet nog worden bepaald.

Retourneert informatie over de service, zoals functies en mogelijkheden. Adobe Workfront gebruikt deze informatie om de gebruikersinterface in Workfront aan te passen. Als de implementatie van de webhaak bijvoorbeeld aangepaste handelingen bevat, moet de JSON deze bewerkingen in de JSON opnemen. Gebruikers kunnen deze acties dan aanroepen vanuit Workfront.

**URL**

GET/serviceInfo

## Zoekparameters

Geen. Bovendien zouden de vraag aan dit eindpunt geen authentificatie moeten vereisen.

## Antwoord

JSON met informatie over deze service

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam</th> 
   <th>Type </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhaakversie </td> 
   <td>String </td> 
   <td>De webhaakversie die door deze service is geïmplementeerd. Dit is het versienummer dat boven aan deze specificatie staat.</td> 
  </tr> 
  <tr> 
   <td>versie </td> 
   <td>String </td> 
   <td>Het interne versienummer voor deze service. Dit nummer wordt bepaald door de webhookprovider en wordt alleen ter informatie gebruikt.<br><br></td> 
  </tr> 
  <tr> 
   <td>uitgever </td> 
   <td>Tekenreeks </td> 
   <td>De naam van het bedrijf dat de webhook-implementatie verzorgt.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>Een lijst die de API Eindpunten bevat die door deze dienst worden uitgevoerd. Dit kan worden gebruikt om ervoor te zorgen dat de gebruikersinterface in Workfront de mogelijkheden weerspiegelt die door de websiteprovider worden aangeboden. Elk punt in de lijst moet de naam van het eindpunt (zoals "onderzoek") omvatten.</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>Een lijst met de aangepaste bewerkingen die door deze webhook zijn geïmplementeerd. Elk lijstitem bevat een naam en een weergavenaam. De weergavenaam wordt weergegeven in het vervolgkeuzemenu Documenthandelingen in Workfront. Wanneer u op het item in de vervolgkeuzelijst klikt, wordt de handeling in de webhook aangeroepen door het eindpunt /customAction aan te roepen.</p></td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld:** `https://www.acme.com/api/serviceInfo`

retourneert

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
