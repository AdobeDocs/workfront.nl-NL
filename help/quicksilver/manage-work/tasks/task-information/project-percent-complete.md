---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Projectpercentage voltooid overzicht
description: De volledige waarde van Percentage van een project wordt berekend gebaseerd op of de Geplande Duur of de Geplande Uren van taken in het project. Uw beheerder van Adobe Workfront of een groepsbeheerder bepaalt welke waarde in rekening wordt gebracht wanneer het berekenen van percent volledig in uw systeem wanneer zij informatie in het gebied van de Voorkeur van het Project vormen. Voor informatie over het vormen van projectvoorkeur, zie systeem-brede projectvoorkeur vormen.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

# Overzicht van projectpercentage voltooid

<!-- Audited 01/2024 -->

De volledige waarde van Percentage van een project wordt berekend gebaseerd op of de Duur of Geplande Uren van taken in het project. Uw beheerder van Adobe Workfront of een groepsbeheerder bepaalt welke waarde in rekening wordt gebracht wanneer het berekenen van percent volledig in uw systeem wanneer zij informatie in het gebied van de Voorkeur van het Project vormen.

Voor informatie over het vormen van projectvoorkeur, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

Percentage voltooid van een oudertaak is gebaseerd op de Duur of Geplande Uren van elk van zijn subtaken.

Evenzo is de Percentage voltooiing van een project gebaseerd op de duur of de geplande uren van elke hoofdtaak in het project.

De belangrijkste taken zijn de oudertaken en de standalone taken die geen kinderen hebben.

>[!TIP]
>
>De belangrijkste taken zijn niet gekarteld in een projectplan.

## Hoe Workfront het percentage voltooit berekent

### Het percentage van een taak bijwerken voltooid {#update-the-percent-complete-on-a-task}

U kunt het percentage van een taak handmatig wijzigen. Dit is geen berekening.

Workfront gebruikt het percentage voltooide van een individuele taak om het percentage te berekenen voltooit van zijn oudertaak of het percentage voltooide van het project.

Voor informatie over het bijwerken van het percentage voltooide van een taak, zie [&#x200B; Mening en werk Percentage bij Voltooid voor taken &#x200B;](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Hoe Workfront Percentage voltooide op een bovenliggende taak berekent {#how-workfront-calculates-percent-complete-on-a-parent-task}

Afhankelijk van wat uw Workfront of groepsbeheerder in de Voorkeur van het Project op het systeem of groepsniveau selecteerde, wordt het percentage volledig voor een oudertaak berekend of gebaseerd op de Duur of de Geplande Uren van taken.

Overweeg de volgende scenario&#39;s:

* Als het systeem het percentage voltooide op Geplande Uren berekent, wordt het voltooide van de oudertaak berekend gebruikend de volgende formule:

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  De totale geplande uren van de ouder vertegenwoordigen de som van alle Geplande Uren van elk van de kinderen.

  ![&#x200B; Project met taken voltooide en geplande uren &#x200B;](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Als het systeem het volledige percentage op de Duur baseert berekent, wordt het voltooide percentage van de oudertaak berekend gebruikend de volgende formule:

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![&#x200B; Project met taken voltooide en duurberekening &#x200B;](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >De totale Duur van de Ouderlijke Taak is het totaal van alle duur van de kindtaken. Bijvoorbeeld, heeft een oudertaak met twee kinderen die een respectieve Duur van 1 Dag en 2 Dagen hebben een Totale Duur van 3 Dagen, zelfs wanneer de twee kinderen op de zelfde dag kunnen beginnen.


### Hoe Workfront het percentage voltooide projecten berekent {#how-workfront-calculates-percent-complete-on-a-project}

Afhankelijk van wat uw Workfront of groepsbeheerder in de Voorkeur van het Project op het systeem of groepsniveau selecteerde, wordt het percentage volledig voor een project berekend of gebaseerd op de Duur of de Geplande Uren van de belangrijkste taken op het project.

* Als het systeem het volledige percentage op Geplande Uren berekent, wordt het volledige projectpercentage berekend gebruikend de volgende formule:

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  De totale geplande uren van het project zijn de som van de geplande uren van alle hoofdtaken van het project.

  ![&#x200B; Project met taken voltooide en geplande urenberekening &#x200B;](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >Taak 1 of Taak 2 kan oudertaken of standalone taken slechts zijn. De geplande uren en het Percentage voltooide kindertaken worden niet gebruikt in deze berekening.

* Als het systeem het volledige percentage op de Duur baseert berekent, wordt het volledige projectpercentage berekend gebruikend de volgende formule:

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >De duur van het Project is het totaal van alle duur van de belangrijkste taken die een volledig percentage tonen. Bijvoorbeeld, zal een project met een standalone taak met een Duur van 2 Dagen en een oudertaak met een Duur van 5 Dagen die het werk hebben voltooid aan hen een Totale Duur van 7 Dagen hebben, zelfs als de twee taken op de zelfde dag kunnen beginnen.

  ![&#x200B; Project met taken voltooide en duurberekening &#x200B;](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >Taak 1 of Taak 2 kan oudertaken of standalone taken slechts zijn. De Duur en Percentage Voltooien van kindtaken worden niet gebruikt in deze berekening.

## Voorbeeld van Percentage voltooid op een project dat Duur gebruikt

Wanneer het gebruiken van de Duur van de taken om het percentage te berekenen voltooit van een project, overweeg het volgende voorbeeld:

![&#x200B; Project met taken voltooide en duurberekening &#x200B;](assets/project-with-tasks-percent-complete-duration-calculation.png)

De volgende informatie wordt gebruikt om het percentage van voltooiing van het project te berekenen

* Het percentage voltooide van de standalone taak (Taak 1 - 20%)
* Het percentage voltooide van de oudertaak (Taak 2 - 25%)
* De duur van Taak 1 (5 dagen)
* De duur van Taak 2 (2 dagen)
* Duur van het project (7 dagen)


Om het percentage te berekenen voltooide van het project gebruikend Duur:

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

of

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->
