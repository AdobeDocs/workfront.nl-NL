---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: alleen items weergeven in een goedkeuringsstatus'
description: U kunt alleen objecten weergeven met een bepaalde status die momenteel in behandeling is. Dit werkt hetzelfde voor elk ander object met een goedkeuringsstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Filter: alleen items weergeven in een goedkeuringsstatus

<!--Audited: 10/2024-->

U kunt alleen objecten weergeven met een bepaalde status die momenteel in behandeling is. Dit werkt hetzelfde voor elk ander object met een goedkeuringsstatus.

U kunt de volgende objecten in een goedkeuringsstatus plaatsen:

* Taken
* Problemen
* Projecten

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

## Alleen items weergeven die de goedkeuringsstatus hebben

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.
1. Kies aan filter door **Project: Status**, dan selecteer de status u door van de lijst wilt filtreren.

   Bijvoorbeeld, in een projectrapport, voeg **Gelijke Planning van de Status** toe, als u slechts projecten wilt tonen die in een status van **Planning - in afwachting van Goedkeuring** zijn.
1. Klik **wijze van de Tekst**.
1. Wijzig de regel `status` door **:A** toe te voegen aan de 3-letterige sleutel van de status:
   <pre>status=PLN:A<br> status_Mod=in</pre>

1. Klik **toepassen** > **sparen als nieuw**.

   De lijst toont slechts projecten die in een status van Planning - in afwachting van Goedkeuring zijn.
