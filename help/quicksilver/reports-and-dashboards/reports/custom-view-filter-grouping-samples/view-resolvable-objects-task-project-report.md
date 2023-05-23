---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: Oplosbare Objecten in een taak- of projectrapport"'
description: U kunt een lijst van alle Resolvable Voorwerpen in een project of taakmening of rapport tonen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Weergave: Oplosbare Objecten in een taak- of projectrapport

U kunt een lijst van alle Resolvable Voorwerpen in een project of taakmening of rapport tonen.

Raadpleeg het artikel voor meer informatie over Oplosbare objecten [Overzicht van Oplossende en Oplosbare objecten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

Deze weergave wordt op dezelfde manier toegepast voor taken en projecten.

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

## Weergeven Oplosbare objecten in een taak- of projectrapport

1. Ga naar een lijst met taken die zijn omgezet vanuit uitgaven.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, klikken **Kolom toevoegen**.

1. Klik op de kop van de nieuwe kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   <pre>displayname=Resolvables<br>listdelimiter=<br><br>listmethod=nested(resolvables).lists<br>textmode=true<br>type=iterate<br>valueField=name<br>valueformat=HTML<br></pre>

1. Klikken **Weergave opslaan**.\
   In de nieuwe kolom wordt een lijst met alle oplosbare objecten weergegeven. De namen van de objecten in de lijst kunnen niet rechtstreeks aan de objecten worden gekoppeld.
