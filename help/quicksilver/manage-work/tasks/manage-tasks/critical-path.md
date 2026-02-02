---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Overzicht van het kritieke pad van het project
description: Het bepalen van het Kritieke Weg van een project is een automatische manier voor Adobe Workfront om een opeenvolging van taken in een project te markeren die het potentieel hebben om de chronologie van het project te beïnvloeden. Taken die de tijdlijn van het project kunnen beïnvloeden, worden gemarkeerd als kritieke padtaken.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Overzicht van het project Kritieke Weg

<!-- Audited: 5/2025 -->

Het bepalen van de Kritieke Weg van een project is een automatische manier voor Adobe Workfront om een opeenvolging van taken in een project te markeren die het potentieel hebben om de chronologie van het project te beïnvloeden. Taken die de tijdlijn van het project kunnen beïnvloeden, worden gemarkeerd als kritieke padtaken.

De volgende functies kunnen van invloed zijn op het kritieke pad van een project:

* De werkverdelingsstructuur van het project.

  Voor meer informatie, zie [&#x200B; de Structuur van de Onderverdeling van het Werk in een project &#x200B;](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md) bepalen.

* De tijd (duur) die elke taak zal vergen om te voltooien.
* De afhankelijkheid tussen de taken.

  Overweeg het volgende:

   * Wanneer een taak op het Kritieke Weg een voorgangersverhouding heeft, zijn predecessors en opvolgers ook op de Kritieke Weg als de veranderingen op de data van de voorgangers of opvolgers hun gebiedsdelen direct beïnvloeden.

     >[!TIP]
     >
     >Wanneer de opvolgerdatum van een taak niet direct de datum van hun afhankelijke taken of de data van het project beïnvloedt, is de opvolgertaak niet op de Kritieke Weg.
     >
     >
     >![&#x200B; Opvolger niet op kritieke weg &#x200B;](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Wanneer een subtaak als Kritieke taak van de Weg wordt geïdentificeerd, wordt de oudertaak ook geïdentificeerd als Kritieke taak van de Weg als de Geprojecteerde Datum van het Begin en de tijd van de oudertaak het zelfde als die van subtask is.

Rekening houdend met deze eigenschappen, berekent het systeem de Kritieke Weg door de langste weg tussen de vroegste taak en de taak te gebruiken die het eind van het project bepaalt. De Kritieke Berekening van de Weg houdt rekening met wat de vroegste en recentste tijd is dat elke taak kan beginnen en beëindigen zonder het project langer te maken. Dit proces bepaalt welke taken &quot;kritiek&quot;zijn (en tot de langste weg behoren) en welke degenen &quot;totale vlotter&quot;hebben (kan worden vertraagd zonder het project langer te maken).

Elke vertraging in de activiteit van een taak op het kritieke pad heeft rechtstreeks invloed op de geplande uitvoeringsdatum van het project (er is geen zwevend pad op het kritieke pad).

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
   <td> 
   <p>Standard<p>
   <p>Werk of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>De mening of hogere toegang tot Taken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven of hoger voor een taak </p></td> 
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
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on a task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Het kritieke pad weergeven

U kunt de taken die tot het Kritieke Weg behoren in de volgende gebieden van de toepassing van Workfront bekijken:

* [&#x200B; Mening de Kritieke Weg in de grafiek van Gantt &#x200B;](#view-the-critical-path-in-the-gantt-chart)
* [Het kritieke pad weergeven in een takenlijst of rapport](#view-the-critical-path-in-a-task-list-or-report)

### Het kritieke pad weergeven in het Gantt-diagram {#view-the-critical-path-in-the-gantt-chart}

Om taken op de Kritieke Weg in de grafiek van Gantt te bekijken:

{{step1-to-projects}}

1. Selecteer een project in de projectlijst.

1. In het linkerpaneel, klik **Taken**. Het **lusje van Taken** opent.

1. In de hoger-juiste hoek van de taaklijst, klik het **pictogram van de Grafiek 0&rbrace; Gantt.**

   ![&#x200B; gantt_chart_icon__1_.png &#x200B;](assets/gantt-icon.png)

1. In de hoger-juiste hoek van de Gantt grafieksectie, klik het **pictogram van Opties** ![&#x200B; pictogram van Opties &#x200B;](assets/options-icon.png), dan selecteer de **optie van de** Kritieke Weg in drop-down die verschijnt. De taken die zich op het Kritieke Weg bevinden hebben nu een rode lijn boven hun chronologie.

   ![&#x200B; kritieke_path_on_gantt__1_.png &#x200B;](assets/crtitical-path-on-gantt--1--350x137.png)

### Het kritieke pad weergeven in een takenlijst of rapport {#view-the-critical-path-in-a-task-list-or-report}

Om te bekijken welke taken op de kritieke weg in een lijst van taken zijn:

{{step1-to-projects}}

1. Selecteer een project in de projectlijst.

1. In het linkerpaneel, klik **Taken**. Het **lusje van Taken** opent.

1. Klik het **pictogram van de Mening** ![&#x200B; van de Mening &#x200B;](assets/view-icon.png) &lbrace;, dan selecteren **Status**. De taken die op de Kritieke Pad zijn tonen a **Kritieke Pad** vlag in de **Vlaggen** kolom van de lijst.

   of

   Klik het **pictogram van de Filter** pictogram ![&#x200B; Filters &#x200B;](assets/filters-icon.png), dan uitgezocht **+ Nieuwe Filter**.
1. Op het eerste gebied, is het type in *Kritiek*, dan selecteer het wanneer het onder de **&#x200B;**&#x200B;sectie van Taken &lbrace;in de lijst verschijnt.

   ![&#x200B; Taak is kritieke filter &#x200B;](assets/task-is-critical.png)

1. Verzeker **waar is** wordt geselecteerd in het tweede drop-down menu.

   ![&#x200B; is ware drop-down &#x200B;](assets/critical-path-filter.png)

1. Sluit het deelvenster Filters. In de takenlijst worden nu alleen taken weergegeven die zich op het kritieke pad bevinden.
