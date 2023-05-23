---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: multi-row projectweergave'
description: In deze projectweergave kunt u ME BEWERKEN.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Weergave: multi-rij projectweergave

In deze projectweergave kunt u:

* Projectinformatie weergeven in een indeling met meerdere rijen.\
   De weergave gebruikt de

   ```
   sharecol=true
   ```

   -tag gebruiken om meerdere velden onder dezelfde kolomkop te combineren. Voor meer informatie over deze tag raadpleegt u [Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Een kolom voor een plaatsaanduiding gebruiken die een HTML-regeleindtag bevat (

   ```
   <br>
   ```

   ) om de beschrijving te dwingen onder de projectnaam weer te geven, bijvoorbeeld.
* Geef de eigenaar van het project tussen haakjes weer achter de projectnaam.
* Toon de Naam van het Project als verbinding aan het project.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## Bouw een multi-rij projectweergave

1. Maak een nieuwe projectweergave. Voor meer informatie over hoe u een nieuwe weergave maakt, raadpleegt u [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. Verwijder tijdens het maken van de weergave alle kolommen, behalve één.
1. Selecteer de resterende kolom en klik op **Overschakelen naar tekstmodus**.
1. Kopieer en plak de tekstmodus onder de kolom:
   <pre>column.0.linkedname=direct<br>column.0.link.valueFormat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.valueField=objCode<br>column.0.link.lookup=link.view<br>column.0.sharecol=true<br>column.0.descriptionKey=name<br>column.0.width=150<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.name=Project Name / Manager / Description<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueFormat=HTML<br>column.1.valueexpression=CONCAT(",{owner}.{name},")")<br>column.1.listsort=nested(owner).string(name)<br>column.1.width=1<br>column.1.linkedname=direct<br>column.1.querysort=owner:name<br>column.1.textmode=true<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueFormat=HTML<br>column.1.sharecol=true<br>column.2.width=1<br>column.2.value=<br><br>column.2.shortview=false<br>column.2.sharecol=true<br>column.2.stretch=0<br>column.2.textmode=true<br>column.2.valueFormat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.descriptionKey=description<br>column.3.linkedname=direct<br>column.3.valueField=description<br>column.3.listsort=string(description)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharecol=true<br>column.3.stretch=0<br>column.3.shortview=false<br>column.3.valueFormat=HTML<br>column.3.width=1<br>column.4.shortview=false<br>column.4.value=<br><br>column.4.sharecol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueFormat=HTML\<br>column.4.stretch=0<br>column.5.name=Planned Dates / Duration<br>column.5.width=150<br>column.5.querysort=SchedulStartDate<br>column.5.sharecol=true<br>column.5.stretch=0<br>column.5.textmode=true<br>column.5.shortview=false<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(scheduledStartDate)<br>column.5.valueField=SchedulStartDate<br>column.5.valueFormat=atDate<br>column.6.sharecol=true<br>column.6.stretch=0<br>column.6.width=1<br>column.6.textmode=true<br>column.6.value=-<br>column.6.valueFormat=HTML<br>column.6.shortview=false<br>column.7.namekey=planningComplementationDate.abbr<br>column.7.width=1<br>column.7.sharecol=true<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.7.linkedname=direct<br>column.7.descriptionkey=planningComplementationDate<br>column.7.textmode=true<br>column.7.querysort=SchedulCompletionDate<br>column.7.valueFormat=atDate<br>column.7.valueField=SchedulCompletionDate<br>column.8.value=<br><br>column.8.width=1<br>column.8.textmode=true<br>column.8.sharecol=true<br>column.8.valueFormat=HTML<br>column.8.stretch=0<br>column.9.textmode=true<br>column.9.listsort=intAsInt(durationMinutes)<br>column.9.stretch=0<br>column.9.valueField=durationFieldLong<br>column.9.descriptionKey=duration<br>column.9.viewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharecol=true<br>column.9.width=100<br>column.9.shortview=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueFormat=compound<br>column.10.textmode=true<br>column.10.stretch=0</pre>

1. Klikken **Weergave opslaan**.
