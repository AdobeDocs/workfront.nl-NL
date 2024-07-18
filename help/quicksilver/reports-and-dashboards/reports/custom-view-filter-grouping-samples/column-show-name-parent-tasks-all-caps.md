---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: naam van bovenliggende taken weergeven als kapitalen'
description: U kunt deze kolom aan een taakmening toevoegen om de naam van de oudertaken in alle hoofdletters te tonen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Weergeven: de naam van bovenliggende taken weergeven als kapitalen

U kunt deze kolom aan een taakmening toevoegen om de naam van de oudertaken in alle hoofdletters te tonen.

![](assets/column-task-with-all-caps-parent-350x112.png)

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
   <td> <p>Verzoek om filters, weergaven en groepen te wijzigen </p>
   <p>Plan voor het wijzigen van rapporten</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om afzonderlijke weergaven te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Naam van bovenliggende taken weergeven als kapitalen

Deze kolom bouwen in een taakmening:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, uitgezochte **past Mening** aan.\
   of\
   Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, klik de kopbal van de kolom die de taaknaam in de lijst toont.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code: <pre>descriptionkey=name <br> displayname=Task Naam <br> textmode=true <br> valueexpression=IF ({numberOfChildren}> &quot;0&quot;, UPPER ({name}), {name}) <br> valueformat=HTML <br> width=150 <br></pre>

1. Klik **sparen Mening**.
