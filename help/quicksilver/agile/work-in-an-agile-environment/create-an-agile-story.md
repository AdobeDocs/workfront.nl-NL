---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Een stapel artikel maken
description: U kunt op verschillende manieren een wendbaar artikel maken. Nadat u een stapel artikel hebt gemaakt, kunt u subtaken aan het artikel toevoegen.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Een stapel artikel maken

U kunt op verschillende manieren een wendbaar artikel maken. Nadat u een stapel artikel hebt gemaakt, kunt u subtaken aan het artikel toevoegen.

Wanneer u een artikel of subtaak in een herhaling toevoegt, wordt het Duur Type geplaatst aan [!UICONTROL Simple] en de Taakbeperking is ingesteld op Vaste datums, met de datums vergrendeld in de herhaling. U kunt het Type van Duur of de Beperking van de Taak in een herhaling niet wijzigen. Bovendien moet de taakduur langer zijn dan 0 minuten.

Voor informatie over hoe u het artikel kunt beheren nadat het aan de herhaling is toegevoegd, raadpleegt u [Herhalingen](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

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
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project waarop het verhaal zich bevindt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een flexibel artikel maken in een herhaling

1. Ga naar de dynamische iteratie waar u het artikel wilt maken:

   1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

   1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw scrubteam in het keuzemenu of zoek naar een team op de zoekbalk.

   1. Selecteer in het linkerdeelvenster de optie **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen, of **[!UICONTROL Current Iteration]**.
   1. Klik op de naam van de specifieke herhaling waar u een artikel wilt maken.

   ![Nieuw artikel toevoegen aan herhaling](assets/iteration-add-story.png)

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
      <td>Selecteer deze optie als het artikel kan worden toegevoegd aan een herhaling. Als deze optie is geselecteerd, wordt aan gebruikers aangegeven welke artikelen in de backlog kunnen worden toegevoegd aan een herhaling.<br>Een artikel kan aan een herhaling worden toegevoegd, ongeacht of het is gemarkeerd <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (punten)</strong></td>
      <td>Geef de schatting voor het artikel op. Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] over het verhaal.<br>Als u bijvoorbeeld een artikel inschat als 3 punten, wordt standaard 24 punten toegevoegd [!UICONTROL Planned Hours] naar het verhaal.<br>Als een artikel subtaken bevat, moet u niet vergeten dat de gecombineerde schattingen voor alle subtaken de schatting van het bovenliggende artikel bepalen. Zie voor meer informatie <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Artikelen toevoegen aan een bestaande herhaling</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Typ de naam van het project waaraan dit artikel is gekoppeld.<br>Standaard wordt de artikelkleur weergegeven als dezelfde kleur als andere artikelen uit dit project.<br>De status van het project moet worden ingesteld op [!UICONTROL Current]. Als de status van het project iets anders is dan [!UICONTROL Current], wordt deze niet weergegeven in het keuzemenu.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>Nadat u een ouderproject kiest, hebt u de optie om een oudertaak te kiezen. Wanneer u een bovenliggende taak selecteert, wordt het artikel gemaakt als een subtaak van de bovenliggende taak van het project dat u hebt geselecteerd.<br>Typ de naam van de bovenliggende taak voor het artikel en klik vervolgens op de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Selecteer aangepaste formulieren die u aan het artikel wilt toevoegen.</td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Save Story]**.

## Een stapel artikel op de achtergrond maken

U kunt een nieuw artikel maken op basis van de stapel-achterstand, zoals beschreven in de sectie [Nieuwe artikelen maken op de achtergrond](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) in het artikel [[!UICONTROL Manage] de oude achterstand](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Een taak of uitgave toevoegen als een stapel artikel

U kunt een bestaande taak of uitgave als een artikel aan een herhaling toevoegen. Zie voor meer informatie [Artikelen toevoegen aan een bestaande herhaling](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) of [Artikelen en problemen toevoegen uit het dialoogvenster [!UICONTROL Scrum] board](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Subtaken maken voor een stapel artikel

U kunt op een van de volgende manieren een subtaak maken van een stapel artikel:

* Met de **[!UICONTROL Subtasks]** tab, zoals beschreven in [Subtaken maken](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Subtaken maken](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Rechtstreeks vanaf het artikelbord, zoals beschreven in [Een herhaling maken](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
