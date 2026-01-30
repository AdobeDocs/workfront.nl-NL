---
product-area: projects
navigation-topic: update-work-in-a-project
title: Taakstatus bijwerken
description: U kunt de status van een taak bijwerken om anderen te informeren over waar de taak is (en het algemene project) en hoe de taak vordert.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Taakstatus bijwerken

<!--Audited: 10/2024-->

U kunt de status van een taak bijwerken om anderen te informeren over waar de taak is (en het algemene project) en hoe de taak vordert.

De standaardstatussen zijn Nieuw, Bezig en Voltooid. Uw Adobe Workfront-beheerder kan aangepaste statussen toevoegen aan uw organisatie. Voor meer informatie, zie [&#x200B; een status &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

U kunt taakstatussen handmatig bijwerken of u kunt Workfront toestaan deze automatisch bij te werken wanneer bepaalde handelingen plaatsvinden.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taak beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p> 
   Or
   <p>Current: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen bij het bijwerken van de status van taken

* Wanneer u een taak markeert als Voltooid, wordt het percentage dat is voltooid van de taak bijgewerkt naar 100%.
* De volgende scenario&#39;s bestaan voor oudertaken:
   * U kunt niet de Status van een oudertaak bijwerken om te voltooien wanneer de Summiere Wijze van de Voltooiing van het project aan Automatisch wordt geplaatst en subtasks niet worden voltooid.
   * U kunt de Status van een oudertaak bijwerken om te voltooien wanneer de Summiere Wijze van de Voltooiing van het project aan Handboek wordt geplaatst en subtaken worden voltooid of onvolledig.

  Voor meer informatie, zie [&#x200B; projecten &#x200B;](../manage-projects/edit-projects.md) uitgeven.

## Taakstatus handmatig bijwerken

U kunt de taakstatus op de volgende gebieden bijwerken:

* De taakkopbal op de taakpagina.
* Het taakvak Bewerken wanneer u een taak bewerkt.
* De sectie Taakdetails op de taakpagina.
* In een taaklijst of rapport wanneer het gebied van de Status in de mening zichtbaar is.
* In het paneel Overzicht van de taak.

De taakstatus in de taakkoptekst handmatig bijwerken:

1. Ga naar een taak waarvoor u de status wilt bijwerken.
1. In de taakkopbal, klik het **gebied van de Status** en selecteer een nieuwe status.
1. Om een visuele aanwijzing van taakvoltooiing te verstrekken, sleep de bel onder **Volledige Percentage** in de kopbal van de taak.

   of

   Dubbelklik binnen de **Volledige** bel van de Percentage &lbrace;om een nieuw percentage manueel in te gaan.

   ![&#x200B; Percentage volledige statuswidgets taakkopbal &#x200B;](assets/percent-complete-status-widgets-task-header.png)

1. (Optioneel) Voer een van de volgende handelingen uit om aanvullende informatie over de update op te geven:

   * Om een nota over de update toe te voegen, ga naar de **sectie van Updates** en klik **Nieuwe commentaar**, dan typ een nota.

     ![&#x200B; Toevoegend een update aan een taak &#x200B;](assets/add-update-to-task.png)

   * Om bepaalde gebruikers over de update op de hoogte te brengen, typ hun namen op het **mensen van de Markering of team** gebied dat verschijnt wanneer u een commentaar typt. Voor meer informatie, zie [&#x200B; Tags anderen op updates &#x200B;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Om de taak bij te werken begaat datum, klik **Details van de Taak**, dan geef het **gebied van de Datum** toe. Voor informatie, zie [&#x200B; taken &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.


   >[!IMPORTANT]
   >
   >  Alleen taaktoewijzing kan de datum vastleggen bijwerken.

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![Drag the progress bar]](assets/drag-the-progress-bar-350x155.png)-->

## Taakstatus automatisch bijwerken

Workfront werkt de bestaande status van een taak automatisch bij naar een andere status wanneer de in de onderstaande tabel vermelde handelingen plaatsvinden.

>[!NOTE]
>
>De statussen in de volgende tabel zijn standaardsysteemstatussen. Uw Workfront-beheerder of een groepsbeheerder kan de naam van de statussen in uw exemplaar van Workfront wijzigen. Voor informatie over het creëren van en het leiden van statussen in Workfront, zie [&#x200B; een status &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Handeling</b></td> 
   <td><b>Oorspronkelijke status</b></td> 
   <td><b>Nieuwe status</b></td> 
  </tr> 
  <tr> 
   <td>Het taakpercentage bijwerken tot 100%</td> 
   <td>Nieuw of Bezig</td> 
   <td>Voltooid</td> 
  </tr> 
  <tr> 
   <td>Werk het taakpercentage bij dat is voltooid van 100% tot een lager getal</td> 
   <td>Voltooid</td> 
   <td>In uitvoering</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span> klik de knoop van de Taak van het Begin om het werken aan een taak goed te keuren die aan u wordt toegewezen </span> </td> 
   <td><span> Nieuw </span> </td> 
   <td> <p>Om het even welke status verbonden aan de knoop van de Taak van het Begin in uw montages van het Team van het Huis.</p> <p>Voor informatie over het vervangen van het Werk op het knoop met een knoop van de Taak van het Begin, zie <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref"> het Werk op het knoop met een knoop van het Begin vervangen </a></span>.</p> <p>Tip: <span> klikkend </span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ongedaan maken knoop </span> na het klikken van de Taak van het Begin keert de status aan Nieuw terug. </p> </td> 
  </tr> 
 </tbody> 
</table>
