---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Rapport: gecombineerde taak en weergave en groepering van problemen'
description: Dit rapport Werkitem toont zowel taken als problemen waarmee gebruikers hebben ingestemd in één rapport. Deze optie is het meest geschikt in combinatie met een aangepaste groepering.
author: Nolan
feature: Reports and Dashboards
exl-id: 6eaae772-229d-44ea-b285-cbaf9e46eade
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Rapport: gecombineerde taak en uitgave weergeven en groeperen

<!--Audited: 10/2024-->

Dit rapport Werkitem toont zowel taken als problemen waarmee gebruikers hebben ingestemd in één rapport. Deze optie is het meest geschikt in combinatie met een aangepaste groepering.

Dit rapport gebruikt `sharecol=true` in de weergave om meerdere velden onder dezelfde kolomkop te combineren. Voor meer informatie over de `sharecol` markering, zie [&#x200B; Mening: fusie informatie van veelvoudige kolommen in één gedeelde kolom &#x200B;](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

>[!TIP]
>
>  In de weergave Werkitem worden alleen taken en problemen weergegeven die zijn geaccepteerd door de gebruikers die aan hen zijn toegewezen. Dit rapport toont het werkpunten niet die niet van de Verzoeken van het Werk of de lijsten van de Verzoeken van het Team in het Werken van de gebruiker aan lijst zijn bewogen.

![&#x200B; work_item_report.png &#x200B;](assets/work-item-report-350x46.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bouw een rapport met gecombineerde taak en de Mening van de kwestie en Groepering

Om een rapport met dit standpunt op te stellen:

1. Klik het **pictogram van het 1&rbrace; Belangrijkste Menu ![&#x200B; pictogram van het Menu &#x200B;](assets/main-menu-icon.png) in de hoger-juiste hoek, of het** Belangrijkste pictogram van het Menu **pictogram ![&#x200B; Belangrijkste lijnen van het Menu &#x200B;](assets/lines-main-menu.png) in de upper-left hoek, als beschikbaar, dan klik** Rapporten **.**

1. Klik **Nieuw Rapport** > **Meer** > **Punt van het Werk** van het drop-down menu.

1. In het **gebied van de Voorproef van de Kolom**, klik de kopbal van de enige getoonde kolom. Dit is de **Ext Ref** kolom.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en de klik **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst die u in het tekstvak zoekt en vervang deze door de volgende code:

   ```
   column.0.description=Task or Issue 
   column.0.name=Issue or Task
   column.0.shortview=false
   column.0.stretch=0
   column.0.textmode=true
   column.0.type=image
   column.0.valueexpression=IF(ISBLANK({opTaskID}),'Task','Issue')
   column.0.valueformat=
   column.0.width=40
   column.1.description=Task or Issue Name
   column.1.isInlineEditable=false
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=task:ID
   column.1.link.linkproperty.0.valueformat=string
   column.1.link.lookup=link.view
   column.1.link.valuefield=task:objCode
   column.1.link.valueformat=val
   column.1.listsort=nested(task).string(name)
   column.1.name=Name
   column.1.sharecol=true
   column.1.shortview=false
   column.1.stretch=50
   column.1.textmode=true
   column.1.valuefield=task:name
   column.1.valueformat=HTML
   column.1.width=120
   column.2.isInlineEditable=false
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=opTask:ID
   column.2.link.linkproperty.0.valueformat=string
   column.2.link.lookup=link.view
   column.2.link.valuefield=opTask:objCode
   column.2.link.valueformat=val
   column.2.linkedname=opTask
   column.2.listsort=nested(opTask).string(name)
   column.2.shortview=false
   column.2.stretch=0
   column.2.textmode=true
   column.2.valuefield=opTask:name
   column.2.valueformat=HTML
   column.2.width=120
   column.3.description=Project Name
   column.3.isInlineEditable=false
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=task:projectID
   column.3.link.linkproperty.0.valueformat=string
   column.3.link.lookup=link.view
   column.3.link.valuefield=task:project:objCode
   column.3.link.valueformat=val
   column.3.listsort=nested(task).nested(project).string(name)
   column.3.name=Project Name
   column.3.sharecol=true
   column.3.shortview=false
   column.3.stretch=50
   column.3.textmode=true
   column.3.valuefield=task:project:name
   column.3.valueformat=HTML
   column.3.width=120
   column.4.isInlineEditable=false
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=opTask:projectID
   column.4.link.linkproperty.0.valueformat=string
   column.4.link.lookup=link.view
   column.4.link.valuefield=opTask:project:objCode
   column.4.link.valueformat=val
   column.4.linkedname=opTask
   column.4.listsort=nested(opTask).nested(project).string(name)
   column.4.shortview=false
   column.4.stretch=0
   column.4.textmode=true
   column.4.valuefield=opTask:project:name
   column.4.valueformat=HTML
   column.4.width=120
   column.5.displayname=Primary Assignee
   column.5.linkedname=assignment
   column.5.namekey=view.relatedcolumn
   column.5.namekeyargkey.0=assignment
   column.5.namekeyargkey.1=assignedToID
   column.5.querysort=assignment:assignedToID
   column.5.textmode=true
   column.5.valuefield=assignment:assignedTo:name
   column.5.valueformat=HTML
   column.6.displayname=Status
   column.6.enumclass=com.attask.common.constants.OpTaskStatusEnum
   column.6.enumtype=OPTASK
   column.6.linkedname=opTask
   column.6.namekey=view.relatedcolumn
   column.6.namekeyargkey.0=opTask
   column.6.namekeyargkey.1=status
   column.6.querysort=opTask:status
   column.6.sharecol=true
   column.6.textmode=true
   column.6.type=enum
   column.6.valuefield=opTask:status
   column.6.valueformat=val
   column.7.displayname=
   column.7.enumclass=com.attask.common.constants.TaskStatusEnum
   column.7.enumtype=TASK
   column.7.linkedname=task
   column.7.namekey=view.relatedcolumn
   column.7.namekeyargkey.0=task
   column.7.namekeyargkey.1=status
   column.7.querysort=task:status
   column.7.textmode=true
   column.7.type=enum
   column.7.valuefield=task:status
   column.7.valueformat=val
   column.8.displayname=Priority
   column.8.enumclass=com.attask.common.constants.TimelinePriorityEnum
   column.8.enumtype=OPTASK
   column.8.linkedname=opTask
   column.8.namekey=view.relatedcolumn
   column.8.namekeyargkey.0=opTask
   column.8.namekeyargkey.1=priority
   column.8.querysort=opTask:priority
   column.8.sharecol=true
   column.8.textmode=true
   column.8.type=enum
   column.8.valuefield=opTask:priority
   column.8.valueformat=val
   column.9.displayname=
   column.9.enumclass=com.attask.common.constants.TimelinePriorityEnum
   column.9.enumtype=TASK
   column.9.linkedname=task
   column.9.namekey=view.relatedcolumn
   column.9.namekeyargkey.0=task
   column.9.namekeyargkey.1=priority
   column.9.querysort=task:priority
   column.9.type=enum
   column.9.valuefield=task:priority
   column.9.valueformat=val
   column.10.isInlineEditable=false
   column.10.linkedname=task
   column.10.listsort=nested(task).atDateAsAtDate(plannedStartDate)
   column.10.name=Planned Start Date
   column.10.sharecol=true
   column.10.shortview=false
   column.10.stretch=0
   column.10.textmode=true
   column.10.valuefield=task:plannedStartDate
   column.10.valueformat=atDate
   column.10.width=100
   column.11.isInlineEditable=false
   column.11.linkedname=opTask
   column.11.listsort=nested(opTask).atDateAsAtDate(plannedStartDate)
   column.11.shortview=false
   column.11.stretch=0
   column.11.textmode=true
   column.11.valuefield=opTask:plannedStartDate
   column.11.valueformat=atDate
   column.11.width=1
   column.12.isInlineEditable=false
   column.12.linkedname=task
   column.12.listsort=nested(task).atDateAsAtDate(projectedCompletionDate)
   column.12.name=Planned Completion Date
   column.12.sharecol=true
   column.12.shortview=false
   column.12.stretch=0
   column.12.textmode=true
   column.12.valuefield=task:projectedCompletionDate
   column.12.valueformat=atDate
   column.12.width=100
   column.13.isInlineEditable=false
   column.13.linkedname=opTask
   column.13.listsort=nested(opTask).atDateAsAtDate(projectedCompletionDate)
   column.13.shortview=false
   column.13.stretch=0
   column.13.textmode=true
   column.13.valuefield=opTask:projectedCompletionDate
   column.13.valueformat=atDate
   column.13.width=1
   column.14.isInlineEditable=false
   column.14.linkedname=task
   column.14.listsort=nested(task).double(percentComplete)
   column.14.name=Percent Complete
   column.14.sharecol=true
   column.14.shortview=false
   column.14.stretch=0
   column.14.textmode=true
   column.14.valueexpression=IF(ISBLANK({taskID}),"",{task}.{percentComplete})
   column.14.valueformat=HTML
   column.14.width=100
   column.15.textmode=true
   column.15.value=
   column.15.valueformat=HTML
   column.15.width=1
   ```

1. Klik **Gedaan**.
1. (Facultatief) klik **Groepen** om een groepering aan het rapport toe te voegen.
1. (Facultatief en voorwaardelijk) als u een groepering toevoegt, klik **Schakelaar aan de Wijze van de Tekst**.
1. (Optioneel) Vervang de tekst binnen het gebied van de groeperingstekstmodus door de volgende code:

   ```
   group.0.name=
   group.0.valueexpression=IF(ISBLANK({opTaskID}),'Task','Issue')
   group.0.valueformat=string
   textmode=true
   ```

   Met deze groepering groepeert u alle taken en alle problemen samen.

1. Klik **sparen + Sluiten**.
1. (Optioneel) Werk de naam van het rapport bij en klik op **Toepassen** .
