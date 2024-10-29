---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: lijstresultaten ordenen met een berekende waarde die wordt gedeeld door alle objecten in de groepering'
description: U zou uw taken kunnen willen bekijken die door Percentage wordt gegroepeerd Voltooien in waaiers van 0-25, 26-50, 51-75, 75-99, en 100. Hiervoor kunt u een groepering maken in de tekstmodus.
author: Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Groeperen: lijstresultaten ordenen met een berekende waarde die hetzelfde is voor alle objecten in de groep

<!--Audited: 10/2024-->

U zou uw taken kunnen willen bekijken die door Percentage wordt gegroepeerd Voltooien in waaiers van 0-25, 26-50, 51-75, 75-99, en 100. Hiervoor kunt u een groepering maken in de tekstmodus.

![](assets/grouping-calculated-value-column-to-all-objects.png)

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

## De lijstresultaten organiseren met een berekende waarde die voor alle voorwerpen in de groepering gemeenschappelijk is

Deze groepering toepassen op een lijst met taken:

1. Ga naar een takenlijst.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Voeg de volgende code toe in de beschikbare ruimte:

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Klik **Gedaan**, dan **sparen Groepering**.
1. (Facultatief) werk de groeperingsnaam bij, dan klik **sparen Groepering**.
