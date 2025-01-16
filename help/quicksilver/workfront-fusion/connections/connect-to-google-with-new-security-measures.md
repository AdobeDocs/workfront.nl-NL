---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Verbind  [!DNL Adobe Workfront Fusion]  met  [!DNL Google Services]  met bijgewerkte veiligheidsmaatregelen
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Verbind [!DNL Adobe Workfront Fusion] met [!DNL Google Services] met bijgewerkte veiligheidsmaatregelen

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ verbind Adobe Workfront Fusion met de Diensten van Google met bijgewerkte veiligheidsmaatregelen ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-google-with-new-security-measures.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

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
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] beperkingen

[!DNL Google] introduceerde beperkingen voor hoe gebruikers hun API kunnen gebruiken vanaf 1 juni 2020. Deze beveiligingsmaatregelen beschermen [!DNL Google] -gebruikers tegen lekkage of misbruik van hun persoonlijke gegevens op [!DNL Google] . De beperkingen hebben betrekking op de apps van [!DNL Gmail] en [!DNL Google Drive] . Voor meer informatie over deze beperkingen, zie &quot;Aanvullende Vereisten voor Specifieke API Scopes&quot;in het [[!DNL Google]  API Beleid van de Gegevens van de Gebruiker van de Diensten ](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Om tot beperkt werkingsgebied toegang te hebben, moet de verbonden dienst ([!DNL Adobe Workfront Fusion] of enige andere dienst die tot de gegevens van de gebruiker via API wil toegang hebben) worden geverifieerd en moet een Brief van Beoordeling hebben om te bewijzen dat de dienst veilig en transparant is over hoe zij de gegevens gebruiken. [!DNL Workfront Fusion] voldoet aan alle vereisten van [!DNL Google] voor toegang tot beperkt bereik. De meeste verbonden services van derden in [!DNL Workfront Fusion] hebben echter geen beoordelingsverklaring en voldoen daarom niet aan de voorwaarden van [!DNL Google] . Daarom mag [!DNL Workfront Fusion] geen gegevens naar deze services verzenden.

## Uitzonderingen op [!DNL Google Services] -beperkingen

Er zijn een paar uitzonderingen die het mogelijk maken om gegevens naar een niet-erkende derdedienst te verzenden die niet de Brief van Beoordeling heeft zonder om het even welke nieuwe beperkingen te schenden. Ze verschillen op basis van [!DNL Google Workspace] met de [!DNL Workfront Fusion] OAuth client [!DNL Google Workspace] met een andere OAuth client, of [!DNL @gmail.com] en [!DNL @google.mail.com] .

* [[!DNL Google Workspace] met  [!DNL Workfront Fusion]  cliënt OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] met een andere OAuth-client](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] en  [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] met [!DNL Workfront Fusion] OAuth-client

[!DNL Workfront Fusion] gebruikt de uitzondering [!UICONTROL Domain-wide Installation] . Installatie in het gehele domein is geschikt voor [!DNL Google Workspace] -gebruikers en staat gebruikers toe om niet-goedgekeurde services zonder beperkingen te integreren. Als u een Google Workspace-gebruiker bent, hoeft u geen extra stappen uit te voeren en kunt u rechtstreeks verbinding maken met niet-goedgekeurde services.

### [!DNL Google Workspace] met een andere OAuth-client

[!DNL Google Workspace] gebruikers die liever hun eigen OAuth-client gebruiken in plaats van de [!DNL Workfront Fusion] OAuth-client, kunnen verbinding maken met [!DNL Google Services] via de [!UICONTROL Internal] Use-benadering. Deze optie is bedoeld voor geavanceerde gebruikers. Voor instructies, zie [  [!DNL Adobe Workfront Fusion]  verbinden  [!DNL Google Services]  gebruikend een cliënt van douaneOAuth ](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] en [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Gebruiker die [!DNL Google Services] tot [!DNL @gmail.com] of [!DNL @googlemail.com] toegang heeft kan met [!DNL Google Services] verbinden door de Persoonlijke benadering van het Gebruik. Deze optie is bedoeld voor geavanceerde gebruikers. Voor instructies, zie [  [!DNL Adobe Workfront Fusion]  verbinden  [!DNL Google Services]  gebruikend een cliënt van douaneOAuth ](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Veelgestelde vragen

* [Welke apps in  [!DNL Adobe Workfront Fusion]  worden beïnvloed?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Heb ik a  [!DNL Google Workspace]  rekening?](#do-i-have-a-g-suite-account)
* [Wat zou ik moeten doen als ik  [!DNL @gmail.com]  of  [!DNL @googlemail.com]  gebruiker ben?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Wat zou ik moeten doen als ik a  [!DNL Google Workspace]  gebruiker ben?](#what-should-i-do-if-im-a-g-suite-user)

### Welke apps in [!DNL Adobe Workfront Fusion] worden beïnvloed? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive] , [!DNL Gmail] en E-mail (verbonden met [!DNL Gmail] -account).

### Heb ik een [!DNL Google Workspace] account? {#do-i-have-a-g-suite-account}

Als uw e-mailadres eindigt met [!DNL @gmail.com] of [!DNL @googlemail.com] is uw account geen [!DNL Google Workspace] -account. Als uw [!DNL Google] -account eindigt met een aangepast domein zoals @my-company.com, is het een [!DNL Google Workspace] -account.

### Wat moet ik doen als ik [!DNL @gmail.com] of [!DNL @googlemail.com] gebruiker ben? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Deze nieuwe beperkingen zijn alleen van toepassing als u [!DNL Google Drive] of [!DNL Gmail] integreert. Als u verbinding wilt maken met [!DNL Google Drive] of [!DNL Gmail] , kunt u

* Overschakelen naar [!DNL Google Workspace]

  of

* Maak een aangepaste OAuth-client. Deze optie is bedoeld voor geavanceerde gebruikers.

  Voor instructies, zie [  [!DNL Adobe Workfront Fusion]  verbinden  [!DNL Google Services]  gebruikend een cliënt van douaneOAuth ](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Als u een andere service dan [!DNL Google Drive] of [!DNL Gmail] wilt integreren, zijn deze beperkingen niet van toepassing.

Voor instructies over het verbinden van andere [!DNL Google Services] met [!DNL Workfront Fusion], zie [ app of Webdienst van de module verbinden met  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) in het artikel [ creeer een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Wat moet ik doen als ik een [!DNL Google Workspace] gebruiker ben? {#what-should-i-do-if-im-a-g-suite-user}

Er is geen vereiste actie.
