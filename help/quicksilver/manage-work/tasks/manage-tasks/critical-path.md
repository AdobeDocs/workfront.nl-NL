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
source-wordcount: '771'
ht-degree: 0%

---

# Overzicht van het project Kritieke Weg

Het bepalen van het Kritieke Weg van een project is een automatische manier voor Adobe Workfront om een opeenvolging van taken in een project te markeren die het potentieel hebben om de chronologie van het project te beïnvloeden. Taken die de tijdlijn van het project kunnen beïnvloeden, worden gemarkeerd als kritieke padtaken.

De volgende functies kunnen van invloed zijn op het kritieke pad van een project:

* De werkverdelingsstructuur van het project.

   Voor meer informatie over de Structuur van de Onderverdeling van het Werk, zie [Structuur van werkverdeling in een project bepalen](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* De tijd (duur) die elke taak zal vergen om te voltooien.
* De afhankelijkheden tussen de taken.

   Overweeg het volgende:

   * Wanneer een taak op de Kritieke Weg een voorgangersverhouding heeft, zijn predecessors en opvolgers ook op de Kritieke Weg als de veranderingen op data van de voorgangers of de opvolgers hun gebiedsdelen direct beïnvloeden.

      >[!TIP]
      >
      >Wanneer de datum van de opvolger van een taak niet direct de datum van hun afhankelijke taken beïnvloedt en het niet de data van het project beïnvloedt, is de opvolgertaak niet op de Kritieke Weg.
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * Wanneer een subtaak als Kritieke taak van de Weg wordt geïdentificeerd, wordt de oudertaak ook geïdentificeerd als Kritieke taak van de Weg, als de Geprojecteerde Datum en de tijd van het Begin van de ouder het zelfde als dat van subtask is.

Rekening houdend met deze eigenschappen, berekent het systeem de Kritieke Weg door de langste weg tussen de vroegste taak en de taak te gebruiken die het eind van het project bepaalt. De Kritieke Berekening van de Weg houdt rekening met wat de vroegste en recentste tijd is dat elke taak kan beginnen en beëindigen zonder het project langer te maken. Dit proces bepaalt welke taken &quot;kritiek&quot;zijn (en tot de langste weg behoren) en welke degenen &quot;totale vlotter&quot;hebben (kan worden vertraagd zonder het project langer te maken).

Elke vertraging in de activiteit van een taak op het kritieke pad heeft rechtstreeks invloed op de verwachte uitvoeringsdatum van het project (er is geen zwevend pad op het kritieke pad).

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
   <td> <p>De mening of hogere toegang tot Taken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven of hoger voor een taak </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Het kritieke pad weergeven

U kunt de taken die tot het Kritieke Weg behoren in de volgende gebieden van de toepassing van Workfront bekijken:

* [Het kritieke pad weergeven in het Gantt-diagram](#view-the-critical-path-in-the-gantt-chart)
* [Het kritieke pad weergeven in een takenlijst of rapport](#view-the-critical-path-in-a-task-list-or-report)

### Het kritieke pad weergeven in het Gantt-diagram {#view-the-critical-path-in-the-gantt-chart}

Om taken op de Kritieke Weg in de grafiek van Gantt te bekijken:

1. Ga naar een project waarvoor u de Kritieke Weg wilt bekijken.
1. Klikken **Taken** in het linkerdeelvenster.
1. Klik op de knop **Gantt Chart** in de rechterbovenhoek van de takenlijst.

   ![gantt_chart_icon_1_.png](assets/gantt-chart-icon--1-.png)

1. Breid uit **Opties** en schakelt u vervolgens het **Kritiek pad** optie.

   De taken die zich op het Kritieke Weg bevinden hebben een rode lijn boven hun chronologie in de grafiek van Gantt.

   ![kritisch_pad_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Het kritieke pad weergeven in een takenlijst of rapport {#view-the-critical-path-in-a-task-list-or-report}

Om te bekijken welke taken op de kritieke weg in een lijst van taken zijn:

1. Ga naar een project waarvoor u de Kritieke Weg wilt bekijken.
1. Klikken **Taken** in het linkerdeelvenster.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Status**.

   De taken die op de Kritieke Weg zijn hebben een **Kritiek pad** vlag in de **Vlaggen** kolom van de lijst.

   U kunt de zelfde mening op een taakrapport toepassen.

   Zie het artikel voor meer informatie over het maken van rapporten [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   of

   Van de **Filter** vervolgkeuzelijst, selecteert u **Nieuw filter**.

1. Klikken **Filterregel toevoegen** en begint te typen **Is kritiek** in de **Alleen taken weergeven waarin ...** veld.

1. Selecteer het wanneer het in de lijst verschijnt.
1. Klikken **Filter opslaan**.

   De lijst zou slechts taken moeten tonen die op de Kritieke Weg zijn.
