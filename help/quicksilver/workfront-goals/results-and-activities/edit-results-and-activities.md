---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Resultaten en activiteiten bewerken in Adobe Workfront Goals
description: Nadat uw Adobe Workfront-beheerder u de juiste toegang tot de doelstellingen van Adobe Workfront heeft verleend, kunt u doelstellingen, resultaten en activiteiten maken en bewerken.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Resultaten en activiteiten bewerken in Adobe Workfront Goals

Nadat uw Adobe Workfront-beheerder u de juiste toegang tot de doelstellingen van Adobe Workfront heeft verleend, kunt u doelstellingen, resultaten en activiteiten maken en bewerken.

Raadpleeg de volgende artikelen voor informatie over het maken van doelen, resultaten en activiteiten:

* [ creeer doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/create-goals.md)
* [ worden begonnen met resultaten en activiteiten in de Doelen van Adobe Workfront ](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [ voeg resultaten aan doelstellingen in de Doelen van Adobe Workfront toe ](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Activiteiten toevoegen aan doelen in Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

## Toegangsvereisten

>[!NOTE]
>
>Uw bedrijf zou kunnen verkiezen om de Doelen van Adobe Workfront verder te gebruiken als zij dit pakket in het verleden kochten. U moet voor meer informatie contact opnemen met uw accountvertegenwoordiger.
>
>Adobe Workfront Goals kan niet meer worden aangeschaft.

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-pakket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie</td>
 <td>
 <p>Medewerker of hoger</p>
<p>Aanvraag of hoger</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuratie op toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Systeembeheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Overwegingen bij het bewerken van resultaten en activiteiten

<!--
According to Vazgen, access levels will add more considerations.)
-->

* U kunt resultaten en activiteiten uitgeven die tot doelstellingen behoren u creeerde of aan doelstellingen die u toestemmingen hebt te leiden.
* U kunt de vooruitgang van projecten die met doelstellingen worden verbonden niet als activiteiten van de Doelen van Workfront uitgeven. De voortgang van projecten wordt bijgewerkt wanneer de taken in het project zijn voltooid. U kunt projecten uit het doel verwijderen door hen los te maken. Voor meer informatie, zie de &quot;losmaakt projecten&quot;sectie in het artikel [ resultaten, activiteiten, en projecten uit doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md) verwijderen.

  >[!NOTE]
  >
  >Als de volgende projectinformatie op het projectniveau bijwerkt, werkt de Doelen van Workfront het op het doelniveau automatisch bij:
  >
  >   
  >   
  >   * Projecteigenaar
  >   * Projectnaam
  >   * Projectpercentage voltooid
  >   
  >   
  >Voor informatie over het verbinden van projecten met doelstellingen, zie [ projecten aan doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md) toevoegen.

* U kunt resultaten en activiteiten van doelstellingen schrappen wanneer zij niet meer relevant voor de doelvooruitgang zijn. Verwijderde resultaten en activiteiten kunnen niet worden hersteld. Voor informatie over het schrappen van resultaten en activiteiten, zie [ resultaten, activiteiten, en projecten uit doelstellingen in de Doelen van Adobe Workfront verwijderen ](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* U kunt resultaten en activiteiten verbonden aan doelstellingen van om het even welke tijdspanne, met inbegrip van in het verleden uitgeven.
* Als u resultaten en activiteiten bewerkt, worden de instellingen bijgewerkt en wordt de voortgang van de bewerkingen niet bijgewerkt. U moet de voortgang van resultaten en activiteiten bijwerken. Voor informatie over het bijwerken van vooruitgang op doelstellingen, resultaten, en activiteiten, zie [ het doel van de Update vooruitgang in de Doelen van Adobe Workfront ](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Resultaten bewerken

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![Results gear icon](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. Klik het **** Belangrijkste pictogram van het Menu ![ Belangrijkste ](assets/main-menu-icon.png), toen **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Selecteer een resultaat in de lijst van Voortgangsindicatoren en klik **uitgeven** pictogram ![ pictogram ](assets/edit-icon.png) uitgeven.

   Het vak Resultaat bewerken wordt geopend.

   ![ geef de doos van het Resultaat uit ](assets/edit-result-box-unshimmed.png)

1. Bewerk de volgende gegevens:
   * **naam van het Resultaat**: De naam van het resultaat. Gebruik een beschrijvende naam die aangeeft welk resultaat u moet behalen om het doel te bereiken.
   * **resultaateigenaar**: De eigenaar van het resultaat. De eigenaar moet een actieve Workfront-gebruiker zijn.
   * **Type van Waarde**: Hoe u de vooruitgang van het resultaat meet.
   * **Aanvankelijke Waarde**: De originele waarde van het resultaat.
   * **Waarde van het Doel**: De gewenste waarde wanneer het resultaat wordt voltooid.
Voor meer informatie over resultaatgebieden, zie [ resultaten aan doelstellingen ](../results-and-activities/add-results-to-goals.md) toevoegen.
1. Klik **sparen**.

## Bewerkingen bewerken

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![Activities gear icon](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Klik het **** Belangrijkste pictogram van het Menu ![ Belangrijkste ](assets/main-menu-icon.png), toen **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Selecteer een activiteit in de lijst van Voortgangsindicatoren en klik **uitgeven** pictogram ![ pictogram geeft pictogram ](assets/edit-icon.png) uit.

   Het vak Activiteit bewerken wordt geopend.

   ![ geef de doos van de Activiteit ](assets/edit-activity-box-unshimmed.png) uit

1. Bewerk de volgende gegevens:
   * **naam van de Activiteit**: De naam van de activiteit. Gebruik een beschrijvende naam die illustreert welke activiteit u zou moeten uitvoeren om erop te wijzen dat het doel voltooit.
   * **Eigenaar van de Activiteit:** De eigenaar van de activiteit. De eigenaar moet een actieve Workfront-gebruiker zijn.\
     Voor meer informatie over activiteitengebieden, zie [ activiteiten aan doelstellingen ](../results-and-activities/add-activities-to-goals.md) toevoegen.
1. Klik **sparen**.


