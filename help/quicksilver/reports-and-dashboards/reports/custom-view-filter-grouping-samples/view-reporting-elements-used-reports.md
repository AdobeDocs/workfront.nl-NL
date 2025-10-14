---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: elementen rapporteren die worden gebruikt in rapporten'
description: Deze mening toont de Mening, de Filter, en de Groepering die worden gebruikt om elk rapport in Adobe Workfront te bouwen wanneer u het in een lijst van rapporten gebruikt.
author: Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Weergave: rapporteringselementen die worden gebruikt in rapporten

<!--Audited: 11/2024-->

Deze mening toont de Mening, de Filter, en de Groepering die worden gebruikt om elk rapport in Adobe Workfront te bouwen wanneer u het in een lijst van rapporten gebruikt.

U kunt zien welke `valuefields` of `valueexpressions` in elk element van het rapport wordt gebruikt.

![&#x200B; report_with_elements_definitions.png &#x200B;](assets/report-with-elements-definitions-350x130.png)

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p> Huidige: 
   <ul>
   <li>Verzoek om een weergave te wijzigen</li> 
   <li>Plan om een rapport te wijzigen</li>
   </ul>
     </p>
     <p> Nieuw: 
   <ul>
   <li>Medewerker om een weergave te wijzigen</li> 
   <li>Standaard voor het wijzigen van een rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rapportelementen weergeven die in rapporten worden gebruikt

1. Ga naar een lijst met rapporten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.
1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=string
   column.0.link.lookup=link.run
   column.0.link.value=val(objCode)
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.descriptionkey=objecttype
   column.1.listsort=nested(view).string(uiObjCode)
   column.1.namekey=objecttype.abbr
   column.1.querysort=uiObjCode
   column.1.valuefield=uiObjCode
   column.1.valueformat=objCodeMessage
   column.1.width=80
   column.2.descriptionkey=enteredby
   column.2.listsort=nested(enteredBy).string(lastName)
   column.2.namekey=enteredby.abbr
   column.2.querysort=enteredBy:lastName
   column.2.valuefield=enteredBy:name
   column.2.valueformat=HTML
   column.2.width=130
   column.3.displayname=Filter definition
   column.3.textmode=true
   column.3.valuefield=filter:definition
   column.3.valueformat=HTML
   column.4.displayname=View definition
   column.4.textmode=true
   column.4.valuefield=view:definition
   column.4.valueformat=HTML
   column.5.displayname=Grouping definition
   column.5.textmode=true
   column.5.valuefield=groupBy:definition
   column.5.valueformat=HTML
   ```

1. Klik **Gedaan** > **sparen Mening**.
