---
product-area: projects
navigation-topic: manage-issues
title: Problemen verplaatsen
description: U kunt kwesties tussen projecten en taken bewegen.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Problemen verplaatsen

<!--Audited: 12/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

U kunt kwesties tussen de volgende voorwerpen bewegen:

* Van een project naar een ander project
* Van een taak aan een andere taak in het zelfde project of in een ander project
* Van een taak aan het project of aan een ander project
* Van een project aan een taak in het zelfde project of een taak in een ander project

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
   <ul><li>Medewerker of hoger</li>
   <li>Licht of hoger om kwesties in de sectie van Kwesties van een project te bewegen</li></ul>
   Of:
   <ul>   <li><p>Aanvraag of hoger</p></li>
   <li><p>Controleer of u een hogere licentie hebt om problemen te verplaatsen in de sectie Issues van een project.</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute-machtigingen voor het item waarnaar u het probleem verplaatst, met de mogelijkheid om problemen toe te voegen.</td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New:</p> 
   <ul><li>Contributor or higher</li>
   <li>Light or higher to move issues in the Issues section of a project</li></ul>
   <p>Current:</p>
   <ul>
   <li><p>Request or higher</p></li>
   <li><p>Review or higher license to move issues in the Issues section of a project.</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are moving the issue with the ability to Add Issues.</td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen bij het verplaatsen van problemen

Houd rekening met het volgende wanneer u problemen verplaatst die documenten bevatten of die zijn gekoppeld aan een aanvraagwachtrij:

* Uw systeem of groepsbeheerder kan u verhinderen kwesties te bewegen die het programma geopende uren, afhankelijk van hoe zij vormen toestaan gebruikers om taken en kwesties met geregistreerde urenvoorkeur in het gebied van de Opstelling te bewegen. Voor informatie, zie [&#x200B; de taak en de uitgevende voorkeur van het systeem brede &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

* **wanneer een kwestie met een verzoekrij wordt geassocieerd:** wanneer u een kwestie aan een ander voorwerp beweegt en de kwestie met een verzoekrij wordt geassocieerd, wordt de verplaatste kwestie niet meer geassocieerd met de originele rij de eerste kwestie voortgekomen uit.
* **wanneer een document aan de kwestie in bijlage is:** wanneer u een kwestie aan een ander voorwerp beweegt en de kwestie een document in bijlage aan het heeft, bewegen het document, zijn versies en de proeven zich ook naar de nieuwe kwestie. Eventuele goedkeuringen die aan het document zijn gekoppeld, worden niet verplaatst.
* **wanneer een kwestie met een document of een omslag wordt verbonden:** wanneer u een kwestie verplaatst die documenten of omslagen verbonden aan een derdedienst zoals de Aandrijving van Google heeft, bewegen de verbindingen aan de documenten met de kwestie.

## Uitgaven in een lijst verplaatsen

U kunt een of meerdere problemen verplaatsen vanuit een lijst met problemen of vanuit een probleemrapport.

1. Ga naar het project dat de kwestie of de kwesties bevat die u wilt bewegen.

   of

   Ga naar een probleemrapport.

1. Als u selecteerde om naar een project te gaan, klik **Kwesties** in het linkerpaneel.
1. Selecteer de kwestie of de kwesties die u wilt bewegen en **Meer menu** bij de bovenkant van de lijst van de kwestie klikken, dan **Beweging aan** klikken.

   ![&#x200B; Exemplaar en Beweging aan verbindingen &#x200B;](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Ga met het bewegen van de kwesties voort, zoals die in de sectie [&#x200B; worden beschreven één enkele kwestie &#x200B;](#move-a-single-issue) die met Stap 2 beginnen.

## Eén probleem verplaatsen {#move-a-single-issue}

U kunt één probleem verplaatsen wanneer u het bekijkt.

### Eén probleem verplaatsen

1. Ga naar een kwestie die u wilt bewegen, **klikken Meer** menu ![&#x200B; &#x200B;](assets/more-icon.png) rechts van de uitgevende naam, dan klik **Beweging aan**.

   ![&#x200B; Beweging op uitgaand niveau &#x200B;](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   De **vertoningen van de Kwestie van de Beweging** doos.

   ![&#x200B; Verplaats de kwestie doos &#x200B;](assets/move-issue-box-nwe-350x280.png)

1. In de **Uitgezochte sectie van het Project van de Bestemming**, specificeer de naam van het project waar u de kwesties wilt bewegen. De naam van het huidige project toont door gebrek.

   >[!TIP]
   >
   >Er worden slechts 100 projecten weergegeven in de lijst.

1. (Voorwaardelijk) klik **verzoektoegang** als u geen toegang hebt om kwesties aan het project te bewegen.
1. (Voorwaardelijk) blijf de kwestie op het geselecteerde bestemmingsproject bewegen zonder toegang te vragen als u toegang hebt om kwesties aan één van de taken op het bestemmingsproject toe te voegen.

   ![&#x200B; de kwestie van de beweging en verzoek toegang &#x200B;](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van kwesties aan deze projecten verhindert. Voor meer informatie, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

1. (Facultatief) in de **sectie van Opties**, schrap om het even welke punten die in de lijst hieronder worden vermeld om hen uit de verplaatste kwestie te verwijderen. Alle opties zijn standaard geselecteerd.

   >[!IMPORTANT]
   >
   >Als u de selectie van items in de lijst Opties opheft, gaan er gegevens verloren. Informatie uit de bestaande uitgave wordt verwijderd en kan niet worden hersteld.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td>Schakel deze optie uit als u alle informatie uit de uitgave wilt verwijderen wanneer u deze naar de nieuwe locatie verplaatst. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td>Verwijdert gebruikers, baanrollen, of teams die aan de kwestie worden toegewezen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voortgang</td> 
      <td>Hiermee verwijdert u het eventuele percentage van de uitgave dat is voltooid. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documenten</p></td> 
      <td> <p>Hiermee verwijdert u alle gegevens op het documenttabblad, inclusief documentversies, gekoppelde documenten en mappen.

   <b> NOTA </b>

   Als u ervoor kiest om de documenten niet samen met de uitgave te laten verplaatsen, worden de documenten verwijderd en gedurende 30 dagen in de prullenbak geplaatst. Een beheerder kan deze herstellen en ze worden hersteld bij het verplaatste probleem.

   Als de uitgave wordt geschrapt nadat het wordt bewogen, zullen de herstelde documenten in het gebied van Documenten van de gebruikerspagina van de beheerder worden geplaatst die hen herstelt.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td>Hiermee verwijdert u de entiteiten waarmee de uitgave wordt gedeeld. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Hiermee verwijdert u opmerkingen uit de sectie Updates van de uitgave.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Facultatief) in de **Uitgezochte Taak** sectie, selecteer de taak waar u de kwestie wilt bewegen.
1. Klik **kwestie van de Beweging** of **de kwesties van de Beweging**, als u veelvoudige kwesties in een lijst selecteerde.

   De verplaatste kwesties worden toegevoegd aan het gespecificeerde project.




