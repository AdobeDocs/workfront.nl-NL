---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: Oplosbare objecten in een taak- of projectrapport'
description: U kunt een lijst van alle Resolvable Voorwerpen in een project of taakmening of rapport tonen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Weergave: Oplosbare objecten in een taak- of projectrapport

<!--Audited: 11/2024-->

U kunt een lijst van alle Resolvable Voorwerpen in een project of taakmening of rapport tonen.

Voor meer informatie over Oplosbare Voorwerpen, zie het artikel [&#x200B; Overzicht van het Oplossen en Oplosbare Voorwerpen &#x200B;](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![&#x200B; list_of_resolvables_in_report.png &#x200B;](assets/list-of-resolvables-in-report-350x54.png)

Deze weergave wordt op dezelfde manier toegepast voor taken en projecten.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p> Huidige: 
   <ul>
   <li>Verzoek om een weergave te wijzigen</li> 
   <li>Plan om een rapport te wijzigen</li>
   </ul>
     </p>
     <p> Nieuw: 
   <ul>
   <li>Medewerker om een weergave te wijzigen</li> 
   <li>Standaard voor het wijzigen van een rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Weergeven Oplosbare objecten in een taak- of projectrapport

1. Ga naar een lijst met taken of projecten die vanuit uitgaven zijn omgezet.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, klik **voegt Kolom** toe.

1. Klik de kopbal van de nieuwe kolom, dan klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Klik **Gedaan** > **sparen Mening**.\
   In de nieuwe kolom wordt een lijst met alle oplosbare objecten weergegeven. De namen van de objecten in de lijst kunnen niet rechtstreeks aan de objecten worden gekoppeld.
