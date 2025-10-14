---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Overzicht van het type duur: Eenvoudig'
description: Het eenvoudige Type van Duur is een Type van Duur dat u voor een taak in Adobe Workfront kunt plaatsen.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Overzicht van het type duur: Eenvoudig

<!-- Audited: 5/2025 -->

Het type eenvoudige duur is een type duur dat u voor een taak in Adobe Workfront kunt instellen. Voor meer informatie over duurtypes in Workfront, zie [&#x200B; Overzicht van het Type van Duur en van de Duur van de Taak &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overzicht van het eenvoudige Duur Type

Uw Workfront of groepsbeheerder kan het standaardduurtype van uw systeem of groep instellen als Eenvoudig. In dit geval worden alle nieuwe taken gemaakt met dit type duur.

Voor informatie over het veranderen van uw taak en geef voorkeur uit als deel van uw systeem-niveau of groep-vlakke projectvoorkeur uit, zie [&#x200B; systeembrede taak en uitgiftevoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

De volgende zaken komen voor wanneer een taak een Eenvoudig duurtype heeft:

* De managers van het project kunnen zowel de Duur als de Geplande Uren van een taak wijzigen wanneer het wijzigen van hoe die uren onder toegewezen personen zouden moeten worden verdeeld.

  Voor informatie, zie [&#x200B; de Geplande Uren en Duur van een taak met een Eenvoudig Type van Duur &#x200B;](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md) bijwerken.

  >[!IMPORTANT]
  >
  >Wanneer u eerst een taak creeert en het het Eenvoudige duurtype toewijst maar geen Duur specificeert, berekent Workfront de duur van de taak die op de hoeveelheid Geplande Uren u voor de taak specificeert. Als u de duur van een eenvoudige taak van de Duur manueel wijzigt, houdt Workfront op aanpassend de Geplande Uren aan de duur omdat het veronderstelt u hen manueel wilt bepalen.
  >
  >Workfront berekent de duur van taken waarvan de duur niet handmatig is gewijzigd met de volgende formule:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Uw Workfront-beheerder definieert de `Typical hours per work day` in het gedeelte Projectvoorkeuren van de Setup van uw instantie.

* Het toewijzingspercentage is verborgen, maar de toewijzingstijden kunnen worden bewerkt.
* Alle nieuwe klanten hebben het systeem-vlakke Type van Duur dat aan Eenvoudig wordt geplaatst.

## Wijzig het Duur Type van een taak in Eenvoudig

Voor informatie over het veranderen van het Type van Duur van een taak, zie [&#x200B; het Type van Duur van een taak &#x200B;](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md) bijwerken.

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
