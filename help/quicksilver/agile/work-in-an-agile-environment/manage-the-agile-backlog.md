---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: De logboekregistratie voor bestanden beheren
description: Taken en problemen kunnen worden toegewezen aan een flexibel team en worden toegevoegd aan de achterstand van dat team als artikelen, afhankelijk van de flexibele methodologie die het team gebruikt.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---

# De logboekregistratie voor bestanden beheren

De volgende het werkpunten kunnen aan een flexibel team worden toegewezen en aan de achterstand van dat team als verhalen worden toegevoegd, afhankelijk van de flexibele methodologie het team gebruikt:

* **[!UICONTROL Scrum agile teams]:** Taken en problemen kunnen worden toegewezen aan het mobiele team en worden toegevoegd aan de achterstand.
* **[!UICONTROL Kanban agile teams]:** Taken kunnen worden toegewezen aan het mobiele team en worden toegevoegd aan de back-up. Gebruikers kunnen de back-up rechtstreeks vanaf de kaart met het flexibele artikel weergeven, zoals wordt beschreven in [[!UICONTROL Add the backlog] aan de Kanban-raad](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). Het team gebruikt deze achterstand om prioriteit te geven aan hun werkvoorraad en deze te beheren.

Taken of problemen kunnen vanaf elke locatie in het team worden toegewezen aan het team (en vervolgens aan de teamachterstand worden toegevoegd) [!DNL Adobe Workfront]. Bijvoorbeeld, zou één enkel team werktaken van veelvoudige projecten kunnen worden toegewezen.

>[!NOTE]
>
>Als u veelvoudige teams aan een achterlogpunt toevoegt, toont de taak of de kwestie slechts op de achtergrond van het primaire team. Het primaire team is eerst toegewezen het team.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie</strong></td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidige: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidige: [!UICONTROL Worker] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project waarop het verhaal zich bevindt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Artikelen op de achtergrond maken en beheren

