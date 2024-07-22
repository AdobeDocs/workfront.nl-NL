---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van verwachte en geschatte data
description: Er zijn verschillende soorten datums die de tijdlijn van taken weergeven tussen het moment waarop ze kunnen starten en het moment waarop ze kunnen worden voltooid.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Overzicht van verwachte en geschatte data

<!--Audited: 07/2024-->

Er zijn verschillende soorten datums die de tijdlijn van taken weergeven tussen het moment waarop ze kunnen starten en het moment waarop ze kunnen worden voltooid. Hier volgen enkele datums die de tijdlijn van taken weergeven:

* Geplande begin- en geplande einddatum
* Geprojecteerde begin- en verwachte einddatum
* Geschatte aanvangs- en geschatte vervaldata
* Feitelijke begin- en einddatum

In dit artikel worden de verschillen beschreven tussen de geraamde en de geraamde data voor projecten.

Wanneer de taak voor het eerst wordt gemaakt, moeten de geplande, geprojecteerde en geschatte datums overeenkomen. Er zijn enkele uitzonderingen.

Voor meer informatie over het project, de taak, en de uitgiftedata in Adobe Workfront, zie [ Overzicht van het Project, de Taak, en de data van de Uitgave in Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Overzicht van geplande datums

De geplande datums zijn de datums die de eigenaar van het project definieert als de begin- en einddatum van de taken. U of de Eigenaar van het Project kunt de Geplande Data op een taak manueel wijzigen.

## Overzicht van werkelijke datums

Wanneer een taak voor het eerst wordt gemaakt, heeft deze geen werkelijke datums omdat deze nog niet is gestart of voltooid.

## Overzicht van verwachte en geschatte data

Tijdens de looptijd van een project zijn de verwachte en geraamde data meer in overeenstemming met de realiteit van het project, aangezien zij rekening houden met wat van invloed kan zijn op het eigenlijke begin en einde van een taak. Hierdoor veranderen ze van de geplande datums.

Houd rekening met het volgende wanneer u werkt met Geprojecteerde en Geschatte datums voor taken:

* U kunt noch de Geschatte noch de Geprojecteerde Datums van taken manueel wijzigen. Ze worden allebei door Adobe Workfront berekend.
* Wanneer u een taak maakt, moeten de geplande en geschatte datums identiek zijn en moeten deze de werkelijke tijden illustreren waarop de taken kunnen beginnen of eindigen.\
  Bepaalde updates die u aanbrengt in taken, zijn rechtstreeks van invloed op de waarden van de Geprojecteerde en Geschatte datums.

  Als de gebruiker bijvoorbeeld een taak start of voltooit, geeft de taak de werkelijke begin- en einddatum weer die van invloed zijn op de geplande en geschatte datum van de taak. Ook, als een toegewezen op de taak de Vastlegdatum wijzigt, beïnvloedt deze datum de Geplande Datum van de taak.

## Verschil tussen Geprojecteerde en Geschatte data

Het verschil tussen de voorspelde en de geschatte datums is:

* De voorspelde Datums worden beïnvloed door een gebruiker die de volgende updates op de taak uitvoert:

   * Voeg een Datum van de Beperking toe door een vaste Beperking van de Taak toe te voegen
   * Toewijzingsdatum toevoegen

* Bij de geschatte data wordt alleen rekening gehouden met de werkelijke voortgang van een taak op een bepaald tijdstip.

**Voorbeeld:** als wij een taak hebben die een Geplande Datum van het Begin van 20 september en een Geplande Voltooiingsdatum van 24 september heeft, en het op Beperking moet beëindigen, de Verwachte Datum van de Voltooiing 24 september. Deze taak duurt 4 dagen.

De geschatte datum van voltooiing wordt berekend op basis van de huidige voortgang van de werkzaamheden. Dus als vandaag 23 september is en de taak nog niet is begonnen, is de geschatte Voltooiingsdatum 27 september (deze moet na vier dagen worden voltooid, ervan uitgaande dat het werk vandaag van start gaat).

Als de taak vandaag voor 50% is voltooid, is de geschatte Voltooiingsdatum op 25 september (deze moet na twee dagen worden voltooid, de helft van de Duur van de taak).


### Begrijp wanneer de Geprojecteerde Datums op taken bijwerken {#understand-when-projected-dates-update-on-tasks}

De geprojecteerde data kunnen ofwel overeenkomen met andere taakdata, ofwel zijn het een berekening van Workfront die rekening houdt met de reële voortgang van de taak.

De volgende lijst toont verscheidene scenario&#39;s wanneer de Geprojecteerde Datums van taken tijdens het leven van een project afhankelijk van wat in echt aan de taak gebeurt worden veranderd:

* Als een taak is gemarkeerd als Voltooid:

  `Projected Dates = Estimated Dates = Actual Dates`

* Wanneer een taak een Werkelijke Datum van het Begin heeft:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* Wanneer een taak geen Werkelijke Datum van het Begin heeft, maar er een gedwongen beperking op de Geplande Datum van het Begin (moet beginnen) is die in de toekomst is:

  `Projected Start Date = Constraint Date`

  Voor informatie over de Datum van de Beperking, zie [ Verklarende woordenlijst van de terminologie van Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Wanneer een taak geen Werkelijke Datum van het Begin heeft en de taak geen gedwongen beperkingsdatum heeft:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* Wanneer de toegewezen persoon de datum van vastleggen bijwerkt:

  `Projected Completion Date = Commit Date`

  Voor informatie over Vastlegdatum, zie [ Overzicht van de Datum van het Vastleggen ](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Wanneer de taak geen bijgewerkte Vastlegdatum heeft en de taak een gedwongen beperking (moet beëindigen) voor de Geplande Voltooiingsdatum heeft die in de toekomst is:

  `Projected Completion Date = Constraint Date`

* Wanneer een taak geen bijgewerkte Vastlegdatum, een gedwongen beperkingsdatum in de toekomst heeft, of het heeft een Datum van de Beperking in het verleden:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Begrijp wanneer de Geschatte Data op taken bijwerken {#understand-when-the-estimated-dates-update-on-tasks}

In vergelijking met de hierboven beschreven scenario&#39;s voor de Geprojecteerde Datums, weerspiegelen de Geraamde Datums altijd een echte analyse van Workfront van wanneer de taak zal beginnen of voltooien ongeacht de Beperkte of Vastleggingsdata.

## Wat beïnvloedt de chronologie van een taak

Hieronder volgen enkele voorbeelden van wat de werkelijke tijdlijn van een taak kan beïnvloeden:

* Voortgang van de taak ten opzichte van de geplande data en de huidige dag
* Percentage voltooide taken tot nu toe
* Voorlopige relatie
* Voortgang van voorgaande
* Gebruikerstoewijzing

  >[!NOTE]
  >
  >De toewijzing van de gebruiker kan de Geschatte VoltooiingsDatum van een taak beïnvloeden als zij de snelheid beïnvloeden waarmee de taak kan worden voltooid. Als het type duur van de taak bijvoorbeeld is ingesteld op Beweven door inspanning, kunt u de taak eerder voltooien door toewijzingen toe te voegen. Als gevolg hiervan verandert de geschatte Voltooiingsdatum.
