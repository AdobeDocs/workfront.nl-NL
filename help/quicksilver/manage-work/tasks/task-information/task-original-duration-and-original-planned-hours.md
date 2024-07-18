---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van taak Oorspronkelijke Duur en Oorspronkelijke Geplande Uren
description: Als deel van het plannen van een project, zou u de waarden voor de Geplande Uren en voor de Duur (of Geplande Duur) van elke taak in het project moeten bepalen.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Overzicht van taak Oorspronkelijke Duur en Oorspronkelijke Geplande Uren

Als deel van het plannen van een project, zou u de waarden voor de Geplande Uren en voor de Duur (of Geplande Duur) van elke taak in het project moeten bepalen.

Voor meer informatie over Geplande Uren op taken, zie [ Gepland overzicht van Uren ](../../../manage-work/tasks/task-information/planned-hours.md).

Voor meer informatie over taakDuur, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

U kunt deze waarden weergeven op het tabblad Taakdetails of tijdens het bewerken van een taak.

Als u een mening voor een taaklijst of een taakrapport bouwt, kunt u de Originele Geplande Uren en de Originele gebieden van de Duur voor de taken extra zien.

## Oorspronkelijk geplande uren

De Oorspronkelijke Geplande Uren van een taak vertegenwoordigen het aantal Geplande Uren dat een taak oorspronkelijk had alvorens het een oudertaak werd. Wanneer een taak een oudertaak wordt, rollen de Geplande Uren van de kindtaken tot de oudertaak om op de Geplande Uren van de ouder te wijzen.

Als u het veld Oorspronkelijk geplande uren weergeeft in een taakrapport of in een lijst, ziet u het oorspronkelijke aantal geplande uren voordat de taak het aantal geplande uren van de onderliggende objecten heeft overgenomen.

>[!NOTE]
>
>Wanneer u een taak maakt, is het aantal Oorspronkelijke geplande uren nul. Als de taak een bovenliggende taak wordt, wordt de waarde van dit veld gevuld met het aantal geplande uren van de taak voordat deze wordt gewijzigd in een bovenliggende taak. Deze waarde blijft in dit veld staan, zelfs als de taak weer op zichzelf staat.

## Oorspronkelijke duur

De Originele Duur van een taak is de Duur die een taak oorspronkelijk had alvorens het een oudertaak, in notulen werd. Wanneer een taak een ouder wordt, rolt de Duur tussen de Geplande Datum van het Begin van het vroegste kind en de Geplande Datum van de Voltooiing van het laatste kind tot de oudertaak en wordt de Duur van de oudertaak. Dit vervangt de Duur van de originele taak.

Het tonen van het Originele gebied van de Duur in een taakrapport of een lijst kunt u het originele aantal dagen voor de Duur van de taak zien alvorens het de Duur van zijn kinderen erft.

>[!NOTE]
>
>Wanneer u een taak creeert, is de Oorspronkelijke Duur nul. Als de taak een oudertaak wordt, wordt de waarde van dit gebied bevolkt met de Duur van de taak alvorens het in een ouder werd veranderd. Deze waarde blijft in dit veld staan, zelfs als de taak weer op zichzelf staat. Deze waarde wordt in minuten weergegeven.

## Voorbeeld

Bijvoorbeeld, wanneer twee taken standalone taken zijn, zijn hun Oorspronkelijke Duur en Oorspronkelijke Geplande Uren nul.

![ original_scheduled_hours_and_duration_without_parent.png ](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Wanneer de eerste taak de ouder van de tweede taak wordt, worden de Originele Duur en Oorspronkelijke Geplande gebieden van Uren bevolkt met de waarden voor de Duur en Geplande Uren van de taak alvorens het een ouder werd. De originele Duur wordt getoond in notulen. De duur en de geplande uren van het kind worden de Duur en de Geplande Uren van de ouder.

![ original_and_scheduled_hours_with_a_parent_task.png ](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Wanneer de ouder een standalone taak opnieuw wordt, keren de Duur en Geplande Uren terug naar de originele waarden, terwijl de Oorspronkelijke Duur en de Oorspronkelijke Geplande Uren bevolkt blijven. Ze keren niet terug naar nul.

![ original_duration_and_scheduled_hours_after_reversal_of_a_parent.png ](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
