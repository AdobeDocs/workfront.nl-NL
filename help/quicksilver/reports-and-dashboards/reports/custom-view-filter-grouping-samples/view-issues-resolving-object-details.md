---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Bekijken: problemen met het oplossen van objectdetails'
description: Deze probleemweergave toont de naam en het voltooide percentage van het oplossende object van het probleem, waardoor de initiator van het probleem inzicht heeft in de voortgang van het probleem, zelfs zonder toegang tot de oplossende taak of het project.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Weergave: problemen met het oplossen van objectdetails

Deze probleemweergave toont de naam en het voltooide percentage van het oplossende object van het probleem, waardoor de initiator van het probleem inzicht heeft in de voortgang van het probleem, zelfs zonder toegang tot de oplossende taak of het project.

Deze weergave gebruikt de

```
sharecol=true
```

Tag om meerdere velden onder dezelfde kolomkop te combineren. Voor meer informatie over de

```
sharecol
```

tag, zie [Weergave: informatie uit meerdere kolommen samenvoegen in één gedeelde kolom ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Willekeurig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties van toegangsniveaus*</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken om een rapport te wijzigen</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of er aanvullende beperkingen zijn ingesteld voor uw toegangsniveau. Zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> voor informatie over hoe een Workfront-beheerder uw toegangsniveau kan wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p> <p>Zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten </a> aanvragen voor informatie over het aanvragen van aanvullende toegang.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder als u wilt weten welk plan, licentietype of toegang u hebt.

## Problemen met het oplossen van objectdetails weergeven

1. Ga naar een lijst met problemen.
1. Selecteer in het vervolgkeuzemenu **Weergave** **Nieuwe weergave**.

1. In het gebied **Column Preview** verwijdert u alle kolommen behalve één.
1. Klik op de kop van de resterende kolom en klik vervolgens op **Schakelen naar tekstmodus**.
1. Beweeg de muisaanwijzer over het tekstmodusgebied en klik op **Klik om tekst** te bewerken.
1. Verwijder de tekst die u in het vak **Tekstmodus** vindt en vervang deze door de volgende code:<pre>column.0.querysort=name</pre><pre>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=sourceobject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject).HTML(name)<br>column.1.namekey=sourceobject.abbr<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=referenceObject:name<br>column.1.valueformat=HTML<br>column.1.viewalias=source<br>column.1.width=100<br>column.2.descriptionkey=assignedto<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=assignedTo:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=assignedTo:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo).string(name)<br>column.2.namekey=assignedto<br>column.2.querysort=assignedTo:name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=assignedTo:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=entryDate<br>column.3.valueformat=atDate<br>column.3.width=150<br>column.4.descriptionkey=description<br>column.4.linkedname=direct<br>column.4.listsort=string(description)<br>column.4.namekey=description.abbr<br>column.4.querysort=description<br>column.4.shortview=false<br>column.4.stretch=75<br>column.4.valuefield=description<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listsort=string(status)<br>column.5.namekey=status.abbr<br>column.5.querysort=status<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.type=enum<br>column.5.valuefield=status<br>column.5.valueformat=val<br>column.5.width=150<br>column.6.displayname=Resolving Object Name<br>column.6.linkedname=resolveTask<br>column.6.namekey=view.relatedcolumn<br>column.6.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column.6.querysort=resolveTask:name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valuefield=resolveTask:name<br>column.6.valueformat=HTML<br>column.7.displayname=<br>column.7.linkedname=resolveOpTask<br>column.7.namekey=view.relatedcolumn<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask:name<br>column.7.sharecol=true<br>column.7.textmode=true<br>column.7.valuefield=resolveOpTask:name<br>column.7.valueformat=HTML<br>column.8.displayname=<br>column.8.linkedname=resolveProject<br>column.8.namekey=view.relatedcolumn<br>column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject:name<br>column.8.textmode=true<br>column.8.valuefield=resolveProject:name<br>column.8.valueformat=HTML<br>column.9.displayname=Resolving Object Percent Complete<br>column.9.textmode=true<br>column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},&#39;&#39;))<br>column.9.valueformat=doubleAsPercentRounded</pre>

1. Klik op **Weergave opslaan**.
