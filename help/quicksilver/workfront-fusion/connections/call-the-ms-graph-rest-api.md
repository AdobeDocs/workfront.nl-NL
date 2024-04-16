---
title: De MS Graph REST API bellen via de [!DNL Adobe Workfront Fusion] HTTP &gt; een OAuth 2.0-aanvraagmodule maken
description: De MS Graph REST API bellen via de [!DNL Adobe Workfront Fusion] HTTP &gt; een OAuth 2.0-aanvraagmodule maken
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# Roep de[!UICONTROL  MS Graph REST API] via de [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module

<!-- Audited: 3/2024-->

Veel [!DNL Microsoft] webservices zijn toegankelijk via [!DNL Microsoft Graph API]. U kunt een verbinding maken met de [!DNL Microsoft Graph API]door de [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Make an OAuth 2.0 request] -module.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidige: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidig: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Verouderd: alle </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Abonnement: uw organisatie moet aankopen [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is opgenomen.</li></ul>
   <p>of</p>
   <p>Huidig: Uw organisatie moet het volgende aanschaffen [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Registreren [!DNL Workfront Fusion] in de [!DNL Microsoft Application Registration Portal]

Een verbinding maken met de [!DNL Microsoft Graph REST API], u moet zich eerst registreren [!DNL Adobe Workfront Fusion].

1. Start met de registratie van een nieuwe toepassing zoals beschreven in [Uw app registreren](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in de [!DNL Microsoft] documentatie.

   Als onderdeel van de registratie: [!DNL Microsoft] vereist de volgende informatie:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Voer een naam in voor de toepassing, bijvoorbeeld "Mijn [!DNL Workfront Fusion] toepassing."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Wanneer u de registratie van de app hebt voltooid, neemt u nota van de [!UICONTROL Application ID].

   >[!IMPORTANT]
   >
   >U hebt de toepassings-id nodig om uw verbinding in te stellen in [!DNL Workfront Fusion].

1. Een [!UICONTROL Application Secret]. Noteer dit geheim.

   Zie voor instructies [Uw app registreren](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in de [!DNL Microsoft] documentatie.

   >[!IMPORTANT]
   >
   >U hebt de [!UICONTROL Application Secret] om uw verbinding in te stellen [!DNL Workfront Fusion].

1. Configureer de machtigingen voor uw toepassing.

   Zie de sectie &quot;Machtigingen voor Microsoft Graph configureren&quot; in [Toegang krijgen zonder een gebruiker](https://docs.microsoft.com/en-us/graph/auth-v2-service) in de [!UICONTROL Microsoft] documentatie.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td>Selecteren <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>Selecteer de volgende machtigingen:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Eventuele andere machtigingen die vereist zijn voor uw integratie (voorbeeld: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Belangrijk</b>: U hebt de geselecteerde machtigingen nodig om uw verbinding in te stellen in [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Doorgaan naar [Configureer uw [!DNL MS Graph API] verbinding in [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configureer uw [!DNL MS Graph API] verbinding in [!DNL Workfront Fusion]

Nadat u zich hebt geregistreerd [!DNL Workfront Fusion] zoals besproken in [Registreren [!DNL Workfront Fusion] in de [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)kunt u uw verbinding configureren in het dialoogvenster [!UICONTROL HTTP] > [!UICONTROL Make an Oauth 2.0] aanvraagmodule.

1. Een [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 call] aan uw scenario.
1. Klikken **[!UICONTROL Add]** naast de [!UICONTROL connection] veld.
1. Configureer de verbindingsvelden als volgt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Voer een naam in voor de verbinding.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Voer de machtigingen in die u in stap 4 van <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registreren [!DNL Workfront Fusion] in de [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Voor elk bereik klikt u op <b>[!UICONTROL Add]</b> en typ de machtiging.</p> <p>Voorbeeld: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Voer de [!UICONTROL Application ID] vanaf stap 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registreren [!DNL Workfront Fusion] in de [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Voer de [!UICONTROL Application Secret] die u in stap 3 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registreren [!DNL Workfront Fusion] in de [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>Voeg de volgende machtigingsparameters toe:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>U hoeft niets in dit veld in te voeren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Refresh token parameters]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klik op <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>In de <b>[!UICONTROL Key]</b> veld, Enter <code>scope</code>.</p> </li> 
        <li value="3"> <p>In de <b>[!UICONTROL Value]</b> veld, voert u alle [!UICONTROL scope]In het bereikveld hebt u een waarde ingevoerd, gescheiden door spaties.</p> <p>Voorbeeld: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>U hoeft niets in dit veld in te voeren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Continue]**.
1. Klik in het venster dat wordt weergegeven op **[!UICONTROL Accept]** om de verbinding te voltooien en aan de module terug te keren.
