---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: alleen items in een goedkeuringsstatus tonen"'
description: U kunt alleen objecten weergeven met een bepaalde status die momenteel in behandeling is. Dit werkt hetzelfde voor elk ander object met een goedkeuringsstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Filter: alleen items in een goedkeuringsstatus weergeven

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

## Alleen items weergeven die de goedkeuringsstatus hebben

1. Ga bijvoorbeeld naar het filter dat u wilt aanpassen voor een lijst met projecten.
1. Klikken **Filterregel toevoegen** voor de **Status** veld van het object in uw lijst.\
   In een projectrapport voegt u bijvoorbeeld **Status Gelijke Planning**, als u alleen projecten wilt weergeven die de status **Planning - In afwachting van goedkeuring**.

1. Klikken **Overschakelen naar tekstmodus**.
1. De

   ```
   status
   ```

   regel door toevoegen **:A** op de 3-letterige sleutel van de status:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Klikken **Gereed** vervolgens **Filter opslaan**.

   De lijst toont slechts projecten die in een status van Planning - in afwachting van Goedkeuring zijn.
