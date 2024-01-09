---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van status voortgang taak
description: Adobe Workfront bepaalt de Voortgangsstatus van een taak door de vooruitgang van de taak over zijn chronologie te bekijken. U kunt Workfront vormen om de Voorwaarde van een project te bepalen dat op de waarde van de Status van de Voortgang van de taken wordt gebaseerd. Voor meer informatie over het vormen van de Voorwaarde van het project, zie het artikelOverzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 70d173ca3781d8d143a66ce7e963dcaf66bece19
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Overzicht van status voortgang taak

<!-- Audited: 1/2024 -->

Adobe Workfront bepaalt de Voortgangsstatus van een taak door de vooruitgang van de taak over zijn chronologie te bekijken. U kunt Workfront vormen om de Voorwaarde van een project te bepalen dat op de waarde van de Status van de Voortgang van de taken wordt gebaseerd. Voor meer informatie over het vormen van de Voorwaarde van het project, zie het artikel [Overzicht van het type Projectvoorwaarde en Voorwaarde](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Criteria die de status van de voortgang van taken bepalen

Voor informatie over de Voortgangsstatus van een project, zie [Overzicht van voortgang van project](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Voor informatie over het volgen van de vooruitgang van uw taken, zie [Overzicht van de modus Taken bijhouden](../../../manage-work/tasks/task-information/task-tracking-mode.md).

De volgende criteria bepalen de Voortgangsstatus van een taak:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Voortgangsstatus</strong> </p> </th> 
   <th> <p><strong>Criteria bepalen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Op tijd</strong> </p> </td> 
   <td scope="col"> <p>Een taak wordt overwogen <strong>Op tijd</strong> wanneer alle geplande datums overeenkomen met de verwachte datums. Deze status van de voortgang kan er ook toe leiden dat het project op schema ligt en dat de geplande data vóór de geplande data liggen.</p> <p>Voor meer informatie over Geprojecteerde Datums, zie <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Overzicht van de geplande afsluitdatum voor projecten, taken en problemen</a>.</p> <p>Raadpleeg de volgende artikelen voor meer informatie over de geplande voltooiingsdatum voor taken:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overzicht van de geplande startdatum van de taak</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overzicht van de geplande voltooiing van de taak</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>Risico</strong> </p> </td> 
   <td><p>Een taak wordt overwogen <strong>Risico</strong> wanneer de geraamde Voltooiingsdatum later is dan de geplande Voltooiingsdatum en later dan de verwachte Voltooiingsdatum. Dit kan gebeuren wanneer een taak een beperking heeft van <strong>Moet worden voltooid op</strong> of <strong>Moet beginnen op</strong> maar het percentage voltooid of de voorgaande relaties van de taak laten zien dat het niet op de opgegeven datums kan worden voltooid of gestart. </p><p> Taakbeperking instellen op <strong>Moet worden voltooid op</strong> Hiermee stelt u de geplande voltooiingsdatum handmatig in op een bepaalde datum. In dit geval komt de voorspelde Voltooiingsdatum overeen met de geplande Voltooiingsdatum. In het geval van deze beperking, analyseert Workfront de taak om te berekenen wanneer het zal eindigen gebaseerd op het voltooide percentage. Deze berekening wordt opgeslagen als de geschatte vervaldatum. Als de geschatte vervaldatum na de verwachte afsluitende datum ligt, bestaat het risico dat de taak te laat wordt uitgevoerd. </p> <p> Taakbeperking instellen op <strong>Moet beginnen op</strong> Hiermee wordt de geplande begindatum handmatig ingesteld op een specifieke datum. De voorspelde begindatum komt in dit geval overeen met de geplande begindatum. In het geval van deze beperking, analyseert Workfront de taak om te berekenen wanneer het op zijn vroegere verhoudingen zal beginnen. Deze berekening wordt opgeslagen als de geschatte begindatum. Als er een gedwongen voorganger is die de taak niet op de gespecificeerde Datum van het Begin toelaat te beginnen, dan kan de Geschatte Datum van het Begin na de Verwachte Datum van de Voltooiing zijn. De taak dreigt te worden vertraagd. </p> <p>Opmerking: Gewoonlijk komen de geschatte datums overeen met de geprojecteerde datums, behalve wanneer <strong>Moet beginnen op</strong> of <strong>Moet worden voltooid op</strong> worden gebruikt. In deze gevallen blijven de geschatte datums berekenen op basis van het percentage complete en andere factoren (eerdere relaties), terwijl de voorspelde datums moeten overeenkomen met de geplande datums die handmatig zijn ingesteld.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Achter</strong> </p> </td> 
   <td> <p>Een taak wordt geacht <strong>Achter</strong> wanneer de geschatte Voltooiingsdatum later is of gelijk is aan de geplande Voltooiingsdatum en eerder dan de verwachte Voltooiingsdatum.</p> <p>De verwachte Voltooiingsdatum is een mening in real time van wanneer de taak zal worden voltooid gebaseerd op voorafgaande vooruitgang. Hoewel de taak te laat is opgestart, wordt deze nog niet als te laat beschouwd, omdat de geplande en verwachte einddatum nog in de toekomst ligt en de taak misschien nog op tijd zal zijn voltooid.</p> <p>Opmerking: De <strong>Achter</strong> en <strong>Risico</strong> Voortgangsstatussen zijn bijna identiek. Maar <strong>Risico</strong> Hiermee geeft u aan dat er op een of beide geplande datums bepaalde dwangtaakbeperkingen gelden (Moet voltooid zijn, Moet starten, Vaste datums). Als er geen gedwongen beperkingen op de taak zijn, zijn de verwachte data gelijk aan de geschatte data en weerspiegelen de systeemberekening van de voltooiingsdatum op basis van de huidige voortgang van de taak. De taak wordt nog niet als laat beschouwd, omdat de geplande en geplande einddatum nog in de toekomst ligt en de taak misschien nog op tijd zal zijn voltooid.<br>Voor meer informatie over de Geprojecteerde en Geschatte Data raadpleegt u <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Verschil tussen Geprojecteerde en Geschatte data </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Late</strong> </p> </td> 
   <td> <p>Een taak is <strong>Late</strong> wanneer de geplande datum van voltooiing vóór de datum van vandaag is.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->