---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: uw huidige projecten weergeven in afwachting van goedkeuring'
description: De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van Portfolio is.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Filter: uw huidige projecten weergeven in afwachting van goedkeuring

<!--Audited: 10/2024-->

De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van Portfolio is.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
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

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Huidige projecten filteren in afwachting van goedkeuring

Dit filter toepassen:

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.

1. Klik **wijze van de Tekst**.
1. Kopieer en plak de volgende code in het weergegeven gebied:
   <pre>status=CUR:A<br> sponsorID=$$USER.ID <br> OF :a: status=CUR:A <br> OF :a: portefeuille:ownerID=$$USER.ID</pre>

1. Klik **toepassen** > **sparen als nieuw**.
