---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Een subtaak toevoegen aan een bestaand artikel op het gebied van de scrum
description: Houd bij het maken van subtaken voor bestaande artikelen rekening met de instelling Voltooiingsmodus voor het project, omdat dit van invloed is op de manier waarop artikelen worden bijgewerkt.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Een subtaak toevoegen aan een bestaand artikel op het [!UICONTROL Scrum] -bord

Houd rekening met het volgende wanneer u subtaken maakt voor bestaande artikelen:

**wanneer het [!UICONTROL Completion Mode] plaatsen voor het project aan [!UICONTROL Manual] wordt geplaatst:**

* Als u een bovenliggend artikel met subtaken verplaatst naar [!UICONTROL Complete] , wordt het bovenliggende artikel bijgewerkt naar 100% en de [!UICONTROL Status] naar [!UICONTROL Complete] . Subtaken worden niet bijgewerkt.
* Als u [!UICONTROL Percent Complete] voor het artikel wilt bijwerken, moet u het bijwerken vanaf de [!UICONTROL Stories] -tab of de [!UICONTROL Details] -pagina van het object.

**wanneer [!UICONTROL Completion Mode] het plaatsen voor het project aan[!UICONTROL Automatic]** wordt geplaatst:

* Als u een bovenliggend artikel met subtaken verplaatst naar [!UICONTROL Complete] , wordt het bovenliggende artikel bijgewerkt naar 100% en de [!UICONTROL Status] naar [!UICONTROL Complete] . Subtaken worden ook bijgewerkt naar 100% en [!UICONTROL Status] wordt bijgewerkt naar [!UICONTROL Complete] .
* Als u [!UICONTROL Percent Complete] voor het artikel wilt bijwerken, moet u [!UICONTROL Percent Complete] voor alle subtaken bijwerken. De waarde [!UICONTROL Percent Complete] voor het artikel wordt berekend op basis van de waarde [!UICONTROL Percent Complete] van alle subtaken.

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
   <td> <p>[!UICONTROL Contribute] of [!UICONTROL Manage] toegang hebben tot de taak waarop de subtaak is uitgevoerd</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een subtaak toevoegen aan een bestaand artikel op het gebied van de scrum

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Teams]** .

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Ga naar de flexibele iteratie of het project dat het artikel bevat waar u een subtaak wilt toevoegen. Voor informatie over hoe te om aan een herhaling te navigeren, zie [ Mening een herhaling ](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Ga naar de artikeltegel op het artikelbord waar u een subtaak wilt toevoegen.
1. Klik op **[!UICONTROL Add Subtask]** op de hoofdartikelkaart om een subtaak voor het artikel te maken.

   ![ voeg subtask ](assets/agile-story-addsubtask-NWE.png) toe

   of

   Klik op **[!UICONTROL Add Subtask]** op een tegel voor een subtaak om een subtaak voor de subtaak te maken.

   [!DNL Workfront] ondersteunt oneindige niveaus van subtaken, maar er worden slechts twee niveaus (subtaken van subtaken) weergegeven op de agile story-board.

   ![ voeg subtask ](assets/agile-story-addsubtask2-NWE.png) toe

   Wanneer u een subtaak toevoegt aan een artikel dat momenteel geen swimanie heeft, wordt de bovenliggende taak opgewaardeerd tot de kolom [!UICONTROL Parent Story] en wordt de subtaak binnen de widget geplaatst.

1. Geef de volgende informatie op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask Name]</strong></td>
      <td> Geef een naam op voor de subtaak.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Geef een beschrijving op voor de subtaak.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Geef de schatting voor de subtaak op.<br><p>Houd rekening met het volgende wanneer u schattingen maakt:</p>
       <ul>
        <li>Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] in het artikel.</li>
        <li>De gecombineerde schattingen voor alle subtaken bepalen de schatting van het bovenliggende artikel. Voor meer informatie, zie <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref"> de status van verhalen en subtaken op het board van het Trommel </a> bijwerken.</li>
        <li>Wanneer u een nieuwe subtaak maakt, is het veld [!UICONTROL Estimate] al ingesteld. Als u de schatting voor de subtaak herstelt, stelt u de schatting voor het bovenliggende artikel opnieuw in (omdat het bovenliggende artikel de som van alle subtaken is).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Hours]</strong></td>
      <td> (Alleen beschikbaar in projecten) Geef het aantal geplande uren voor de taak op.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>Typ de naam van het team waaraan u de subtaak wilt toewijzen en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.</td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Create]**.
