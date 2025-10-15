---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Foutbericht bij het uitvoeren van een rapport: ''U bent momenteel niet aangemeld.'''
description: Meer informatie over het foutbericht Je bent momenteel niet aangemeld.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# Foutbericht bij het uitvoeren van een rapport: &quot;U bent momenteel niet aangemeld.&quot;

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
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Probleem

Wanneer het runnen van een rapport, of het tonen van het in een dashboard, keert de volgende fout terug:\
*proberen opnieuw dat. U wordt momenteel niet het programma geopend.*

Er worden geen resultaten weergegeven in het rapport.

## Oorzaak

Het rapport is momenteel geplaatst om als gedeactiveerde gebruiker te lopen.

## Oplossing

U moet beheerderstoestemmingen aan het rapport hebben om de rapportmontages te kunnen veranderen.\
U kunt als volgt het rapport aanpassen en de resultaten bekijken:

1. Ga naar het rapport.
1. Klik **de Acties van het Rapport** > **uitgeven** > **Montages van het Rapport**.

1. Specificeer de naam van een actieve gebruiker in de **Looppas dit rapport met de Rechten van de Toegang van:** gebied.\
   of\
   Verlaat **dit rapport met de Rechten van de Toegang van:** gebied leeg in werking stellen.

1. Klik **Gedaan**.
1. Klik **sparen + Sluiten**.\
   De fout zou niet opnieuw moeten verschijnen wanneer het runnen van dit rapport.
