---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Overzicht van taakbeperking: vaste datums'
description: U kunt de taakbeperking Vaste datums gebruiken wanneer u specifieke informatie wilt over de exacte begindatum en einddatum van uw taken. Voor meer informatie over taakbeperkingen, zie het overzicht van de Restrictie van de Taak.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Overzicht van taakbeperking: Vaste datums

U kunt de taakbeperking Vaste datums gebruiken wanneer u specifieke informatie wilt over de exacte begindatum en einddatum van uw taken. Voor meer informatie over taakbeperkingen, zie [ Overzicht van de Beperking van de Taak ](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Overzicht van de beperking Vaste datums

Houd rekening met het volgende wanneer u de beperking Vaste datums gebruikt:

* Als u de taakbeperking Vaste datums (FIXT) selecteert, moet u de geplande begindatum en de geplande voltooiingsdatum van de taak opgeven. In dit geval wordt de eerdere relatie van de taak genegeerd.
* Het veld Duur van de taak kan niet worden bewerkt met de beperking FIXT. De duur wordt berekend als het verschil tussen de Geplande Begin en Geplande Datum van de Voltooiing van de taak.
* Als het Type van Duur van de taak Gedreven de inspanning is, beïnvloedt het aantal wijzers op de taak ook de Duur van de taak.
* Wanneer u een taak met een beperking FIXT aan een ander project beweegt of kopieert, zou de beperking van de taak of de data van het project afhankelijk van kunnen veranderen wat de beperkingsdata zijn en wat de Datums van het Begin en van de Voltooiing van het project zijn. De volgende scenario&#39;s bestaan:

   * Wanneer het bestemmingsproject van Begin wordt gepland:

      * Wanneer om het even welke beperkingsdata van de taak vroeger zijn dan de Datum van het Begin van het Project, verandert de taakbeperking in zo spoedig mogelijk.
      * Wanneer om het even welke of beide beperkingsdata van de taak later zijn dan de Geplande VoltooiingsDatum van het project, verandert de Geplande Datum van de Voltooiing van het project om de voltooiingsbeperkingsdatum van de taak aan te passen.

   * Wanneer het bestemmingsproject van Voltooiing wordt gepland:

      * Wanneer om het even welke beperkingsdata van de taak later zijn dan de Datum van de Voltooiing van het Project, verandert de taakbeperking in zo laat mogelijk.
      * Wanneer om het even welk of beide beperkingsdata van de taak vroeger zijn dan de Geplande Datum van het Begin van het project, verandert de Geplande Datum van het Begin van het project om de beginbeperkingsdatum van de taak aan te passen.

   * Ongeacht het programma van het project, wanneer de beperkingsdata van de taak binnen de Data van het Begin en van de Voltooiing van het project zijn, zijn er geen veranderingen in de Restrictie van de Taak of de projectdata.

  Voor informatie over het bewegen van taken, zie [ de taken van de Beweging ](../../../manage-work/tasks/manage-tasks/move-tasks.md). Voor informatie over het kopiëren van taken, zie [ Kopiëren en dupliceren taken ](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Voor informatie over hoe te om de Restrictie van de Taak op een taak bij te werken, zie [ de Restrictie van de Taak van een taak ](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md) bijwerken.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
