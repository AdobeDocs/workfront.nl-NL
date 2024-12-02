---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Foutbericht bij het uitvoeren van een rapport: ''U bent momenteel niet aangemeld.'''
description: Meer informatie over het foutbericht Je bent momenteel niet aangemeld.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Foutbericht bij het uitvoeren van een rapport: &quot;U bent momenteel niet aangemeld.&quot;

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
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

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
