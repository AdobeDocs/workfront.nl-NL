---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van afhandelingsdatum taak
description: De Handoff Datum is de datum dat een taak voor het werk beschikbaar wordt. Dit betekent doorgaans dat de voorgangers zijn opgelost en dat de opdrachtgever van de taak eraan kan beginnen te werken.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# Overzicht van afhandelingsdatum taak

De Handoff Datum is de datum dat een taak voor het werk beschikbaar wordt. Dit betekent doorgaans dat de voorgangers zijn opgelost en dat de opdrachtgever van de taak eraan kan beginnen te werken.

>[!TIP]
>
>Handoff-data bestaan niet voor problemen en projecten.

## Hoe Adobe Workfront de Handoff-datum berekent

>[!NOTE]
>
>De afhandelingsdatum wordt alleen berekend als de projectstatus gelijk is aan de volgende statussen:
>
>* In de wachtstand
>* Huidig
>* Voltooid
>* Dead
>

Workfront hanteert de volgende regels voor het berekenen van de afhandelingsdatum van een taak:

* **wanneer de taak een onvolledige voorganger** heeft: De Handoff Datum voor de taak is ongeldig.
* **wanneer de taak een volledige voorganger** heeft: De Handoff Datum is het zelfde als de Ware Datum van de Voltooiing van de voorgangertaak. Als de voorganger een vertraging heeft, berekent Workfront de afhandelingsdatum van de opvolgertaak aan de hand van de volgende formule:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Voor informatie over vertragingstijd, zie [&#x200B; Overzicht van de Types van Markeringen &#x200B;](../use-prdcssrs/lag-types.md).

  Als de opvolgertaak meer dan één voorganger heeft, wordt de afhandelingsdatum berekend op basis van de laatste werkelijke Voltooiingsdatum van de voorgangers. Als de werkelijke Voltooiingsdata van de twee voorgangers bijvoorbeeld 8 november 2022 en 20 november 2022 zijn, is de Handoff Date van de opvolger 20 november 2022.

  >[!NOTE]
  >
  >   Het berekenen van de Handoff Datum van een opvolgertaak die op de Ware Datum van Voltooiing of een voorgangertaak wordt gebaseerd is het zelfde of voorganger wordt afgedwongen of niet. Voor meer informatie over gedwongen predecessors, zie [&#x200B; predecessors &#x200B;](../use-prdcssrs/enforced-predecessors.md) afdwingen.


* **wanneer de taak geen voorganger en** heeft:

   * **de Geplande Datum van het Begin is in het verleden**: De Handoff Datum is het zelfde als de Geplande Datum van het Begin van het project als de taak geen gedwongen geplaatste beperking heeft. In de gevallen waarin taken gedwongen beperkingen hebben, raadpleegt u de sectie &quot;Wanneer de taak een gedwongen beperking voor de geplande datums heeft&quot; hieronder.
   * **de Geplande Datum van het Begin is in de toekomst (om het even welke datum na de huidige datum)**: De Handoff Datum is het zelfde als de Geplande Datum van het Begin van de taak als de taak geen gedwongen geplaatste beperking heeft. In de gevallen waarin taken gedwongen beperkingen hebben, raadpleegt u de sectie &quot;Wanneer de taak een gedwongen beperking voor de geplande datums heeft&quot; hieronder.

>[!NOTE]
>
>Wanneer de taak een dwars-projectvoorganger heeft, berekent de handoff datum van de opvolger slechts wanneer één van beiden van het volgende voorkomt:
>
>* U berekent manueel de chronologie van het project van de opvolger opnieuw. U moet over beheerdersmachtigingen voor het project beschikken om de tijdlijn opnieuw te berekenen.
>* De tijdlijn van het project van de opvolger wordt automatisch &#39;s nachts opnieuw berekend.
>
>Voor informatie over het opnieuw berekenen van de chronologie van het project, zie [&#x200B; projectchronologie &#x200B;](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

* **wanneer de taak een gedwongen beperking voor de Geplande Datums** heeft: De Datum van de Aflevering varieert afhankelijk van het type van beperking en of de taak een Ware Datum van het Begin heeft of niet.\
  De volgende taken zijn geforceerde beperkingen:

   * Moet beginnen op
   * Moet worden voltooid op
   * Niet eerder starten dan
   * Niet later starten dan
   * Vaste datum

  De volgende scenario&#39;s bestaan:

   * **wanneer de taak een beperking van moet beginnen op of Begin niet vroeger dan** heeft: Als de datum van de taakbeperking in het verleden is en er geen Werkelijke Datum van het Begin op de taak (de taak is nog niet begonnen) is de Datum van Handoff de dichtstbijzijnde mogelijke datum de taak kan worden begonnen om te worden gewerkt aan. Als de taak is begonnen, evenaart de Datum van Handoff de begindatum van het project.
   * **wanneer de taak een beperking van moet op of Begin niet later dan** beëindigen: Als de datum van de taakbeperking in de toekomst is en er geen Ware Datum van het Begin op de taak (de taak is nog niet begonnen) is de Datum van de Afhandeling de Geplande Datum van het Begin van de taak. Als er op de taak als Werkelijke Datum van het Begin is dan is de Datum van Handoff de begindatum van het project.
   * **wanneer de taak een beperking van Vaste Datums** heeft: De Handoff Datum is de Geplande Datum van het Begin van de taak, ongeacht of het een predecessor of niet heeft en ongeacht of predecessor wordt voltooid of niet.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## De Handoff-datum zoeken

U kunt de Handoff Datum van een taak in een taakrapport of de mening van een taaklijst tonen.\
Voor meer informatie over de bouw van een rapport, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
