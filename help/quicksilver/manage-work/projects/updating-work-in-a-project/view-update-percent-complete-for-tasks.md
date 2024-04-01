---
product-area: projects
navigation-topic: update-work-in-a-project
title: Percentage van voltooiing weergeven en bijwerken voor taken
description: U kunt het percentage van voltooiing van een taak bijwerken om de vooruitgang aan te geven die u op de taak hebt gemaakt om het te voltooien.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Percentage van voltooiing weergeven en bijwerken voor taken

<!--Audited:01/2024-->

U kunt het percentage van voltooiing van een taak bijwerken om de vooruitgang aan te geven die u op de taak hebt gemaakt om het te voltooien.

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
   <td> <p>Nieuwe licentie: standaard</p> 
   of
   <p>Huidige licentie: werken of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taak beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Gebieden waar u het percentage van voltooiing van een taak kunt bijwerken

U kunt het voltooide percentage voor een taak op een van de volgende gebieden bijwerken:

* **In een takenlijst**: U kunt het voltooide percentage van een taak bijwerken wanneer de kolom Percentage voltooid wordt weergegeven.\
  Zie voor meer informatie over inline bewerken [Items inline bewerken in een lijst in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In de milestone-weergave**: U kunt het percentage bijwerken voltooide van een taak wanneer het gebruiken van de mening van de Mijlpaal op een projectlijst of een projectrapport. Zie voor meer informatie [De milestone-weergave gebruiken](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **In de taakkoptekst**: U kunt het percentage van een taak bijwerken in de taakkoptekst. Zie voor meer informatie [Taken bewerken](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **In het deelvenster Samenvatting van een taak**: U kunt het percentage van een taak dat is voltooid boven in het deelvenster Overzicht bijwerken wanneer u de taak in de volgende gebieden weergeeft:

   * Taaklijst of rapport
   * Tijdschema
   * Werklastverdeling

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Zie voor meer informatie [Overzicht van samenvattingen](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)


## Overwegingen bij het bijwerken van het percentage voltooide taken

* Wanneer u een taak markeert als 100% voltooid, wordt de taakstatus bijgewerkt naar Voltooid.
* De volgende scenario&#39;s bestaan voor oudertaken:
   * U kunt niet het percentage bijwerken volledig van een oudertaak aan 100% wanneer de Summiere Wijze van de Voltooiing van het project aan Automatisch wordt geplaatst en de subtaken niet worden voltooid.
   * U kunt het percentage volledig van een oudertaak aan 100% bijwerken wanneer de Summiere Wijze van de Voltooiing van het project aan Handboek wordt geplaatst en subtaken worden voltooid of onvolledig.

  Zie voor meer informatie [Projecten bewerken](../manage-projects/edit-projects.md).

## Het percentage van een taak bijwerken

1. Ga naar een van de volgende gebieden in Workfront:

   * Een takenlijst
   * Een lijst met projecten en past de Mijlpaal-weergave toe
   * Een taak, door tot de taakpagina toegang te hebben
1. Zoek de **Percentage voltooid** veld voor de taak waarvan het percentage is voltooid dat u wilt bijwerken.
1. Klik in het veld Percentage voltooid en typ een getal tussen 0 en 100

   of

   Klik en sleep de **Percentage voltooid** bar aan het noodzakelijke aantal om erop te wijzen hoeveel van de taak u, indien beschikbaar voltooide.

   >[!NOTE]
   >
   >Als u aangeeft dat 100% van de taak is voltooid, wordt de status van de taak ook bijgewerkt naar Voltooien.


1. Druk op Enter op het toetsenbord om het volledige percentage op te slaan.

Het percentage Voltooien van het project wordt ook automatisch bijgewerkt.

