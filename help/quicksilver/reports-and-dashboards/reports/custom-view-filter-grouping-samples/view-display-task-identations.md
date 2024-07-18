---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: taakinspringingen weergeven in een takenlijst'
description: In deze taakmening, kunt u code aan de kolom van de Naam van de Taak toevoegen om de taken te tonen die volgens de Structuur van de Onderverdeling van het Werk van het project worden ingesprongen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Weergeven: taakinspringingen weergeven in een takenlijst

In deze taakmening, kunt u code aan de kolom van de Naam van de Taak toevoegen om de taken te tonen die volgens de Structuur van de Onderverdeling van het Werk van het project worden ingesprongen.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Taken weergeven in een kolom van een takenlijst

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** en beginnen &quot;Naam van de Taak&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Van de nieuwe kolom, klik **Schakelaar aan de Wijze van de Tekst**.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Verwijder de tekst die u zoekt op de regel `valuefield=` en vervang deze door de volgende code:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klik **sparen**, dan **sparen Mening**.
