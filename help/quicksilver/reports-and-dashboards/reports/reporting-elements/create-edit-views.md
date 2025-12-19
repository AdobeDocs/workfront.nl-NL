---
product-area: reporting
navigation-topic: reporting-elements
title: Weergaven maken of bewerken in Adobe Workfront
description: U kunt het type informatie aanpassen dat u op het scherm weergeeft met behulp van weergaven. In Adobe Workfront kunt u verschillende typen weergaven gebruiken.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 0%

---

# Weergaven maken of bewerken in Adobe Workfront

<!-- Audited: 11/2024 -->

U kunt het type informatie aanpassen dat u op het scherm weergeeft met behulp van weergaven. In Adobe Workfront kunt u verschillende typen weergaven gebruiken.

In dit artikel wordt beschreven hoe u standaardweergaven voor lijsten en rapporten maakt en bewerkt.

Voor meer informatie, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</strong></td> 
   <td> 
    <p>Medewerker of hoger</p>
    <p>Aanvraag of hoger</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een weergave in een rapport te maken</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren om een weergave in een rapport te maken of te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Een weergave maken of aanpassen

Het proces voor het maken of aanpassen van een weergave is afhankelijk van het feit of u een standaardweergave of een weergave op het toetsenbord maakt of aanpast.

### Een standaardweergave maken of aanpassen {#create-or-customize-a-standard-view}

U kunt een nieuwe standaardweergave maken of een bestaande standaardweergave aanpassen die u eerder hebt gemaakt.

1. Klik het **drop-down menu van de Mening** op om het even welke lijst waar u een mening tot stand wilt brengen of aanpassen.

1. Klik op de knop **+ Nieuwe weergave** om een nieuwe weergave te maken.
of
Klik **uitgeven** pictogram ![ geeft pictogram ](assets/edit-icon.png) uit dat op muis over rechts van een bestaande mening verschijnt u wilt uitgeven.
**past de vertoningen van de de dialoogdoos van de Mening** aan.

1. In de **sectie van de Voorproef van de Kolom**, doe om het even welke volgend:

   * Wijzig de waarde van om het even welke kolom door de kolomtitel te klikken en dan een nieuw gebied te selecteren.
   * Voeg een kolom toe door **te klikken voeg Kolom** toe, begin typend de naam van de kolom die u wilt toevoegen, dan het klikken wanneer het in de drop-down lijst verschijnt.
   * Pas de volgorde van de kolommen aan door de kolomtitel naar een nieuwe locatie te slepen.

   * In het **gebied van de Montages van de Kolom**, klik **vat deze kolom door** samen, en kies hoe u de gegevens in de kolom wilt tonen. Deze optie is beschikbaar voor de volgende kolomtypen:
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Datumvelden</strong></td> 
           <td><ul>
           <li>Maximum</li>
         <li>Minimaal</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Valutamarkten</strong></td> 
           <td><ul>
           <li>Aantal</li>
         <li>Som</li>
           <li>Gemiddelde</li>
         <li>Maximum</li>
           <li>Minimaal</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Tekenreeks- en Booleaanse velden</strong></td> 
           <td><ul><li>Aantal</li></ul>
           <p>Opmerking: Workfront raadt doorgaans niet aan een booleaans veld op aantal samen te vatten, omdat de waarde altijd true/false is.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >De volgende uitzonderingen zijn van toepassing op bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvat voor de volgende velden in groepen:
     >   
     > * In alle velden voor getallen en valuta&#39;s, met uitzondering van werkelijke uren (bijvoorbeeld geplande/werkelijke loonkosten, geplande/werkelijke kosten, geplande/werkelijke kosten, geplande uren) wordt een overzicht gegeven van de waarden voor alleen kindertaken en zelfstandige taken. Zij vatten de waarden voor de oudertaken of de ouders van ouders niet samen.
     > * Werkelijke uren geeft een overzicht van de waarden voor de hoofdbovenliggende taken en de zelfstandige taken; deze geven geen overzicht van de getallen voor de bovenliggende taken of de onderliggende taken.
     > * De gegevensgebieden van de douane voor aantal en muntwaarden vatten alle taken samen: ouders, kinderen, ouders van ouders, en standalone taken.
     >
     >Voor meer informatie over het gebruiken van groeperingen in een rapport, zie het artikel [ overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facultatief) klik **Geavanceerde Opties** om de volgende informatie voor de kolom te specificeren:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Aangepast kolomlabel</strong></td> 
           <td><p>Geef een aangepast label voor de kolom op. Dit label vervangt het standaardlabel. We raden u aan alleen UTF-8-tekens te gebruiken om compatibiliteitsproblemen te voorkomen.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Veldindeling</strong></td> 
           <td>Selecteer de indeling waarin u de waarden voor de velden in de kolom wilt weergeven.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Deze kolom tonen wanneer deze zich op een dashboard bevindt</strong></td> 
           <td><p>Selecteer deze optie om deze kolom op een dashboard te tonen, wanneer het rapport naast elkaar met een ander rapport wordt getoond. Als deze optie is uitgeschakeld, wordt deze kolom niet weergegeven wanneer u het rapport weergeeft op een dashboard waar rapporten naast elkaar worden weergegeven.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Kolomregels</strong></td> 
           <td><p>Klik <strong>+ voeg een Regel voor deze Kolom </strong> toe om een regel voor de kolom te bepalen. Nadat u een regel hebt toegevoegd, kunt u veld- en tekststijlen definiëren voor de weergave van velden die overeenkomen met die regel. Klik <strong> toevoegen Regel </strong> nadat u het bepalen van de regel hebt gebeëindigd.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Voor meer informatie over voorwaardelijk het formatteren van meningen in rapporten, zie het artikel [ Voorwaardelijke het formatteren van het Gebruik in de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Voorwaardelijk) als u **Geavanceerde Opties** klikte, klik **Gedaan**.

1. Klik **sparen Mening** om een nieuwe mening tot stand te brengen of de huidige mening met uw veranderingen te vervangen.\
   of\
   Klik **sparen als Nieuwe Mening** om uw veranderingen als nieuwe mening te bewaren.

   >[!TIP]
   >
   >**sparen als Nieuwe Mening** is de enige beschikbare optie wanneer u een ingebouwde mening van Workfront aanpast.

   Uw toegang bepaalt hoe de weergave wordt opgeslagen. Als u de weergave hebt gemaakt, kunt u de wijzigingen opslaan. Als u dit niet doet, wordt u gevraagd een versie op te slaan. Houd er rekening mee dat wijzigingen die u aanbrengt in de weergave van invloed zijn op gebruikers met wie de weergave is gedeeld.

### Een toetsenbordweergave maken of aanpassen {#create-or-customize-an-agile-view}

U kunt projecten beheren volgens een Agile-methode met behulp van een Board-weergave.

De meningen van de raad zijn beschikbaar slechts voor lijsten van taken en kwesties betreffende een project.

Zij zijn preconfigured, maar u kunt bepaalde montages voor hen wijzigen.

Voor meer informatie over de meningen van de Gelijkheid of van de Raad, zie het artikel [ leiden een project van de Gelijkheid in de mening van de Raad ](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
