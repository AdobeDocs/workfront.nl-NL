---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: verzendpad voor problemen'
description: U kunt het pad waarlangs een kwestie in de mening van een uitgiftenrapport is voorgelegd tonen. De weg wijst op de Rij, de Groep van het Onderwerp, en het Onderwerp van de Rij waar de kwestie oorspronkelijk werd voorgelegd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Weergeven: verzendpad voor problemen

U kunt het pad waarlangs een kwestie in de mening van een uitgiftenrapport is voorgelegd tonen. De weg wijst op de Rij, de Groep van het Onderwerp, en het Onderwerp van de Rij waar de kwestie oorspronkelijk werd voorgelegd.

![ issue_submission_path.png ](assets/issue-submission-path-350x66.png)

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

## Het verzendingspad weergeven voor problemen

1. Ga naar een lijst met problemen.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, klik **voegt Kolom** toe.

1. Klik de kopbal van de nieuwe kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>displayname= Pad van de Uitgave <br> linkedname=direct <br> namekey=displayQueueBreadcrumb <br> valueField=displayQueueBreadcrumb <br> valueFormat=HTML<br></pre>

1. Klik **sparen Mening**.
