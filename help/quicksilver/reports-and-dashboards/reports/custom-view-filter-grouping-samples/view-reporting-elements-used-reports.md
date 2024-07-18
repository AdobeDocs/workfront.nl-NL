---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: rapporteringselementen gebruikt in rapporten'
description: Deze mening toont de Mening, de Filter, en de Groepering die worden gebruikt om elk rapport in Adobe Workfront te bouwen wanneer u het in een lijst van rapporten gebruikt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Weergave: rapporteringselementen die worden gebruikt in rapporten

Deze mening toont de Mening, de Filter, en de Groepering die worden gebruikt om elk rapport in Adobe Workfront te bouwen wanneer u het in een lijst van rapporten gebruikt.

U kunt de

```
valuefields
```

of

```
valueexpressions
```

gebruikt in elk onderdeel van het verslag.

![ report_with_elements_definitions.png ](assets/report-with-elements-definitions-350x130.png)

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

## Rapportelementen weergeven die in rapporten worden gebruikt

1. Ga naar een lijst met rapporten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=string <br> column.0.link.lookup=link.run <br> column.0.link.value=val (objCode) 5} column.0.listsort=string (naam) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=200 <br> column.1.descriptionkey=objecttype {1 2} column.1.listsort=nested (mening).string(uiObjCode) <br> column.1.namekey=objecttype.abbr <br> column.1.querysort=uiObjCode <br> column.1.valuefield=uiObjCode <br> column.1.valueformat=obb jCodeMessage <br> column.1.width=80 <br> column.2.descriptionkey=enteredby <br> column.2.listsort=nested (enteredBy).string(lastName) <br> column.2.namekey=enteredby.abbr <br> column.2.querysort=enteredBy:last <br> column.2.valueField=enteredBy:name <br> column.2.valueformat=HTML <br> column.2.width=130 <br> column.3.displayname=Filter definitie <br> column.3.textmode=true <br> column.3.valueField=filter:definitie <br>} column.3.valueformat=HTML <br> column.4.displayname=View definitie <br> column.4.textmode=true <br> column.4.valuefield=view:definitie <br> column.4.valueformat=HTML <br> column.5.displayname=Grouping definitie <br> column.5.5.=true <br> column.5.valueField=groupBy:definitie <br> column.5.valueformat=HTML<br><br><br></pre>

1. Klik **sparen Mening**.
