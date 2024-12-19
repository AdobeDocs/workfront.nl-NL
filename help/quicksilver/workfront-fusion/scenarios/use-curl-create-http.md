---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gebruik cURL om een HTTP-module toe te voegen
description: U kunt een cURL-aanvraag in uw scenario plakken en Fusion maakt een HTTP-module die is geconfigureerd via de cURL-aanvraag.
author: Becky
feature: Workfront Fusion
source-git-commit: 4cc881f4f5a28bd105e6898ad7ffb57c1dafb563
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Gebruik cURL om een HTTP-module toe te voegen

U kunt een cURL-aanvraag in uw scenario plakken en Fusion maakt een HTTP-module die is geconfigureerd via de cURL-aanvraag.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront-plan</td>  
      <td>Alle</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-licentie</td>  
      <td>
        Nieuw: Standaard <br>
        Of<br>
        Huidig: Werk of hoger
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-licentie</td>  
      <td> 
        Huidig: Geen Workfront Fusion-licentievereisten.<br>
        Of<br>
        Verouderd: alle
      </td>  
    </tr>  
    <tr>  
      <td>Product</td>  
      <td> 
        Nieuw: Select- of Prime Workfront-abonnement: uw organisatie moet Adobe Workfront Fusion aanschaffen.<br>
        Ultimate Workfront Plan: Workfront Fusion is inbegrepen.<br>
        Of<br>
        Huidig: Uw organisatie moet Adobe Workfront Fusion aanschaffen.
      </td>  
    </tr> 
  </tbody>  
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Een HTTP-module maken van een cURL-aanvraag


Een HTTP-module maken met cURL:

1. Maak de tekst van het cURL-verzoek buiten Fusion, bijvoorbeeld in een teksteditor.

   >[!IMPORTANT]
   >
   >Als u Fusion gebruikt op een Windows-computer, mag uw cURL-aanvraag geen regeleinden bevatten.
1. Kopieer de cURL-aanvraag naar het klembord.
1. Klik op de tab **[!UICONTROL Scenario]** in het linkerdeelvenster.
1. Selecteer het scenario waar u de module wilt tot stand brengen.
1. Klik overal op het scenario om de redacteur van het Scenario in te gaan.
1. Klik op om het even welke witte ruimte in de scenarioredacteur met de rechtermuisknop aan en selecteer **Deeg**.

   of

   Druk op Ctrl + V (Windows) of Cmd + V (Mac).


   Er wordt een HTML-module gemaakt.
1. Sleep de module om het met uw scenario te verbinden.

## Problemen oplossen

Als uw cURL niet in uw scenario kleeft, controleer het volgende:

* Controleer de browserinstellingen om ervoor te zorgen dat plakken vanaf het klembord is ingeschakeld.
* Als u Windows uitvoert, controleert u het cURL-verzoek om ervoor te zorgen dat er geen regeleinden worden opgenomen.



