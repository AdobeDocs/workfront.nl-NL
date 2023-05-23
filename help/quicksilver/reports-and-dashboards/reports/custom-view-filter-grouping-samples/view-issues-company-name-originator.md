---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: problemen met de bedrijfsnaam van de maker'
description: In deze weergave wordt de bedrijfsnaam weergegeven van de gebruiker die de uitgave heeft verzonden.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Weergave: problemen met de bedrijfsnaam van de afzender

In deze weergave wordt de bedrijfsnaam weergegeven van de gebruiker die de uitgave heeft verzonden.

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## Problemen met de bedrijfsnaam van de maker weergeven

Deze weergave toepassen:

1. Ga naar een lijst met problemen.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>column.0.descriptionKey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=ownerID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=owner:objCode<br>column.1.link.valueFormat=val<br>column.1.listsort=nested(owner).string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner:name<br>column.1.valueField=owner:name<br>column.1.valueFormat=HTML<br>column.1.width=151<br>column.2.descriptionKey=entrydate<br>column.2.listsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column.2.valueField=entryDate<br>column.2.valueFormat=atDate<br>column.2.width=75<br>column.3.descriptionKey=age<br>column.3.listsort=doubleAsDouble(age)<br>column.3.namekey=age<br>column.3.querysort=age<br>column.3.valueField=howOld<br>column.3.valueFormat=val<br>column.3.width=80<br>column.4.viewalias=standscons<br>column.4.displayName=Flags<br>column.4.linkedname=direct<br>column.4.namekey=standscons<br>column.4.valueField=<br>column.4.valueFormat=HTML<br>column.4.querysort=<br>column.4.tile.name=component.issuesUsicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter=<br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=Originator's Company Name<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valueField=owner:companyID<br>column.5.link.linkproperty.0.valueFormat=int<br>column.5.link.lookup=link.view<br>column.5.link.valueField=owner:company:objCode<br>column.5.link.valueFormat=val<br>column.5.listsort=nested(owner:company).string(name)<br>column.5.name=Originator Company<br>column.5.querysort=owner:company:name<br>column.5.valueField=owner:company:name<br>column.5.valueFormat=HTML<br>column.5.width=151</pre>

1. Klikken **Weergave opslaan**.
