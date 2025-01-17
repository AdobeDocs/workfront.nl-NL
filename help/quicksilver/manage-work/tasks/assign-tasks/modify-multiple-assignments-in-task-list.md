---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Meerdere gebruikerstoewijzingen in een takenlijst wijzigen
description: Wanneer het beheren van taaktaken, kunt u hen voor veelvoudige taken tegelijkertijd wijzigen door de bulkbewerkingseigenschap in een lijst van taken te gebruiken.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Meerdere gebruikerstoewijzingen in een takenlijst wijzigen

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Wanneer het beheren van taaktaken, kunt u hen voor veelvoudige taken tegelijkertijd wijzigen door de bulkbewerkingseigenschap in een lijst van taken te gebruiken.

In dit artikel wordt verwezen naar het wijzigen van meerdere gebruikerstoewijzingen voor meerdere taken in een takenlijst. Zie ook de volgende artikelen voor het wijzigen van toewijzingen voor meerdere taken op andere gebieden:

* Voor informatie over het toewijzen van taken die de Balancer van de Werklast gebruiken, zie [ Overzicht van het toewijzen van het werk in de Balancer van de Werkbelasting ](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Voor informatie over het toewijzen van een taak aan één middel in een lijst, zie [ taken toewijzen ](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute- of hogere machtigingen voor taken</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Toewijzingen wijzigen voor meerdere taken

1. Ga naar de lijst die de taken bevat waar u taken wilt wijzigen.
1. (Optioneel) Maak een filter om alleen taken weer te geven die zijn toegewezen aan de ontvanger die u wilt wijzigen.

   Bijvoorbeeld, als uw project een specifieke rol als standaardontvanger voor veelvoudige taken bevat, kunt u een filter tot stand brengen om slechts taken met die rol als toegewezen te tonen. Vervolgens kunt u de rol vervangen door een specifieke gebruiker.

   Voor informatie over het creëren van een filter, zie [ filters ](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.


1. Om op een rol te filtreren, uitgezochte **Rollen van de Taak**, dan klik **identiteitskaart**.

   >[!TIP]
   >
   >Gebruik niet **Toegewezen aan** gebied. Dit vindt slechts de Primaire Eigenaar voor de taak in plaats van om het even welke rollen die aan hen konden worden toegewezen.

   of

   Om voor een gebruiker te filtreren, uitgezochte **Gebruikers van de Taak,** dan klik **identiteitskaart.**

   >[!TIP]
   >
   >Gebruik niet **Toegewezen aan** gebied. Hiermee vindt u alleen de primaire eigenaar voor de taak in plaats van de gebruikers die aan hen kunnen worden toegewezen.

1. Selecteer de taken waarvoor u taken wilt wijzigen, dan klik **uitgeven** pictogram ![](assets/edit-icon.png).

   De pagina Taken bewerken wordt weergegeven. De items die u bewerkt, worden in de linkerbovenhoek van de pagina weergegeven.

1. Ga naar de **sectie van Taken**.
1. Voer een van de volgende handelingen uit om toewijzingen toe te voegen of te verwijderen:

   >[!IMPORTANT]
   >
   >Het verwijderen van toewijzingen kan van invloed zijn op de taakuren en toewijzingspercentages. Voor meer informatie, zie de sectie [ hoe het verwijderen van toegewezen taakuren en toewijzingspercentages ](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in dit artikel beïnvloedt.

   * Een nieuwe ontvanger toevoegen:

      1. In de **sectie van Taken**, uitgezochte **Ontvanger**.

         Informatie die algemeen is voor alle geselecteerde taken, wordt weergegeven. Bijvoorbeeld, als de zelfde gebruiker aan alle taken wordt toegewezen, toont die gebruiker in de **Assignee** kolom. Als de informatie niet over de geselecteerde taken gemeenschappelijk is, wordt geen informatie weergegeven.

      1. Begin de naam van een gebruiker, een rol, of een team te typen, dan het te selecteren wanneer het in de lijst toont. De toewijzing wordt toegevoegd en vervangt niet de huidige toewijzingen voor de geselecteerde taken.


     >[!TIP]
     >
     > * U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
     >   
     > * Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt. De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [ toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
     >   
     >     * Wijs het werkitem opnieuw toe aan actieve bronnen.
     >     * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.


   * Afzonderlijke toewijzingen verwijderen:

      1. Klik het **pictogram van X** naast de naam van de ontvanger die u wilt verwijderen als de bestemmingsvertoningen in de lijst van Taken.

         of

         (Voorwaardelijk) als de ontvanger die u wilt verwijderen niet in de sectie van Taken toont omdat de ontvanger aan slechts enkele taken wordt toegewezen die u hebt geselecteerd, **verwijdert Ontvanger** en begint de naam van de ontvanger te typen die u wilt verwijderen, dan klikken de naam wanneer het in de drop-down lijst verschijnt.

   * Alle bestaande toewijzingen verwijderen:

      1. Klik **verwijderen Alle Bestaande Toewijzers**, dan klik **ja, schrap Alle Toewijzers**.

         Hierdoor worden niet alleen algemene toewijzingen (toewijzingen die in het dialoogvenster Bewerken worden weergegeven), maar ook alle toewijzingen voor alle geselecteerde taken verwijderd.

     Het verwijderen van gebruikers uit taken kan taakuren en toewijzingspercentages beïnvloeden.

     Voor meer informatie, zie [ Overzicht van het wijzigen van taaktaken ](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Optioneel) Wijzig een of meer van de volgende opties voor toewijzingen:

   * (Voorwaardelijk) **toewijzing % of Uren**: specificeer een nieuw toewijzingspercentage of uren.

     >[!NOTE]
     >
     >Deze optie kan slechts worden gewijzigd als het Type van Duur het zelfde over alle taken is die worden uitgegeven. Wanneer het Type van Duur het Getoonde Werk of de Bediende van de inspanning wordt berekend kunt u de Toewijzing % bijwerken. Wanneer het Type van Duur Eenvoudig is kunt u de Uren bijwerken. Voor informatie over het Type van Duur, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Als het veld leeg is, betekent dit dat de waarde voor alle taken anders is. U kunt de waarde echter wel wijzigen.

   * **Eigenaar van de Taak**: Selecteer deze optie om de toegewezen eigenaar van de taak voor alle taken te maken die worden uitgegeven.
   * **Rol van de Ontvanger**: Selecteer een rol van de drop-down lijst. Als deze optie niet is geselecteerd, selecteert Adobe Workfront automatisch de primaire rol van de gebruiker.

1. Klik **sparen Veranderingen.**
