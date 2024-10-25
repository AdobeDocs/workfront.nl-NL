---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: alleen items in een goedkeuringsstatus weergeven'
description: U kunt alleen objecten weergeven met een bepaalde status die momenteel in behandeling is. Dit werkt hetzelfde voor elk ander object met een goedkeuringsstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
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

## Alleen items weergeven die de goedkeuringsstatus hebben

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe filter**.
1. Kies aan filter door **Project: Status**, dan selecteer de status u door van de lijst wilt filtreren.

   Bijvoorbeeld, in een projectrapport, voeg **Gelijke Planning van de Status** toe, als u slechts projecten wilt tonen die in een status van **Planning - in afwachting van Goedkeuring** zijn.
1. Klik **wijze van de Tekst**.
1. Wijzig de `status` lijn door **toe te voegen:A** aan de 3 letterige sleutel van de status:
   <pre>status=PLN:A<br> status_Mod=in</pre>

1. Klik **toepassen** > **sparen als nieuw**.

   De lijst toont slechts projecten die in een status van Planning - in afwachting van Goedkeuring zijn.
