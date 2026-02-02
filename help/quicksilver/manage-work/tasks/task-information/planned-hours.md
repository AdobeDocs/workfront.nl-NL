---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van geplande uren
description: De geplande uren verbonden aan een taak, een kwestie, of een project vertegenwoordigen de hoeveelheid tijd die voor de toegewezen gebruikers wordt vereist om de taak, de kwestie, of het project te voltooien.
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '2815'
ht-degree: 0%

---

# Overzicht van geplande uren

<!-- Audited: 01/2024 -->

De geplande uren verbonden aan een taak, een kwestie, of een project vertegenwoordigen de hoeveelheid tijd die voor de toegewezen gebruikers wordt vereist om de taak, de kwestie, of het project te voltooien.

## Overwegingen over geplande uren in Adobe Workfront

* De geplande uren worden hoofdzakelijk geassocieerd met het werkpunten (taken en kwesties) in Adobe Workfront. De geplande uren van de het werkpunten rollen tot de Geplande Uren van hun projecten.
* Standaard verdeelt Workfront de taak en geeft het geplande aantal uren gelijk uit aan alle dagen in de duur van de taak of uitgave.
* Wanneer gebruikers en rollen aan taken en kwesties worden toegewezen, worden de Geplande Uren van de taken en de kwesties geassocieerd met gebruiker of roltaken.
* U moet de waarde van Geplande Uren voor taken en kwesties bepalen als u de hulpmiddelen van het Beheer van Middelen in Workfront wilt gebruiken.
* U kunt de waarde van Geplande Uren op taken slechts voor sommige Types van Duur wijzigen.

  Voor meer informatie over het wijzigen van Geplande Uren op taken met betrekking tot het Type van Duur van de taken, zie de sectie [ Geplande die taak van de Update Uren op het Type van Duur ](#update-task-planned-hours-based-on-duration-type) in dit artikel worden gebaseerd.

* U kunt de waarde van Geplande Uren op kwesties op elk ogenblik wijzigen.
* U kunt de waarde van Geplande Uren van projecten of oudertaken niet wijzigen, aangezien zij een berekend totaal van alle Geplande Uren van al hun taken en subtaken zijn.
* Het beheren van gebruikerstoewijzingen met behulp van de hulpmiddelen van het middelbeheer zou het aantal Geplande Uren van taken, kwesties, en projecten, en dat van de taken verbonden aan het werkpunten kunnen veranderen.

## Geplande uren op taken versus geplande uren op projecten {#planned-hours-on-tasks-vs-planned-hours-on-projects}

De geplande uren van taken rollen tot de Geplande Uren van het project. De geplande uren van kwesties rollen niet altijd tot de Geplande Uren van het project.

Deze sectie beschrijft verschillen tussen de taak en project Geplande Uren. Het beschrijft ook waar u de kwestie Geplande Uren kunt bekijken die tot het project rollen.

### Geplande uren op taken {#planned-hours-on-tasks}

De geplande uren van een taak geven aan hoeveel tijd naar schatting nodig is om de taak daadwerkelijk uit te voeren. Standaard verdeelt Workfront het totale aantal geplande uren voor elke dag binnen de duur van elke taak gelijkmatig. De dagelijkse hoeveelheid geplande uren wordt de dagelijkse toewijzingen voor de taak. Als de taak aan veelvoudige middelen wordt toegewezen, wordt elk middel toegewezen een gelijke hoeveelheid dagelijkse uren, door gebrek.

Met de werklastbalans kunt u de dagelijkse toewijzingen wijzigen voor de gebruikers die aan de taken zijn toegewezen. Dit kan ook de Geplande Uren van de taak bijwerken wanneer het Type van taakDuur Eenvoudig is. Voor meer informatie, zie de &quot;Taak Geplande Uren van de Update wanneer het beheren van gebruikerstoewijzingen&quot;sectie in artikel [ gebruikerstoewijzingen in de Balancer van de Werkbelasting ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md) beheren.

Wanneer een taak subtaken bevat, is de Geplande Uren van de oudertaak de som alle Geplande Uren op om het even welke subtaken. U kunt de geplande uren van een bovenliggende taak niet bijwerken.

>[!NOTE]
>
>In tegenstelling tot Geplande Uren, zijn de Werkelijke Uren op een oudertaak uren die rechtstreeks op de oudertaak worden geregistreerd. Zij vertegenwoordigen geen som van de werkelijke uren van de kindertaken.\
>Voor meer informatie over Werkelijke Uren, zie [ Werkelijke Uren van de Mening ](../../../manage-work/tasks/task-information/actual-hours.md).

### Geplande uren op projecten {#planned-hours-on-projects}

U kunt de hoeveelheid geplande uren voor een project niet bewerken. De geplande uren op een project zijn een berekende som van alle Geplande Uren van alle taken op het project.

Of de kwesties in de berekening voor Geplande Uren inbegrepen zijn hangt van de plaats binnen het project af waar u Geplande Uren bekijkt. U kunt project Gepland Uren in de volgende plaatsen binnen een project bekijken:

* **de sectie van de Details van het Project en het Edit vakje van het Project**: Slechts worden de Geplande Uren voor de taken op het project in aanmerking genomen. De geplande uren voor de kwesties op het project worden niet in aanmerking genomen wanneer het bekijken van het totale aantal Geplande Uren voor het project in de sectie van de Details van het Project of het Edit vakje van het Project.

* **de Balancer van de Werkbelasting**: Slechts de Geplande Uren verbonden aan de taken zichtbaar in de vertoning van de Balancer van de Werklast in de Balancer van de Werkbelasting voor projecten. De dagelijkse toewijzingen van gebruikers kunnen de dagelijks geplande uren van het project in de Werklastbalans veranderen.
* **sectie van het Gebruik**: De Geplande Uren verbonden aan de gebruikers die aan de taken worden toegewezen en de kwesties op het project worden in aanmerking genomen wanneer het bekijken van het totale aantal Geplande Uren voor het project in de sectie van het Gebruik.
* **het paneel van de Toewijzing van de Rol** in de taaklijst: De Geplande Uren voor de taken en de kwesties op het project die aan een baanrol of een gebruiker worden toegewezen verbonden aan een vertoning van de baanrol op dit gebied. De geplande uren verbonden aan taken en kwesties die unassigned of toegewezen aan teams zijn tonen niet op dit gebied. Voor meer informatie, zie [ het project van de Mening Gepland Uren in het paneel van de Toewijzing van de Rol ](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md).

## Verdeling van geplande uren over de duur van een taak

Door gebrek, verdeelt Workfront de Geplande Uren gelijkmatig over de Duur van een taak, die een gelijk aantal Geplande Uren voor elke dag van de taak, volgens de beschikbaarheid van het projectprogramma toewijst.

Als een taak bijvoorbeeld om 16.00 uur moet beginnen en het schema op de eerste dag van de taak één uur over heeft, plaatst Workfront op de eerste dag van de taakduur één gepland uur en verdeelt de rest van de geplande uren gelijkelijk tussen de rest van de dagen in de taakduur.

>[!NOTE]
>
>De geplande uren per dag of de dagelijkse toewijzing is de toewijzing van de geplande uren voor elke dag tijdens de duur van de taak. Als de taak één taak heeft, dan vertegenwoordigt dit aantal de Geplande Uren per Dag per taak. Als de taak meerdere taken heeft, verschilt de geplande uren per dag per toewijzing van de taken van de geplande uren per dag. Er is geen visuele weergave in Workfront voor de geplande uren per dag per toewijzing, voor taken met meerdere toewijzingen.

## De waarden voor Geplande uren zoeken en begrijpen

U kunt de waarden voor Geplande uren in verschillende gebieden van Workfront vinden.

Het aantal geplande uren dat wordt weergegeven, is afkomstig van de werkitems in het project of wordt anders berekend, afhankelijk van het gebied waarin en het object waarin u deze weergeeft.

U kunt de geplande uren vinden in de volgende gebieden van Workfront:

* [ de sectie van Details van een project, een taak of een kwestie ](#the-details-section-of-a-project-task-or-issue)
* [ de Edit Taak of geeft doos van de Uitgave uit ](#the-edit-task-or-edit-issue-box)
* [ Rapporten ](#reports)
* [ de Balancer van de Werkbelasting ](#the-workload-balancer)
* [ de Planner van het Middel ](#the-resource-planner)
* [ het rapport van het Gebruik ](#the-utilization-report)
* [Het deelvenster Roltoewijzing](#the-role-allocation-panel)

### De sectie Details van een project, taak of kwestie {#the-details-section-of-a-project-task-or-issue}

![ Geplande Uren op de sectie van Details ](assets/planned-hours-on-details-for-project.png)

De geplande uren in de sectie van Details van een taak, een kwestie, of een project zijn de totale Geplande Uren verbonden aan het punt.

Voor meer informatie over project Geplande Uren, zie de [ Geplande Uren op taken vs. Geplande Uren op projecten ](#planned-hours-on-tasks-vs-planned-hours-on-projects) sectie in dit artikel.

### Het vak Taak bewerken of Uitgave bewerken {#the-edit-task-or-edit-issue-box}

![ geef Taakdoos ](assets/planned-hours-on-edit-task-box-nwe.png) uit

De geplande uren in het Edit vakje van een taak of een kwestie zijn de totale Geplande Uren van het respectieve punt.

Voor meer informatie over project Geplande Uren, zie de [ Geplande Uren op taken vs. Geplande Uren op projecten ](#planned-hours-on-tasks-vs-planned-hours-on-projects) sectie in dit artikel.

Voor taken, kunt u de hoeveelheid Geplande Uren slechts voor bepaalde Types van Duur uitgeven. Voor informatie, zie de [ taak Geplande die Uren van de Update op het Type van Duur ](#update-task-planned-hours-based-on-duration-type) sectie in dit artikel wordt gebaseerd.

U kunt de individuele toewijzing van Geplande Uren voor elke gebruiker of baanrol bekijken die aan de taak of kwestie in het gebied van Taken wordt toegewezen.

### Rapporten {#reports}

![ Geplande Uren op rapport ](assets/planned-hours-on-task-report.png)

U kunt het Geplande gebied van Uren in project toevoegen, taak, en geeft rapporten uit.

De kolom Geplande uren is standaard opgenomen in de standaardweergave van een takenlijst.

De geplande uren in een taak, kwestie, of projectrapport zijn de totale Geplande Uren van het respectieve punt zoals zij in de sectie van Details of Edit doos van de punten tonen.

Voor informatie over het creëren van rapporten, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

>[!NOTE]
>
>Als u een project (Financiële Gegevens) rapport creeert en het groepert door datum, zouden de Geplande Uren een deel van de Geplande Uren van het project afhankelijk van de chronologie van de taken op het project kunnen tonen. Door gebrek, verdeelt Workfront de Geplande Uren van taken gelijkelijk voor elke dag van de taakDuur. De geplande uren voor een bepaald tijdkader komen overeen met de gelijke verdeling die Workfront voor dat tijdkader heeft ingesteld in het projectrapport (Financial Data).

<!--
### The Scheduling areas  {#the-scheduling-areas}

![Task detail expanded in scheduler with Planned Hours and Adjusted Daily allocations](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

The Planned Hours for tasks and issues display in the Scheduling areas in the Planned Hours field.

You can view the daily allocation of Planned Hours for each user assigned to a task or an issue in the Scheduling areas.

The daily hour amount represents one of the following:

* the default amount equally distributed by Workfront for each day of the Duration of the tasks or issues
* the adjusted daily allocation managed by resource managers.

  For information about adjusting daily allocations in the Scheduling tools, see [Manage user allocations in the Scheduling areas](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
-->

### De werklastbalans {#the-workload-balancer}

![ Geplande Uren in de Balancer van de Werklast ](assets/planned-hours-on-wb-expanded-with-pti-info.png)

De volgende Geplande Uren voor taken, kwesties, en projecten tonen in de Balancer van de Werkbelasting rechts van de taak, de kwestie, of de projectnaam:

* Voor taken en kwesties, de Geplande Uren verbonden aan hen toont.
* Voor projecten, een totaal van Geplande Uren van de taken en kwesties zichtbaar op de het schermvertoning.

  >[!TIP]
  >
  >In Workload Balancer worden niet alle geplande uren van een project weergegeven als zichtbaar in het gebied met projectdetails.

U kunt de dagelijkse toewijzing van Geplande Uren voor elke gebruiker bekijken die aan een taak of een kwestie in de Balancer van de Werkbelasting wordt toegewezen.

De dagelijkse hoeveelheid geplande uren in uren is een van de volgende:

* het standaardbedrag gelijk verdeeld door Workfront voor elke dag van de Duur van de taken, de kwesties, of het project
* de aangepaste dagelijkse toewijzing die door de grondstoffenbeheerders wordt beheerd

  Voor informatie over het aanpassen van dagelijkse toewijzingen in de Balancer van de Werklast, zie [ gebruikerstoewijzingen in de Balancer van de Werklast beheren ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

### De bronnenplanner {#the-resource-planner}

![ Geplande Uren in de Planner van het Middel ](assets/planned-hours-on-all-objects-in-resource-planned-expanded.png)

In het venster Resource Planner worden de geplande uren voor projecten, taken en problemen weergegeven.

U kunt wekelijkse toewijzingen van Geplande Uren voor de gebruikers en baanrollen bekijken verbonden aan het werkpunten in de kolom PLN van de Planner van het Middel.

>[!TIP]
>
>Aanpassingen van dagelijkse toewijzingen in de werklastbalans beïnvloeden wekelijkse toewijzingen voor taken en problemen in de bronnenplanner.

Het aantal geplande uren voor elk object is afhankelijk van de weergave die u toepast op de bronnenplanner. Voor meer informatie, zie [ Overzicht van uren, FTE, en kosteninformatie in het Project en de meningen van de Rol van de Planner van het Middel ](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

De hoeveelheid geplande uren per week voor taken en uitgaven is een van de volgende:

* het wekelijkse standaardbedrag dat Workfront gelijkelijk over elke dag van de Duur van de taken of emissies uitkeert
* de aangepaste wekelijkse toewijzing die door middelmanagers in de Balancer van de Werklast wordt beheerd

  Voor informatie over het aanpassen van dagelijkse toewijzingen in de Balancer van de Werklast, zie [ gebruikerstoewijzingen in de Balancer van de Werklast beheren ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Het wekelijkse bedrag voor projecten, gebruikers en rollen wordt beïnvloed door de wekelijkse hoeveelheden geplande uren voor de taken en kwesties die ermee verband houden.

### Het gebruiksrapport {#the-utilization-report}

De geplande uren van het project zijn degenen verbonden aan de taken op elke taak en kwestie.

>[!IMPORTANT]
>
>Merk op dat de Geplande Uren in het rapport van het Gebruik met de taken en niet met de taken en kwesties zelf worden geassocieerd. De geplande uren in het gebruiksrapport komen niet altijd overeen met de geplande uren voor de taken en problemen van het project. De geplande uren komen echter wel overeen met de uren die zijn gekoppeld aan de taken en uitgaven.

U kunt de volgende typen geplande uren weergeven in het gebruiksrapport:

* de totale geplande uren van alle toewijzingen voor het project gedurende de totale looptijd van de opgenomen projecten
* het totale aantal geplande uren van alle toewijzingen alleen voor het opgegeven datumbereik (u kunt een afzonderlijke week of maand opgeven).

  Wanneer de dagelijkse toewijzing van de gebruiker voor uren is aangepast met behulp van Werklastbalans, kunnen de Geplande Uren voor een specifieke datumwaaier worden beïnvloed als de data die in het rapport van het Gebruik worden geselecteerd slechts een deel van de Duur van een taak of van de kwestie bevatten. Voor informatie over het aanpassen van dagelijkse toewijzingen voor gebruikers, zie [ gebruikerstoewijzingen in de Balancer van de Werklast beheren ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Voor meer informatie, zie [ informatie van het middelgebruik van de Mening ](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

### Het deelvenster Roltoewijzing

De geplande uren in het deelvenster Roltoewijzing geven het aantal geplande uren weer dat is gekoppeld aan elke taakrol die is toegewezen aan de taken of problemen van het project voor de totale duur van het project. Het aantal past de rol Geplande Uren van de Planner van het Middel aan.

>[!TIP]
>
>De geplande uren die aan gebruikers zijn gekoppeld, worden niet weergegeven in het deelvenster Roltoewijzing.

Voor meer informatie, zie [ roltoewijzing voor projecten en initiatieven in de Balancer van de Werkbelasting ](../../../scenario-planner/show-role-allocation-workload-balancer.md) tonen.

## Taak geplande uren bijwerken op basis van het type duur {#update-task-planned-hours-based-on-duration-type}

U kunt de totale geplande uren voor taken alleen bijwerken als de taken een bepaald Duur-type hebben.

De volgende scenario&#39;s bestaan:

* U kunt Geplande Uren voor taken slechts wijzigen wanneer het gebruiken van de Berekende Toewijzing of de Eenvoudige Types van Duur wanneer het uitgeven van een taak.

  Voor meer informatie over het Berekende Type van Duur van de Taak, zie [ Overzicht van het Type van Duur: Berekende Toewijzing ](../../../manage-work/tasks/taskdurtn/calculated-assignment.md).

  Voor meer informatie over het Eenvoudige Type van Duur, zie [ overzicht van het Type van Duur: Eenvoudig ](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

* U kunt taken die gepland zijn in de werklastbalans alleen bijwerken voor eenvoudige taken van het type Duur wanneer u de toewijzingen van gebruikers aan taken beheert. Voor informatie over het beheren van gebruikerstoewijzingen in de Balancer van de Werklast, zie [ gebruikerstoewijzingen in de Balancer van de Werkbelasting ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md) beheren.
* U kunt de geplande uren voor taken met een Duur Type van Gedreven of Berekend Werk niet wijzigen. In deze gevallen, bepaalt Workfront Geplande Uren die op de Duur van de taak worden gebaseerd; nochtans, in dit geval zijn de Geplande Uren altijd gelijk aan de Duur (in uren) en zij worden niet beïnvloed door de perceptie van de toegewezen middelen.

  Voor meer informatie over het Door inspanning Gedreven Type van Duur, zie [ overzicht van het Type van Duur: Gedreven inspanning ](../../../manage-work/tasks/taskdurtn/effort-driven.md).

  Voor meer informatie over het Berekende Type van Duur van het Werk, zie [ Overzicht van het Type van Duur: Berekend Werk ](../../../manage-work/tasks/taskdurtn/calculated-work.md).

## Taak geplande uren bijwerken bij het beheren van gebruikerstoewijzingen

U kunt geplande uren voor taken bijwerken wanneer u de gebruikers- of taakroltoewijzingen handmatig bijwerkt aan taken. Dit is alleen mogelijk wanneer taken een Duur van Eenvoudig hebben.

Voor meer informatie, zie [ overzicht van het Type van Duur: Eenvoudig ](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

U kunt of de algemene toewijzing van de gebruikers en rollen bijwerken die aan de taak worden toegewezen, of de gebruikers dagelijkse toewijzingen wanneer het gebruiken van de Balancer van de Werkbelasting.

Voor informatie over het beheren van algemene gebruikers en baanroltoewijzingen voor taken, zie [ gebruikers en roltoewijzingstijden op taken ](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) leiden.

Voor informatie over het beheren van dagelijkse toewijzingen voor taken, zie [ gebruikerstoewijzingen in de Balancer van de Werklast beheren ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

De volgende scenario&#39;s bestaan wanneer manueel het bijwerken van gebruiker of baanroltoewijzingen voor taken:

* Wanneer u de individuele gebruiker of de roltoewijzingen niet manueel hebt bijgewerkt om een verandering in de taak Geplande Uren teweeg te brengen, blijven de Geplande Uren ongewijzigd wanneer u toevoegt, verwijdert, of, taken op de taak vervangt. Wanneer u een nieuwe toewijzing aan de taak toevoegt, worden de afzonderlijke toewijzingen opnieuw verdeeld over alle toewijzingen.
* Wanneer u de toewijzingen handmatig hebt bijgewerkt om een wijziging in de geplande uren te activeren, nemen de geplande uren af wanneer u toewijzingen uit de taak verwijdert. Ze blijven ongewijzigd wanneer u een toewijzing vervangt.
* Wanneer u de toewijzingen handmatig hebt bijgewerkt om een wijziging in de geplande uren te activeren en u een toewijzing aan de taak toevoegt, wordt de nieuwe toewijzing standaard 0 uur toegewezen. U moet hun toewijzing aan de taak manueel bijwerken, die de Geplande Uren zou kunnen beïnvloeden.
* Als u de toewijzingen niet handmatig hebt bijgewerkt om een wijziging in de geplande uren te activeren en u alle toewijzingen voor de taak verwijdert, blijven de geplande uren ongewijzigd.
* Wanneer u de toewijzingen handmatig hebt bijgewerkt om een wijziging in de geplande uren te activeren en u alle toewijzingen voor de taak verwijdert, worden ook de geplande uren verwijderd en de geplande uren van de taak 0.

>[!NOTE]
>
>Als een taak bijvoorbeeld 10 geplande uren heeft en u twee toewijzingen hebt, worden deze standaard toegewezen aan elk 5 uur.
>
>* Als u de individuele gebruikerstoewijzing of de dagelijkse toewijzingen niet bijwerkt gebruikend de Balancer van de Werkbelasting en u om het even welke of alle toegewezen personen uit de taak verwijdert, blijven de taak Gepland Uren 10 uren.
>* Als u de toewijzingen handmatig wijzigt in respectievelijk 4 en 6 uur en u de gebruiker verwijdert die is toegewezen aan 6 uur en hun functie, wordt de taak Geplande uren bijgewerkt naar 4 uur. Als u ook de gebruiker verwijdert die aan 4 uren wordt toegewezen maar de baanrol verbonden aan de verwijderde gebruiker houdt, blijven de Geplande Uren van de taak 4 uren. Als u de laatste gebruiker verwijdert die aan 4 uren evenals hun baanrol wordt toegewezen en de taak niet toegewezen blijft, wordt de taak Geplande Uren 0.

## Werk taken die u wilt plannen automatisch bij met de werkinspanning

Wanneer u de Werkinspanning van het Werk gebruikt om de inspanning te schatten nodig voor een taak om te voltooien, de hoeveelheid Geplande Uren voor de taken werkt automatisch bij. Dit is alleen mogelijk voor taken met een eenvoudig type duur.

Voor informatie over het gebruiken van de Werkinspanning van het Werk om taakinspanning te schatten, zie [ Overzicht van de Werkinspanning van het Werk ](../../../manage-work/tasks/task-information/work-effort.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p> </p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
