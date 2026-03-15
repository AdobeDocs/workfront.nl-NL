---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Create an Agile story in an Iteration
description: This article describes how to create a new Agile story when you are already in the iteration.
author: Courtney
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Create an Agile story in an iteration

This article describes how to create a new Agile story when you are already in the iteration. For information about creating an Agile story from a task, issue, or other area of [!DNL Adobe Workfront], see [Add stories to an existing iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Manage access to the project the story is on </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create an Agile story in an iteration

1. Ga naar de letterlijke tekst waar u het artikel wilt maken:

   {{step1-to-team}}

   1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![&#x200B; Schakelaar teampictogram &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

   1. Selecteer **[!UICONTROL Iterations]** in het linkerdeelvenster.
   1. Click the name of the specific iteration where you want to create a story.
   1. Selecteer **[!UICONTROL Stories]** in het linkerdeelvenster.

1.  Klik op **[!UICONTROL New Story]** .
1. Geef de volgende informatie op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Type a name for the story.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Type a description for the story.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Select this option if the story is ready to be added to an iteration. When this option is selected, it indicates to users which stories in the backlog are ready to be added to an iteration.<br>A story can be added to an iteration whether or not it is marked <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (points)</strong></td>
      <td>Specify the estimate for the story. Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] in het artikel.<br>For example, if you estimate a story as 3 points, the default behavior is to add 24 Planned Hours to the story.<br>If a story contains subtasks, remember that the combined estimates for all subtasks determines the estimate of the parent story. For more information, see <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Add a subtask to an existing story on the [!UICONTROL Scrum] board</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Begin typing the name of the project that this story will be associated with.<br>By default, the story color is displayed as the same color as other stories from this project.<br>The status of the project must be set to [!UICONTROL Current]. Als de status van het project iets anders is dan [!UICONTROL Current] , wordt het niet weergegeven in het vervolgkeuzemenu.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>After you choose a parent project, you have the option to choose a parent task. When you select a parent task, the story is created as a subtask of the parent task on the project that you selected.<br>Begin typing the name of the parent task for the story, then click it when it appears in the drop-down list.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Select any custom forms to add to the story.</td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Save Story]**.
