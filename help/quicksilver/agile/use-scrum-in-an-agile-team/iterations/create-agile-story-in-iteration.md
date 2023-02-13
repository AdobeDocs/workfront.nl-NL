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
source-wordcount: '526'
ht-degree: 0%

---

# Een flexibel artikel maken in een herhaling

In dit artikel wordt beschreven hoe u een nieuw, flexibel artikel kunt maken wanneer u zich al in de herhaling bevindt. Voor informatie over het maken van een &#39;agile&#39; artikel op basis van een taak, uitgave of ander gebied van [!DNL Adobe Workfront], zie [Artikelen toevoegen aan een bestaande herhaling](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project waarop het verhaal zich bevindt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een flexibel artikel maken in een herhaling

1. Ga naar de dynamische iteratie waar u het artikel wilt maken:

   1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront, klik vervolgens op **[!UICONTROL Teams]**.

   1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw scrubteam in het keuzemenu of zoek naar een team op de zoekbalk.

   1. Selecteer in het linkerdeelvenster de optie **[!UICONTROL Iterations]**.
   1. Klik op de naam van de specifieke herhaling waar u een artikel wilt maken.
   1. Selecteer in het linkerdeelvenster de optie **[!UICONTROL Stories]**.

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
      <td>Selecteer deze optie als het artikel kan worden toegevoegd aan een herhaling. Als deze optie is geselecteerd, wordt aan gebruikers aangegeven welke artikelen in de backlog kunnen worden toegevoegd aan een herhaling.<br>Een artikel kan aan een herhaling worden toegevoegd, ongeacht of het is gemarkeerd <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (punten)</strong></td>
      <td>Geef de schatting voor het artikel op. Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] over het verhaal.<br>Als u bijvoorbeeld een artikel instelt op 3 punten, wordt standaard 24 geplande uren aan het artikel toegevoegd.<br>Als een artikel subtaken bevat, moet u niet vergeten dat de gecombineerde schattingen voor alle subtaken de schatting van het bovenliggende artikel bepalen. Zie voor meer informatie <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Een subtaak toevoegen aan een bestaand artikel op het tabblad [!UICONTROL Scrum] board</a>.</td>
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
