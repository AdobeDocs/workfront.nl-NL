---
product-area: projects
navigation-topic: manage-issues
title: Problemen verplaatsen
description: U kunt kwesties tussen projecten en taken bewegen.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# Problemen verplaatsen

U kunt kwesties tussen de volgende voorwerpen bewegen:

* Van een project naar een ander project
* Van een taak aan een andere taak in het zelfde project of in een ander project
* Van een taak aan het project of aan een ander project
* Van een project aan een taak in het zelfde project of een taak in een ander project

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> <p>Controleer of u een hogere licentie hebt om problemen te verplaatsen in de sectie Issues van een project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref"> Toegang van de Verlening tot kwesties </a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute geeft toestemming aan het item waar u het probleem verplaatst met de mogelijkheid om problemen toe te voegen.</p> <p> Voor informatie over het verlenen van toestemmingen aan kwesties, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> een kwestie delen </a></p> <p>Voor informatie bij het vragen van extra toestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> Toegang tot voorwerpen verzoeken </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Overwegingen bij het verplaatsen van problemen

Houd rekening met het volgende wanneer u problemen verplaatst die documenten bevatten of die zijn gekoppeld aan een aanvraagwachtrij:

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

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Ga met het bewegen van de kwestie voort, zoals die in de sectie [ wordt beschreven Beweeg één enkele kwestie ](#move-a-single-issue) die met Stap 2 begint.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

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




