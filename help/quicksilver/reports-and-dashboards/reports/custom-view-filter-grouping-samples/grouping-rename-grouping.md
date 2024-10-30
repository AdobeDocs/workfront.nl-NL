---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: de weergavenaam in een groep bewerken'
description: U kunt de namen van groepen in lijsten en rapporten wijzigen in iets wat de gebruikers beter bekend is.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Groeperen: de weergavenaam in een groep bewerken

<!--Audited: 01/2024-->

U kunt de namen van groepen wijzigen in iets wat de gebruikers beter bekend is.

Bijvoorbeeld, wanneer u de standaardgroepering van de Naam van het Portfolio op een lijst van projecten toepast, verschijnt de naam van de groepering als *Portfolio: Naam:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

U kunt deze groepering wijzigen door in de tekstmodus een naam weer te geven die beter leesbaar is.

![](assets/grouping-edited-name-350x160.png)

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

## De weergavenaam in een groep bewerken

De weergavenaam wijzigen in een projectgroep:

1. Ga naar een lijst met projecten.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **toevoegen groepering**, en beginnen &quot;Naam van het Portfolio&quot;in de **Groep te typen door:** gebied, dan selecteer het wanneer het in de lijst toont.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Voer een van de volgende handelingen uit:

   * Voeg de volgende code aan de bestaande tekst beschikbaar in de **Groep uw doos van het Rapport** toe:


     `group.0.displayname=Your Value`


     Voeg bijvoorbeeld de volgende code toe om de weergavenaam te wijzigen in &quot;Portfolio&quot;:

     `group.0.displayname=Portfolio`

   * Verwijder alle regels in de interface van de tekstmodus van de groep die het woord &quot;naam&quot; bevatten en voeg vervolgens de regel toe:

     `group.0.name=Your Value`

     Voeg bijvoorbeeld de volgende code toe om de weergavenaam te wijzigen in &quot;Portfolio&quot;:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >U kunt ook de regels `group.0.name=` en `group.0.displayname=` leeg laten. In dat geval geeft de groepering de waarde weer waarop u groepeert.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Klik **Gedaan**, dan **sparen Groepering**.
1. (Facultatief) werk de groeperingsnaam bij, dan klik **sparen Groepering**.

   De standaardnaam voor de groepering wordt gewijzigd op basis van de gegevens in de tekstmodus.
