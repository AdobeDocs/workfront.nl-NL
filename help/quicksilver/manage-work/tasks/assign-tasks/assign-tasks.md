---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Taken toewijzen
description: U kunt taken aan gebruikers, rollen, of teams toewijzen om erop te wijzen wie voor de voltooiing van de taken verantwoordelijk is. U kunt een taak aan meer dan één middel tegelijkertijd toewijzen.
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '2479'
ht-degree: 0%

---

# Taken toewijzen

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<div class="preview">

De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Dezelfde functies zijn ook beschikbaar in de productieomgeving voor alle klanten vanaf een week na de release Preview.

Voor meer informatie, zie [&#x200B; Tweede Kwartaal 2026 releaseoverzicht &#x200B;](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).

</div>

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

Het aantal gebruikers dat aan een taak en het programma van de taakeigenaar wordt toegewezen kan de geplande data van een taak wijzigen die in het veranderen van de chronologie van het project resulteert. Voor informatie over het effect van het toewijzen van veelvoudige gebruikers aan een taak, zie [&#x200B; Overzicht van het wijzigen van taaktaken &#x200B;](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Naast dit artikel raden we u aan de volgende artikelen te lezen voor meer informatie over het toewijzen van taken:

* [&#x200B; Overzicht van het wijzigen van taaktaken &#x200B;](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [&#x200B; Slim overzicht van taken &#x200B;](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [&#x200B; maak slimme taken &#x200B;](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [&#x200B; creeer geavanceerde taken &#x200B;](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [&#x200B; wijzigt veelvoudige gebruikerstoewijzingen in een taaklijst &#x200B;](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [&#x200B; geef taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uit
* [&#x200B; Plan een projectoverzicht &#x200B;](../../../manage-work/projects/planning-a-project/plan-project.md)
* [&#x200B; Overzicht van de taak Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [&#x200B; plaats het project Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [&#x200B; vorm systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Overzicht van het toewijzen van werk in de werklastverdeler](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p> </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td>
   <td>Contribute of hoger machtigingen voor de taak</td>
  </tr>
 </tbody>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers

Overweeg het volgende wanneer het toewijzen van veelvoudige middelen aan een het werkpunt:

* Gebruikers kunnen meer dan één taakrol aan hun profiel koppelen. Voor informatie over het associëren van gebruikers met baanrollen, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

* Als u meerdere gebruikers aan een taak of uitgave toewijst, wordt de eerste gebruiker die u selecteert, automatisch aangewezen als de eigenaar van de taak of uitgave.
Voor instructies bij het veranderen van dit, zie de informatie over de Primaire optie van het Merk in het artikel [&#x200B; Geavanceerde taken &#x200B;](create-advanced-assignments.md) creëren.

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
   <p>Voor informatie over de primaire rol van een gebruiker en andere rollen, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"> het profiel van een gebruiker </a> uitgeven.</p>
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
1. Klik **toewijzen aan** in het **3&rbrace; gebied van Taken &lbrace;in de kopbal van de taak**

   of

   Klik op de naam van de toewijzingen als de taak al is toegewezen.

   ![&#x200B; Taken &#x200B;](assets/assignments-from-task-header-0825.png)

1. Voer een van de volgende handelingen uit:

   * Typ de naam van een gebruiker, taakrol of team die u wilt toewijzen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.

     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [&#x200B; toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   * (Voorwaardelijk) klik één van de namen in de **Gebruikers en teams** of **de rollen van de Baan** lijsten wanneer zij tonen. Voor meer informatie, zie [&#x200B; Slim toewijzingsoverzicht &#x200B;](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     U kunt de naam typen van een gebruiker, team of taakrol die u wilt toewijzen aan de taak, en deze vervolgens selecteren wanneer deze wordt weergegeven in de lijst.

   * Klik **Geavanceerd**.

     Voor informatie over hoe te om geavanceerde taken te maken, zie [&#x200B; Geavanceerde taken &#x200B;](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

1. Klik **sparen**.
1. (Facultatief en voorwaardelijk) klik het **pictogram van X** naast de naam van de taak in het juiste paneel van de taak om een taak te verwijderen, als u **Geavanceerd** klikte.

## Een taak in een lijst toewijzen bij inlinebewerking

U kunt taken toewijzen in een lijst of rapport wanneer een van de toewijzingsvelden zichtbaar is in de lijstweergave. Dit is een snellere manier om taken toe te wijzen. In dit artikel wordt beschreven hoe u toewijzingen voor één taak in een lijst kunt wijzigen. Voor informatie over het wijzigen van veelvoudige taken voor veelvoudige taken in een lijst, zie [&#x200B; veelvoudige gebruikerstoewijzingen in een taaklijst &#x200B;](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md) wijzigen.

Afhankelijk van welk veld zichtbaar is in de weergave, kunt u de volgende entiteiten aan de taak toewijzen:

| Veld | Toegewezen entiteiten |
|---|---|
| **toewijzen aan** | Eén gebruiker toewijzen |
| **Toegewezen** | Eén gebruiker toewijzen |
| **Taken** | Gebruikers, taakrollen of teams toewijzen |

Taken in een lijst toewijzen:

1. Ga naar een lijst met taken waarvoor de velden Toegewezen aan, Toegewezen of Toegewezen in de weergave staan.
1. (Facultatief) klik **Autosave** drop-down menu en selecteer van de volgende opties:

   | Optie | Optiebeschrijving |
   |---|---|
   | Automatisch opslaan | Wijzigingen die u aanbrengt in de taken worden automatisch opgeslagen en u kunt ze niet terugzetten |
   | Handmatig opslaan | U moet uw wijzigingen handmatig opslaan. U kunt uw wijzigingen herstellen voordat u ze opslaat. |
   | Tijdlijnplanning | U moet uw wijzigingen handmatig opslaan. U kunt uw wijzigingen herstellen voordat u ze opslaat. Het opslaan van uw wijzigingen en alle projectafhankelijkheden is sneller dan wanneer u Handmatig opslaan selecteert. |

   Voor meer informatie over besparingstaken aangezien u hen in een lijst uitgeeft, zie [&#x200B; taken in een lijst &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) uitgeven.

1. Voer een van de volgende handelingen uit om taken toe te wijzen:

   * Klik binnen **Toegewezen aan** of **toegewezen** gebieden en begin de naam van een actieve gebruiker te typen die u aan de taak wilt toewijzen, dan het te klikken wanneer het in de lijst toont.
   * Klik binnen het **gebied van Taken** en begin de naam van een actieve gebruiker, baanrol, of team te typen die u aan de taak wilt toewijzen, dan het klikken wanneer het in de lijst toont.

     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. (Voorwaardelijk) op het gebied van Taken, klik **Geavanceerd** bij de bodem van de lijst, of het **pictogram van Mensen** ![&#x200B; het pictogram van Mensen &#x200B;](assets/teams.png) in de hoger-juiste hoek van de toewijzingsdoos, om **Geavanceerde de doos van Toewijzingen** te openen en geavanceerde taken tot stand te brengen.

   Voor meer informatie, zie [&#x200B; Geavanceerde taken &#x200B;](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

   >[!TIP]
   >
   >U kunt geen geavanceerde toewijzingen maken vanuit de velden Toegewezen aan of Toegewezen.

1. Nadat u de toewijzingen aan de taak hebt toegevoegd, drukt u op Enter of klikt u ergens op de pagina om de wijzigingen op te slaan als u Automatisch opslaan hebt geselecteerd. Anders, klik **sparen**.

## Meerdere taken bulksgewijs vanuit een lijst toewijzen

Het toewijzen van meerdere taken in bulk vanuit een lijst hangt af van de omgeving die u kiest.

### Meerdere taken bulksgewijs vanuit een lijst in de productieomgeving toewijzen

1. Ga naar een lijst van taken die u in bulk wilt toewijzen.
1. (Voorwaardelijk) zorg ervoor dat de **optie Autosave** wordt geselecteerd als u op een lijst van taken onder een project bent.

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig in een project opslaat.

1. Selecteer verschillende taken in de takenlijst.
1. Klik **uitgeven**.

   Het **geeft de dialoogvakje van Taken** uit opent in de nieuwe ervaring.

1. U kunt de taken blijven toewijzen met de nieuwe ervaring.

   Voor meer informatie, zie de sectie [&#x200B; veelvoudige taken in bulk van een lijst in de nieuwe ervaring &#x200B;](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) in dit artikel toewijzen.

1. (Facultatief) klik **Schakelaar terug naar oude ervaring** bij de bodem van **uitgeeft de doos van Taken** om de oude ervaring te openen.

1. (Voorwaardelijk) Gebruikend de oude ervaring, in het **gebied van Taken**, selecteer de **Ontvanger** doos, dan begin het typen van de naam van een gebruiker, baanrol, of team dat u aan alle taken wilt toewijzen.

   >[!IMPORTANT]
   >
   >Als om het even welke taken reeds wordt toegewezen, worden de middelen u hier op wijst toegevoegd aan de taken in plaats van het vervangen van de bestaande middelen op de taken.

1. (Facultatief) selecteer het radioknoop in de **kolom van de Eigenaar van de Taak** om op te geven welk middel de primaire ontvanger of de Eigenaar van de taak is, wanneer u meer dan één middel aan de taak toewijst. Dit is niet beschikbaar voor teams.
1. (Voorwaardelijk) specificeer **Toewijzing %** voor elk middel dat aan de taak wordt toegewezen als alle taken u selecteerde een Type van Duur van Gedreven of Berekende Toewijzing hebben. Dit wijst op hoeveel van hun tijd deze middelen aan de voltooiing van de taak zouden moeten uitgeven. Dit is alleen beschikbaar voor gebruikers en taakrollen.

   of

   Specificeer de hoeveelheid **Uren** voor elk middel dat aan de taak wordt toegewezen als alle taken u selecteerde een Type van Duur van Eenvoudig hebben. Het totaal van alle uren voor alle middelen zou het aantal Geplande Uren voor de taak moeten evenaren.

   >[!IMPORTANT]
   >
   >U kunt niet het toewijzingspercentage of het aantal uren per middel specificeren als de taken u selecteerde verschillende Types van Duur of van de taken hebben u selecteerde verschillende Types van Duur.

   Voor informatie over het Type van Duur op taken, zie [&#x200B; Overzicht van het Type van Duur van de Taak en van de Duur &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Facultatief) selecteer een rol die de gebruiker op de taak van **zou moeten vervullen kies een rol** drop-down menu in de **3&rbrace; kolom van de Rol van de Ontvanger &lbrace;wanneer u gebruikers aan taken toewijst.** Als u geen rol selecteert, selecteert Workfront automatisch de Primaire Rol van de gebruiker.

1. (Optioneel) Als u bestaande toewijzingen uit alle taken wilt verwijderen, voert u een van de volgende handelingen uit:

   1. Begin het typen van de naam van een gebruiker, een rol, of een team u uit de taak wilt verwijderen, dan het selecteren wanneer het op de lijst verschijnt en **verwijdert Assignee** klikken om meer toegewezen te verwijderen.
   1. Klik **verwijderen Alle Bestaande Assignees** om alle toegewezen uit alle geselecteerde taken te verwijderen.

1. Klik **sparen Veranderingen**.
1. (Facultatief en voorwaardelijk) wanneer de Toegewezen aan of de gebieden van Taken in uw lijst van taken tonen, binnen één van deze kolommen voor een taak klikken, dan klik het **X pictogram** naast de naam van een toegewezen om het uit de taak te verwijderen.


#### Meerdere taken bulksgewijs vanuit een lijst in de nieuwe ervaring toewijzen

1. Ga naar een lijst van taken die u in bulk wilt toewijzen.
1. (Voorwaardelijk) zorg ervoor dat de **optie Autosave** wordt geselecteerd als u op een lijst van taken onder een project bent.

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig in een project opslaat.

1. Selecteer verschillende taken in de takenlijst.
1. Klik **uitgeven**.

   Het **geeft de dialoogvakje van Taken** uit opent.

1. In het **gebied van Taken**, begin de naam van gebruikers, teams, of rollen in het **Gebieden de mensen van het Onderzoek, rollen, of teams** gebied, dan klikken hen wanneer zij in de lijst tonen

   of

   Klik **toewijzen aan me** om het aan zich toe te wijzen.

   >[!IMPORTANT]
   >
   >Als om het even welke taken reeds wordt toegewezen, worden de middelen u hier op wijst toegevoegd aan de taken in plaats van het vervangen van de bestaande middelen op de taken.

1. Klik binnen het **gebied van het Type van Duur 0&rbrace; &lbrace;en kies een Type van Duur.**

   Voor informatie over het Type van Duur op taken, zie [&#x200B; Overzicht van het Type van Duur van de Taak en van de Duur &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Voorwaardelijk) afhankelijk van welk **Type van Duur** u selecteerde, werk de volgende gebieden bij:

   * Duur
   * Geplande uren

     Voor meer informatie, zie [&#x200B; taken &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

1. (Optioneel) Als u bestaande toewijzingen uit alle taken wilt verwijderen, klikt u op **x** naast hun naam in het **gebied van het Onderzoek mensen, rollen, of teams**.

1. Klik **sparen**.
1. (Facultatief en voorwaardelijk) wanneer **aan** of de **3&rbrace; gebieden van Taken &lbrace;in uw lijst van taken wordt toegewezen, klik binnen één van deze kolommen voor een taak, dan klik het** X pictogram **naast de naam van een ontvanger om het uit de taak te verwijderen.**

<div class="preview">

### Meerdere taken bulksgewijs vanuit een lijst in de voorvertoningsomgeving toewijzen

1. Ga naar een lijst van taken die u in bulk wilt toewijzen.
1. (Voorwaardelijk) zorg ervoor dat de **optie Autosave** wordt geselecteerd als u op een lijst van taken onder een project bent.

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig in een project opslaat.

1. Selecteer verschillende taken in de takenlijst.
1. Klik **uitgeven**.

   Het **geeft de doos van Taken** uit opent.

1. In het **gebied van Taken**, begin de naam van gebruikers, teams, of rollen in het **Gebieden de mensen van het Onderzoek, rollen, of teams** gebied, dan klikken hen wanneer zij in de lijst tonen

   >[!IMPORTANT]
   >
   >Als om het even welke taken reeds wordt toegewezen, worden de middelen u hier op wijst toegevoegd aan de taken in plaats van het vervangen van de bestaande middelen op de taken.

1. Geef de volgende velden op voor de geselecteerde taken:

   * Beweeg over de toewijzingsnaam, dan klik **Primair maken** om erop te wijzen welke ontvanger de eigenaar van de taak is.
   * **Type van Duur**

     Voor informatie over het Type van Duur op taken, zie [&#x200B; Overzicht van het Type van Duur van de Taak en van de Duur &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duur**
   * **Geplande Uren**

     Voor meer informatie, zie [&#x200B; taken &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

1. (Optioneel) Als u bestaande toewijzingen uit alle taken wilt verwijderen, klikt u op **x** naast hun naam in het **gebied van het Onderzoek mensen, rollen, of teams**.

1. Klik **sparen**.
1. (Facultatief en voorwaardelijk) wanneer **aan** of de **3&rbrace; gebieden van Taken &lbrace;in uw lijst van taken wordt toegewezen, klik binnen één van deze kolommen voor een taak, dan klik het** X pictogram **naast de naam van een ontvanger om het uit de taak te verwijderen.**

</div>

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


