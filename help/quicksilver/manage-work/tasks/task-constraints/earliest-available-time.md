---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Overzicht van taakbeperking: vroegst beschikbare tijd'
description: De vroegste Beschikbare Tijd is een Restrictie van de Taak die een taak plant om bij de vroegste beschikbare tijd na het overwegen van om het even welke voorgangersverhoudingen te beginnen.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Overzicht van taakbeperking: vroegst beschikbare tijd

De vroegste Beschikbare Tijd is een Restrictie van de Taak die een taak plant om bij de vroegste beschikbare tijd na het overwegen van om het even welke voorgangersverhoudingen te beginnen.

Voor informatie over hoe te om de Restrictie van de Taak op een taak bij te werken, zie [&#x200B; de Restrictie van de Taak van een taak &#x200B;](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md) bijwerken.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## Het verschil tussen de vroegste beschikbare tijd en zo snel mogelijk

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

De oudste beschikbare tijdbeperking verschilt van de restrictie Zo snel mogelijk wanneer alle volgende criteria bestaan:

* Het project is gepland vanaf voltooiing
* De taken in het project hebben een voorgangersverhouding
* De voorgaande taak heeft een flexibele taakbeperking

In deze situatie:

* **Vroegst Beschikbare Tijd:** Gebruikend de vroegst Beschikbare beperking van de Tijd op de opvolgertaak geeft prioriteit aan de flexibele beperking van de voorganger.

  **VOORBEELD**

  Taak A is een voorganger aan Taak B. Taak B heeft de Vroegst Beschikbare Beperking van de Tijd en Taak A heeft de ZO laat mogelijk beperking. In deze situatie is taak B zo dicht mogelijk bij de voltooiing van het project gepland.

  ![&#x200B; vroegst Beschikbare beperking van de Tijd wanneer de taak de data dicht bij de Datum van de Voltooiing van het project &#x200B;](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png) heeft

* **zo spoedig mogelijk:** in dit scenario, die zo spoedig mogelijk de beperking op de opvolgertaak gebruiken geeft de prioriteit aan de opvolgertaak.

  **VOORBEELD**

  Taak A is een voorganger aan Taak B. Taak B heeft zo spoedig mogelijk de beperking en Taak A heeft de Zo laat mogelijk beperking. In deze situatie is taak B zo dicht mogelijk bij de start van het project gepland.

  ![&#x200B; zo spoedig mogelijk beperking wanneer de taak de data dicht bij de Datum van het Begin van het project &#x200B;](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png) heeft
