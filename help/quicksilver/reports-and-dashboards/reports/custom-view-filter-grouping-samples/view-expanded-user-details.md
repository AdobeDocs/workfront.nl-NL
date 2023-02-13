---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: uitgebreide gebruikersgegevens'
description: In deze gebruikersweergave wordt informatie over uw gebruikers weergegeven. Naast hun naam, toegangsniveaus, en Bedrijf, toont het ook lijsten van hun Groepen, Teams, en de Rollen van de Baan.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Weergave: uitgebreide gebruikersgegevens

In deze gebruikersweergave wordt informatie over uw gebruikers weergegeven. Naast hun naam, toegangsniveaus, en Bedrijf, toont het ook lijsten van hun Groepen, Teams, en de Rollen van de Baan.

![extended_user_view.png](assets/expanded-user-view-350x75.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Uitgebreide gebruikersgegevens weergeven

Deze weergave toepassen:

1. Ga naar een lijst met gebruikers.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionKey=name <br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionKey=accesslevel<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=accessLevel:ID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=accessLevel:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=accessLevel<br>column.1.listsort=string(displayName)<br>column.1.namekey=accesslevel<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=accessLevel:displayName<br>column.1.valueFormat=HTML<br>column.1.viewalias=accessLevel:displayName<br>column.1.width=100<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=val(objCode)<br>column.2.listdelimiter=<br>column.2.listmethod=nested(userGroup).lists<br>column.2.namekey=group.plural<br>column.2.stretch=50<br>column.2.type=iterate<br>column.2.valueField=group:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.displayName=Teams<br>column.3.listdelimiter=<br>column.3.listmethod=nested(teams).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={name}<br>column.3.valueFormat=HTML<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valueField=ID<br>column.4.link.linkproperty.0.valueFormat=int<br>column.4.link.lookup=link.view<br>column.4.link.value=val(objCode)<br>column.4.listdelimiter=<br>column.4.listmethod=nested(userRoles).lists<br>column.4.namekey=jobrole.plural<br>column.4.stretch=50<br>column.4.type=iterate<br>column.4.valueField=role:name<br>column.4.valueFormat=HTML<br>column.4.width=150<br>column.5.descriptionkey=company<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valueField=company:ID<br>column.5.link.linkproperty.0.valueFormat=int<br>column.5.link.lookup=link.view<br>column.5.link.valueField=company:objCode<br>column.5.link.valueFormat=val<br>column.5.linkedname=company<br>column.5.listsort=nested(company).string(name)<br>column.5.namekey=company<br>column.5.querysort=company:name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueField=company:name<br>column.5.valueFormat=HTML<br>column.5.width=150</pre>

1. Klikken **Weergave opslaan**.
