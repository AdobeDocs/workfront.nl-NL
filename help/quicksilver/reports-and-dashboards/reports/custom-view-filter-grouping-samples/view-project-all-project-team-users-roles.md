---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: project met alle gebruikers en rollen van het projectteam'
description: Deze projectmening toont een lijst van gebruikers en baanrollen die aan het projectteam worden toegewezen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Weergave: project met alle gebruikers en rollen van het projectteam

Deze projectmening toont een lijst van gebruikers en baanrollen die aan het projectteam worden toegewezen.

>[!NOTE]
>
>Als de baanrol op de zelfde rij zoals een gebruiker vermeld is, impliceert dit niet dat de gebruiker die rol op het project vult, noch dat de gebruiker die rol in hun profiel wordt toegewezen.

![ project_custom_view_with_all_users_and_rollen_on_the_project_.png ](assets/project-custom-view-350x52.png)

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

## Een project weergeven met alle gebruikers en rollen van het projectteam

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueFormat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode <br> column.0.link.valuefat=val <br> column.0.linkedname=direct <br> column.0.listsort=string (naam) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=60 <br> column.0.valueField=name <br>} column.0.valueformat=HTML <br> column.0.width=150 <br> column.1.description=Team Gebruikers <br> column.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.valueField=userID <br> column.1.link.linkproperty.0.0 valueformat=int <br> column.1.link.page=/userView.cmd<br> column.1.listdelimiter= <br> column.1.listmethod=nested (projectUsers).lists <br> column.1.namekey=user.plural <br> column.1.stretch=30 <br> column.1.type=iterate <br> column.1.valueField=user:name <br> column.1.valueformat=HTML <br> column.1.width=150 <br> column.2.description=Team Roles <br> column.2.link.linkproperty.0.name=ID <br> column.2.link.linkproperty.0.valuield=ID <br> column.2.link.linkproperty.0.valueformat=int <br> column.2.link.page=/roleView.cmd<br> column.2.listdelimiter= <br> column.2.listmethod=nested (rollen).lists <br> column.2.namekey=jobrole.plural <br> column.2.stretch=10 <br> column.2.type=iterate <br> column.2.valueField=name <br> column.2.valueformat=HTML <br> column.2.width=150.stretch=0</pre>

1. Klik **sparen Mening**.
