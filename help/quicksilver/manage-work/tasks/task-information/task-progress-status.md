---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Status voortgang taak
description: Adobe Workfront bepaalt de Voortgangsstatus van een taak door de vooruitgang van de taak over zijn chronologie te bekijken. U kunt Workfront vormen om de Voorwaarde van een project te bepalen dat op de waarde van de Status van de Voortgang van de taken wordt gebaseerd. Voor meer informatie over het vormen van de Voorwaarde van het project, zie het artikelOverzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Overzicht van status voortgang taak

<!-- Audited: 1/2024 -->

Adobe Workfront bepaalt de Voortgangsstatus van een taak door de vooruitgang van de taak over zijn chronologie te bekijken. U kunt Workfront vormen om de Voorwaarde van een project te bepalen dat op de waarde van de Status van de Voortgang van de taken wordt gebaseerd. Voor meer informatie over het vormen van de Voorwaarde van het project, zie het artikel [ Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project ](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Criteria die de status van de voortgang van taken bepalen

Voor informatie over de Voortgangsstatus van een project, zie [ Overzicht van de Status van de Voortgang van het Project ](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Voor informatie over het volgen van de vooruitgang van uw taken, zie [ het Traceren van de Wijze overzicht van de Taak ](../../../manage-work/tasks/task-information/task-tracking-mode.md).

De volgende criteria bepalen de Voortgangsstatus van een taak:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Status van de Voortgang </strong> </p> </th> 
   <th> <p><strong> het Bepalen Criteria </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong> op Tijd </strong> </p> </td> 
   <td scope="col"> <p>Een taak wordt beschouwd als <strong> op Tijd </strong> wanneer alle Geplande Datums de Geprojecteerde Datums aanpassen. Deze status van de voortgang kan er ook toe leiden dat het project op schema ligt en dat de geplande data vóór de geplande data liggen.</p> <p>Voor meer informatie over Geprojecteerde Datums, zie <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref"> Overzicht van de Geprojecteerde Datum van de Voltooiing voor projecten, taken, en kwesties </a>.</p> <p>Raadpleeg de volgende artikelen voor meer informatie over de geplande voltooiingsdatum voor taken:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref"> Overzicht van de taak Geplande Datum van het Begin </a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref"> Overzicht van de taak Geplande Datum van de Voltooiing </a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong> Bij Risico </strong> </p> </td> 
   <td><p>Een taak wordt beschouwd als <strong> bij risico </strong> wanneer de Geschatte Datum van de Voltooiing later is dan de Geplande Datum van de Voltooiing en later dan de Verwachte Datum van de Voltooiing. Dit kan gebeuren wanneer een taak een beperking van <strong> heeft op </strong> moet beëindigen of <strong> moet </strong> beginnen maar het percentage voltooit of de voorgangersverhoudingen van de taak tonen dat het niet op de gespecificeerde data kan beëindigen of beginnen. </p><p> Het plaatsen van de Beperking van de Taak aan <strong> moet op </strong> manueel beëindigen plaatst de Geplande Datum van de Voltooiing aan een specifieke datum. In dit geval komt de voorspelde Voltooiingsdatum overeen met de geplande Voltooiingsdatum. In het geval van deze beperking, analyseert Workfront de taak om te berekenen wanneer het zal eindigen gebaseerd op het voltooide percentage. Deze berekening wordt opgeslagen als de geschatte vervaldatum. Als de geschatte vervaldatum na de verwachte afsluitende datum ligt, bestaat het risico dat de taak te laat wordt uitgevoerd. </p> <p> Het plaatsen van de Beperking van de Taak aan <strong> moet </strong> manueel beginnen plaatst de Geplande Datum van het Begin aan een specifieke datum. De voorspelde begindatum komt in dit geval overeen met de geplande begindatum. In het geval van deze beperking, analyseert Workfront de taak om te berekenen wanneer het op zijn vroegere verhoudingen zal beginnen. Deze berekening wordt opgeslagen als de geschatte begindatum. Als er een gedwongen voorganger is die de taak niet op de gespecificeerde Datum van het Begin toelaat te beginnen, dan kan de Geschatte Datum van het Begin na de Verwachte Datum van de Voltooiing zijn. De taak dreigt te worden vertraagd. </p> <p>Nota: Typisch, aanpassen de Geschatte Data Geprojecteerde Data behalve wanneer <strong> moet beginnen op </strong> of <strong> op </strong> worden gebruikt. In deze gevallen blijven de geschatte datums berekenen op basis van het percentage complete en andere factoren (eerdere relaties), terwijl de voorspelde datums moeten overeenkomen met de geplande datums die handmatig zijn ingesteld.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Achter </strong> </p> </td> 
   <td> <p>Een taak wordt beschouwd om <strong> achter </strong> te zijn wanneer de Geschatte Datum van de Voltooiing later of gelijk is dan de Geplande Datum van de Voltooiing en vroeger dan de Verwachte Datum van de Voltooiing.</p> <p>De verwachte Voltooiingsdatum is een mening in real time van wanneer de taak zal worden voltooid gebaseerd op voorafgaande vooruitgang. Hoewel de taak te laat is opgestart, wordt deze nog niet als te laat beschouwd, omdat de geplande en verwachte einddatum nog in de toekomst ligt en de taak misschien nog op tijd zal zijn voltooid.</p> <p>Nota: <strong> Achter </strong> en <strong> bij de status van de Voortgang van het Risico </strong> zijn bijna identiek. Nochtans, <strong> Op risico </strong> wijst op er sommige gedwongen de Beperkingen van de Taak (moet eindigen, moet beginnen, Vaste Datums) op één of beide Geplande Datums). Als er geen gedwongen beperkingen op de taak zijn, zijn de verwachte data gelijk aan de geschatte data en weerspiegelen de systeemberekening van de voltooiingsdatum op basis van de huidige voortgang van de taak. De taak wordt nog niet als laat beschouwd, omdat de geplande en geplande einddatum nog in de toekomst ligt en de taak misschien nog op tijd zal zijn voltooid.<br> voor meer informatie over de Geprojecteerde en Geschatte Datums, zie <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref"> Overzicht van Geprojecteerde en Geschatte Datums </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> laat </strong> </p> </td> 
   <td> <p>Een taak is Late <strong> wanneer de Geplande Datum van de Voltooiing vóór de datum van vandaag is.</strong><br></p> </td> 
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
