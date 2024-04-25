---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen maken voor Adobe Workfront-doelen
description: Of u nu CEO, manager of individuele medewerker bent, u kunt doelstellingen in de Doelen van Adobe Workfront creëren om uw werk met uw doelstellingen en de doelstellingen te richten die de strategie van uw organisatie schetsen.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Doelen maken voor Adobe Workfront-doelen

Of u nu CEO, manager of individuele medewerker bent, u kunt doelstellingen in de Doelen van Adobe Workfront creëren om uw werk met uw doelstellingen en de doelstellingen te richten die de strategie van uw organisatie schetsen.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront-plan</td>
 <td>
 <p>Alle</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie*</td>
 <td>
 <p>Nieuwe licentie: Medewerker of hoger</p>
 of
 <p>Huidige licentie: aanvragen of hoger</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> Nieuwe productbehoefte, één van het volgende: </p>
<ul>
<li>Een Select- of Prime Adobe Workfront-abonnement en een extra Adobe Workfront Goals-licentie.</li>
<li>Een Ultimate Workfront-plan dat standaard Workfront Goals bevat. </li></ul>
 <p>of</p>
 <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td>
 </tr>
<tr>
<td role="rowheader">Toegangsniveau*</td>
<td> <p>Toegang tot doelen bewerken</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Objectmachtigingen</td>
<td>
<p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
<p>Machtigingen beheren om het te bewerken</p>
<p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Richtlijnen voor het maken van doelen

Voordat we beginnen met Workfront Goals, raden we u aan om te lezen over onze aanbevelingen en richtlijnen voor het effectief beheren van doelen. Voor meer informatie over richtlijnen voor het creëren van en het beheren van doelstellingen, zie [Overzicht van Adobe Workfront-doelen](../../workfront-goals/goal-management/wf-goals-overview.md).

## Doelen maken

In dit artikel wordt beschreven hoe u een strategisch doel maakt in Workfront Goals. Voor informatie over het creëren van een bedrijfscasedoel, zie [Zakelijke hoofddoelen maken](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

U kunt een strategisch doel op een van de volgende manieren maken:

* [Een geheel nieuwe doelstelling maken](#create-a-goal-from-scratch)
* [Een bestaand doel kopiëren](#copy-an-existing-goal)
* [Een resultaat of activiteit omzetten in een doel](#convert-a-result-or-activity-to-a-goal)

### Een geheel nieuwe doelstelling maken {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Doelen**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   De vertoningen van de doellijst.
1. Klikken **Nieuw doel**.

   De Nieuwe doeldoos toont.

   ![](assets/new-goal-box-unshimmed.png)

1. Voer in de volgende velden gegevens in:
   * **Doelnaam**: Voer een naam in voor het doel. Dit is een verplicht veld.
   * **Periode**: Selecteer een vooraf gedefinieerd kwartaal of jaar in het menu **Periode** vervolgkeuzelijst

     of

     Selecteer de **Aangepaste datums inschakelen** en selecteert u vervolgens een **Start** en **Einddatum** voor het doel.

     De voorgaande, huidige en volgende jaren en hun respectieve kwartalen worden vermeld als vooraf gedefinieerde opties in het vervolgkeuzeveld Periode.

     De Periode van het doel wijst op het tijdkader wanneer u het doel verwacht te voltooien.

   * **Goedereneigenaar**: Begin de naam van een gebruiker, een team, een groep, of van uw organisatie te typen om erop te wijzen wie de eigenaar van het doel is. U wordt standaard geselecteerd als de eigenaar van het doel.
   * **Beschrijving**: Voer aanvullende informatie in over het doel.
1. Klikken **Doel maken**.

   Het nieuwe doel wordt vermeld in de lijst van het Beleid en het heeft het statuut van **Concept**.

   U moet een doel koppelen aan een voortgangsindicator om het te activeren en er aan te gaan werken.

   Voer ten minste een van de volgende handelingen uit om een te activeren doel voor te bereiden:
   * Een resultaat toevoegen

     Zie voor informatie over het toevoegen van resultaten [Resultaten toevoegen aan doelen in Adobe Workfront-doelen](../results-and-activities/add-results-to-goals.md).
   * Een activiteit toevoegen

     Voor informatie over het toevoegen van activiteiten raadpleegt u [Activiteiten toevoegen aan doelen in Adobe Workfront](../results-and-activities/add-activities-to-goals.md).
   * Nog een doel uitlijnen

     Voor informatie over het richten van doelstellingen, zie [Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden](../goal-alignment/align-goals-by-connecting-them.md).


### Een bestaand doel kopiëren {#copy-an-existing-goal}

U kunt een doel creëren door bestaande te kopiëren.

Voor informatie over het kopiëren van doelstellingen, zie [Doelstellingen kopiëren in Adobe Workfront-doelen](../../workfront-goals/goal-management/copy-goals.md).

### Een resultaat of activiteit omzetten in een doel {#convert-a-result-or-activity-to-a-goal}

U kunt een doel tot stand brengen door het resultaat of de activiteit van een bestaand doel in een doel om te zetten. Het nieuwe doel wordt uitgelijnd op het oorspronkelijke doel.

Voor informatie over het omzetten van resultaten en activiteiten in doelstellingen, zie [Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

