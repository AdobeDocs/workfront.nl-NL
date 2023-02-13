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
source-wordcount: '592'
ht-degree: 0%

---

# Een subtaak toevoegen aan een bestaand artikel op het tabblad [!UICONTROL Scrum] board

Houd rekening met het volgende wanneer u subtaken maakt voor bestaande artikelen:

**Wanneer de [!UICONTROL Completion Mode] instellen voor het project is ingesteld op [!UICONTROL Manual]:**

* Een bovenliggend artikel met subtaken verplaatsen naar [!UICONTROL Complete] Hiermee werkt u het bovenliggende artikel bij naar 100% en de [!UICONTROL Status] tot [!UICONTROL Complete]. Subtaken worden niet bijgewerkt.
* Als u het dialoogvenster [!UICONTROL Percent Complete] voor het artikel moet u het bijwerken vanuit de [!UICONTROL Stories] of van de [!UICONTROL Details] pagina van het object.

**Wanneer de [!UICONTROL Completion Mode] instellen voor het project is ingesteld op[!UICONTROL Automatic]**:

* Een bovenliggend artikel met subtaken verplaatsen naar [!UICONTROL Complete] Hiermee werkt u het bovenliggende artikel bij naar 100% en de [!UICONTROL Status] tot [!UICONTROL Complete]. Subtaken worden ook bijgewerkt naar 100% en de [!UICONTROL Status] wordt bijgewerkt naar [!UICONTROL Complete].
* Als u het dialoogvenster [!UICONTROL Percent Complete] voor het artikel moet u de [!UICONTROL Percent Complete] voor alle subtaken. De [!UICONTROL Percent Complete] voor het artikel wordt berekend op basis van de [!UICONTROL Percent Complete] van alle subtaken.

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
   <td> <p>[!UICONTROL Contribute] of [!UICONTROL Manage] toegang tot de taak subtask is</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een subtaak toevoegen aan een bestaand artikel op het gebied van de scrum

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw scrubteam in het keuzemenu of zoek naar een team op de zoekbalk.

1. Ga naar de flexibele iteratie of het project dat het artikel bevat waar u een subtaak wilt toevoegen. Voor informatie over hoe u naar een herhaling kunt navigeren, raadpleegt u [Een herhaling weergeven](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Ga naar de artikeltegel op het artikelbord waar u een subtaak wilt toevoegen.
1. Klikken **[!UICONTROL Add Subtask]** op de hoofdartikelkaart om een subtaak van het artikel te maken.

   ![Subtaak toevoegen](assets/agile-story-addsubtask-NWE.png)

   of

   Klikken **[!UICONTROL Add Subtask]** op een subtaaktegel om een subtaak aan subtask tot stand te brengen.

   [!DNL Workfront] ondersteunt oneindige niveaus van subtaken, maar er worden slechts twee niveaus (subtaken van subtaken) weergegeven op de &#39;agile story board&#39;.

   ![Subtaak toevoegen](assets/agile-story-addsubtask2-NWE.png)

   Wanneer u een subtaak toevoegt aan een artikel dat momenteel geen swimanet heeft, wordt de bovenliggende taak opgewaardeerd tot de [!UICONTROL Parent Story] de kolom en de subtaak worden binnen de widget verplaatst.

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
        <li>Als uw mobiele team wordt gevormd om verhalen in punten te schatten, dan door gebrek 1 punt evenaart 8 uren. Schattingen worden toegevoegd als [!UICONTROL Planned Hours] over het verhaal.</li>
        <li>De gecombineerde schattingen voor alle subtaken bepalen de schatting van het bovenliggende artikel. Zie voor meer informatie <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">De status van artikelen en subtaken bijwerken op het Klembord</a>.</li>
        <li>Wanneer u een nieuwe subtaak maakt, [!UICONTROL Estimate] is al ingesteld. Als u de schatting voor de subtaak herstelt, stelt u de schatting voor het bovenliggende artikel opnieuw in (omdat het bovenliggende artikel de som van alle subtaken is).</li>
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
