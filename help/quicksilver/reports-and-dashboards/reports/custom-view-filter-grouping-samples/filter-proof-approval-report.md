---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Goedkeuringsrapport proefdrukken om vorige proefversies weg te laten'
description: Voor een rapport van de Goedkeuring van het Bewijs, kunt u het Is Huidige filter van de Versie van het Document gebruiken om slechts de huidige versies van proeven te omvatten die op uw goedkeuring wachten.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Filter: rapport Goedkeuring proef om vorige proefversies weg te laten

<!--Audited: 10/2024-->

Op een rapport van de Goedkeuring van het Bewijs, kunt u **gebruiken is Huidige filter van de Versie van het Document** om slechts de huidige versies van proeven te omvatten die op uw goedkeuring wachten.

Dit is bijvoorbeeld handig als u is gevraagd proefdrukken met meerdere versies goed te keuren. Wanneer u het rapport Goedkeuring van het Bewijs met het Huidige filter van de Versie van het Document van Is in werking stelt, maakt het rapport een lijst van slechts de huidige versie van elke proef die op uw goedkeuring wacht, die vroegere versies weglaat die u niet meer hoeft te werken.

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

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rapport Goedkeuring proef filteren om vorige proefversies weg te laten

U kunt een filter voor een rapport van de Goedkeuring van het Bewijs tot stand brengen.

1. Open het rapport als u al een proefgoedkeuringsrapport hebt.

   of

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Om uw eigen rapport van de Goedkeuring van het Proef te creëren, klik het **pictogram van het Belangrijkste Menu ![ pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, of het** Belangrijkste pictogram van het Menu **pictogram ![ Belangrijkste lijnen van het Menu ](assets/lines-main-menu.png) in de upper-left hoek, dan klik** het pictogram van Rapporten **](assets/reports-in-main-menu.png).**![

1. Klik **Nieuw Rapport**. De lijst met objecttypen wordt weergegeven.
1. Klik **Goedkeuring van het Bewijs** in de lijst.
De rapportaannemer opent.
1. Klik **Filters**, dan klik **voegt een Regel van de Filter** toe.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klik binnen de **Vastgestelde Regels van de Filter voor uw doos van het Rapport**, dan uitgezochte **Goedkeuring van het Bewijs** van de lijst.
1. Klik **is Huidige Versie van het Document** in de lijst onder het **voorwerp van de Goedkeuring van het Bewijs**.
1. Kies Gelijk voor uw filterbepaling, dan uitgezochte Waar.
1. Klik **sparen + Sluiten** in de laag-linkerhoek van Adobe Workfront, dan klik **** in de doos toepassen die verschijnt.

   In het rapport Goedkeuring proef worden alleen de proefdrukken weergegeven die zijn gekoppeld aan de huidige versies van een document, als de proefdrukgoedkeuringen aan deze filtercriteria voldoen.
