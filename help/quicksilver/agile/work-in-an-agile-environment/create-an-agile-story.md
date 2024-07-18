---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Een flexibel verhaal maken
description: U kunt op verschillende manieren een flexibel verhaal op een herhaling maken. Nadat u een artikel hebt gemaakt, kunt u subtaken aan het artikel toevoegen.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Een flexibel verhaal maken

U kunt op verschillende manieren een flexibel verhaal op een herhaling maken. Nadat u een stapel artikel hebt gemaakt, kunt u subtaken aan het artikel toevoegen.

Wanneer u een artikel of subtaak toevoegt in een herhaling, wordt het Duur-type ingesteld op [!UICONTROL Simple] en wordt Taakbeperking ingesteld op Vaste datums, met de datums vergrendeld in de herhaling. U kunt het Type Duur of de Beperking van de Taak in een herhaling niet wijzigen. Bovendien moet de taakduur langer zijn dan 0 minuten.

Voor informatie over hoe te om het verhaal te beheren nadat het aan de herhaling wordt toegevoegd, zie [ Herhalingen ](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project waarop het verhaal zich bevindt</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een flexibel artikel in een herhaling maken

1. Ga naar de galerij-iteratie waar u het artikel wilt maken:

   1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Teams]** .

   1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram ![ pictogram van de Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

   1. Selecteer in het linkerdeelvenster **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen of selecteer **[!UICONTROL Current Iteration]** .
   1. Klik op de naam van de specifieke herhaling waarin u een artikel wilt maken.

   ![ voeg nieuw verhaal aan herhaling toe ](assets/iteration-add-story.png)

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
      <td>Geef de schatting voor het artikel op. Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] in het artikel.<br> bijvoorbeeld, als u een verhaal als 3 punten schat, is het standaardgedrag 24 [!UICONTROL Planned Hours] aan het verhaal toe te voegen.<br> als een verhaal subtaken bevat, herinner dat de gecombineerde ramingen voor alle subtaken de schatting van het ouderverhaal bepalen. Voor meer informatie, zie <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref"> verhalen aan een bestaande herhaling </a> toevoegen.</td>
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
      <td>Selecteer de aangepaste formulieren die u aan het artikel wilt toevoegen.</td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Save Story]**.

## Een flexibel artikel op de achtergrond maken

U kunt een veranderlijk verhaal van agile backlog tot stand brengen, zoals die in de sectie [ wordt beschreven nieuwe verhalen op de backlog ](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) in het artikel [[!UICONTROL Manage] de agile backlog ](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) creëren.

## Een taak of uitgave toevoegen als een stapel artikel

U kunt een bestaande taak of uitgave als een artikel aan een herhaling toevoegen. Voor meer informatie, zie [ verhalen aan een bestaande herhaling ](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) toevoegen of [ verhalen en kwesties van de [!UICONTROL Scrum] raad ](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md) toevoegen.

## Subtaken maken voor een stapel artikel

U kunt op een van de volgende manieren een subtaak maken van een stapel artikel:

* Door het **[!UICONTROL Subtasks]** lusje te gebruiken, zoals die in [ wordt beschreven leidt subtasks ](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [ tot subtasks ](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Direct van de verhaalraad, zoals die in [ wordt beschreven creeer een herhaling ](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
