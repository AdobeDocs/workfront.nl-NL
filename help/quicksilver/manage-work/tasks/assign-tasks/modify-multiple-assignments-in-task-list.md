---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Meerdere gebruikerstoewijzingen in een takenlijst wijzigen
description: Wanneer het beheren van taaktaken, kunt u hen voor veelvoudige taken tegelijkertijd wijzigen door de bulkbewerkingseigenschap in een lijst van taken te gebruiken.
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# Meerdere gebruikerstoewijzingen in een takenlijst wijzigen

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Wanneer het beheren van taaktaken, kunt u hen voor veelvoudige taken tegelijkertijd wijzigen door de bulkbewerkingseigenschap in een lijst van taken te gebruiken.

In dit artikel wordt verwezen naar het wijzigen van meerdere gebruikerstoewijzingen voor meerdere taken in een takenlijst. Zie ook de volgende artikelen voor het wijzigen van toewijzingen voor meerdere taken op andere gebieden:

* Voor informatie over het wijzigen van taken op veelvoudige taken in het Plannende gebied, zie [Meerdere gebruikerstoewijzingen wijzigen voor taken in de planningsgebieden](../../../resource-mgmt/resource-scheduling/modify-multipl-assignments-scheduling-areas.md).
* Voor informatie over het toewijzen van taken met behulp van Workload Balancer raadpleegt u [Overzicht van het toewijzen van werk in de werklastverdeler](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Voor informatie over het toewijzen van een taak aan één middel in een lijst, zie [Taken toewijzen](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor taken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
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

   Voor informatie over het maken van een filter raadpleegt u [Filters maken of bewerken](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Als u op een rol wilt filteren, selecteert u **Toewijzingsrollen** en klik vervolgens op **ID**.

   >[!TIP]
   >
   >Gebruik de **Toegewezen aan** veld. Dit vindt slechts de Primaire Eigenaar voor de taak in plaats van om het even welke rollen die aan hen konden worden toegewezen.

   of

   Als u voor een gebruiker wilt filteren, selecteert u **gebruikers van de toewijzing,** klik vervolgens op **ID.**

   >[!TIP]
   >
   >Gebruik de **Toegewezen aan** veld. Hiermee vindt u alleen de primaire eigenaar voor de taak in plaats van de gebruikers die aan hen kunnen worden toegewezen.

1. Selecteer de taken waarvoor u toewijzingen wilt wijzigen en klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png).

   De pagina Taken bewerken wordt weergegeven. De items die u bewerkt, worden in de linkerbovenhoek van de pagina weergegeven.

1. Ga naar de **Toewijzingen** sectie.
1. Voer een van de volgende handelingen uit om toewijzingen toe te voegen of te verwijderen:

   >[!IMPORTANT]
   >
   >Het verwijderen van toewijzingen kan van invloed zijn op de taakuren en toewijzingspercentages. Zie de sectie voor meer informatie [Hoe het verwijderen van toegewezen beïnvloedt taakuren en toewijzingspercentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in dit artikel.

   * Een nieuwe ontvanger toevoegen:

      1. In de **Toewijzingen** sectie, selecteert u **Geadresseerde**.

         Informatie die algemeen is voor alle geselecteerde taken, wordt weergegeven. Als bijvoorbeeld dezelfde gebruiker aan alle taken is toegewezen, wordt die gebruiker in het dialoogvenster **Geadresseerde** kolom. Als de informatie niet over de geselecteerde taken gemeenschappelijk is, wordt geen informatie weergegeven.

      1. Begin de naam van een gebruiker, een rol, of een team te typen, dan het te selecteren wanneer het in de lijst toont. De toewijzing wordt toegevoegd en vervangt niet de huidige toewijzingen voor de geselecteerde taken.
      >[!TIP]
      >
      > * U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
      >   
      > * Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.

         > 
         >   Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
         >   
         >     * Wijs het werkitem opnieuw toe aan actieve bronnen.
         >     * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.



   * Afzonderlijke toewijzingen verwijderen:

      1. Klik op de knop **X-pictogram** naast de naam van de toegewezen persoon die u wilt verwijderen als de toegewezen persoon wordt weergegeven in de lijst Toewijzingen.

         of

         (Voorwaardelijk) Als de toegewezen persoon die u wilt verwijderen niet in de sectie Toewijzingen wordt weergegeven omdat de toegewezen persoon aan slechts enkele van de geselecteerde taken is toegewezen, klikt u op **Toegewezen verwijderen** en typ de naam van de toegewezen persoon die u wilt verwijderen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
   * Alle bestaande toewijzingen verwijderen:

      1. Klikken **Alle bestaande toewijzingen verwijderen** en klik vervolgens op **Ja, alle toewijzingen verwijderen**.

         Hierdoor worden niet alleen algemene toewijzingen (toewijzingen die in het dialoogvenster Bewerken worden weergegeven), maar ook alle toewijzingen voor alle geselecteerde taken verwijderd.
      Het verwijderen van gebruikers uit taken kan taakuren en toewijzingspercentages beïnvloeden.

      Zie voor meer informatie [Overzicht van het wijzigen van taaktaken](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. (Optioneel) Wijzig een of meer van de volgende opties voor toewijzingen:

   * (Voorwaardelijk) **Toewijzing % of uren**: Geef een nieuw toewijzingspercentage of nieuwe uren op.

      >[!NOTE]
      >
      >Deze optie kan slechts worden gewijzigd als het Type van Duur het zelfde over alle taken is die worden uitgegeven. Wanneer het Type van Duur het Getoonde Werk of de Bediende van de inspanning wordt berekend kunt u de Toewijzing % bijwerken. Wanneer het Type van Duur Eenvoudig is kunt u de Uren bijwerken. Voor informatie over het Type van Duur, zie [Overzicht van het Type van Duur en van de Duur van de Taak](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      Als het veld leeg is, betekent dit dat de waarde verschillend is voor alle taken. u kunt deze echter nog wijzigen .

   * **Taakeigenaar**: Selecteer deze optie als u de toegewezen eigenaar van de taak wilt maken voor alle taken die worden bewerkt.
   * **Rol van de gemachtigde**: Selecteer een rol in de vervolgkeuzelijst. Als deze optie niet is geselecteerd, selecteert Adobe Workfront automatisch de primaire rol van de gebruiker.

1. Klikken **Wijzigingen opslaan.**
