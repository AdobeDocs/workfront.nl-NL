---
product-area: projects
navigation-topic: manage-issues
title: Problemen verplaatsen
description: U kunt kwesties tussen projecten en taken bewegen.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Problemen verplaatsen

<!--Audited: 12/2024-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt kwesties tussen de volgende voorwerpen bewegen:

* Van een project naar een ander project
* Van een taak aan een andere taak in het zelfde project of in een ander project
* Van een taak aan het project of aan een ander project
* Van een project aan een taak in het zelfde project of een taak in een ander project

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
   <td> <p>Nieuw:</p> 
   <ul><li>Medewerker of hoger</li>
   <li>Licht of hoger om kwesties in de sectie van Kwesties van een project te bewegen</li></ul>
   <p>Huidige:</p>
   <ul>
   <li><p>Aanvraag of hoger</p></li>
   <li><p>Controleer of u een hogere licentie hebt om problemen te verplaatsen in de sectie Issues van een project.</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute geeft toestemming aan het item waar u het probleem verplaatst met de mogelijkheid om problemen toe te voegen.</td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het verplaatsen van problemen

Houd rekening met het volgende wanneer u problemen verplaatst die documenten bevatten of die zijn gekoppeld aan een aanvraagwachtrij:

* **wanneer een kwestie met een verzoekrij wordt geassocieerd:** wanneer u een kwestie aan een ander voorwerp beweegt en de kwestie met een verzoekrij wordt geassocieerd, wordt de verplaatste kwestie niet meer geassocieerd met de originele rij de eerste kwestie voortgekomen uit.
* **wanneer een document aan de kwestie in bijlage is:** wanneer u een kwestie aan een ander voorwerp beweegt en de kwestie een document in bijlage aan het heeft, bewegen het document, zijn versies en de proeven zich ook naar de nieuwe kwestie. Eventuele goedkeuringen die aan het document zijn gekoppeld, worden niet verplaatst.
* **wanneer een kwestie met een document of een omslag wordt verbonden:** wanneer u een kwestie verplaatst die documenten of omslagen verbonden aan een derdedienst zoals de Aandrijving van Google heeft, bewegen de verbindingen aan de documenten met de kwestie.

<div class="preview">

* Uw systeem of groepsbeheerder kan u verhinderen kwesties te bewegen die het programma geopende uren, afhankelijk van hoe zij vormen toestaan gebruikers om taken en kwesties met geregistreerde urenvoorkeur in het gebied van de Opstelling te bewegen. Voor informatie, zie [ de taak en de uitgevende voorkeur van het systeem brede ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

</div>

## Uitgaven in een lijst verplaatsen

U kunt een of meerdere problemen verplaatsen vanuit een lijst met problemen of vanuit een probleemrapport.

1. Ga naar het project dat de kwestie of de kwesties bevat die u wilt bewegen.

   of

   Ga naar een probleemrapport.

1. Als u selecteerde om naar een project te gaan, klik **Kwesties** in het linkerpaneel.
1. Selecteer de kwestie of de kwesties die u wilt bewegen en **Meer menu** bij de bovenkant van de lijst van de kwestie klikken, dan **Beweging aan** klikken.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Ga met het bewegen van de kwesties voort, zoals die in de sectie [ worden beschreven één enkele kwestie ](#move-a-single-issue) die met Stap 2 beginnen.

## Eén probleem verplaatsen {#move-a-single-issue}

U kunt één probleem verplaatsen wanneer u het bekijkt.

### Eén probleem verplaatsen in de voorvertoningsomgeving

1. Ga naar een kwestie die u wilt kopiëren, **Meer** menu ![](assets/more-icon.png) aan het recht van de voorwaardennaam klikken, dan **Beweging** aan selecteren.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   De **vertoningen van de Kwestie van de Beweging** doos.

   ![](assets/move-issue-box-nwe-350x280.png)

1. In de **Uitgezochte sectie van het Project van de Bestemming**, specificeer de naam van het project waar u de kwesties wilt bewegen. De naam van het huidige project toont door gebrek.

   >[!TIP]
   >
   >Er worden slechts 100 projecten weergegeven in de lijst.

1. (Voorwaardelijk) klik **verzoektoegang** als u geen toegang hebt om kwesties aan het project te bewegen.
1. (Voorwaardelijk) blijf de kwestie op het geselecteerde bestemmingsproject bewegen zonder toegang te vragen als u toegang hebt om kwesties aan één van de taken op het bestemmingsproject toe te voegen.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van kwesties aan deze projecten verhindert. Voor meer informatie, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

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




