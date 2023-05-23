---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: uitgiftegegevens voor taken en projecten"'
description: Wanneer een kwestie in een taak of een project wordt omgezet wordt een het oplossen van objecten verhouding gevestigd tussen de taak of het project en de kwestie. In deze weergave worden de volgende velden van de uitgave weergegeven die automatisch worden ingevuld wanneer de taak of het project is voltooid - BEWERK ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Weergave: het voortkomen uitgeeft details voor taken en projecten

Wanneer een kwestie in een taak of een project wordt omgezet wordt een het oplossen van objecten verhouding gevestigd tussen de taak of het project en de kwestie. In deze weergave worden de volgende velden van de uitgave weergegeven die automatisch worden voltooid wanneer de taak of het project is voltooid:

* Naam
* Invoerdatum
* Geplande afsluitdatum
* Werkelijke afsluitdatum
* Type aanvraag
* Naam van maker
* Toegewezen aan gebruiker

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Zie ook voor meer informatie [Weergave: toon originele uitgifteinformatie over taak en projectlijsten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Uitstekende details voor taken en projecten weergeven

1. Ga naar een lijst met taken of een lijst met projecten.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Klikken **Weergave opslaan**.
