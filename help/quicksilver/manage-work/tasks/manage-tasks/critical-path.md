---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Overzicht van het project Kritieke Weg
description: Het bepalen van het Kritieke Weg van een project is een automatische manier voor Adobe Workfront om een opeenvolging van taken in een project te markeren die het potentieel hebben om de chronologie van het project te beïnvloeden. Taken die de tijdlijn van het project kunnen beïnvloeden, worden gemarkeerd als kritieke padtaken.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Overzicht van het project Kritieke Weg

Het bepalen van het Kritieke Weg van een project is een automatische manier voor Adobe Workfront om een opeenvolging van taken in een project te markeren die het potentieel hebben om de chronologie van het project te beïnvloeden. Taken die de tijdlijn van het project kunnen beïnvloeden, worden gemarkeerd als kritieke padtaken.

De volgende functies kunnen van invloed zijn op het kritieke pad van een project:

* De werkverdelingsstructuur van het project.

  Voor meer informatie over de Structuur van de Onderverdeling van het Werk, zie [ de Structuur van de Onderverdeling van het Werk in een project ](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md) bepalen

* De tijd (duur) die elke taak zal vergen om te voltooien.
* De afhankelijkheid tussen de taken.

  Overweeg het volgende:

   * Wanneer een taak op de Kritieke Weg een voorgangersverhouding heeft, zijn predecessors en opvolgers ook op de Kritieke Weg als de veranderingen op data van de voorgangers of de opvolgers hun gebiedsdelen direct beïnvloeden.

     >[!TIP]
     >
     >Wanneer de datum van de opvolger van een taak niet direct de datum van hun afhankelijke taken beïnvloedt en het niet de data van het project beïnvloedt, is de opvolgertaak niet op de Kritieke Weg.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Wanneer een subtaak als Kritieke taak van de Weg wordt geïdentificeerd, wordt de oudertaak ook geïdentificeerd als Kritieke taak van de Weg, als de Geprojecteerde Datum en de tijd van het Begin van de ouder het zelfde als dat van subtask is.

Rekening houdend met deze eigenschappen, berekent het systeem de Kritieke Weg door de langste weg tussen de vroegste taak en de taak te gebruiken die het eind van het project bepaalt. De Kritieke Berekening van de Weg houdt rekening met wat de vroegste en recentste tijd is dat elke taak kan beginnen en beëindigen zonder het project langer te maken. Dit proces bepaalt welke taken &quot;kritiek&quot;zijn (en tot de langste weg behoren) en welke degenen &quot;totale vlotter&quot;hebben (kan worden vertraagd zonder het project langer te maken).

Elke vertraging in de activiteit van een taak op het kritieke pad heeft rechtstreeks invloed op de geplande uitvoeringsdatum van het project (er is geen zwevend pad op het kritieke pad).

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
   <td> <p>De mening of hogere toegang tot Taken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven of hoger voor een taak </p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Het kritieke pad weergeven

U kunt de taken die tot het Kritieke Weg behoren in de volgende gebieden van de toepassing van Workfront bekijken:

* [ Mening de Kritieke Weg in de grafiek van Gantt ](#view-the-critical-path-in-the-gantt-chart)
* [Het kritieke pad weergeven in een takenlijst of rapport](#view-the-critical-path-in-a-task-list-or-report)

### Het kritieke pad weergeven in het Gantt-diagram {#view-the-critical-path-in-the-gantt-chart}

Om taken op de Kritieke Weg in de grafiek van Gantt te bekijken:

1. Ga naar een project waarvoor u de Kritieke Weg wilt bekijken.
1. Klik **Taken** in het linkerpaneel.
1. Klik het **pictogram van de Grafiek van de Gantt** in de hoger-juiste hoek van de taaklijst.

   ![ gantt_chart_icon__1_.png ](assets/gantt-chart-icon--1-.png)

1. Breid het **menu van Opties** uit, dan laat de **Kritieke Pad** optie toe.

   De taken die zich op het Kritieke Weg bevinden hebben een rode lijn boven hun chronologie in de grafiek van Gantt.

   ![ kritieke_path_on_gantt__1_.png ](assets/crtitical-path-on-gantt--1--350x137.png)

### Het kritieke pad weergeven in een takenlijst of rapport {#view-the-critical-path-in-a-task-list-or-report}

Om te bekijken welke taken op de kritieke weg in een lijst van taken zijn:

1. Ga naar een project waarvoor u de Kritieke Weg wilt bekijken.
1. Klik **Taken** in het linkerpaneel.
1. Van het **drop-down menu van de Mening**, uitgezochte **Status**.

   De taken die op de Kritieke Weg zijn hebben a **Kritieke 1&rbrace; vlag van de Weg in de** Vlaggen **kolom van de lijst.**

   U kunt de zelfde mening op een taakrapport toepassen.

   Voor meer informatie over het creëren van rapporten, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

   of

   Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe Filter**.

1. Klik **toevoegen de Regel van de Filter** en beginnen te typen **is Kritiek** in **toont me slechts Taken waarin het...** gebied.

1. Selecteer het wanneer het in de lijst verschijnt.
1. Klik **sparen Filter**.

   De lijst zou slechts taken moeten tonen die op de Kritieke Weg zijn.
