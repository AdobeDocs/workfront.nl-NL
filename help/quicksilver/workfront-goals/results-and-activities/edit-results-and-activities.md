---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Resultaten en activiteiten bewerken in Adobe Workfront Goals
description: Nadat uw Adobe Workfront-beheerder u de juiste toegang tot de doelstellingen van Adobe Workfront heeft verleend, kunt u doelstellingen, resultaten en activiteiten maken en bewerken.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '763'
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

U moet het volgende hebben:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> 
   <p>Voor het nieuwe plan en de nieuwe licentiestructuur:
  <ul><li>Een ultiem plan </li></ul>
   </p>
<p>Voor het huidige plan en de licentiestructuur: 
<ul><li> Een Pro of hoger </li>
  <li>Een Adobe Workfront Goals-licentie in aanvulling op een Workfront-licentie.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie*</td>
 <td>
 <p>Nieuwe licentie: Medewerker of hoger</p>
 of
 <p>Huidige licentie: aanvragen of hoger</p> <p>Voor meer informatie, zie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> het vergunningsoverzicht van Adobe Workfront </a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> Nieuwe productbehoefte, één van het volgende: </p>
<ul>
<li>Een Select- of Prime Adobe Workfront-abonnement en een extra Adobe Workfront Goals-licentie.</li>
<li>Een Ultimate Workfront-plan dat standaard Workfront Goals bevat. </li></ul>
 <p>of</p>
 <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Voor informatie, zie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref"> Vereisten om de Doelen van Workfront </a> te gebruiken. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Toegangsniveau</p></td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref"> een doel in de Doelen van Workfront delen </a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

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


1. Klik het **Belangrijkste Menu** ![](assets/main-menu-icon.png), toen **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Selecteer een resultaat in de lijst van Voortgangsindicatoren en klik **uitgeven** pictogram ![](assets/edit-icon.png).

   Het vak Resultaat bewerken wordt geopend.

   ![](assets/edit-result-box-unshimmed.png)

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
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Klik het **Belangrijkste Menu** ![](assets/main-menu-icon.png), toen **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Selecteer een activiteit in de de indicatorenlijst van de Voortgang en klik **uitgeven** pictogram ![](assets/edit-icon.png).

   Het vak Activiteit bewerken wordt geopend.

   ![](assets/edit-activity-box-unshimmed.png)

1. Bewerk de volgende gegevens:
   * **naam van de Activiteit**: De naam van de activiteit. Gebruik een beschrijvende naam die illustreert welke activiteit u zou moeten uitvoeren om erop te wijzen dat het doel voltooit.
   * **Eigenaar van de Activiteit:** De eigenaar van de activiteit. De eigenaar moet een actieve Workfront-gebruiker zijn.\
     Voor meer informatie over activiteitengebieden, zie [ activiteiten aan doelstellingen ](../results-and-activities/add-activities-to-goals.md) toevoegen.
1. Klik **sparen**.


