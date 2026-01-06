---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Overzicht van taakbeperking: voltooien niet eerder dan'
description: Eindigen Neen vroeger dan (FNET) is een Restrictie van de Taak die een taak plant na de datum te voltooien u specificeert.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Overzicht van taakbeperking: voltooien niet eerder dan

Eindigen Neen vroeger dan (FNET) is een Restrictie van de Taak die een taak plant na de datum te voltooien u specificeert.

## Overzicht van de beperking Geen eerdere finish dan

Overweeg het volgende wanneer het gebruiken van Eindig Nr. vroeger dan (FNET) beperking voor een taak:

* U zou deze beperking moeten gebruiken wanneer het project van de Datum van de Voltooiing gepland is. In dit geval, kunt u een zachte beperking op de taak verstrekken alvorens andere afhankelijke taken te dwingen om bij Risico te tonen.
* Wanneer u FNET op een project gebruikt dat **van Datum van het Begin** wordt gepland, dan plant de beperking de taak aangezien het het zou plannen als de beperking zo spoedig mogelijk was.
* Wanneer u een taak met een beperking FNET aan een ander project beweegt of kopieert, zou de beperking van de taak of de data van het project afhankelijk van kunnen veranderen wat de beperkingsdatums zijn en wat de Datums van het Begin en van de Voltooiing van het project zijn. De volgende scenario&#39;s bestaan:

   * Wanneer het bestemmingsproject van Begin wordt gepland:

      * Wanneer de beperkingsdatum van de taak vroeger is dan de geplande begindatum van het project, verandert de taakbeperking in zo snel mogelijk.
      * Wanneer de beperkingsdatum van de taak later is dan de geplande de VoltooiingsDatum van het project, verandert de geplande Datum van de Voltooiing van het project om de voltooiingsbeperkingsdatum van de taak aan te passen.

   * Wanneer het bestemmingsproject van Voltooiing wordt gepland:

      * Wanneer de beperkingsdatum van de taak later is dan de Datum van de Voltooiing van het Project, verandert de taakbeperking in zo laat mogelijk.
      * Wanneer de beperkingsdatum van de taak vroeger is dan de Geplande Datum van het Begin van het project, verandert de Geplande Datum van het Begin van het project om de beginbeperkingsdatum van de taak aan te passen.

   * Ongeacht het programma van het project, wanneer de beperkingsdatum van de taak binnen de Datums van het Begin en van de Voltooiing van het project is, zijn er geen veranderingen in de Beperking van de Taak of de projectdata.

  Voor informatie over het bewegen van taken, zie [&#x200B; de taken van de Beweging &#x200B;](../../../manage-work/tasks/manage-tasks/move-tasks.md). Voor informatie over het kopiëren van taken, zie [&#x200B; Kopiëren en dupliceren taken &#x200B;](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

  Voor informatie over hoe te om de Restrictie van de Taak op een taak bij te werken, zie [&#x200B; de Restrictie van de Taak van een taak &#x200B;](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md) bijwerken.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
