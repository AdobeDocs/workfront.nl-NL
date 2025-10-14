---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: persoonlijke taken'
description: Met dit taakfilter worden ad-hocverzoeken geretourneerd die naar een gebruiker zijn verzonden, of naar-do items die door gebruikers in hun thuisgebied zijn toegevoegd. De persoonlijke taken worden niet verbonden met een project maar zij kunnen aan een project worden verplaatst, indien nodig.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Filter: persoonlijke taken

<!--Audited: 10/2024-->

Dit taakfilter retourneert ad-hocwerkverzoeken die naar een gebruiker zijn verzonden of om items te doen die door gebruikers in de widget Aan/Uit in het gebied Home zijn toegevoegd.

Ad-hocverzoeken voor werk en items voor taken worden in Adobe Workfront opgeslagen als persoonlijke taken.

De persoonlijke taken worden niet verbonden met een project maar zij kunnen aan een project worden verplaatst, indien nodig. Voor informatie, zie [&#x200B; persoonlijke taken &#x200B;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md) creëren.

![&#x200B; Persoonlijke takenrapport &#x200B;](assets/personal-tasks-report.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Persoonlijke taken filteren

Dit filter maken:

1. Ga naar een lijst met taken of een taakrapport.
1. Van het **drop-down menu van de Filter**, klik **Nieuwe filter**.
1. (Voorwaardelijk) klik **voeg een filterregel** van u toe heeft toegang tot de filter van een rapport, of begin uw filtercriteria op het eerste gebied te selecteren, als u tot de filter van een lijst toegang hebt.
1. (Voorwaardelijk) selecteer de volgende het filtreren criteria:

   * Van een lijstfilter: **Taak** > **Persoonlijk** **is waar**
   * Van een rapportfilter: **Taak** > **Persoonlijk** > **Gelijk (gevoelig geval)** > **Waar**.
1. Sla het filter op.

   De lijst toont slechts persoonlijke taken die niet op om het even welke projecten zijn.
