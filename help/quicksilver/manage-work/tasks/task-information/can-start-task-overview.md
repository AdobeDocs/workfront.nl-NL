---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van "Can Start" voor taken
description: Wanneer een taak klaar is om te beginnen, voegt Adobe Workfront een Kan indicator van het Begin aan de taak toe om gemakkelijk te identificeren dat het voor u veilig is om aan de taak te beginnen werken. U kunt deze indicator in de mening van een taaklijst of een rapport bekijken.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Overzicht van &quot;Kan starten&quot; voor taken

Wanneer een taak klaar is om te beginnen, voegt Adobe Workfront een Kan indicator van het Begin aan de taak toe om gemakkelijk te identificeren dat het voor u veilig is om aan de taak te beginnen werken. U kunt deze indicator in de mening van een taaklijst of een rapport bekijken.

Wanneer de taak klaar is om aan worden gewerkt, wordt het gebied van de Begin van het Kan aan de taak geplaatst aan Waar.

## Hoe Workfront een taak markeert als &quot;Kan starten&quot;

Workfront controleert de volgende dingen alvorens het een taak als Waar voor het gebied van het Begin van het Kan merkt:

* Of de waarde van Can Start voor de ouder het plaatste aan Waar, als de taak een ouder heeft. Als de waarde voor de ouder Vals is, dan hebben alle subtaken de waarde van kan Begin aan Vals, eveneens wordt geplaatst.
* Of de voorgangers van de taak en de voorgangers van hun ouders compleet zijn. Als zij volledig zijn, kan de waarde van het Begin voor de taak worden geplaatst aan Waar. Als om het even welke taak predecessors of hun ouderpredecessors niet volledig zijn, of een status van Volledige In afwachting van Goedkeuring hebben, dan kan de waarde van het Begin voor de taak worden geplaatst aan Vals.
* Of het type van taakgebiedsdeel of Begin-Begin of Begin-Afwerking is. Als het gebiedstype begin-Begin of begin-Afwerking is, zal de afhankelijke taak de vlag &quot;kunnen&quot;hebben die aan Waar wordt geplaatst nadat de voorgangerstaak lopend is (of nadat het percentage voltooide van de voorgangertaak groter is dan 1%).

  Voor informatie over taakvoordecessors, zie [&#x200B; Overzicht van taakvoordecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Overwegingen over het identificeren van taken die klaar zijn om te beginnen

* Als het Type van Afhankelijkheid tussen een taak en zijn predecessors Begin-Begin is, moet predecessor beginnen alvorens de voorgangersverhouding wordt beschouwd als opgelost en de opvolgertaken kunnen beginnen. Voor informatie over gebiedsdeeltypes, zie [&#x200B; Overzicht van de types van taakgebiedsdeel &#x200B;](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Als een taak een voorganger voor meerdere projecten heeft, wordt door de voltooiing van de voorganger de indicator Kan starten niet automatisch toegepast op de opvolger. U moet de chronologie van het project van de opvolger manueel opnieuw berekenen of Workfront moet het automatisch opnieuw berekenen, alvorens de opvolgertaak als taak Van het Begin van het Kan toont. Voor meer informatie over het opnieuw berekenen van projectchronologie, zie [&#x200B; projectchronologie &#x200B;](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

  Voor informatie over dwars-project predecessors, zie [&#x200B; creëren dwars-project predecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
