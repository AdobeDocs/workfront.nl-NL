---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Metagegevens ophalen voor een bestand of map
description: Metagegevens ophalen voor een bestand of map
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Metagegevens ophalen voor een bestand of map

Retourneert metagegevens voor het opgegeven bestand of de opgegeven map.

**URL**

GET /metadata?id= [ document of omslagidentiteitskaart ]

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
   <td>id</td> 
   <td>De id van het bestand of de map, waarnaar wordt verwezen door de websiteprovider. Dit is anders dan de Adobe Workfront-document-id. Gebruik de waarde '/' om de metagegevens van de hoofdmap op te halen.
   <p>Opmerking: de id mag maximaal 255 tekens lang zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Antwoord

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Type </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>titel </td> 
   <td>String </td> 
   <td>De naam van het document of de map</td> 
  </tr> 
  <tr> 
   <td>aardig </td> 
   <td>String </td> 
   <td>Hiermee wordt opgegeven of dit item een bestand of map ('bestand' of 'map') is</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>De id van het bestand of de map.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>Het URL-pad dat door een gebruiker wordt gebruikt om het document in een browservenster weer te geven. De URL kan worden gehost door de documentprovider of de native externe opslagprovider.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>Het URL-pad dat door een gebruiker wordt gebruikt om het document in een browservenster te downloaden. De URL kan worden gehost door de documentprovider of de native externe opslagprovider.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>Het MIME-type voor het bestand. (optioneel)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>De laatste keer dat dit bestand is gewijzigd (RFC 339-tijdstempel opgemaakt)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Lang</td> 
   <td> De grootte van het bestand in bytes. (optioneel)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolean</td> 
   <td> Hiermee wordt aangegeven of dit bestand of deze map alleen-lezen is voor de geverifieerde gebruiker.(optioneel) </td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld:** https://www.acme.com/api/metadata?id=12345
<pre>&lbrace;<br> titel:"Mijn Document", <br> soort:"dossier"<br> identiteitskaart":"12345", <br> viewLink:"https://www.acme.com/viewDocument?id=12345", <br> downloadLink:"https://www.acme.com/downloadDocument?id=12345", <br> mimeType:"image/png", <br> dateModified:"2014065T 17 :39: 45.251Z", <br> grootte: "32554694"<br></pre>

>[!NOTE]
>
>Foutafhandeling moet consistent zijn voor alle API-aanroepen. Zie de sectie &quot;Foutverwerking&quot; hieronder voor meer informatie.
