---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Overzicht van het type duur: eenvoudig'
description: Het eenvoudige Type van Duur is een Type van Duur dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie Overzicht van het Type van Duur en van de Duur van de Taak.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Overzicht van het type duur: Eenvoudig

Het eenvoudige Type van Duur is een Type van Duur dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overzicht van het eenvoudige Duur Type

Uw Workfront of een groepsbeheerder kan het standaardtype Duur van uw systeem of groep instellen als Eenvoudig. In dit geval, zullen alle nieuwe taken met dit Type van Duur worden gecreeerd. Voor informatie over het veranderen van uw taak en geef voorkeur uit als deel van uw systeem-niveau of groep-vlakke projectvoorkeur uit, zie [ systeembrede taak en uitgiftevoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

De volgende dingen komen voor wanneer een taak een Type van Duur van Eenvoudig heeft:

* De managers van het project kunnen zowel de Duur als de Geplande Uren van een taak wijzigen wanneer het wijzigen van hoe die uren onder toegewezen personen zouden moeten worden verdeeld.

  Voor informatie, zie [ de Geplande Uren en Duur van een taak met een Eenvoudig Type van Duur ](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md) bijwerken.

  >[!IMPORTANT]
  >
  >Wanneer u eerst een taak creeert en het Eenvoudige Type van Duur aan het toewijst en geen Duur specificeert, berekent Workfront de Duur van de taak die op de hoeveelheid Geplande Uren wordt gebaseerd u voor de taak specificeert. Als u manueel de Duur van een Eenvoudige taak van de Duur wijzigt, houdt Workfront op aanpassend de Geplande Uren aan de Duur omdat het veronderstelt u hen manueel wilt bepalen zelf.
  >
  >Workfront berekent de duur van taken waarvan de duur niet handmatig is gewijzigd met de volgende formule:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Uw Workfront-beheerder definieert de `Typical hours per work day` in het gedeelte Projectvoorkeuren van de Setup van uw instantie.

* Het toewijzingspercentage is verborgen en de toewijzingstijden kunnen worden bewerkt.
* Alle nieuwe klanten hebben het systeem-vlakke Type van Duur dat aan Eenvoudig wordt geplaatst.

## Wijzig het Duur Type van een taak in Eenvoudig

Voor informatie over het veranderen van het Type van Duur van een taak, zie [ het Type van Duur van een taak ](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md) bijwerken.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
