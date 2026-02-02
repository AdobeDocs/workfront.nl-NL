---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Overzicht van taakafhankelijke lus
description: Wanneer het toevoegen van predecessor verhoudingen aan taken zou u gebiedsdeellijnen kunnen ontmoeten. Voor informatie over predecessors, zie Overzicht van taakvoordecessors.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Overzicht van taakafhankelijkheidslus

Wanneer het toevoegen van predecessor verhoudingen aan taken zou u gebiedsdeellijnen kunnen ontmoeten. Voor informatie over predecessors, zie [&#x200B; Overzicht van taakvoordecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Overzicht van afhankelijkheidslus

De lijnen van de afhankelijkheid gebeuren wanneer u twee of meer taken hebt die van elkaar afhangen om worden voltooid. Adobe Workfront staat u niet toe om een voorganger verhouding tussen taken tot stand te brengen als het tot een gebiedsdeellijn leidt.

**Voorbeeld:** Taak 2 is een voorganger aan Taak 1, wat betekent u Taak 2 moet voltooien alvorens u aan Taak 1 kunt beginnen te werken.

Als u probeert om Taak 1 een voorganger aan Taak 2 te maken, krijgt u een fout van de gebiedsdeellijn omdat u geen Taak 1 kunt beginnen tot Taak 2 is voltooid, maar taak 2 kan niet zijn begonnen tot Taak 1 wordt gebeëindigd.

![&#x200B; bericht van de de lusfout van de Afhankelijkheid &#x200B;](assets/dependency-loop-error-message-350x209.png)

![&#x200B; lijn van de Afhankelijkheid in taaklijst &#x200B;](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Overwegingen over gebiedsdeellijnen

* De lijnen van de afhankelijkheid kunnen meer dan twee taken impliceren. Soms zijn om het even welk aantal ouders van de taken u met een voorgangersverhouding verbindt degenen die tot de gebiedsdeellijn leiden.
* Een gebiedsdeellijn kan ook voorkomen als u probeert om een ouder tot voorganger van een kind te maken.
* In het geval van een gebiedsdeellijn kunt u niet de taken of het project bewaren. Om de gebiedsdeellijn te bevestigen, moet u de voorgangersverhouding tussen de taken opnieuw evalueren die in het foutenbericht worden vermeld en de conflicten verwijderen alvorens u de taken of het project kunt bewaren.


