---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Een canvasdashboard delen
description: U kunt een Canvas-dashboard delen met andere Adobe Workfront-gebruikers, zodat deze het kunnen bekijken of bewerken.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: ed5a8725442a0b3de993a4e8f47280bfc7d88160
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Een canvasdashboard delen

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Onderdelen van het onderdeel zijn mogelijk niet compleet of werken niet zoals bedoeld in deze fase. Gelieve te dienen om het even welke terugkoppelen betreffende uw ervaring door de instructies in [&#x200B; te volgen verstrekt &#x200B;](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) sectie in het de bètaoverzichtsartikel van de dashboards van het Canvas.<br>
>Als u feedback hebt over een mogelijk probleem met een probleem of een technisch probleem, stuurt u een ticket naar Workfront Support. Voor meer informatie, zie [&#x200B; de Steun van de Klant van het Contact &#x200B;](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Deze bètaversie is niet beschikbaar op de volgende cloudproviders:
>
>* Je eigen sleutel voor Amazon Web Services
>* Azure
>* Google Cloud Platform

U kunt een Canvas-dashboard delen met andere Adobe Workfront-gebruikers, zodat deze het kunnen bekijken of bewerken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td> 
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td> 
   <td><p>Toegang tot rapporten, dashboards en kalenders weergeven</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td><p>Machtigingen voor het dashboard weergeven om het dashboard te delen</p>
   <p>Machtigingen voor het dashboard beheren om dashboardmachtigingen toe te wijzen</p>
  </td> 
  </tr>
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Overwegingen bij het delen van dashboards

* De dashboards kunnen aan gebruiker, team, groep, baanrol, of bedrijfmiddelen worden gedeeld.

* Standaard heeft de maker van een dashboard beheermachtigingen voor het dashboard.

* Systeembeheerders en gebruikers met de machtiging Beheren kunnen View of Manage toegang verlenen tot een dashboard.

* Gebruikers met de machtiging Weergave voor een dashboard kunnen View toegang tot een dashboard verlenen.

* Wanneer het delen van een dashboard, zullen de middelen het met wordt gedeeld toestemmingen aan de rapporten erven die op het dashboard worden getoond.

* Wanneer een dashboard door een lay-outmalplaatje wordt verdeeld, wordt een automatische toestemming van de Mening voor het dashboard (en zijn rapporten) verleend aan alle middelen die aan het lay-outmalplaatje worden toegewezen.


## Een canvasdashboard delen


{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Op de **pagina van de Dashboards van het Canvas**, selecteer het dashboard u wilt delen.

1. In de hoger-juiste hoek van de pagina, klik de **knoop van het Aandeel**. Het **Dashboard dat** dialoogvakje deelt verschijnt.

   ![&#x200B; knoop van het Aandeel &#x200B;](assets/share-button.png)

1. Op **geef toegang tot** gebied, begin het typen van de naam van een specifieke gebruiker, een team, een rol, een groep, of een bedrijf u het Dashboard van het Canvas met wilt delen, dan het wanneer het in de drop-down lijst verschijnt.

1. (Facultatief) om de toegang van een middel tot het dashboard uit te geven, klik **Mening** naast hun naam, dan uitgezocht **leidt** in de drop-down lijst die verschijnt.

   >[!NOTE]
   >
   > Wanneer gebruikers niet de Edit toestemmingen aan een dashboard hebben die door hun toegangsniveau wordt toegewezen, kunnen zij niet worden toegewezen leidt toestemmingen aan een dashboard.

1. Herhaal stap 5-6 voor elke bron waarmee u het dashboard wilt delen.

1. Klik de **knoop van het Aandeel**. De ontvangers ontvangen een e-mailbericht informerend hen dat het dashboard met hen is gedeeld, die zij bij **dashboards** kunnen nu toegang hebben > **de Dashboards van het Canvas** > **Gedeelde dashboards**.

   >[!NOTE]
   >
   > Individuele gebruikersvoorkeuren en systeemuitsluitingen voor e-mailberichten kunnen van toepassing zijn. <br>
   > Meldingen worden alleen verzonden wanneer ze rechtstreeks met een gebruiker worden gedeeld. Het delen aan groepen, rollen, bedrijven, en de teams produceren geen e-mailberichten.<br>
   > De toestemmingen die van een lay-outmalplaatje worden geërft zullen geen e-mailbericht over de toegang tot het dashboard produceren.
