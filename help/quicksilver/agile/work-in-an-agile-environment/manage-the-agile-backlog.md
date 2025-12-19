---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: De Google Backlog beheren
description: Taken en problemen kunnen worden toegewezen aan een Agile-team en worden toegevoegd aan de achterstand van dat team als artikelen, afhankelijk van de Agile-methode die het team gebruikt.
author: Jenny
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# De Google-achterstand beheren

De volgende het werkpunten kunnen aan een team worden toegewezen van de Gelijkheid en aan de achterstand van dat team als verhalen worden toegevoegd, afhankelijk van de methodologie van de Gelijkheid het team gebruikt:

* **[!UICONTROL Scrum Agile teams]:** Taken en problemen kunnen worden toegewezen aan het team van Adobe en worden toegevoegd aan de achterstand.
* **[!UICONTROL Kanban Agile teams]:** de taken kunnen aan het team van de Gelijkheid worden toegewezen en aan de achterstand worden toegevoegd. De gebruikers kunnen de achterstand van de het verhaalraad van de Giel, zoals die in [[!UICONTROL Add the backlog] aan de Kanban raad ](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md) wordt beschreven direct bekijken. Het team gebruikt deze achterstand om prioriteit te geven aan hun werkvoorraad en deze te beheren.

Taken of problemen kunnen vanaf elke locatie in [!DNL Adobe Workfront] aan het team worden toegewezen (en vervolgens aan de teamachterstand worden toegevoegd). Bijvoorbeeld, zou één enkel team werktaken van veelvoudige projecten kunnen worden toegewezen.

>[!NOTE]
>
>Als u veelvoudige teams aan een achterlogpunt toevoegt, toont de taak of de kwestie slechts op de achtergrond van het primaire team. Het primaire team is eerst toegewezen het team.

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

## Artikelen op de achtergrond maken en beheren

