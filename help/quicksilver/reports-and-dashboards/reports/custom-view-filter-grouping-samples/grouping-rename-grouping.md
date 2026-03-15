---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: de weergavenaam in een groep bewerken'
description: U kunt de namen van groepen in lijsten en rapporten wijzigen in iets dat uw gebruikers beter kennen.
author: Courtney
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Groeperen: de weergavenaam in een groep bewerken

<!--Audited: 01/2024-->

U kunt de namen van groepen wijzigen in iets wat de gebruikers beter bekend is.

Bijvoorbeeld, wanneer u de standaardPortfolio Naam groepering op een lijst van projecten toepast, verschijnt de naam van de groepering als *Portfolio: Naam:`<name of portfolio>`*.

![ groepering door onuitgegeven naam ](assets/grouping-unedited-name-350x167.png)

U kunt deze groepering wijzigen in de tekstmodus om een naam weer te geven die beter leesbaar is.

![ groepering door uitgegeven naam ](assets/grouping-edited-name-350x160.png)

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven. 

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
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De weergavenaam in een groep bewerken

De weergavenaam in een projectgroep wijzigen:

1. Ga naar een lijst met projecten.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **toevoegen groepering**, en beginnen &quot;Naam van Portfolio&quot;in de **Groep te typen door:** gebied, dan selecteer het wanneer het in de lijst toont.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Voer een van de volgende handelingen uit:

   * Voeg de volgende code aan de bestaande tekst beschikbaar in de **Groep toe uw vakje van het Rapport**:


     `group.0.displayname=Your Value`


     Voeg bijvoorbeeld de volgende code toe om de weergavenaam te wijzigen in &quot;Portfolio&quot;:

     `group.0.displayname=Portfolio`

   * Verwijder alle regels in de tekstmodusinterface van de groep waarin het woord &quot;naam&quot; staat en voeg vervolgens de regel toe:

     `group.0.name=Your Value`

     Voeg bijvoorbeeld de volgende code toe om de weergavenaam te wijzigen in &quot;Portfolio&quot;:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >U kunt ook de regels `group.0.name=` en `group.0.displayname=` leeg laten. In dat geval wordt in de groep de waarde weergegeven waarop u groepeert.


     ![ groepering door uitgegeven naam zonder naam ](assets/grouping-edited-name-no-name-350x162.png)

1. Klik **Gedaan**, dan **sparen Groepering**.
1. (Facultatief) werk de groeperingsnaam bij, dan klik **sparen Groepering**.

   De standaardnaam voor de groepering wordt gewijzigd op basis van de gegevens in de tekstmodus.
