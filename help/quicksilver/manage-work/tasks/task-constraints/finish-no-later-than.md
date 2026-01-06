---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Overzicht van taakbeperking: uiterlijk voltooien'
description: Voltooien Uiterlijk (FNLT) is een Taakbeperking die een taak plant die moet worden voltooid vóór de datum die u opgeeft.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Overzicht van taakbeperking: uiterlijk voltooien

Voltooien Uiterlijk (FNLT) is een Taakbeperking die een taak plant die moet worden voltooid vóór de datum die u opgeeft.

## Overzicht van de beperking Afwerking niet later dan

Houd rekening met het volgende wanneer u de FNLT-beperking (Finish No Later Than) gebruikt voor een taak:

* U zou deze beperking moeten gebruiken wanneer het project van de Datum van het Begin wordt gepland. In dit geval, kunt u een zachte beperking op een taak verstrekken alvorens het andere afhankelijke taken dwingt om als Op Risico te tonen.
* Wanneer u de beperking FNLT met een project van het Programma van de Datum van de Voltooiing gebruikt, plant deze beperking de taak aangezien het een Zo laat mogelijk taak zou zijn.
* Wanneer u een taak met een beperking FNET aan een ander project beweegt of kopieert, zou de beperking van de taak of de data van het project afhankelijk van kunnen veranderen wat de beperkingsdatums zijn en wat de Datums van het Begin en van de Voltooiing van het project zijn. De volgende scenario&#39;s bestaan:

   * Wanneer het bestemmingsproject van Begin wordt gepland:

      * Wanneer de beperkingsdatum van de taak vroeger is dan de geplande begindatum van het project, verandert de taakbeperking in zo snel mogelijk.
      * Wanneer de beperkingsdatum van de taak later is dan de geplande de VoltooiingsDatum van het project, verandert de geplande Datum van de Voltooiing van het project om de voltooiingsbeperkingsdatum van de taak aan te passen.

      * Wanneer het bestemmingsproject van Voltooiing wordt gepland:

         * Wanneer de beperkingsdatum van de taak later is dan de Datum van de Voltooiing van het Project, verandert de taakbeperking in zo laat mogelijk.
         * Wanneer de beperkingsdatum van de taak vroeger is dan de Geplande Datum van het Begin van het project, verandert de Geplande Datum van het Begin van het project om de beginbeperkingsdatum van de taak aan te passen.

      * Ongeacht het programma van het project, wanneer de beperkingsdatum van de taak binnen de Datums van het Begin en van de Voltooiing van het project is, zijn er geen veranderingen in de Beperking van de Taak of de projectdata.

  Voor informatie over het bewegen van taken, zie [ de taken van de Beweging ](../../../manage-work/tasks/manage-tasks/move-tasks.md). Voor informatie over het kopiëren van taken, zie [ Kopiëren en dupliceren taken ](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Voor informatie over hoe te om de Restrictie van de Taak op een taak bij te werken, zie [ de Restrictie van de Taak van een taak ](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md) bijwerken.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
