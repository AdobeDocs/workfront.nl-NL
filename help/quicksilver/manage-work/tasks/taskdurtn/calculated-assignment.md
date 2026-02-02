---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Type duur overzicht: berekende toewijzing'
description: Berekende toewijzing is een Duur Type dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie Overzicht van het Type van Duur en van de Duur van de Taak.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Overzicht duur: berekende toewijzing

<!-- Audited: 5/2025 -->

Berekende toewijzing is een Duur Type dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie [&#x200B; Overzicht van het Type van Duur en van de Duur van de Taak &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overzicht van het berekende Type van Duur van de Toewijzing

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Wanneer u een Berekend Type van Duur van de Taak gebruikt, moet u zowel een Duur als een aantal Geplande Uren voor de taak specificeren. Workfront verdeelt dan de hoeveelheid Geplande Uren door de hoeveelheid uren in de Duur, dan door het aantal middelen die aan de taak worden toegewezen om het toewijzingspercentage (berekent de taak) voor elke middel te berekenen. Elke bron heeft dezelfde waarde voor het toewijzingspercentage. In dit geval kunt u de toewijzingswaarden voor elke bron niet wijzigen.
* Uw Workfront of een groepsbeheerder kan het standaard Duur Type van uw systeem of groep als Berekende Toewijzing plaatsen. In dit geval, zullen alle nieuwe taken met dit Type van Duur worden gecreeerd. Voor informatie over het veranderen van uw taak en geef voorkeur uit als deel van uw systeem-niveau of groep-vlakke projectvoorkeur uit, zie [&#x200B; systeembrede taak en uitgiftevoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

  In dit geval, heeft de taak een gebrek van een Duur van één dag en een gebrek van 0 uren Geplande Uren. Tenzij de projectmanager een nauwkeurigere Duur plaatst en het Geplande gebied van Uren met een realistische raming bevolkt, dan lijken de middelen onderverdeeld.

De berekende Toewijzing is het aangewezen Type van Duur in de volgende situaties:

* Wanneer de taken een venster van activiteit hebben maar niet de volledige die Duur nemen wordt toegewezen om hun werk te voltooien. Bijvoorbeeld, wordt u toegewezen om een rapport aan uw supervisor tegen het eind van de week te leveren. U hebt een duur van vijf dagen, maar het duurt slechts tien uur om het document te maken.
* Wanneer één enkel middel aan een taak wordt toegewezen omdat de projectmanager de geplande Duur en de geplande hoeveelheid inspanning onafhankelijk van elkaar kan schatten.

  U kunt het Berekende Type van Duur van het Werk voor het zelfde resultaat gebruiken, maar de projectmanager moet een percentaletoewijzing voor het middel invoeren om de berekende waarde voor Geplande Uren te beïnvloeden. Dit maakt projectplanning moeilijker en tijdrovend.

Het toewijzingspercentage voor elke bron wordt als volgt berekend:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

In het onderstaande scenario heeft elke taak bijvoorbeeld een Duur van 3 dagen. De projectmanager voert handmatig zowel de Duur (3 dagen of 24 uur) als de Geplande Uren in, waardoor het toewijzingspercentage (of het toewijzingspercentage) wordt berekend:

![&#x200B; Berekend type van toewijzingsduur &#x200B;](assets/calcassign-350x80.png)

## Verander het Type van Duur van een taak in Berekende Taak

Voor informatie over het veranderen van het Type van Duur van een taak, zie [&#x200B; het Type van Duur van een taak &#x200B;](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md) bijwerken.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
