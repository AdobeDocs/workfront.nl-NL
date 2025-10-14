---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Foutbericht op kalender: "Deze kalender heeft de weergaverechten van een gedeactiveerde gebruiker.""'
description: Meer informatie over het foutbericht 'Deze kalender heeft de weergaverechten van een gedeactiveerde gebruiker'.
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Foutbericht op kalender: &quot;Deze kalender heeft de weergaverechten van een gedeactiveerde gebruiker.&quot;

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan, werk</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een kalender beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Probleem

U ontvangt de volgende fout wanneer u een kalender opent die met u wordt gedeeld: 

*Deze kalender heeft de meningsrechten van een gedeactiveerde gebruiker. Gelieve te hebben een beheerder de kalendervoorrechten bevestigen.*

## Oorzaak

De gebruiker die deze kalender heeft gemaakt (de oorspronkelijke eigenaar) is een gebruiker die is gedeactiveerd. 

## Oplossing

U kunt dit op de volgende manier oplossen:

1. Kopieer de oorspronkelijke kalender. Wanneer u een kalender kopieert, wordt u de eigenaar van de kalender. De gekopieerde kalender moet alle informatie uit de oorspronkelijke kalender bevatten.\
   Voor meer informatie over het kopiëren van een kalender, zie [&#x200B; Kopieer een kalenderrapport &#x200B;](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Deel de gekopieerde kalender met dezelfde gebruikers als de oorspronkelijke kalender. Alle gebruikers moeten dezelfde informatie op de nieuwe kalender zien.
1. (Optioneel en voorwaardelijk) Als u machtigingen hebt om de oorspronkelijke kalender te beheren, verwijdert u alle andere gebruikers met wie de kalender wordt gedeeld uit het gebied voor het delen van kalender. Dit voorkomt verwarring bij gebruikers die de verkeerde kalender proberen weer te geven.
