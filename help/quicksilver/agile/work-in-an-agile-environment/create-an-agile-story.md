---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Een flexibel artikel maken
description: U kunt op verschillende manieren een wendbaar artikel maken. Nadat u een stapel artikel hebt gemaakt, kunt u subtaken aan het artikel toevoegen.
author: Jenny
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Een flexibel artikel maken

U kunt op verschillende manieren een eenvoudig artikel maken voor een herhaling. Nadat u een artikel hebt gemaakt, kunt u subtaken aan het artikel toevoegen.

Wanneer u een artikel of subtaak toevoegt in een herhaling, wordt het Duur Type geplaatst aan [!UICONTROL Simple] en de Beperking van de Taak wordt geplaatst aan Vaste Datums, met de data die binnen de herhaling worden gesloten. U kunt het Type van Duur of de Beperking van de Taak in een herhaling niet wijzigen. Bovendien moet de taakduur langer zijn dan 0 minuten.

Voor informatie over hoe te om het verhaal te beheren nadat het aan de herhaling wordt toegevoegd, zie [ Herhalingen ](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>Toegang beheren tot het project waarop het artikel zich bevindt </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een flexibel artikel maken in een herhaling

1. Ga naar de letterlijke tekst waar u het artikel wilt maken:

   {{step1-to-team}}

   1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

   1. Selecteer in het linkerdeelvenster **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen of selecteer **[!UICONTROL Current Iteration]** .
   1. Klik op de naam van de specifieke herhaling waar u een artikel wilt maken.

   ![ voeg nieuw verhaal aan herhaling toe ](assets/iteration-stories-list.png)

1. Klik op **[!UICONTROL New Story].**
1. Geef de volgende informatie op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Typ een naam voor het artikel.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Typ een beschrijving voor het artikel.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Selecteer deze optie als het artikel kan worden toegevoegd aan een herhaling. Als deze optie is geselecteerd, wordt aan gebruikers aangegeven welke artikelen in de backlog kunnen worden toegevoegd aan een herhaling.<br> het verhaal van A kan aan een herhaling worden toegevoegd al dan niet het <strong>[!UICONTROL Ready] duidelijk is.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (punten)</strong></td>
      <td>Geef de schatting voor het artikel op. Als uw Agile team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] in het artikel.<br> bijvoorbeeld, als u een verhaal als 3 punten schat, is het standaardgedrag 24 [!UICONTROL Planned Hours] aan het verhaal toe te voegen.<br> als een verhaal subtaken bevat, herinner dat de gecombineerde ramingen voor alle subtaken de schatting van het ouderverhaal bepalen. Voor meer informatie, zie <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref"> verhalen aan een bestaande herhaling </a> toevoegen.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Typ de naam van het project waaraan dit artikel is gekoppeld.<br> door gebrek, wordt de verhaalkleur getoond als de zelfde kleur zoals andere verhalen van dit project.<br> de status van het project moet aan [!UICONTROL Current] worden geplaatst. Als de status van het project iets anders is dan [!UICONTROL Current] , wordt het niet weergegeven in het vervolgkeuzemenu.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>Nadat u een ouderproject kiest, hebt u de optie om een oudertaak te kiezen. Wanneer u een bovenliggende taak selecteert, wordt het artikel gemaakt als een subtaak van de bovenliggende taak van het project dat u hebt geselecteerd.<br> begint met het typen van de naam van de oudertaak voor het verhaal, dan klik het wanneer het in de drop-down lijst verschijnt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Selecteer aangepaste formulieren die u aan het artikel wilt toevoegen.</td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Save Story]**.

## Een flexibel artikel maken op de achtergrond

U kunt een verhaal van de Gelijkheid van de Reparatie tot stand brengen, zoals die in de sectie [ wordt beschreven creeer nieuwe verhalen op de achterstand ](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) in het artikel [[!UICONTROL Manage] de looppas ](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Een taak of uitgave toevoegen als een mobiel artikel

U kunt een bestaande taak of uitgave als een artikel aan een herhaling toevoegen. Voor meer informatie, zie [ verhalen aan een bestaande herhaling ](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) toevoegen of [ verhalen en kwesties van de [!UICONTROL Scrum] raad ](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md) toevoegen.

## Subtaken maken voor een mobiel artikel

U kunt op een van de volgende manieren een subtaak maken van een artikel in de assistent:

* Door het **[!UICONTROL Subtasks]** lusje te gebruiken, zoals die in [ wordt beschreven leidt subtasks ](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [ tot subtasks ](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Direct van de verhaalraad, zoals die in [ wordt beschreven creeer een herhaling ](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
