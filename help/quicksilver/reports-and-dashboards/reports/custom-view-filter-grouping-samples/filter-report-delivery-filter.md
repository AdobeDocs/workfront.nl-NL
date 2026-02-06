---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Rapporten weergeven gepland voor levering'
description: Dit rapportfilter geeft alle rapporten weer die automatisch worden geleverd in Adobe Workfront. U kunt deze instelling het beste gebruiken in de standaardweergave.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: be102fd5f490b12837a231774253c030973c1c4f
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Filter: weergaverapporten die zijn gepland voor levering

<!--Audited: 10/2024-->

Dit rapportfilter geeft alle rapporten weer die automatisch worden geleverd in Adobe Workfront. U kunt deze instelling het beste gebruiken in de standaardweergave.

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

## Rapportfilter

Dit filter toepassen:

1. Ga naar een lijst met rapporten.

1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe Filter**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.

1. In het **plaats de Regels van de Filter voor uw gebied van het Rapport**, kopieer en kleef de volgende code:

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Klik **sparen Filter**.
