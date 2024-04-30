---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen bijwerken in het venster Goederendetails in Adobe Workfront Goals
description: U kunt informatie voor individuele doelstellingen bijwerken door tot het paneel van de Details van het Doel toegang te hebben.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Doelen bijwerken in de sectie Gooddetails in Adobe Workfront Goals

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

U kunt informatie voor individuele doelstellingen bijwerken door tot het paneel van de Details van het Doel toegang te hebben.

>[!NOTE]
>
>U kunt geen doelstellingen bijwerken met de status Gesloten.


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

## Doelen bijwerken in de sectie met de details van het doel

U kunt tot een individueel doel van een lijst van doelstellingen toegang hebben.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Klik de naam van een doel in de Lijst van het Doel, dan klik de naam van een doel.

   Hierdoor wordt het **Doelgegevens** aan de linkerkant.

   ![](assets/goal-page-unshimmed.png)

1. Klik op de knop **Pictogram Bewerken** ![](assets/edit-icon.png) in de rechterbovenhoek klikt u op **Alles bewerken** of **Overzicht**

   of

   Typ gegevens in een van de bewerkbare velden in de sectie met details over het doel. De sectie wordt bewerkbaar.

   >[!IMPORTANT]
   >
   >Niet alle velden die worden weergegeven in de sectie met algemene details kunnen worden bewerkt. Workfront berekent een aantal velden en deze zijn alleen-lezen.

1. Werk de volgende velden bij of bekijk deze:

   * **Beschrijving**: Voeg informatie over het doel toe of werk deze bij.
   * **Voortgang**: Geeft aan welk percentage van het doel tot dusver is bereikt. U kunt de voortgang van een doel niet handmatig bijwerken. De voortgang van het doel is een berekening van alle voortgangsindicatoren.
   * **Voorwaarde**: Geeft aan of het doel nieuw is en nog niet is bijgewerkt, of het op doel staat om op tijd te worden voltooid of een achterstand heeft. U kunt de voorwaarde van een doel niet bijwerken. De voorwaarde van het doel wordt automatisch berekend door Worfront.\
     Voor meer informatie over doelvoorwaarde en vooruitgang, zie
     [Overzicht van de voortgang en conditie van het doel in de Adobe Workfront-doelstellingen](../goal-management/calculate-goal-progress.md).
   * **Status**: U kunt de status van een doel niet handmatig bijwerken. Zie voor meer informatie [Overzicht van de status van objecten in Adobe Workfront Goals](../goal-management/goal-status-overview.md).
   * **Goedereneigenaar**: Klik om de naam van de eigenaar van het doel bij te werken. Typ de naam van een gebruiker, team, groep of de naam van uw organisatie en selecteer deze vervolgens wanneer deze in de lijst wordt weergegeven. U kunt slechts één eigenaar voor een doel hebben.
   * **Bovenliggende doelstelling**: Typ de naam van een doel dat u als bovenliggend element wilt instellen voor het doel dat u hebt geselecteerd. De voortgang van het geselecteerde doel wordt automatisch aangepast aan de voortgang van het bovenliggende doel.

     >[!TIP]
     >
     >U kunt de volgende informatie over een hoofddoel niet bijwerken:
     >    * Bovenliggende doelperiode
     >    * Voortgang bovenliggende doelstelling
     >    * Eigenaar van bovenliggend doel.
     >      
     >U moet deze informatie over het ouderdoel zelf bijwerken.

   * **Periode**: Klik om de tijdsperiode voor het doel bij te werken\
     of\
     Selecteren **Aangepaste datums inschakelen** om data voor het doel te specificeren **Start** en **Einddata**.
   * **Slotopmerkingen**: Dit veld is alleen zichtbaar voor doelen met de status Gesloten. Gesloten doelen kunnen niet worden bewerkt. Als u een gesloten doel opnieuw opent, worden de afsluitende notities permanent verwijderd.