* [Artikelen opnieuw ordenen](#reorder-stories)
* [[!UICONTROL Break down] artikelen](#break-down-stories)
* [Artikelen bewerken](#edit-stories)

### Artikelen opnieuw ordenen {#reorder-stories}

U kunt de volgorde van artikelen in de lijst met terugverwijzingen wijzigen met slepen en neerzetten.

1. Ga naar de Google-blog waar u de artikelen opnieuw wilt rangschikken.
1. Selecteer in het vervolgkeuzemenu **[!UICONTROL View]** de **[!UICONTROL Backlog]** -weergave of een aangepaste weergave die de **[!UICONTROL Order]** -kolom bevat.

   >[!NOTE]
   >
   >Als een taak of een kwestie een toegewezen team van Agile heeft en het project niet in een status is die met Huidig vergelijkt, tonen zij niet op de achterstand. Nochtans, beïnvloeden zij nog de backlogtelling in de kolom van de Orde.

1. Selecteer een of meer artikelen en sleep de artikelen naar de volgorde waarin u ze op de achtergrond wilt weergeven.
   ![ belemmering en dalings achterlogpunten ](assets/agile-backlog-drag-and-drop.png)

### Artikelen onderverdelen {#break-down-stories}

Omdat de grootte van artikelen in een backlog varieert, kunnen gebruikers deze opsplitsen in werkbare grootten voor een herhaling. Als u een artikel omlaag splitst, worden er subtaken gemaakt voor de taak die het artikel vertegenwoordigt en wordt de oorspronkelijke taak op de achtergrond vervangen. U kunt een oudertaak of zijn subtaken hebben die aan een team van het Geavanceerd worden toegewezen, maar u kunt niet allebei aan een team gelijktijdig hebben toegewezen.

>[!NOTE]
>
>Houd rekening met de volgende beperkingen bij het opsplitsen van artikelen:
>
>* Alleen artikelen die taken vertegenwoordigen, kunnen worden opgesplitst. U kunt geen artikelen opsplitsen die problemen vertegenwoordigen.
>* Artikelen kunnen alleen worden opgesplitst als ze aan een project zijn gekoppeld.


Een artikel onderbreken:

1. Ga naar de achtergrond die het artikel bevat dat u wilt onderbreken.
1. Selecteer het artikel dat u wilt onderbreken en klik op **[!UICONTROL Breakdown Story]** .
Het dialoogvenster [!UICONTROL Breakdown Story] wordt weergegeven.
   ![ de dialoog van het Verhaal van de Onderbreking ](assets/backlog-breakdown-dialog.png)

1. Geef een naam en een schatting voor het artikel op en geef aan of het artikel gereed is.
1. Klik op **[!UICONTROL Add Story]** om een ander artikel te maken van het originele artikel.
1. Klik op **[!UICONTROL Save]**.

### Artikelen bewerken {#edit-stories}

U kunt verhalen van [!UICONTROL Stories] of [!UICONTROL Issues] lusjes op de Achtergrond direct uitgeven aangezien u om het even welke taken of kwesties binnen een project in massa zou uitgeven, zoals die in [ worden beschreven taken in bulk ](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) in [ uitgeeft taken ](../../manage-work/tasks/manage-tasks/edit-tasks.md), en [ uitgeeft kwesties ](../../manage-work/issues/manage-issues/edit-issues.md).

## Nieuwe artikelen maken op de achtergrond {#create-new-stories-on-the-backlog}

U kunt nieuwe artikelen op de achtergrond maken door het artikel rechtstreeks vanaf de achtergrond te maken of door een bestaande taak of uitgave toe te wijzen aan een team van Adobe.

* [Een artikel maken op basis van de historie](#create-a-story-from-the-backlog)
* [Een taak of uitgave toewijzen aan een Agile-team](#assign-a-task-or-issue-to-an-agile-team)

### Een artikel maken op basis van de historie {#create-a-story-from-the-backlog}

Wanneer u een artikel maakt op basis van de achterstand, wordt het artikel gemaakt als een taak of uitgave in een project.

Een artikel maken op basis van de historie:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Teams]**.

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu, of onderzoek naar een team in de onderzoeksbar en selecteer het wanneer het verschijnt.

1. Selecteer **[!UICONTROL Backlog]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit, afhankelijk van of u een taak of een uitgave wilt maken:

   * **om een taak te creëren:** klik **[!UICONTROL Stories]**.

   * **om een kwestie tot stand te brengen:** klik **[!UICONTROL Issues]**.

1. Klik op **[!UICONTROL New Story]** of **[!UICONTROL New Issue]** .

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
      <td>Typ de naam van het project waar dit artikel wordt gemaakt en klik vervolgens op de naam wanneer het wordt weergegeven in de vervolgkeuzelijst.<br> de status van het project moet aan [!UICONTROL Current] worden geplaatst. Als de status van het project iets anders is dan [!UICONTROL Current] , wordt het niet weergegeven in het vervolgkeuzemenu.</td>
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

### Een taak of uitgave toewijzen aan een Agile-team {#assign-a-task-or-issue-to-an-agile-team}

U kunt een taak of een kwestie aan een team van de Gielen toewijzen. Nadat deze is toegewezen, wordt de taak of uitgave weergegeven als een nieuw artikel op de teamachterstand.

U kunt als volgt een taak of uitgave toewijzen aan een Agile-team:

1. Ga naar het project dat de taak bevat die u wilt toewijzen.
1. Selecteer de taak of het probleem in de lijst.
1. Klik op **[!UICONTROL Edit]**.
1. Klik op **[!UICONTROL Assignments]**.
1. (Optioneel) Verwijder eventuele bestaande toewijzingen.
1. Klik op **[!UICONTROL Add Assignee]**.
1. Typ de naam van het gangbare team dat u aan de taak of uitgave wilt toewijzen en klik vervolgens op de teamnaam wanneer deze in de vervolgkeuzelijst wordt weergegeven.
1. Klik op **[!UICONTROL Save Changes]** .
De taak of kwestie is nu beschikbaar op de teamachterstand.

## Artikelen naar of van de achtergrond verplaatsen

* [Artikelen van de achtergrond verplaatsen naar een herhaling of board](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Bestaande artikelen naar de achtergrond verplaatsen](#move-existing-stories-to-the-backlog)
* [Artikelen exporteren uit de logbestandweergave](#export-stories-from-the-backlog)

### Artikelen van de achtergrond verplaatsen naar een herhaling of board

1. Ga naar de achterstand van het Agile-team.
1. Selecteer de artikelen die u naar een herhaling of Kanban-bord wilt verplaatsen en klik op **[!UICONTROL More]** > **[!UICONTROL Move to]** .
Als u het artikel naar een [!UICONTROL Kanban] -bord verplaatst, wordt het [!UICONTROL Move Story to the Kanban] -bord weergegeven.
Als u het artikel naar een herhaling verplaatst, wordt het dialoogvenster [!UICONTROL Move Story to an Iteration] weergegeven.
   ![ de dialoog van het Artikel van de Beweging ](assets/agile-backlog-addtoiteration.png)

1. Voer een van de volgende handelingen uit:

   * **voor de teams van het Trommel:** op het **[!UICONTROL Select Iteration]** gebied, selecteer de herhaling waar u de verhalen wilt bewegen.

   * **voor Kanban teams:** op het **[!UICONTROL Select Kanban Board]** gebied, selecteer uw team [!UICONTROL Kanban]. (Kanban-teams kunnen slechts één [!UICONTROL Kanban] -bord hebben.)

1. Klik op **[!UICONTROL Move Story]**.

### Bestaande artikelen naar de achtergrond verplaatsen {#move-existing-stories-to-the-backlog}

Als u besluit dat uw team nog niet klaar is om aan een artikel te werken, kunt u het artikel naar de achtergrond verplaatsen.

Voor meer informatie, zie [ een verhaal van de Beweging van de Gelijkheid ](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Artikelen exporteren uit de logbestandweergave {#export-stories-from-the-backlog}

U kunt een of meer artikelen (inclusief taken en problemen) rechtstreeks vanaf de achtergrond exporteren.

U voert verhalen van de achterstand op de zelfde manier uit dat u andere gegevens in [!DNL Workfront], zoals die in [ worden beschreven de gegevens van de Uitvoer ](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) uitvoert.
