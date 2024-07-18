---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: uitgebreide gebruikersgegevens'
description: In deze gebruikersweergave wordt informatie over uw gebruikers weergegeven. Naast hun naam, toegangsniveaus, en Bedrijf, toont het ook lijsten van hun Groepen, Teams, en de Rollen van de Baan.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Weergeven: uitgebreide gebruikersgegevens

In deze gebruikersweergave wordt informatie over uw gebruikers weergegeven. Naast hun naam, toegangsniveaus, en Bedrijf, toont het ook lijsten van hun Groepen, Teams, en de Rollen van de Baan.

![ extended_user_view.png ](assets/expanded-user-view-350x75.png)

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

## Uitgebreide gebruikersgegevens weergeven

Deze weergave toepassen:

1. Ga naar een lijst met gebruikers.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode 5} column.0.link.valueformat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(name) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=0 <br> 0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=150 <br> column.1.descriptionkey=accesslevel <br> column.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.valueField=accessLevel:ID <br> column.1.link.linkproperty.0.valueformat=int <br> column.1.link.lookup=link.view <br> column.1.link.valueField=accessLevel:objCode <br> column.1.link.valueformat=val <br> column.1.linkedname=accessLevel <br> column.1.listsort=string (displayName) <br> column.1.namekey=accesslevel <br> column.1.querysort=name <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField=accessLevel:displayName <br> column.1.valuing ormat=HTML <br> column.1.viewalias=accessLevel:displayName <br> column.1.width=100 <br> column.2.link.linkproperty.0.name=ID <br> column.2.link.linkproperty.0.valueField=ID <br> column.2.link.linkformat.0.valuefefefield at=int <br> column.2.link.lookup=link.view <br> column.2.link.value=val (objCode) <br> column.2.listdelimiter= <br> column.2.listmethod=nested (usergroups).lists <br> column.2.namekey=group.plural <br> column.2.stretch=50 <br> column.2.type=iterate <br> column.2.valueField=group:name <br> column.2.valueformat=HTML <br> column.2.width=150 <br> column.3.displayname=Teams <br> column.3.listdelimiter= <br> 7} column.3.listmethod=nested (teams).lists <br> column.3.textmode=true <br> column.3.type=iterate <br> column.3.valueexpression= {name} <br> column.3.valueformat=HTML <br> column.4.link.linkproperty.0.name=ID <br>}column.4.link.linkproperty.0.valueField=ID <br> column.4.link.linkproperty.0.valueformat=int <br> column.4.link.lookup=link.view <br> column.4.link.value=val (objCode) <br> column.4.listdelimiter= <br> column.4.4 listmethod=nested (userRoles).lists <br> column.4.namekey=jobrole.plural <br> column.4.stretch=50 <br> column.4.type=iterate <br> column.4.valuefield=rol:name <br> column.4.valueformat=HTML <br> 4.width=150 <br> column.5.descriptionkey=company <br> column.5.link.linkproperty.0.name=ID <br> column.5.link.linkproperty.0.valueField=company:ID <br> column.5.link.linkproperty.0.valueformat=int <br> column.5.link.link up=link.view <br> column.5.link.valuefield=company:objCode <br> column.5.link.valueformat=val <br> column.5.linkedname=company <br> column.5.listsort=nested (bedrijf).string(naam) <br> column.5.namekey=company <br>.5.querysort=company:naam <br> column.5.shortview=false <br> column.5.stretch=0 <br> column.5.valueField=company:name <br> column.5.valueformat=HTML <br> column.5.width=150<br></pre>

1. Klik **sparen Mening**.
