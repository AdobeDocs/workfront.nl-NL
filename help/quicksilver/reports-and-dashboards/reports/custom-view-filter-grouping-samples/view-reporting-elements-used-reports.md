---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: in rapporten gebruikte rapportelementen'
description: Deze mening toont de Mening, de Filter, en de Groepering die worden gebruikt om elk rapport in Adobe Workfront te bouwen wanneer u het in een lijst van rapporten gebruikt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Weergave: in rapporten gebruikte rapporteringselementen

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

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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

## Rapportelementen weergeven die in rapporten worden gebruikt

1. Ga naar een lijst met rapporten.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>column.0.descriptionKey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=200<br>column.1.descriptionkey=objecttype<br>column.1.listsort=nested(view).string(uiObjCode)<br>column.1.namekey=objecttype.abbr<br>column.1.querysort=uiObjCode<br>column.1.valueField=uiObjCode<br>column.1.valueFormat=objCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enter<br>column.2.listsort=nested(enteredBy).string(lastName)<br>column.2.namekey=enteredby.abbr<br>column.2.querysort=enteredBy:lastName<br>column.2.valueField=enteredBy:name<br>column.2.valueFormat=HTML<br>column.2.width=130<br>column.3.displayName=Filter, definitie<br>column.3.textmode=true<br>column.3.valueField=filter:definition<br>column.3.valueFormat=HTML<br>column.4.displayName=View definition<br>column.4.textmode=true<br>column.4.valueField=view:definition<br>column.4.valueFormat=HTML<br>column.5.displayName=Grouping definition<br>column.5.textmode=true<br>column.5.valueField=groupBy:definition<br>column.5.valueFormat=HTML<br></pre>

1. Klikken **Weergave opslaan**.
