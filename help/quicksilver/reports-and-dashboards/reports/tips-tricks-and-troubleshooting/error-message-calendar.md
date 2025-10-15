---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Foutbericht op kalender: ''Deze kalender heeft de weergaverechten van een gedeactiveerde gebruiker.'''
description: Meer informatie over het foutbericht 'Deze kalender heeft de weergaverechten van een gedeactiveerde gebruiker'.
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Foutbericht op kalender: &quot;Deze kalender heeft de weergaverechten van een gedeactiveerde gebruiker.&quot;

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
     <p>Standard</p>
     <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een kalender beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
