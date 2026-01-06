---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van projectduur
description: Adobe Workfront berekent de duur van een project door rekening te houden met de begindatum van de vroegste taak en de afsluitende datum van de laatste taak en telt het aantal dagen tussen de twee data.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Overzicht van de duur van het project

Adobe Workfront berekent de duur van een project door rekening te houden met de begindatum van de vroegste taak en de afsluitende datum van de laatste taak en telt het aantal dagen tussen de twee data.

## Projectduur

De duur van het project wordt berekend aan de hand van de volgende formule:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>De duur van kwesties op het project beïnvloedt niet de Duur van het Project.

De duur van het project telt het aantal dagen tussen de twee taakdata die op Programma verbonden aan het project of de gebruikers worden gebaseerd die aan de taken worden toegewezen. Voor informatie over welk programma Workfront gebruikt om duur te berekenen, zie [&#x200B; Overzicht van Programma&#39;s &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Soorten projectduur

Er zijn twee soorten de Duur van het Project en de formules waardoor Workfront hen berekent:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Geplande Duur**:

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Ware Duur**:

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Zoek de projectduur

U kunt het geplande project en de werkelijke duur vinden in de volgende gebieden van Workfront:

* . In het gebied van de Details van het Project, in de sectie van het Overzicht.

  Voor meer informatie over het Overzicht sub-lusje van een project, zie het artikel [&#x200B; informatie in het gebied van het projectoverzicht &#x200B;](../../../manage-work/projects/manage-projects/understand-project-overview-area.md) leiden.

* In een rapport van het Project, door de Duur of de Ware gebieden van de Duur in het rapport op te nemen.

  Voor meer informatie over het creëren van rapporten, zie het artikel [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
