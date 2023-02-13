---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van afhandelingsdatum taak
description: De Handoff Datum is de datum een taak voor het werk beschikbaar wordt. Dit betekent doorgaans dat de voorgangers zijn opgelost en dat de opdrachtgever van de taak eraan kan beginnen te werken.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 39efbf1d678cf85e9b6b61744fb046664992370c
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Overzicht van afhandelingsdatum taak

De Handoff Datum is de datum een taak voor het werk beschikbaar wordt. Dit betekent doorgaans dat de voorgangers zijn opgelost en dat de opdrachtgever van de taak eraan kan beginnen te werken.

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

* **Als de taak een onvolledige voorganger heeft**: De afhandelingsdatum voor de taak is null.
* **Als de taak een volledige voorganger heeft**: De afhandelingsdatum is dezelfde als de werkelijke afsluitende datum van de vorige taak. Als de voorganger een vertraging heeft, berekent Workfront de afhandelingsdatum van de opvolgertaak aan de hand van de volgende formule:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Voor informatie over vertragingstijd raadpleegt u [Overzicht van labeltypen](../use-prdcssrs/lag-types.md).

   Als de opvolgertaak meer dan één voorganger heeft, wordt de afhandelingsdatum berekend op basis van de laatste werkelijke Voltooiingsdatum van de voorgangers. Als de werkelijke Voltooiingsdata van de twee voorgangers bijvoorbeeld 8 november 2022 en 20 november 2022 zijn, is de Handoff Date van de opvolger 20 november 2022.

   >[!NOTE]
   >
   >   Het berekenen van de Handoff Datum van een opvolgertaak die op de Ware Datum van Voltooiing of een voorgangertaak wordt gebaseerd is het zelfde of voorganger wordt afgedwongen of niet. Voor meer informatie over gedwongen predecessors, zie [Voorgangers afdwingen](../use-prdcssrs/enforced-predecessors.md).


* **Als de taak geen voorganger heeft en**:

   * **De geplande begindatum ligt in het verleden**: De afhandelingsdatum is gelijk aan de geplande begindatum van het project.
   * **De geplande begindatum is in de toekomst (elke datum na de huidige datum)**: De afhandelingsdatum is gelijk aan de geplande begindatum van het project.

>[!NOTE]
>
>Wanneer de taak een dwars-projectvoorganger heeft, berekent de handoff datum van de opvolger slechts wanneer één van beiden van het volgende voorkomt:
>
>* U berekent manueel de chronologie van het project van de opvolger opnieuw. U moet over beheerdersmachtigingen voor het project beschikken om de tijdlijn opnieuw te berekenen.
>* De tijdlijn van het project van de opvolger wordt automatisch &#39;s nachts opnieuw berekend.
>
>Voor informatie over het opnieuw berekenen van de tijdlijn van het project raadpleegt u [Projecttijdlijnen opnieuw berekenen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Wanneer de taak een gedwongen beperking voor de Geplande Datums heeft**: De afhandelingsdatum is altijd dezelfde als de datum die door de beperking wordt ingesteld, ongeacht enige andere voorwaarde.\
   De volgende taken zijn geforceerde beperkingen:

   * Moet beginnen op
   * Moet worden voltooid op
   * Niet eerder starten dan
   * Niet later starten dan
   * Vaste datum

## De Handoff-datum zoeken

U kunt de Handoff Datum van een taak in een taakrapport of de mening van een taaklijst tonen.\
Ga voor meer informatie over het samenstellen van een rapport naar [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
