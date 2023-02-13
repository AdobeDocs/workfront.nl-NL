---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] met bijgewerkte veiligheidsmaatregelen
description: Google heeft onlangs beperkingen geïntroduceerd op de manier waarop gebruikers hun API kunnen gebruiken. In dit artikel wordt beschreven hoe u verbinding kunt maken [!DNL Adobe Workfront Fusion] naar Google, met verantwoording voor deze bijgewerkte beveiligingsmaatregelen.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] met bijgewerkte veiligheidsmaatregelen

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] beperkingen

[!DNL Google] zijn beperkingen ingevoerd voor de manier waarop gebruikers hun API kunnen gebruiken vanaf 1 juni 2020. Deze beveiligingsmaatregelen beschermen [!DNL Google] gebruikers door lekkage of misbruik van hun persoonsgegevens over [!DNL Google]. De beperkingen houden verband met de [!DNL Gmail] en [!DNL Google Drive] apps. Zie voor meer informatie over deze beperkingen &quot;Aanvullende vereisten voor specifieke API-bereiken&quot; in het gedeelte [[!DNL Google] Gebruikersgegevensbeleid voor API-services](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Om toegang te krijgen tot beperkt bereik, de verbonden dienst ([!DNL Adobe Workfront Fusion] of elke andere service die via de API toegang wil krijgen tot de gegevens van de gebruiker, moet worden geverifieerd en moet een beoordelingsverklaring hebben om aan te tonen dat de service veilig en transparant is over de manier waarop de gegevens worden gebruikt. [!DNL Workfront Fusion] voldoet aan alle [!DNL Google]de vereisten voor toegang tot beperkte reikwijdte. De meeste verbonden diensten van derden in [!DNL Workfront Fusion] niet over de beoordelingsverklaring beschikken en daarom niet voldoen aan [!DNL Google] voorwaarden. Daarom, [!DNL Workfront Fusion] mogen geen gegevens naar deze services verzenden.

## Uitzonderingen op [!DNL Google Services] beperkingen

Er zijn een paar uitzonderingen die het mogelijk maken om gegevens naar een niet-erkende derdedienst te verzenden die niet de Brief van Beoordeling heeft zonder om het even welke nieuwe beperkingen te schenden. Ze verschillen op basis van [!DNL G Suite] met de [!DNL Workfront Fusion] OAuth-client, [!DNL G Suite] met een andere OAuth-client, of [!DNL @gmail.com] en [!DNL @google.mail.com].

* [[!DNL G-suite] met [!DNL Workfront Fusion] OAuth-client](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G-suite] met een andere OAuth-client](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] en [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] with [!DNL Workfront Fusion] OAuth-client

[!DNL Workfront Fusion] gebruikt de [!UICONTROL Domain-wide Installation] uitzondering. Installatie in het gehele domein is geschikt voor [!DNL G Suite] gebruikers, en staat gebruikers toe om de niet erkende diensten zonder enige beperkingen te integreren. Als u een gebruiker van de Reeks van G bent, moet u geen extra stappen uitvoeren en kunt direct met niet goedgekeurde diensten verbinden.

### [!DNL G suite] met een andere OAuth-client

[!DNL G Suite] gebruikers die liever hun eigen OAuth-client gebruiken in plaats van de [!DNL Workfront Fusion] OAuth-client kan verbinding maken met [!DNL Google Services] via de [!UICONTROL Internal] Gebruik deze benadering. Deze optie is bedoeld voor geavanceerde gebruikers. Zie voor instructies [Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] en [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Gebruiker die toegang heeft [!DNL Google Services] doorheen [!DNL @gmail.com] of [!DNL @googlemail.com] kan verbinding maken met [!DNL Google Services] door de Persoonlijke benadering van het Gebruik. Deze optie is bedoeld voor geavanceerde gebruikers. Zie voor instructies [Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Veelgestelde vragen

* [Toepassingen in [!DNL Adobe Workfront Fusion] worden beïnvloed?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Heb ik een [!DNL G Suite] account?](#do-i-have-a-g-suite-account)
* [Wat moet ik doen als ik [!DNL @gmail.com] of [!DNL @googlemail.com] gebruiker?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Wat moet ik doen als ik een [!DNL G Suite] gebruiker ben?](#what-should-i-do-if-im-a-g-suite-user)

### Toepassingen in [!DNL Adobe Workfront Fusion] worden beïnvloed? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]en e-mail (verbonden met [!DNL Gmail] account).

### Heb ik een [!DNL G Suite] account? {#do-i-have-a-g-suite-account}

Als uw e-mailadres eindigt met [!DNL @gmail.com] of [!DNL @googlemail.com] uw account is geen [!DNL G Suite] account. Als uw [!DNL Google] account eindigt met een aangepast domein, zoals @my-company.com, dan is het een [!DNL G Suite] account.

### Wat moet ik doen als ik [!DNL @gmail.com] of [!DNL @googlemail.com] gebruiker? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Deze nieuwe beperkingen zijn alleen van toepassing als u [!DNL Google Drive] of [!DNL Gmail]. Als u verbinding wilt maken met [!DNL Google Drive] of [!DNL Gmail], kunt u

* Overschakelen op [!DNL G Suite]

   of

* Maak een aangepaste OAuth-client. Deze optie is bedoeld voor geavanceerde gebruikers.

   Zie voor instructies [Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Als u een andere dienst wilt integreren dan [!DNL Google Drive] of [!DNL Gmail]Deze beperkingen zijn echter niet van toepassing.

Voor instructies over het verbinden van elkaar [!DNL Google Services] tot [!DNL Workfront Fusion], zie [Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) in het artikel [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Wat moet ik doen als ik een [!DNL G Suite] gebruiker? {#what-should-i-do-if-im-a-g-suite-user}

Er is geen vereiste actie.
