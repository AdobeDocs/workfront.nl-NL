---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Taken toewijzen
description: U kunt taken aan gebruikers, rollen, of teams toewijzen om erop te wijzen wie voor de voltooiing van de taken verantwoordelijk is. U kunt een taak aan meer dan één middel tegelijkertijd toewijzen.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 13a1d9ebee75c468ce55794db130f01ba658f125
workflow-type: tm+mt
source-wordcount: '1953'
ht-degree: 0%

---

# Taken toewijzen

{{highlighted-preview}}

U kunt taken aan gebruikers, baanrollen, of teams toewijzen om erop te wijzen wie voor de voltooiing van de taken verantwoordelijk is. U kunt een taak aan meer dan één middel tegelijkertijd toewijzen.

>[!TIP]
>
>U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
>
>Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
>
>* Wijs het werkitem opnieuw toe aan actieve bronnen.
>* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.
>

Het aantal gebruikers dat aan een taak en het programma van de taakeigenaar wordt toegewezen kan de geplande data van een taak wijzigen die in het veranderen van de chronologie van het project resulteert. Voor informatie over het effect van het toewijzen van meerdere gebruikers aan een taak raadpleegt u [Overzicht van het wijzigen van taaktaken](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Naast dit artikel raden we u aan de volgende artikelen te lezen voor meer informatie over het toewijzen van taken:

* [Overzicht van het wijzigen van taaktaken](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Overzicht van slimme toewijzingen](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Slimme toewijzingen maken](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Geavanceerde toewijzingen maken](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Meerdere gebruikerstoewijzingen in een takenlijst wijzigen](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Een projectoverzicht plannen](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Overzicht van de geplande voltooiing van de taak](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Geplande afsluitdatum van project instellen](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Overzicht van het toewijzen van werk in de werklastverdeler](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Toegangsvereisten

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor taken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers

Overweeg het volgende wanneer het toewijzen van veelvoudige middelen aan een het werkpunt:

* Gebruikers kunnen meer dan één taakrol aan hun profiel koppelen. Voor informatie over het associëren van gebruikers met baanrollen, zie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Als u meerdere gebruikers aan een taak of uitgave toewijst, wordt de eerste gebruiker die u selecteert, automatisch aangewezen als de eigenaar van de taak of uitgave.
Raadpleeg de informatie over de optie Primair maken in het artikel voor instructies over het wijzigen van deze instelling [Geavanceerde toewijzingen maken](create-advanced-assignments.md).

* Een team kan geen primaire ontvanger zijn voor een taak of kwestie. Alleen een gebruiker of een taakrol kan worden aangewezen als primair op een taak of kwestie.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* De taken en de kwesties op een project zouden eerst aan één of meerdere teams of baanrollen kunnen worden toegewezen. Wanneer het project klaar is te beginnen, zouden zij ook aan gebruikers kunnen moeten worden toegewezen:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Teams</td>
   <td>Als u een taak aan een team toewijst en u ook een gebruiker toewijst, blijft de taak toegewezen aan het team en aan de gebruiker, zelfs als de gebruiker geen lid van het team is.</td>
  </tr>
  <tr>
   <td>Functies</td>
   <td><p>Als u een taak of een kwestie aan één of veelvoudige rollen toewijst en dan ook een gebruiker toewijst, besluit welke baanrol aan de extra gebruiker (als om het even welk) te associëren volgens de volgende regels:</p>
     <ul>
      <li>Als er slechts één toegewezen baanrol is en het de primaire rol van de gebruiker (die in hun profiel wordt gevormd) aanpast, wordt de taak of de kwestie toegewezen slechts aan die gebruiker.</li>
      <li>Als de veelvoudige rollen worden toegewezen en minstens één van hen één van de andere rollen van de gebruiker aanpast, wordt de taak of de kwestie toegewezen aan de gebruiker (de rol wordt willekeurig geselecteerd als er veelvoudige gelijken zijn), samen met om het even welke extra rollen die worden toegewezen</li>
      <li>Als minstens één baanrol wordt toegewezen en er geen gelijken aan de de baanrollen van de gebruiker zijn, wordt de taak of de kwestie toegewezen aan zowel de rol of de rollen als aan de gebruiker.</li>
     </ul>
   <p>Voor informatie over de primaire rol van een gebruiker en andere rollen, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Gebruikersprofiel bewerken</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Eén taak toewijzen

1. Ga naar een taak die u wilt toewijzen.
1. Klikken **Toewijzen aan** in de **Toewijzingen** in de koptekst van de taak of uitgave.

   of

   Klik op de naam van de toewijzingen als de taak of uitgave al is toegewezen.

   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. Voer een van de volgende handelingen uit:

   * Typ de naam van een gebruiker, rol of team die u wilt toewijzen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.


     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Zie voor meer informatie [Toegang verlenen aan gebruikers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">Wanneer u een taakroltoewijzing toevoegt, kunt u zoeken naar de taakrol of -locatie. Selecteer Systeem/StandaardRol van de Baan om het standaardfactureringspercentage voor de taak te gebruiken, of een Rol van de Kaart van het Tarief te selecteren om het facturerings tarief van de tariefkaart te gebruiken. Zie voor meer informatie over tariefkaarten [Creditcards beheren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Voorwaardelijk) Klik op een van de namen in het dialoogvenster **Voorgestelde toewijzingen** als deze lijst wordt weergegeven. Zie voor meer informatie [Overzicht van slimme toewijzingen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * Klikken **Geavanceerd**

     Voor informatie over hoe te om geavanceerde taken te maken, zie [Geavanceerde toewijzingen maken](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Klikken **Opslaan**.
1. (Optioneel en voorwaardelijk) Klik op de knop **X-pictogram** naast de naam van de toewijzing in het rechtervenster van de taak om een toewijzing te verwijderen, als u klikte **Geavanceerd**.

## Een taak in een lijst toewijzen

U kunt taken toewijzen in een lijst of rapport wanneer een van de toewijzingsvelden zichtbaar is in de lijstweergave. Dit is een snellere manier om taken toe te wijzen. In dit artikel wordt beschreven hoe u toewijzingen voor één taak in een lijst kunt wijzigen. Voor informatie over het wijzigen van veelvoudige taken voor veelvoudige taken in een lijst, zie [Meerdere gebruikerstoewijzingen in een takenlijst wijzigen](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Afhankelijk van welk veld zichtbaar is in de weergave, kunt u de volgende entiteiten aan de taak toewijzen:

| Veld | Toegewezen entiteiten |
|---|---|
| **Toewijzen aan** | Eén gebruiker toewijzen |
| **Toegewezen** | Eén gebruiker toewijzen |
| **Toewijzingen** | Gebruikers, taakrollen of teams toewijzen |

Taken in een lijst toewijzen:

1. Ga naar een lijst met taken waarvoor de velden Toegewezen aan, Toegewezen of Toegewezen in de weergave staan.
1. (Optioneel) Klik op de knop **Automatisch opslaan** vervolgkeuzelijst en selecteer een van de volgende opties:

   | Optie | Optiebeschrijving |
   |---|---| 
   | Automatisch opslaan | Wijzigingen die u aanbrengt in de taken worden automatisch opgeslagen en u kunt ze niet terugzetten |
   | Handmatig opslaan | U moet uw wijzigingen handmatig opslaan. U kunt uw wijzigingen herstellen voordat u ze opslaat. |
   | Tijdlijnplanning | U moet uw wijzigingen handmatig opslaan. U kunt uw wijzigingen herstellen voordat u ze opslaat. Het opslaan van uw wijzigingen en alle projectafhankelijkheden is sneller dan wanneer u Handmatig opslaan selecteert. |

   Voor meer informatie over het opslaan van taken aangezien u hen in een lijst uitgeeft, zie [Taken in een lijst bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Voer een van de volgende handelingen uit om taken toe te wijzen:

   * Klik in het dialoogvenster **Toegewezen aan** of **Toegewezen** en typ de naam van een actieve gebruiker die u aan de taak wilt toewijzen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de lijst.
   * Klik in het dialoogvenster **Toewijzingen** veld en typ de naam van een actieve gebruiker, taakrol of team die u aan de taak wilt toewijzen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.

     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Zie voor meer informatie [Toegang verlenen aan gebruikers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">Wanneer u een taakroltoewijzing toevoegt, kunt u zoeken naar de taakrol of -locatie. Selecteer Systeem/StandaardRol van de Baan om het standaardfactureringspercentage voor de taak te gebruiken, of een Rol van de Kaart van het Tarief te selecteren om het facturerings tarief van de tariefkaart te gebruiken. Zie voor meer informatie over tariefkaarten [Creditcards beheren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Voorwaardelijk) Indien zichtbaar in het dialoogvenster **Toewijzingen** veld, klikt u op de knop **Mensen** in de rechterbovenhoek van het toewijzingsvak om het dialoogvenster **Geavanceerde toewijzingen** en maak geavanceerde toewijzingen.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Zie voor meer informatie [Geavanceerde toewijzingen maken](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >U kunt geen geavanceerde toewijzingen maken vanuit de velden Toegewezen aan of Toegewezen.

1. Nadat u de toewijzingen aan de taak hebt toegevoegd, drukt u op Enter of klikt u ergens op de pagina om de wijzigingen op te slaan als u Automatisch opslaan hebt geselecteerd. Anders klikt u op **Opslaan**.

## Meerdere taken aan een gebruiker toewijzen

1. Ga naar een lijst van taken die u in bulk wilt toewijzen.
1. (Voorwaardelijk) Zorg ervoor dat de **Automatisch opslaan** wordt geselecteerd als u op een lijst van taken onder een project bent.

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig in een project opslaat.

1. Selecteer verschillende taken in de takenlijst.
1. Klikken **Bewerken**.

   De **Taken bewerken** wordt geopend.

1. In de **Toewijzingen** gebied, selecteert u de **Geadresseerde** typt u vervolgens de naam van een gebruiker, taakrol of team die u aan alle taken wilt toewijzen.

   >[!IMPORTANT]
   >
   >Als om het even welke taken reeds wordt toegewezen, worden de middelen u hier op wijst toegevoegd aan de taken in plaats van het vervangen van de bestaande middelen op de taken.

1. (Optioneel) Selecteer het keuzerondje in het dialoogvenster **Taakeigenaar** kolom om aan te geven welke bron de primaire ontvanger of de eigenaar van de taak is, wanneer u meer dan één bron aan de taak toewijst. Dit is niet beschikbaar voor teams.
1. (Voorwaardelijk) Geef de **Toewijzing %** voor elke die bron aan de taak wordt toegewezen als alle taken u selecteerde een Type van Duur van Gedreven of Berekende Taak hebben. Dit wijst op hoeveel van hun tijd deze middelen aan de voltooiing van de taak zouden moeten uitgeven. Dit is alleen beschikbaar voor gebruikers en taakrollen.

   of

   Geef de hoeveelheid op van **Uren** voor elke die bron aan de taak wordt toegewezen als alle taken u selecteerde een Type van Duur van Eenvoudig hebben. Het totaal van alle uren voor alle middelen zou het aantal Geplande Uren voor de taak moeten evenaren.

   >[!IMPORTANT]
   >
   >U kunt niet het toewijzingspercentage of het aantal uren per middel specificeren als de taken u selecteerde verschillende Types van Duur of van de taken hebben u selecteerde verschillende Types van Duur.

   Voor informatie over het Type van Duur op taken, zie [Overzicht van het Type van Duur en van de Duur van de Taak](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optioneel) Selecteer een rol die de gebruiker op de taak moet uitvoeren vanuit de **Een rol kiezen** vervolgkeuzemenu in het dialoogvenster **Rol van de gemachtigde** wanneer u gebruikers aan taken toewijst. Als u geen rol selecteert, selecteert Workfront automatisch de Primaire Rol van de gebruiker.

1. (Optioneel) Als u bestaande toewijzingen uit alle taken wilt verwijderen, voert u een van de volgende handelingen uit:

   1. Typ de naam van een gebruiker, rol of team die u uit de taak wilt verwijderen en selecteer deze vervolgens wanneer deze in de lijst wordt weergegeven en klik op **Toegewezen verwijderen** om meer toewijzingen te verwijderen.
   1. Klikken **Alle bestaande toewijzingen verwijderen** om alle toewijzingen te verwijderen uit alle geselecteerde taken.

1. Klikken **Wijzigingen opslaan**.
1. (Optioneel en voorwaardelijk) Wanneer de velden Toegewezen aan of Toewijzingen in uw lijst met taken worden weergegeven, klikt u in een van deze kolommen voor een taak en klikt u vervolgens op de knop **X-pictogram** naast de naam van een toegewezen persoon om deze uit de taak te verwijderen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


