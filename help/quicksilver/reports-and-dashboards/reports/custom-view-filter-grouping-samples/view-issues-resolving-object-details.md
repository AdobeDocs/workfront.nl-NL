---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: problemen met het oplossen van objectdetails'
description: In deze weergave worden de naam en het percentage weergegeven dat is voltooid met het object dat het probleem heeft opgelost, zodat de maker van het probleem inzicht heeft in de voortgang van het probleem, zelfs zonder toegang tot de taak of het project die het probleem heeft opgelost.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Weergave: problemen met het oplossen van objectdetails

In deze weergave worden de naam en het percentage weergegeven dat is voltooid met het object dat het probleem heeft opgelost, zodat de maker van het probleem inzicht heeft in de voortgang van het probleem, zelfs zonder toegang tot de taak of het project die het probleem heeft opgelost.

In deze weergave worden de

```
sharecol=true
```

-tag gebruiken om meerdere velden onder dezelfde kolomkop te combineren. Voor meer informatie over de

```
sharecol
```

tag, zie [Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Problemen met het oplossen van objectdetails weergeven

1. Ga naar een lijst met problemen.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:<pre>column.0.querysort=name</pre><pre>column.0.stretch=0<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionKey=sourceObject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject).HTML(name)<br>column.1.namekey=sourceObject.abbr<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=referenceObject:name<br>column.1.valueFormat=HTML<br>column.1.viewalias=source<br>column.1.width=100<br>column.2.descriptionkey=assign to<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=assignedTo:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=assignedTo:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo).string(name)<br>column.2.namekey=assigned to<br>column.2.querysort=assignedTo:name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valueField=assignedTo:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.descriptionKey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueField=entryDate<br>column.3.valueFormat=atDate<br>column.3.width=150<br>column.4.descriptionKey=description<br>column.4.linkedname=direct<br>column.4.listsort=string(description)<br>column.4.namekey=description.abbr<br>column.4.querysort=description<br>column.4.shortview=false<br>column.4.stretch=75<br>column.4.valueField=description<br>column.4.valueFormat=HTML<br>column.4.width=150<br>column.5.descriptionKey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listsort=string(status)<br>column.5.namekey=status.abbr<br>column.5.querysort=status<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.type=enum<br>column.5.valueField=status<br>column.5.valueFormat=val<br>column.5.width=150<br>column.6.displayName=Resolving Object Name<br>column.6.linkedname=resolveTask<br>column.6.namekey=view.related column<br>column.6.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column.6.querysort=resolveTask:name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valueField=resolveTask:name<br>column.6.valueFormat=HTML<br>column.7.displayName=<br>column.7.linkedname=resolveOpTask<br>column.7.namekey=view.related column<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask:name<br>column.7.sharecol=true<br>column.7.textmode=true<br>column.7.valueField=resolveOpTask:name<br>column.7.valueFormat=HTML<br>column.8.displayName=<br>column.8.linkedname=resolveProject<br>column.8.namekey=view.related column<br>column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject:name<br>column.8.textmode=true<br>column.8.valueField=resolveProject:name<br>column.8.valueFormat=HTML<br>column.9.displayName=Resolving Object Percent Complete<br>column.9.textmode=true<br>column.9.valueexpression=IF (ISBLANK({resolveTask}).{ID}),{resolveProject}.{percentComplete}, IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},&#39;&#39;)<br>column.9.valueFormat=doubleAsPercentRounded</pre>

1. Klikken **Weergave opslaan**.
