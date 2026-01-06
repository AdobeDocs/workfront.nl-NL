---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Overzicht van taakbeperking: begin niet eerder dan'
description: Gebruik het Begin Geen vroeger dan (SNET) de Beperking van de Taak om een taak te plannen na de datum te beginnen u specificeert.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Overzicht van taakbeperking: begin niet eerder dan

Gebruik het Begin Geen vroeger dan (SNET) de Beperking van de Taak om een taak te plannen na de datum te beginnen u specificeert.

## Overzicht van Begin niet vroeger dan de Beperking van de Taak

Overweeg het volgende wanneer het gebruiken van Begin Nr vroeger dan de Beperking van de Taak:

* U zou Begin niet vroeger dan beperking moeten gebruiken wanneer het project van de Datum van het Begin gepland is. In dit geval, kunt u een zachte beperking op een taak verstrekken alvorens het andere afhankelijke taken dwingt om als Op Risico te tonen.
* Begin Nr. vroeger dan is de standaardbeperking als een project van de Datum van het Begin gepland is en als het systeem of de groep standaardbegindatum voor een nieuwe taak aan Vandaag wordt geplaatst. Voor informatie over het vormen van gebreken voor taken, zie [&#x200B; systeembrede taak vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Als u het project van de Datum van het Begin plant en de systeem standaardbegindatum voor een nieuwe taak wordt geplaatst aan Gebaseerd op het Geplande Project Datum, is de standaardbeperking voor een nieuwe taak zo spoedig mogelijk.
* Als u het project van het Project van de Datum van de Voltooiing plant en de systeem standaardbegindatum voor een nieuwe taak wordt geplaatst aan Vandaag, dan plant het Begin Geen vroeger dan beperking de taak aangezien het een ZO laat Zo Late taak.
* Wanneer u een taak met een beperking SNET aan een ander project beweegt of kopieert, zou de beperking van de taak of de data van het project afhankelijk van kunnen veranderen wat de beperkingsdatums zijn en wat de Datums van het Begin en van de Voltooiing van het project zijn. De volgende scenario&#39;s bestaan:

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
