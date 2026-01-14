---
product-area: projects
navigation-topic: manage-issues
title: Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst
description: Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

U kunt gebruikerstoewijzingen aan veelvoudige kwesties gelijktijdig wijzigen. Zie ook de volgende artikelen voor informatie over het bewerken van uitgaven of het een voor een toewijzen van uitgaven:

* [ geeft kwesties ](../../../manage-work/issues/manage-issues/edit-issues.md) uit
* [Problemen toewijzen](../../../manage-work/issues/manage-issues/assign-issues.md)

Voor algemene informatie over het toewijzen van kwesties, zie [ Overzicht van het wijzigen van uitgiftetaken ](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>U moet ten minste over Contribute-machtigingen beschikken om een uitgave te kunnen toewijzen aan de uitgave.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of de hogere toegang tot Projecten en Taken om één kwestie toe te wijzen</p> </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute-machtigingen of hoger voor het project of de taak waar de uitgave zich bevindt, wanneer u meerdere uitgaven toewijst.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Toewijzingen wijzigen voor meerdere problemen

1. Ga naar de lijst van de kwestie die de kwesties bevat waarvan taken u wilt wijzigen.
1. (Optioneel) Maak een filter om alleen uitgaven weer te geven die zijn toegewezen aan de ontvanger die u wilt wijzigen.

   U kunt bijvoorbeeld een filter maken om alleen uitgaven weer te geven die een specifieke rol als toegewezen persoon hebben.  Vervolgens kunt u de rol vervangen door een specifieke gebruiker. Ga als volgt te werk:

   1. Klik de **drop-down lijst van Filters**, dan klik **Nieuwe filter**.

   1. Op het eerste gebied, begin het typen **Rollen van de Taak** en kies **Rollen van de Taak: Naam** van de lijst.
   1. Selecteer **is om het even welk van** van het bepalingsdrop-down menu, dan begin de naam van een rol te typen en het te selecteren wanneer het in de lijst toont. U kunt meerdere rollen typen.

      >[!TIP]
      >
      >Gebruik niet **Toegewezen aan** omdat dit gebied slechts naar de Eigenaar van de Uitgave en niet naar alle toegewezen verwijst.

      De lijst met uitgaven filtert automatisch voor uw filtercriteria.
   1. (Facultatief) klik **sparen als nieuw**, dan **sparen**.

1. Selecteer de kwesties waarvoor u taken wilt wijzigen, dan klik **uitgeven** pictogram ![ uitgeven pictogram ](assets/qs-edit-icon.png).

   **geeft Kwesties** vertoningen uit. Het aantal geselecteerde items wordt in de linkerbovenhoek van de pagina weergegeven.

1. Klik **Taken** in het linkerpaneel, dan klik het **x** pictogram naast toegewezen u wilt verwijderen.

   >[!TIP]
   >
   >Slechts wijzen die aan alle geselecteerde kwesties worden toegewezen tonen in het **1} gebied van Taken {.**

   ![ gebied van Taken in bulk-geef kwesties ](assets/assignments-area-on-bulk-edit-issues.png) uit

1. Typ de naam van een gebruiker, rol of team om toewijzingen toe te voegen aan alle geselecteerde problemen.

   >[!TIP]
   >
   >U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
   >
   >Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
   >
   >* Wijs het werkitem opnieuw toe aan actieve bronnen.
   >* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

   De toegevoegde toewijzingen worden toegevoegd aan de bestaande toewijzingen. Zij vervangen niet de bestaande voor elke geselecteerde kwestie.

1. (Facultatief) klik **toewijzen aan me** om alle kwesties aan zich toe te wijzen.
1. Klik **sparen**.


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




