---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: uw huidige projecten weergeven in afwachting van goedkeuring'
description: De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van het Portfolio is.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Filter: uw huidige projecten weergeven in afwachting van goedkeuring

<!--Audited: 10/2024-->

De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van het Portfolio is.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Huidige projecten filteren in afwachting van goedkeuring

Dit filter toepassen:

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. Klik **wijze van de Tekst**.
1. Kopieer en plak de volgende code in het weergegeven gebied:
   <pre>status=CUR:A<br> sponsorID=$$USER.ID <br> OF :a: status=CUR:A <br> OF :a: portefeuille:ownerID=$$USER.ID</pre>

1. Klik **toepassen** > **sparen als nieuw**.
