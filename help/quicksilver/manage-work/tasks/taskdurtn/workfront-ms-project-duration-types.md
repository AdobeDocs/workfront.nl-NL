---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Duur typen in Adobe Workfront- en Microsoft-project
description: De types van Duur beschikbaar in Adobe Workfront zijn verschillend dan hun tegenhangers in het Project van Microsoft die de Types van Taak worden genoemd. Dit kan soms verwarrend zijn bij het exporteren of importeren van projecten tussen Workfront en Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Duur typen in Adobe Workfront- en Microsoft-project

De types van Duur beschikbaar in Adobe Workfront zijn verschillend dan hun tegenhangers in het Project van Microsoft die de Types van Taak worden genoemd. Dit kan soms verwarrend zijn bij het exporteren of importeren van projecten tussen Workfront en Microsoft Project.

Raadpleeg de volgende artikelen voor informatie over het importeren en exporteren van projecten tussen Workfront en Microsoft Project:

* [ Uitvoer een project naar het Project van Microsoft ](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Een project importeren uit Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Duur typen in Workfront- en Microsoft-project

Workfront heeft vier typen taakduur:

* eenvoudig
* Inzet gedreven
* Berekend werk
* Berekende toewijzing

Voor informatie, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Deze soorten duur worden niet herkend door Microsoft Project. Microsoft Project heeft momenteel drie taaktypen die lijken op Duur-typen in Workfront:

* Vaste eenheden
* Vast werk
* Vaste duur

## Wijzigingen in Duur bij exporteren van Workfront naar MS-project

Wanneer u projecten exporteert van Workfront naar Microsoft Project, worden taken die zijn gebaseerd op inspanningen, Vast werk. De eenvoudige, Berekende Werkruimte, en de Berekende Toewijzing worden Vaste Eenheden.

## Wijzigingen in Duur bij importeren van MS Project naar Workfront

Wanneer u projecten importeert van Microsoft Project in naar Workfront, worden Vaste eenheden gebaseerd op inspanningen. Vast werk en Vaste Duur ontvangen het standaardduurtype dat uw beheerder van Workfront voor uw systeem selecteerde. Voor informatie, zie [ de taak en de uitgevende voorkeur van het systeem brede ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
