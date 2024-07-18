---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: lijst met projectgebruikers met taakrollen'
description: U kunt deze mening in een projectlijst of een rapport toepassen om een lijst van gebruikers te tonen die met het project, evenals een lijst van de baanrollen worden geassocieerd zij op het project uitvoeren.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Weergave: lijst met projectgebruikers met taakrollen

U kunt deze mening in een projectlijst of een rapport toepassen om een lijst van gebruikers te tonen die met het project, evenals een lijst van de baanrollen worden geassocieerd zij op het project uitvoeren.

De informatie in dit verslag is ook te vinden in het gebied Mensen van het project.

>[!TIP]
>
>Als geen baanrollen voor de gebruikers maar u weten dat zij met baanrollen in hun gebruikersprofielen worden geassocieerd, zou dit kunnen betekenen zij aan taken en kwesties worden toegewezen maar zij zouden niet met een baanrol op de taak of de kwestie kunnen worden geassocieerd, of de gebruikers die in het rapport worden vermeld zijn niet de toegewezen taken en kwesties, maar vervullen andere rollen op het project (bijvoorbeeld, Eigenaar of Sponsor.)

![ project_with_user_and_role_information_report.png ](assets/project-with-user-and-role-information-report-350x100.png)

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

## Een lijst met projectgebruikers met taakrollen weergeven

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.link.valueformat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(name) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.section=0 <br> column.0.shortview=false <br> column.0.stretch=10 0<br> column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=200 <br> column.1.displayname=Project Gebruikers <br> column.1.listdelimiter=&lt;br&gt; <br> column.1.listmethod=nested (projectUsers).lists <br> column.1.textmode=true <br> column.1.type=iterate <br> column.1.valueexpression= {user}.{name} <br> column.1.valueformat=HTML <br> column.2.displayname=Project Roles <br> column.2.listdelimiter=&lt;br&gt; <br> column.2.listmethod=nested (projectUserRoles).lists <br> column.2.textmode=true <br> column.2.type=iterate <br> column.2.value expression={role}.{name} <br> column.2.valueformat=HTML</pre>

1. Klik **sparen Mening**.
