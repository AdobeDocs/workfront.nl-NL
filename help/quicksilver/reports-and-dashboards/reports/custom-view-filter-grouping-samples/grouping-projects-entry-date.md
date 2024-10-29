---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groepering: projecten op datum van binnenkomst"
description: In deze aangepaste projectgroep kunt u projecten weergeven die zijn gegroepeerd op hun entry-datumwaarden.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Groepering: projecten op datum van binnenkomst

In deze aangepaste projectgroep kunt u projecten weergeven die zijn gegroepeerd op hun entry-datumwaarden.

Elke groepering toont projecten met een Datum van de Ingang binnen:

* De laatste 30 dagen
* 30-60 dagen
* 60 dagen of ouder

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

## Projecten groeperen per ingangsdatum

Deze groep toepassen:

1. Ga naar een bestaand projectrapport, of creeer een nieuw projectrapport.\
   Voor meer informatie over het creëren van een rapport, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
1. Klik **de Acties van het Rapport** > **uitgeven**.
1. Van het **Groeperen** lusje, klik **Groepering** toevoegen.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Verwijder de tekst in de **Groep door** gebied.
1. Vervang de tekst door de volgende code:

   group.0.linkedname=direct
group.0.name=Project Entry
group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))&lt;=30,&quot;Last 30 Days&quot;,IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&amp;&amp;ABS(DATEDIFF({entryDate},$$TODAY))&lt;=60,&quot;30 -60 dagen&quot;,&quot;ouder dan 60 dagen&quot;)
group.0.valueFormat=atDateAsMonthString
textmode=true

1. Klik **Gedaan** > **sparen Groepering**.
1. (Facultatief) werk de naam van de groepering bij, dan klik **sparen Groepering**.
