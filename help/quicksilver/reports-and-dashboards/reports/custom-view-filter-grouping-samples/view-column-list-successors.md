---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: een lijst met taakopvolgers toevoegen in een kolom'
description: U kunt een kolom aan een taakmening toevoegen om een lijst van de opvolgers van de taken te tonen. De kolom Opvolgers van de Taak omvat het aantal van de opvolger evenals de naam.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Weergave: voeg een lijst met taakopvolgers toe in een kolom

U kunt een kolom aan een taakmening toevoegen om een lijst van de opvolgers van de taken te tonen. De **kolom van de Opvolgers van de Taak** omvat het aantal van de opvolger evenals de naam.

![ task_view_with_a_list_of_succesors_.png ](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Een lijst met taakopvolgers toevoegen in een kolom

Deze kolom toevoegen aan een taakweergave:

1. Ga naar een bestaande taakweergave.
1. Breid het drop-down menu van de Mening uit, en selecteer **Mening** aanpassen.
1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over **toont in dit kolom** gebied, en klikt **om tekst** uit te geven.

1. Verwijder alle tekst in het vak Tekstmodus en vervang deze door de volgende code:
   <pre>displayname=Task Opvolgers <br> listdelimiter= <br><br> listmethod=nested (opvolgers).lists <br> textmode=true <br> type=iterate <br> valueexpression=CONCAT ({successor}).{taskNumber},' - ',{successor}.{name}) <br> valueformat=HTML</pre>

1. Klik **sparen Mening**.