* [Artikelen opnieuw ordenen](#reorder-stories)
* [[!UICONTROL Break down] verhalen](#break-down-stories)
* [Artikelen bewerken](#edit-stories)

### Artikelen opnieuw ordenen {#reorder-stories}

U kunt de volgorde van artikelen in de lijst met terugverwijzingen wijzigen met slepen en neerzetten.

1. Ga naar de &#39;agile&#39;-achterstand waar u artikelen opnieuw wilt rangschikken.
1. In de **[!UICONTROL View]** vervolgkeuzelijst, selecteert u de **[!UICONTROL Backlog]** of een aangepaste weergave die de **[!UICONTROL Order]** kolom.

   >[!NOTE]
   >
   >Als een taak of een kwestie een flexibel toegewezen team heeft en het project niet in een status is die met Huidig vergelijkt, tonen zij niet op de backlog. Nochtans, beïnvloeden zij nog de backlogtelling in de kolom van de Orde.

1. Selecteer een of meer artikelen en sleep de artikelen naar de volgorde waarin u ze op de achtergrond wilt weergeven.\
   ![Achterlogitems slepen en neerzetten](assets/agile-backlog-drag-and-drop.png)

### Artikelen onderverdelen {#break-down-stories}

Omdat de grootte van artikelen in een backlog varieert, kunnen gebruikers deze opsplitsen in werkbare grootten voor een herhaling. Als u een artikel omlaag splitst, worden er subtaken gemaakt voor de taak die het artikel vertegenwoordigt en wordt de oorspronkelijke taak op de achtergrond vervangen. U kunt een oudertaak of zijn subtaken hebben die aan een veranderlijk team worden toegewezen, maar u kunt niet allebei aan een team gelijktijdig hebben toegewezen.

>[!NOTE]
>
>Houd rekening met de volgende beperkingen bij het opsplitsen van artikelen:
>
>* Alleen artikelen die taken vertegenwoordigen, kunnen worden opgesplitst. U kunt geen artikelen opsplitsen die problemen vertegenwoordigen.
>* Artikelen kunnen alleen worden opgesplitst als ze aan een project zijn gekoppeld.


Een artikel onderbreken:

1. Ga naar de achtergrond die het artikel bevat dat u wilt onderbreken.
1. Selecteer het artikel dat u wilt onderbreken en klik op **[!UICONTROL Breakdown Story]**.\
   De [!UICONTROL Breakdown Story] wordt weergegeven.\
   ![Dialoogvenster Artikel indelen](assets/backlog-breakdown-dialog.png)

1. Geef een naam en een schatting voor het artikel op en geef aan of het artikel gereed is.
1. Klikken **[!UICONTROL Add Story]** om een ander artikel te maken van het originele artikel.
1. Klik op **[!UICONTROL Save]**.

### Artikelen bewerken {#edit-stories}

U kunt artikelen rechtstreeks vanuit het dialoogvenster [!UICONTROL Stories] of [!UICONTROL Issues] tabs op de Backlog omdat u taken of problemen in een project bulksgewijs zou bewerken, zoals beschreven in [Taken bulksgewijs bewerken](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) in [Taken bewerken](../../manage-work/tasks/manage-tasks/edit-tasks.md), en [Problemen bewerken](../../manage-work/issues/manage-issues/edit-issues.md).

## Nieuwe artikelen maken op de achtergrond {#create-new-stories-on-the-backlog}

U kunt nieuwe artikelen op de achtergrond maken door het artikel rechtstreeks vanaf de achtergrond te maken of door een bestaande taak of uitgave toe te wijzen aan een bestandsteam.

* [Een artikel maken op basis van de historie](#create-a-story-from-the-backlog)
* [Een taak of uitgave toewijzen aan een bestandsteam](#assign-a-task-or-issue-to-an-agile-team)

### Een artikel maken op basis van de historie {#create-a-story-from-the-backlog}

Wanneer u een artikel maakt op basis van de achterstand, wordt het artikel gemaakt als een taak of uitgave in een project. U kunt geen artikel maken op basis van de achterstand.

Een artikel maken op basis van de historie:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Teams]**.

1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw scrubteam in het keuzemenu of zoek naar een team in de zoekbalk en selecteer het team wanneer het wordt weergegeven.

1. Selecteren **[!UICONTROL Backlog]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit, afhankelijk van of u een taak of een uitgave wilt maken:

   * **Een taak maken:** Klikken **[!UICONTROL Stories]**.

   * **Een probleem maken:** Klikken **[!UICONTROL Issues]**.

1. Klikken **[!UICONTROL New Story]** of **[!UICONTROL New Issue]**.

1. Geef de volgende informatie op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> Typ een naam voor het artikel.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>(Optioneel) Typ een beschrijving voor het artikel.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Selecteer of het artikel kan worden toegevoegd aan een herhaling. Deze instelling is alleen ter informatie. Artikelen kunnen aan een herhaling worden toegevoegd, ongeacht de status van deze instelling.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Geef een punt of uurschatting voor het artikel op. Schattingen zijn van invloed op de burndown-grafiek. Het burndown-diagram voor een herhaling is alleen correct als elk artikel een nauwkeurige schatting bevat. (Als u een puntschatting opgeeft, moet u in de teaminstellingen al hebben aangegeven hoeveel uren elk punt vertegenwoordigt.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Typ de naam van het project waar dit artikel wordt gemaakt en klik vervolgens op de naam wanneer het wordt weergegeven in de vervolgkeuzelijst.<br>De status van het project moet worden ingesteld op [!UICONTROL Current]. Als de status van het project iets anders is dan [!UICONTROL Current], wordt deze niet weergegeven in het keuzemenu.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>(Optioneel) Typ de naam van de bovenliggende taak waaraan dit artikel is gekoppeld, en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Optioneel) Selecteer de aangepaste formulieren die u aan dit artikel wilt toevoegen.</td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Save Story]**.

### Een taak of uitgave toewijzen aan een bestandsteam {#assign-a-task-or-issue-to-an-agile-team}

U kunt een taak of een kwestie aan een agile team toewijzen. Nadat deze is toegewezen, wordt de taak of uitgave weergegeven als een nieuw artikel op de teamachterstand.

Om een taak of een kwestie aan een agile team toe te wijzen:

1. Ga naar het Project dat de taak bevat die u wilt toewijzen.
1. Selecteer de taak of het probleem in de lijst.
1. Klik op **[!UICONTROL Edit]**.
1. Klik op **[!UICONTROL Assignments]**.
1. (Optioneel) Verwijder eventuele bestaande toewijzingen.
1. Klik op **[!UICONTROL Add Assignee]**.
1. Typ de naam van het bestandsteam dat u wilt toewijzen aan de taak of uitgave en klik vervolgens op de naam van het team wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. Klik op **[!UICONTROL Save Changes]**.\
   De taak of kwestie is nu beschikbaar op de teamachterstand.

## Artikelen naar of van de achtergrond verplaatsen

{#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Artikelen van de achtergrond verplaatsen naar een herhaling of een toetsenbord](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Bestaande artikelen naar de achtergrond verplaatsen](#move-existing-stories-to-the-backlog)
* [Artikelen exporteren uit de logbestandweergave](#export-stories-from-the-backlog)

### Artikelen van de achtergrond verplaatsen naar een herhaling of een toetsenbord

1. Ga naar de achtergrond van het agile team.
1. Selecteer de artikelen die u naar een herhalings- of Kanban-bord wilt verplaatsen en klik op **[!UICONTROL More]** > **[!UICONTROL Move to]**.\
   Als u het artikel naar een [!UICONTROL Kanban] de [!UICONTROL Move Story to the Kanban] Het toetsenbord wordt weergegeven.\
   Als u het artikel naar een herhaling verplaatst, wordt het [!UICONTROL Move Story to an Iteration] wordt weergegeven.\
   ![Het dialoogvenster Artikel verplaatsen](assets/agile-backlog-addtoiteration.png)

1. Voer een van de volgende handelingen uit:

   * **Voor rumteams:** In de **[!UICONTROL Select Iteration]** selecteert u de herhaling waarin u de artikelen wilt verplaatsen.

   * **Voor Kanban-teams:** In de **[!UICONTROL Select Kanban Board]** veld, selecteer uw team [!UICONTROL Kanban] bord. (Kanban-teams kunnen slechts één team hebben [!UICONTROL Kanban] bord.)

1. Klik op **[!UICONTROL Move Story]**.

### Bestaande artikelen naar de achtergrond verplaatsen {#move-existing-stories-to-the-backlog}

Als u besluit dat uw team nog niet klaar is om aan een artikel te werken, kunt u het artikel naar de achtergrond verplaatsen.

Zie voor meer informatie [Een stapel artikel verplaatsen](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Artikelen exporteren uit de logbestandweergave {#export-stories-from-the-backlog}

U kunt een of meer artikelen (inclusief taken en problemen) rechtstreeks vanaf de achtergrond exporteren.

U exporteert artikelen van de achtergrond op dezelfde manier als andere gegevens in [!DNL Workfront], zoals beschreven in [Gegevens exporteren](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
