---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gebruik cURL om een HTTP-module toe te voegen
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Gebruik cURL om een HTTP-module toe te voegen

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Gebruik cURL om een module van HTTP toe te voegen ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/use-curl-create-http.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

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

Als uw cURL niet in uw scenario kleeft, controleer uw browser montages om ervoor te zorgen dat het kleven van het klembord wordt toegelaten.


