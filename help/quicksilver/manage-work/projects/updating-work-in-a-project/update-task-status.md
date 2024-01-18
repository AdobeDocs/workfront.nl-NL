---
product-area: projects
navigation-topic: update-work-in-a-project
title: Taakstatus bijwerken
description: U kunt de status van een taak bijwerken om anderen te informeren over waar de taak is (en het algemene project) en hoe de taak vordert.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Taakstatus bijwerken

U kunt de status van een taak bijwerken om anderen te informeren over waar de taak is (en het algemene project) en hoe de taak vordert.

De standaardstatussen zijn Nieuw, Bezig en Voltooid. Uw Adobe Workfront-beheerder kan aangepaste statussen toevoegen aan uw organisatie. Zie voor meer informatie [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

U kunt taakstatussen handmatig bijwerken of u kunt Workfront toestaan deze automatisch bij te werken wanneer bepaalde handelingen plaatsvinden.

## Toegangsvereisten

U moet de volgende toegang hebben om taken handmatig bij te werken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard</p> 
   of
   <p>Huidig: Werk of hoger</p>
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

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het bijwerken van de status van taken

* Wanneer u een taak markeert als Voltooid, wordt het percentage dat is voltooid van de taak bijgewerkt naar 100%.
* De volgende scenario&#39;s bestaan voor oudertaken:
   * U kunt niet de Status van een oudertaak bijwerken om te voltooien wanneer de Summiere Wijze van de Voltooiing van het project aan Automatisch wordt geplaatst en subtaken niet worden voltooid.
   * U kunt de Status van een oudertaak bijwerken om te voltooien wanneer de Summiere Wijze van de Voltooiing van het project aan Handboek wordt geplaatst en subtaken worden voltooid of onvolledig.

  Zie voor meer informatie [Projecten bewerken](../manage-projects/edit-projects.md).

## Taakstatus handmatig bijwerken

U kunt de taakstatus in de volgende gebieden van Workfront bijwerken:

* De taakkopbal op de taakpagina.
* Het taakvak Bewerken wanneer u een taak bewerkt.
* De sectie Taakdetails op de taakpagina.
* In een taaklijst of rapport, wanneer het gebied van de Status in de mening zichtbaar is.
* In het paneel Overzicht van de taak.

De taakstatus in de taakkoptekst handmatig bijwerken:

1. Ga naar een taak waarvoor u de status wilt bijwerken.
1. Klik op de knop **Status** in de taakkopbal en selecteer een nieuwe status.
1. Om een visuele aanwijzing van taakvoltooiing te verstrekken, sleep of klik de bel onder tweemaal **Percentage voltooid** in de takenkoptekst

   of

   Klik binnen de bel in de kopbal van de taak om een percentage in te gaan.

   ![](assets/percent-complete-status-widgets-task-header.png)

1. (Optioneel) Voer een van de volgende handelingen uit om aanvullende informatie over de update op te geven:

   * Als u een notitie over de update wilt toevoegen, gaat u naar de **Updates** sectie en klik op **Nieuwe opmerking** Typ vervolgens een notitie.

     ![](assets/add-update-to-task.png)

   * Als u bepaalde gebruikers op de hoogte wilt stellen van de update, typt u hun namen in het dialoogvenster **Tags toewijzen aan personen of teams** wordt weergegeven wanneer u een opmerking typt. Zie voor meer informatie [Andere tags toepassen op updates](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Als u de taakdatum vastleggen wilt bijwerken, klikt u op **Taakdetails** en bewerkt u vervolgens de **Vastlegdatum** veld. Zie voor meer informatie [Taken bewerken](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).


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
     ![](assets/drag-the-progress-bar-350x155.png)-->

## Taakstatus automatisch bijwerken

Workfront werkt de bestaande status van een taak automatisch bij naar een andere status wanneer de in de onderstaande tabel vermelde handelingen plaatsvinden.

>[!NOTE]
>
>De statussen in de volgende tabel zijn standaardsysteemstatussen. Uw Workfront-beheerder of een groepsbeheerder kan de naam van de statussen in uw exemplaar van Workfront wijzigen. Voor informatie over het maken en beheren van statussen in Workfront raadpleegt u [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td><span>Klik op de knop Taak starten om te accepteren dat u aan een taak werkt die aan u is toegewezen</span> </td> 
   <td><span>Nieuw</span> </td> 
   <td> <p>Om het even welke status verbonden aan de knoop van de Taak van het Begin in uw montages van het Team van het Huis.</p> <p>Voor informatie over het vervangen van het Werk op het met een knoop van de Taak van het Begin, zie <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a></span>.</p> <p>Tip: <span>Klikken</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">de knop Ongedaan maken</span>nadat u op Taak starten hebt geklikt, wordt de status teruggezet naar Nieuw. </p> </td> 
  </tr> 
 </tbody> 
</table>
