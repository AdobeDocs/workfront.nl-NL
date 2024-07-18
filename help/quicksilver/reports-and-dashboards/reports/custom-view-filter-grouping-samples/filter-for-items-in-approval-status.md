---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: alleen items in een goedkeuringsstatus weergeven'
description: U kunt alleen objecten weergeven met een bepaalde status die momenteel in behandeling is. Dit werkt hetzelfde voor elk ander object met een goedkeuringsstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Filter: alleen items weergeven in een goedkeuringsstatus

U kunt alleen objecten weergeven met een bepaalde status die momenteel in behandeling is. Dit werkt hetzelfde voor elk ander object met een goedkeuringsstatus.

U kunt de volgende objecten in een goedkeuringsstatus plaatsen:

* Taken
* Problemen
* Projecten

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
   <td> <p>Verzoek om een filter te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Alleen items weergeven die de goedkeuringsstatus hebben

1. Ga bijvoorbeeld naar het filter dat u wilt aanpassen voor een lijst met projecten.
1. Klik **toevoegen een Regel van de Filter** voor het **3} gebied van de Status {van het voorwerp van uw lijst.**\
   Bijvoorbeeld, in een projectrapport, voeg **Gelijke Planning van de Status** toe, als u slechts projecten wilt tonen die in een status van **Planning - in afwachting van Goedkeuring** zijn.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Wijzig de

   ```
   status
   ```

   lijn door **toe te voegen:A** aan de 3 lettersleutel van de status:
   <pre>status=PLN:A<br> status_Mod=in</pre>

1. Klik **Gedaan**, dan **sparen Filter**.

   De lijst toont slechts projecten die in een status van Planning - in afwachting van Goedkeuring zijn.
