---
title: Roep de WEERGAVE API van de Grafiek van MS via  [!DNL Adobe Workfront Fusion]  HTTP &gt; maak een OAuth 2.0 verzoekmodule
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Roep de module [!UICONTROL  MS Graph REST API] aan via de module [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] .

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Vraag de REST API van de Grafiek van MS ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

<!-- Audited: 3/2024-->

Veel [!DNL Microsoft] -webservices zijn toegankelijk via [!DNL Microsoft Graph API] . U kunt een verbinding met de [!DNL Microsoft Graph API] maken met de module [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Make an OAuth 2.0 request] .

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
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidig: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidig: Geen [!DNL Workfront Fusion] vereiste licentie.</p>
   <p>of</p>
   <p>Verouderd: alle </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Plan: Uw organisatie moet het abonnement aanschaffen [!DNL Adobe Workfront Fusion] .</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Overzicht: [!DNL Workfront Fusion] is opgenomen.</li></ul>
   <p>of</p>
   <p>Huidig: Uw organisatie moet [!DNL Adobe Workfront Fusion] aanschaffen.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Registreren [!DNL Workfront Fusion] in de [!DNL Microsoft Application Registration Portal]

Als u een verbinding met de [!DNL Microsoft Graph REST API] wilt maken, moet u eerst [!DNL Adobe Workfront Fusion] registreren.

1. Begin registrerend een nieuwe toepassing zoals die in [ wordt beschreven registreer uw app ](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in de [!DNL Microsoft] documentatie.

   Als onderdeel van de registratie vereist [!DNL Microsoft] de volgende informatie:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Voer een naam voor de toepassing in, bijvoorbeeld "Mijn [!DNL Workfront Fusion] toepassing".</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Wanneer u de registratie van de app hebt voltooid, noteert u de [!UICONTROL Application ID] .

   >[!IMPORTANT]
   >
   >U hebt de toepassings-id nodig om de verbinding in te stellen in [!DNL Workfront Fusion] .

1. Een [!UICONTROL Application Secret] genereren. Noteer dit geheim.

   Voor instructies, zie [ registreren uw app ](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in de [!DNL Microsoft] documentatie.

   >[!IMPORTANT]
   >
   >U hebt de [!UICONTROL Application Secret] nodig om uw verbinding in te stellen in [!DNL Workfront Fusion] .

1. Configureer de machtigingen voor uw toepassing.

   Voor details bij het bepalen van en het vormen van deze gebieden, zie de &quot;toestemmingen voor de Grafiek van Microsoft&quot;sectie in [ toegang zonder een gebruiker ](https://docs.microsoft.com/en-us/graph/auth-v2-service) in de [!UICONTROL Microsoft] documentatie krijgen.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td>Selecteer <code>[!UICONTROL Delegated permissions]</code> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>Selecteer de volgende machtigingen:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Eventuele andere machtigingen die vereist zijn voor uw integratie (bijvoorbeeld: <code>User.Read</code>)</p> </li> 
       </ul> <p><b> Belangrijk </b>: U zult de geselecteerde toestemmingen aan opstelling uw verbinding in [!DNL Workfront Fusion] nodig hebben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ga aan [ te werk vormen uw  [!DNL MS Graph API]  verbinding in  [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Uw [!DNL MS Graph API] verbinding configureren in [!DNL Workfront Fusion]

Nadat u [!DNL Workfront Fusion] zoals besproken in [ Register  [!DNL Workfront Fusion]  in  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal) registreert, kunt u uw verbinding in [!UICONTROL HTTP] vormen > [!UICONTROL Make an Oauth 2.0] verzoekmodule.

1. Voeg een module [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 call] toe aan uw scenario.
1. Klik op **[!UICONTROL Add]** naast het veld [!UICONTROL connection] .
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
      <td> <p>Ga de toestemmingen in die u in stap 4 van <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref"> Register [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a> selecteerde.</p> <p>Voor elk bereik klikt u op <b>[!UICONTROL Add]</b> en typt u de machtiging.</p> <p>Voorbeeld: <code>offline_access</code> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Ga [!UICONTROL Application ID] van stap 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref"> Register [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a> in.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Ga [!UICONTROL Application Secret] in dat u in stap 3 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref"> Register [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a> produceerde.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>Voeg de volgende machtigingsparameters toe:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value] : <code>query</code></p> </li> 
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
        <li value="2"> <p>Typ <code>scope</code> in het veld <b>[!UICONTROL Key]</b> .</p> </li> 
        <li value="3"> <p>Voer in het veld <b>[!UICONTROL Value]</b> alle [!UICONTROL scope] s in die u in het bereikveld hebt ingevoerd, gescheiden door spaties.</p> <p>Voorbeeld: <code>offline_access openid User.Read</code></p> </li> 
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
1. Klik in het venster dat wordt weergegeven op **[!UICONTROL Accept]** om de verbinding te voltooien en terug te keren naar de module.
