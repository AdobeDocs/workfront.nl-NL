---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Een flexibel artikel maken in een herhaling
description: In dit artikel wordt beschreven hoe u een nieuw, flexibel artikel kunt maken wanneer u zich al in de herhaling bevindt.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Een flexibel artikel maken in een herhaling

In dit artikel wordt beschreven hoe u een nieuw, flexibel artikel kunt maken wanneer u zich al in de herhaling bevindt. Voor informatie over het creëren van een flexibel verhaal van een taak, kwestie, of ander gebied van [!DNL Adobe Workfront], zie [ verhalen aan een bestaande herhaling ](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) toevoegen.

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
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project waarop het verhaal zich bevindt</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een flexibel artikel maken in een herhaling

1. Ga naar de dynamische iteratie waar u het artikel wilt maken:

   1. Klik op het pictogram **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront en klik vervolgens op **[!UICONTROL Teams]** .

   1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

   1. Selecteer **[!UICONTROL Iterations]** in het linkerdeelvenster.
   1. Klik op de naam van de specifieke herhaling waar u een artikel wilt maken.
   1. Selecteer **[!UICONTROL Stories]** in het linkerdeelvenster.

1.  Klik op **[!UICONTROL New Story].**
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
      <td>Geef de schatting voor het artikel op. Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] in het artikel.<br> bijvoorbeeld, als u een verhaal als 3 punten schat, is het standaardgedrag 24 Geplande Uren aan het verhaal toe te voegen.<br> als een verhaal subtaken bevat, herinner dat de gecombineerde ramingen voor alle subtaken de schatting van het ouderverhaal bepalen. Voor meer informatie, zie <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref"> een subtask aan een bestaand verhaal op de [!UICONTROL Scrum] raad </a> toevoegen.</td>
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
