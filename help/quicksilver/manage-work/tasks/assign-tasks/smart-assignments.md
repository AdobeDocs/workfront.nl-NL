---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Overzicht van slimme toewijzingen
description: Bij het beheren van taken en uitgaven kunt u slimme toewijzingen gebruiken om te bepalen wie de beste gebruiker het werk moet voltooien. De slimme taken zijn suggesties die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst die op een algoritme worden gebaseerd dat het meest aangewezen middel voor de baan bepaalt.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 4d76ef1b34d484e3da2af94543a5fd660ad0a4ef
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Overzicht van slimme toewijzingen

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze functie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten of in de productieomgeving voor klanten die snelle releases hebben ingeschakeld.</span>

<span class="preview">Voor informatie over snelle versies raadpleegt u [Snelle releases voor uw organisatie in- of uitschakelen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Voor informatie over de huidige versie raadpleegt u [Overzicht release derde kwartaal 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Bij het beheren van taken en uitgaven kunt u slimme toewijzingen gebruiken om te bepalen wie de beste bron is om het werk te voltooien. De slimme taken zijn suggesties die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst die op een algoritme worden gebaseerd dat het meest aangewezen middel voor de baan bepaalt. De slimme taken kunnen gebruikers, baanrollen, of teams zijn.

>[!NOTE]
>
>Bij het voorstellen van gebruikers houden slimme toewijzingen geen rekening met de beschikbaarheid van de gebruiker. De beschikbaarheid volgens de planning is echter van invloed op de geplande en verwachte datum van taken en problemen wanneer deze worden toegewezen. Raadpleeg het artikel voor informatie over schema&#39;s [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Dit artikel bevat algemene informatie over slimme toewijzingen. Voor informatie over het gebruiken van slimme taken om taken en kwesties aan gebruikers toe te wijzen, zie [Slimme toewijzingen maken](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Overzicht van slimme toewijzingen

Houd rekening met het volgende wanneer u werkt met slimme toewijzingen:

* Het algoritme werkt onafhankelijk voor taken en kwesties. Dit betekent dat de lijst met voorgestelde gebruikers voor problemen kan afwijken van de lijst met voorgestelde gebruikers voor een taak, omdat Workfront de lijsten samenstelt op basis van criteria die betrekking hebben op problemen en taken afzonderlijk.
* De slimme taken adviseren baanrollen of teams niet. In plaats daarvan zijn dit suggesties van gebruikers die het meest geschikt zijn om een taak of een probleem te voltooien.
* De voorgestelde toewijzingen zijn altijd actieve gebruikers.
* De eerst vermelde gebruiker zou de beste gelijke voor de taak moeten zijn.

## Suggesties voor slimme toewijzingen zoeken

U kunt slimme toewijzingen weergeven op de volgende plaatsen waar u taken of problemen kunt toewijzen:

* Een uitgiftenlijst of rapport in de kolom Toewijzingen

  ![](assets/smart-assignments-issue-list.png)

* <span class="preview">Een taaklijst of rapport in de kolom van Taken </span>

  <span class="preview">![](assets/smart-assignments-task-list.png)</span>

* <span class="preview">Een taakkoptekst in het veld Toewijzingen</span>

  <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>

* Een uitgiftekop in het veld Toewijzingen

  ![](assets/smart-assignments-issue-header.png)

* Het deelvenster Overzicht van taken of uitgaven in het gebied Toewijzingen

  ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* <span class="preview">Het gebied van Toewijzingen in de Nieuwe doos van de Taak, wanneer het toevoegen van een taak aan een project</span>

  <span class="preview">![](assets/smart-assignments-new-task-modal.png)</span>

* Het veld Toewijzingen voor een item dat wordt vermeld in het gebied Home wanneer u een taak opent of een uitgave afgeeft

  ![](assets/smart-assignments-in-home-nwe-350x216.png)

* Werklastverdeling in het gedeelte Toegewezen aan als u een taak of uitgave toewijst

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Criteria voor slimme toewijzingen

<div class="preview">

Slimme toewijzingen werken anders voor taken dan voor problemen.

### Slimme toewijzingscriteria voor taken

De taak slimme toewijzingsberekening werkt in twee fasen die twee verschillende algoritmen gebruiken.

Afhankelijk van welk algoritme de slimme taak vindt, worden de taken vermeld onder twee afzonderlijke secties in het gebied van Taken. Zie voor meer informatie [Slimme toewijzingen maken](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md).

![](assets/smart-assignments-task-list.png)

#### Eerste fase van berekening van slimme toewijzing voor taken

In de eerste fase van het berekenen van slimme toewijzingen, berekent Workfront een gelijkheidsscore voor elke taak.

>[!NOTE]
>
>De eerste fase van de berekening van de slimme toewijzingen is niet van toepassing op de volgende taakgebieden:
>
>* Bulktoewijzingen in Workload Balancer.
>* Aangesloten kaarten op borden.


Bij de berekening van de score op basis van gelijkenis en de volgorde waarin de toewijzingen worden vermeld, wordt rekening gehouden met het volgende:

* Een score van 100% wordt gegeven aan een bestaande taak waar de taak, het project, en de portefeuillenamen identiek aan de taak zijn u probeert toe te wijzen. De project- en portfolionamen van de taak van een bestaande toewijzing moeten ook overeenkomen met het project en de portfolio van de taak die u wilt toewijzen.

* Als slechts een deel van deze informatie uit andere toewijzingen overeenkomt met de bestaande taken, kan de score lager zijn dan 100%.

  Als u bijvoorbeeld een taak toewijst met de naam &quot;Mijn tweede taak&quot; voor een project met de naam &quot;Mijn project&quot; in een portfolio met de naam &quot;Mijn portfolio&quot; en u een bestaande taak hebt met de naam &quot;Mijn taak&quot; in een ander project met de naam &quot;Mijn project&quot;, krijgt de gebruiker met de naam &quot;Mijn taak&quot; een score van 95% omdat de naam van de bestaande taak en de taak die u nu wilt toewijzen vergelijkbaar zijn, maar niet identiek.

  >[!TIP]
  >
  >  Workfront zoekt alleen naar overeenkomsten in de velden Naam van taken, projecten en portfolio&#39;s en niet op andere velden.

* Een toewijzing zou een hogere score kunnen krijgen wanneer zij aan veel taken in het systeem worden toegewezen die gelijkaardige namen hebben. Als bijvoorbeeld een team met de naam &quot;Ontwikkeling&quot; wordt toegewezen aan 50% van de taken in het systeem die &quot;AI&quot; in de naam bevatten en u nu een andere taak toewijst met &quot;AI&quot; in de naam, is de score van het team &quot;Ontwikkeling&quot; hoger. In dit geval zijn de namen van projecten en portefeuilles niet zo belangrijk.

* Rekening houdend met dit scoresysteem worden de eerste 7 suggesties vermeld als slimme toewijzingen, in dalende volgorde van hun scores. Toewijzingen met scores lager dan 40% worden niet weergegeven.

* Als meerdere toewijzingen identieke scores hebben, worden deze weergegeven in volgorde van de datum waarop de toewijzingen zijn gedaan, te beginnen op de meest recente datum.

  Bijvoorbeeld, als Rick eerder vandaag aan een gelijkaardige taak werd toegewezen en Jennifer twee dagen geleden aan een gelijkaardige taak werd toegewezen, toont Rick eerst.

* In deze fase geïdentificeerde toewijzingen worden vermeld in de    **Voorgestelde toewijzingen**  in het veld Toewijzingen.

* Als er geen gelijken gebruikend deze berekening zijn, begint de tweede fase van slimme taken die gebruikend een verschillend algoritme wordt berekend.

#### Tweede fase van berekening van slimme toewijzing voor taken

Als de eerste stap van taak slimme taken geen gelijken heeft gevonden, berekent Workfront slimme taken voor taken op dezelfde manier als ze voor problemen worden berekend.

Zie de sectie voor meer informatie [Criteria voor slimme toewijzingen voor taken en problemen](#smart-assignments-criteria-for-tasks-and-issues) in dit artikel.

In deze fase geïdentificeerde toewijzingen worden vermeld in de   **Overige toewijzingen** (of de Gebruikers en teams, of de roltaken van de Taak) sectie van het gebied van Taken voor taken.

### Criteria voor slimme toewijzingen voor taken en problemen

</div>

>[!NOTE]
>
><span class="preview">De volgende criteria zijn alleen van toepassing op taken wanneer de eerste fase van de berekening van de intelligente taak geen overeenkomsten heeft gevonden. Zie de sectie [Eerste fase van berekening van slimme toewijzing voor taken](#first-phase-of-smart-assignment-calculation-for-tasks) in dit artikel. De volgende criteria zijn standaard altijd van toepassing op problemen. </span>

![](assets/smart-assignments-issue-header.png)

De gebruikers worden geadviseerd in de slimme drop-down lijst van Toewijzingen die op een combinatie van de volgende criteria (die in orde van belangrijkst tot minst belangrijk worden vermeld) wordt gebaseerd:

1. Gebruikers die in de afgelopen 30 dagen aan andere werkitems zijn toegewezen door de gebruiker die de toewijzing maakt. De eerste 50 gebruikers die aan deze criteria voldoen, worden weergegeven. De gebruiker die het vaakst wordt toegewezen toont eerst.

2. Als het het werkpunt aan een team of een rol wordt toegewezen, wordt de lijst van voorgestelde gebruikers gefiltreerd verder rekening houdend met de bestaande taken hieronder. In dit geval worden alleen de volgende gebruikers weergegeven in de lijst met suggesties:

   * Gebruikers van wie het Team van het Huis het team is dat aan het het werkpunt wordt toegewezen.
   * Gebruikers waarvan de primaire rol de rol is die aan het werkitem is toegewezen.

>[!TIP]
>
>* Als er geen rol of team aan de taak of kwestie wordt toegewezen, toont Workfront alle gebruikers die voor de laatste 30 dagen, tot 50 gebruikers worden toegewezen.
>
>* Als u geen taken in de afgelopen 30 dagen hebt gemaakt, slechts gebruikers die tot of het toegewezen team behoren of de rol hebben die aan het het werkpunt wordt toegewezen tonen in de slimme lijst van taken.

<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
