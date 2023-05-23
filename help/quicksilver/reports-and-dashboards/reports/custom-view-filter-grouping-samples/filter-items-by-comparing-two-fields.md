---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: items in een lijst verwijderen door twee velden te vergelijken'
description: U kunt items uit een lijst filteren door twee van de velden te vergelijken. U kunt bijvoorbeeld alleen taken weergeven als de datum van feitelijke voltooiing van de taak groter is dan de geplande voltooiingsdatum.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Filter: items in een lijst verwijderen door twee velden te vergelijken

U kunt items uit een lijst filteren door twee van de velden te vergelijken. U kunt bijvoorbeeld alleen taken weergeven als de datum van feitelijke voltooiing van de taak groter is dan de geplande voltooiingsdatum.

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Items filteren door twee velden te vergelijken

1. Ga naar een takenlijst.
1. Van de **Filter** vervolgkeuzelijst, selecteert u **Nieuw filter**.

1. Klikken **Filterregel toevoegen** en toevoegen **Werkelijke afsluitdatum** >**Groter dan** > **Selecteer een datum**.

   >[!TIP]
   >
   >Kies de filteroptie die u voor het geselecteerde veld wilt gebruiken, indien beschikbaar.

1. Klikken **Overschakelen naar tekstmodus**.
1. In de **Filterregels instellen voor uw rapport** voegt u de volgende code toe:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Klikken **Gereed** vervolgens **Filter opslaan**.
