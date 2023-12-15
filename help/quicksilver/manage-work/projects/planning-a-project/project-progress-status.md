---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van voortgang van project
description: Adobe Workfront bepaalt de Voortgangsstatus van een project door de vooruitgang van het project over zijn chronologie te bekijken. U kunt Workfront vormen om de Voorwaarde van een project te bepalen dat op de waarde van de Status van de Voortgang van de taken wordt gebaseerd. Meer informatie over de status van projectvoortgang vindt u in dit artikel.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Overzicht van voortgang van project

<!--Audited: 12/2023-->

Adobe Workfront bepaalt de Voortgangsstatus van een project door de vooruitgang van het project over zijn chronologie te bekijken. U kunt Workfront vormen om de Voorwaarde van een project te bepalen dat op de waarde van de Status van de Voortgang van de taken wordt gebaseerd. Voor meer informatie over het vormen van de Voorwaarde van het project, zie het artikel [Overzicht van het type Projectvoorwaarde en Voorwaarde](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Hieronder vindt u de stand van de projecten in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Op tijd</td> 
   <td> De status van een project voortgang is <strong>Op tijd</strong> if:<ul><li>Als zowel de verwachte als de geschatte voltooiingsdata eerder zijn dan of gelijk zijn aan de geplande uitvoeringsdatum van het project</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Risico</td> 
   <td> De status van een project voortgang is <strong>Risico</strong> indien <strong>alles</strong> van de volgende punten zijn waar:<ul><li>Zowel de geschatte als de verwachte voltooiingsdata zijn in de toekomst</li><li> Zowel de geschatte als de voorspelde voltooiingsdatums zijn later dan de geplande voltooiingsdatum</li><li> De geschatte voltooiingsdatum valt later dan de verwachte afsluitdatum</li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Achter</td> 
   <td> De status van een project voortgang is <strong>Achter</strong> indien <strong>alles</strong> van de volgende punten zijn waar:<ul><li>Zowel de geschatte als de verwachte voltooiingsdata zijn in de toekomst</li><li> Zowel de geschatte als de verwachte voltooiingsdata zijn later dan de geplande uitvoeringsdatum van het project</li><li> De geschatte voltooiingsdatum is niet later dan de verwachte afsluitdatum</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Late</td> 
   <td> 
     De status van een project voortgang is <strong>Late</strong> indien <strong>ofwel</strong> van de volgende punten zijn waar:<ul><li>Het project is voltooid en de datum waarop het daadwerkelijk is voltooid is later dan de geplande datum van voltooiing <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Het project is niet voltooid en de geplande einddatum van het project is in het verleden <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Overweeg het volgende:

* De verwachte afsluitende datum van het project wordt bepaald door de taak op het kritieke pad met de meest recente geplande afwerkingsdatum.
* De geschatte uitvoeringsdatum van het project wordt bepaald door de taak op het kritieke pad met de meest recente geschatte uitvoeringsdatum.

Voor informatie over het project Kritieke Weg, zie [Overzicht van het project Kritieke Weg](../../../manage-work/tasks/manage-tasks/critical-path.md).

Voor informatie over de Geprojecteerde Datums van de Voltooiing, zie [Overzicht van de geplande afsluitdatum voor projecten, taken en problemen](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
