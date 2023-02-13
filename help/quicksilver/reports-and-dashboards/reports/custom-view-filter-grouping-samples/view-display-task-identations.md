---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: taakinspringingen weergeven in een takenlijst"'
description: In deze taakmening, kunt u code aan de kolom van de Naam van de Taak toevoegen om de taken te tonen die volgens de Structuur van de Onderverdeling van het Werk van het project worden ingesprongen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Weergave: taakinspringingen weergeven in een takenlijst

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

## Taakinspringingen weergeven in een kolom van een takenlijst

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** en begint &quot;Taaknaam&quot; te typen in het dialoogvenster **Tonen in deze kolom** selecteert u het veld wanneer het in de lijst wordt weergegeven.

1. Klik in de nieuwe kolom op **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster

   ```
   valuefield=
   ```

   regel en vervang deze door de volgende code:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
