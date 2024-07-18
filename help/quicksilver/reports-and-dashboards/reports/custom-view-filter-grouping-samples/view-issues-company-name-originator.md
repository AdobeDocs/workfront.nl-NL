---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: issues with the company name of the originator'
description: In deze weergave wordt de bedrijfsnaam weergegeven van de gebruiker die de uitgave heeft verzonden.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Weergave: problemen met de bedrijfsnaam van de maker

In deze weergave wordt de bedrijfsnaam weergegeven van de gebruiker die de uitgave heeft verzonden.

![ custom_view_for_issues_with_originator_company_name.png ](assets/custom-view-for-issues-350x33.png)

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

## Problemen met de bedrijfsnaam van de maker weergeven

Deze weergave toepassen:

1. Ga naar een lijst met problemen.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=val <br> column.0.link.lookup=link.view <br> column.0.link.value=val (objCode) 5} column.0.listsort=string (naam) <br> column.0.namekey=name <br> column.0.querysort=name <br> column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=140 <br> column.1.descriptionkey=originator <br>.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.valueField=ownerID <br> column.1.link.linkproperty.0.valueformat=int <br> column.1.link.lookup=link.view <br> column.1.link.valuefield=owner:objCode {1 7} column.1.link.valueformat=val <br> column.1.listsort=nested (eigenaar).string(naam) <br> column.1.namekey=originator.abbr <br> column.1.querysort=owner:name <br> column.1.valuefield=owner:name <br> column.1.valuefefefefefefefefe at=HTML <br> column.1.width=151 <br> column.2.descriptionkey=entrydate <br> column.2.listsort=atDateAsAtDate(entryDate) <br> column.2.namekey=entrydate.abbr <br> column.2.querysort=entryDate {2Date 8} column.2.valueField=entryDate <br> column.2.valueformat=atDate <br> column.2.width=75 <br> column.3.descriptionkey=age <br> column.3.listsort=doubleAsDouble (leeftijd) <br> column.3.namekey=age <br> 3.querysort=age <br> column.3.valuefield=howOld <br> column.3.valueformat=val <br> column.3.width=80 <br> column.4.viewalias=statusicons <br> column.4.displayname=Flags <br> column.4.linkedname=direct {4 1} column.4.namekey=statusicons <br> column.4.valueField= <br> column.4.valueformat=HTML <br> column.4.querysort= <br> column.4.tile.name=component.issueUsicons <br> column.4.tile.pdfcomponent=issueStatusIcons s<br> column.4.delimiter= <br> column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br> column.5.description=Originator's Bedrijfsnaam <br> column.5.link.linkproperty.0.name=ID <br> column.5.link.linkproperty.0.valueField=owner:companyID <br> column.5.link.linkproperty.0.valueformat=int <br> column.5.link.lookup=link.view <br> column.5.link.valueField=owner :company: objCode <br> column.5.link.valueformat=val <br> column.5.listsort=nested (eigenaar:bedrijf).string(naam) <br>} column.5.name=Originator Bedrijf <br> column.5.querysort=owner :company: naam <br> column.5.valueField=owner :company: naam <br> column.5.valueformat=HTML <br> column.5.width=151<br><br><br><br></pre>

1. Klik **sparen Mening**.
