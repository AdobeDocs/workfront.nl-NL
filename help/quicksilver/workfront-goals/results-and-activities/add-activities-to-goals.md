---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Activiteiten toevoegen aan doelen in Adobe Workfront
description: Met activiteiten wordt de voortgang van een doel gemeten. Zonder bijbehorende resultaten, activiteiten, of gerichte doelstellingen, kan een doel niet worden geactiveerd en de vooruitgang kan niet op het worden geregistreerd.
author: Alina
feature: Workfront Goals
exl-id: 4d6ef324-4b5c-402b-b64d-b1a2a7d2ab57
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Activiteiten toevoegen aan doelen in Adobe Workfront

Met activiteiten wordt de voortgang van een doel gemeten. Zonder resultaten, activiteiten, projecten, of gerichte doelstellingen te associëren, kunt u geen doel activeren en u kunt geen vooruitgang op het registreren.

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
  <ul><li>Een ultiem plan </li>
  of
  <li>Een extra licentie voor Adobe Workfront Goals voor de Adobe Workfront-plannen voor de Premier of Select. </li></ul> </p>
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
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

U moet een bestaand doel hebben om er activiteiten aan toe te voegen.

Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Een doel kan niet meer dan 1000 activiteiten, resultaten, of gerichte doelstellingen hebben.

Zie voor meer informatie over activiteiten [Aan de slag met resultaten en activiteiten in Adobe Workfront Goals](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md).

## Een activiteit toevoegen aan een doel

<!--
Adding activities to goals differs depending on which environment you use.

### Add an activity to a goal in the Production environment

1. Go to the goal for which you want to add an activity and click the name to open the **Goal Details** panel.
1. Click **Add activities**.

   ![](assets/add-activity-inside-goal-details-highlighted-350x152.png)

1. From the **Activity Type** drop-down menu, select the type of activity you want to associate with your goal.&nbsp;Select **Manual progress bar** or **Project**. Manual progress bar is the default selection. 
1. (Conditional) Depending on which activity type you selected, do the following:

   1. If you selected **Manual progress bar**:

      1. Start typing a name for your activity in the **Activity** field. 
      1. (Optional) If you want to set the activity owner as someone other than yourself, click your name in the **Owner** field and begin typing the name of the user that you want to assign as the activity owner, then click it when it appears in the drop-down list.

         >[!NOTE]
         >
         >You cannot assign a team or group as an activity owner.

         When you update the progress of an activity, the progress of the goal automatically updates.

   1. If you selected **Project**:

      1. Click the **Connect projects** field.

         Existing projects that you have access to View display in the Connect projects list. Projects that are in a status of Dead do not display in the list. 
      
      1. Click the name of a project to add it as an activity to the goal. You can select several projects at one time.

         Workfront uses the project percent complete of all the attached projects to calculate the progress of the goal.

         For more information about associating projects with goals, see [Add projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

         >[!TIP]
         >
         >   
         >   * The owner of the project becomes the owner of this activity. If the project has no owner, then the activity has no owner. 
         >   * You cannot manually update the progress of a project. Workfront calculates the progress of the project based on the project percent complete. When the project percent complete updates in Workfront this also updates the connected project in Workfront Goals including the percent complete of the goal. 
         >   
         >

1. Click **Save**.

   The activity is saved for the selected goal. After you activate the goal, the progress of the goal automatically updates when you update the progress of an activity or when the percent complete of a project updates. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

-->


1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-icon.png)vervolgens **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de pagina met het doel te openen.
1. Klikken **Voortgangsindicatoren** in het linkerdeelvenster.
1. Klik in het vervolgkeuzemenu van de indicator Nieuwe vordering op **Actie maken**.

   Het vak Nieuwe activiteit wordt geopend.

   ![](assets/new-activity-box-unshimmed.png)

1. Typ een naam voor de activiteit in het veld Naam activiteit. Dit is een verplicht veld.
1. (Optioneel) Verwijder uw naam uit het dialoogvenster **Eigenaar activiteit** veld als u de activiteit aan een andere gebruiker wilt toewijzen. Standaard bent u de eigenaar van een activiteit die u maakt.

   >[!NOTE]
   >
   >U kunt geen team, groep, of het bedrijf als activiteiteneigenaar toewijzen.

1. Klikken **Actie maken** om het op te slaan en toe te voegen aan het geselecteerde doel.

   De activiteit toont in de de indicatorensectie van de Voortgang van de doelpagina, onder de groepering van de Activiteit.





