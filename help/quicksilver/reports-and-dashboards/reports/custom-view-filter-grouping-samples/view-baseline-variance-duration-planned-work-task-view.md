---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: basislijnvariatie voor Duur en Gepland werk in een taakweergave'
description: Bekijk de basislijnvariatie voor Duur en Gepland werk.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Weergave: basislijnvariatie voor Duur en Gepland werk in een taakweergave

In deze weergave wordt het volgende weergegeven in een taakweergave:

* Taakgegevens met basislijntaakgegevens.
* Het verschil tussen Duur en de Standaardduur van de Basislijn.
* Het verschil tussen de Geplande Werk en Standaard Geplande Werk van de Basislijn.

>[!NOTE]
>
> De gegevens die in de volgende mening worden getoond vergelijkt daadwerkelijke taakwaarden met de waarden verbonden aan de Standaardtaken van de Basislijn.

 

![ baseline_variance_in_a_task_view.png ](assets/baseline-variance-in-a-task-view-350x38.png)

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De basislijnvariatie van de mening voor Duur en Gepland Werk in een taakmening

1. Ga naar een takenlijst.
1. In het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. Verwijder alle kolommen in de weergave, behalve de eerste.
1. Met de eerste geselecteerde kolom, klik **Schakelaar aan de Wijze van de Tekst**.
1. Kopieer de onderstaande tekst en plak deze in de eerste kolom van de weergave:
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode 5} column.0.link.valueformat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(naam) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=100 {1 2} column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=150 <br> column.0.displayname=Task Naam <br> column.1.descriptionkey=duration <br> column.1.linkedname=direct <br> column.1.listint AsInt (durationMinutes) <br> column.1.namekey=duration.abbr <br> column.1.querysort=durationMinutes <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField=durationFieldLong <br> column.1.valuefefefefefefefefefefefefex at=compound <br> column.1.viewalias=duration <br> column.1.width=100 <br> column.1.displayname=Task Duur <br> column.2.descriptionkey=view.relatedcolumn <br> column.2.descriptionkeyargkey.0=default baselinetask <br> column.2.2 descriptionkeyargkey.1=duration <br> column.2.linkedname=defaultBaselineTask <br> column.2.listsort=intAsInt (durationMinutes) <br> column.2.namekey=duration <br> column.2.namekeyargkey.0=default baselinetask.abbr <br> column 2.namekeyargkey.1=duration.abbr <br> column.2.querysort=defaultBaselineTask:durationMinutes <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valuefield=defaultBaselineTask:durationFieldLong <br> column.2.value Format=compound <br> column.2.viewalias=defaultBaselineTask:duration <br> column.2.width=100 <br> column.2.displayname=Dflt Baseline Tsk: Dur <br> column.2.durationunitfield=durationUnit.value <br> column.3.description=DurationVariance.3.linkedname=direct <br> column.3.listsort=intAsInt (durationMinutes) <br> column.3.name=Duration Variance <br> column.3.querysort=durationMinutes <br> column.3.shortview=false <br> column.3.stretch=0 <br> expression=value CONCAT(SUB ({duration}, {defaultBaselineTask}.<br><br>{duration})/480," Dagen") <br> column.3.valueformat=HTML <br> column.3.viewalias=duration <br> column.3.width=100 <br> column.3.displayname=Duration Variance <br> column.4.descriptionkey=workrequired <br> column.4.linkedname=direct <br> 4.listsort=doubleAsDouble (workRequired) <br> column.4.namekey=workrequired.abbr <br> column.4.querysort=workRequired <br> column.4.shortview=false <br> column.4.stretch=0 <br> column.4.valuefield=workFieldLong <br> column.4.valuated eformat=compound <br> column.4.viewalias=workrequired <br> column.4.width=100 <br> column.4.displayname=Wrk Req <br> column.5.descriptionkey=view.relatedcolumn <br> column.5.descriptionkeyargkey.0=default baselinetask <br> column.5.descriptionkeyargkey.1=workrequired <br> column.5.linkedname=defaultBaselineTask <br> column.5.listsort=doubleAsDouble(workRequired) <br> column.5.namekey=view.relatedcolumn <br> column.5.namekeyargkey.0=default baselinetask.0 abbr <br> column.5.namekeyargkey.1=workrequired.abbr <br> column.5.querysort=defaultBaselineTask:workRequired <br> column.5.shortview=false <br> column.5.stretch=0 <br> column.5.valuefield=defaultBaselineTask:workField <br> column.5.valueformat=compound <br> column.5.viewalias=defaultBaselineTask:werk vereiste <br> column.5.width=100 <br> column.5.displayname=Dflt Baseline Tsk: De Rek <br> column.6.descriptionkey=workrequired <br> 6.linkedname=direct <br> column.6.listsort=doubleAsDouble (workRequired) <br> column.6.name=Effort Variantie <br> column.6.querysort=workRequired <br> column.6.shortview=false <br> column.6.stretch=0 <br> expression=valueCONCAT(SUB ({workRequired}, {defaultBaselineTask}).{workRequired})/60," Uren") <br> column.6.valueformat=HTML <br> column.6.viewalias=workrequired <br> column.6.width=100 <br> column.6.displayname=Efficiënte Variantie</pre>

1. Klik **sparen Mening**.