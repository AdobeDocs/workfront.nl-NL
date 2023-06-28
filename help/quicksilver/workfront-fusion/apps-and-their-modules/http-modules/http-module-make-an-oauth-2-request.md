---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP &gt; Een OAuth 2.0-aanvraagmodule maken
description: Om een [!DNL Adobe Workfront Fusion] HTTP(S) verzoek aan servers die een vergunning OAuth 2.0 vereisen, moet u eerst een verbinding OAuth tot stand brengen. [!DNL Adobe Workfront Fusion] zorgt ervoor dat alle vraag die met deze verbinding wordt gemaakt de aangewezen vergunningskopballen heeft en automatisch bijbehorende tokens verfrist wanneer vereist.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1919'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] vereist een [!DNL Adobe Workfront Fusion] naast een [!DNL Adobe Workfront] licentie.

Om een [!DNL Adobe Workfront Fusion] HTTP(S) verzoek aan servers die een vergunning OAuth 2.0 vereisen, moet u eerst een verbinding OAuth tot stand brengen. [!DNL Adobe Workfront Fusion] zorgt ervoor dat alle vraag die met deze verbinding wordt gemaakt de aangewezen vergunningskopballen heeft en automatisch bijbehorende tokens verfrist wanneer vereist.

[!DNL Workfront Fusion] steunt de volgende OAuth 2.0 authentificatiestromen:

* Vergunningscode-stroom
* Impliciete stroom

Andere stromen, zoals de Stroom van de Referenties van het Wachtwoord van de Eigenaar van het Middel en de Stroom van de Referenties van de Cliënt, worden niet automatisch gesteund door deze module.

Voor meer informatie over OAuth 2.0 authentificatie, zie [OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749).

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Verbinding maken voor een [!DNL OAuth] verzoek

* [Algemene instructies voor het maken van een verbinding in HTTP > Een OAuth 2.0-aanvraagmodule maken](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Instructies voor het maken van een verbinding met Google via HTTP >[!UICONTROL Make] een OAuth 2.0 verzoekmodule](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Instructies voor verbinding met de Microsoft Graph API via HTTP > Make an OAuth 2.0 request module](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Algemene instructies voor het maken van een verbinding in het dialoogvenster [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module

1. Een OAuth-client maken in het dialoogvenster [!DNL target] de dienst waarmee u wilt [!DNL Adobe Workfront Fusion] om te communiceren. Deze optie is meestal te vinden in het dialoogvenster [!UICONTROL Developer] van de dienst.

   1. Wanneer u een client maakt, voert u de juiste URL in het dialoogvenster `[!UICONTROL Redirect URL]` of `[!UICONTROL Callback URL]` veld:

      | Amerika/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. Nadat u de cliënt creeert, toont de bepaalde dienst 2 sleutels: `[!UICONTROL Client ID]` en `[!UICONTROL Client Secret]`. Sommige services noemen dit `[!UICONTROL App Key]` en `[!UICONTROL App Secret]` . Sla de sleutel en het geheim op een veilige locatie op, zodat u deze kunt opgeven wanneer u de verbinding maakt in Workfront Fusion.

1. Zoek de `[!UICONTROL Authorize URI]` en `[!UICONTROL Token URI]` in de API-documentatie van de desbetreffende service. Dit zijn URL-adressen waardoor [!DNL Workfront Fusion] communiceert met de [!DNL target] service. De adressen dienen voor vergunning OAuth.

   >[!NOTE]
   >
   >Als de dienst Impliciete stroom gebruikt, zult u slechts nodig hebben `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Voorbeeld:** Yahoo-adressen:
   >
   >* URI autoriseren:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* Token-URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Voorwaardelijk) als de doeldienst werkingsgebied (toegangsrechten) gebruikt, controleer hoe de dienst individueel werkingsgebied scheidt en zorg ervoor u de separator in de geavanceerde montages dienovereenkomstig plaatst. Als het scheidingsteken niet correct is ingesteld, [!DNL Workfront Fusion] kan geen verbinding maken en er is een ongeldige bereikfout opgetreden.
1. Nadat u de bovenstaande stappen hebt uitgevoerd, kunt u de OAuth-verbinding maken in [!DNL Workfront Fusion]. Voeg de OAuth 2.0 HTTP(S) verzoek en reactieverwerkingsmodule aan uw scenario toe.
1. Klik in het veld Verbinding van de module op **[!UICONTROL Add]**.

1. Vul de volgende velden in om een verbinding te maken:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Voer de naam van de verbinding in.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>Selecteer de stroom voor het verkrijgen van tokens.</p> 
       <ul> 
        <li><strong>[!UICONTROL Authorization Code]</strong>: Voer de <code>[!UICONTROL Authorize URI]</code> en <code>[!UICONTROL Token URI]</code> uit de API-documentatie van de service.</li> 
        <li><strong>[!UICONTROL Implicit]</strong>: Voer de <code>[!UICONTROL Authorize URI]</code> uit de API-documentatie van de service.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Afzonderlijk bereik toevoegen. U kunt deze informatie in de bepaalde de ontwikkelaar (API) documentatie van de dienst vinden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>Selecteer door welk bereik de bovenstaande gegevens moeten worden gescheiden. U kunt deze informatie in de bepaalde de ontwikkelaar (API) documentatie van de dienst vinden.</p> <p>Waarschuwing: Als het scheidingsteken niet correct is ingesteld, [!DNL Workfront Fusion] kan geen verbinding maken en er is een ongeldige bereikfout opgetreden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Voer de client-id in. U hebt de client-id opgehaald toen u een OAuth-client hebt gemaakt in de service waarmee u verbinding wilt maken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> Voer het clientgeheim in. U verkrijgt het Geheime punt van de Cliënt toen u een cliënt OAuth in de dienst creeerde u wilt verbinden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>Voeg om het even welke parameters toe die u in de vergunningsvraag wilt omvatten. De volgende standaardparameters worden altijd automatisch opgenomen en hoeven niet te worden toegevoegd.</p> <p>Standaardparameters:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>for [!UICONTROL Authorization Code flow] en <code>token </code>for [!UICONTROL Implicit flow]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amerika/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> De client-id die u hebt ontvangen bij het maken van de account</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Access token parameters]</p> </td> 
      <td> <p>Voeg om het even welke parameters toe die u in de symbolische vraag wilt omvatten. De volgende standaardparameters worden altijd automatisch opgenomen en hoeven niet te worden toegevoegd.</p> <p>Standaardparameters:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amerika/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: De client-id die u hebt ontvangen bij het maken van de account, wordt automatisch opgenomen in de aanvraaginstantie</li> 
        <li><strong>client_geheime</strong>: Het clientgeheim dat u hebt ontvangen bij het maken van de account, wordt automatisch opgenomen in de aanvraaginstantie</li> 
        <li><strong>code</strong>: De code die door het vergunningsverzoek wordt geretourneerd</li> 
       </ul> <p>Opmerking:  <p>De norm OAuth 2.0 steunt minstens 2 methodes van cliëntauthentificatie tijdens deze stap (<code>[!UICONTROL client_secret_basic]</code> en <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] verzendt automatisch de opgegeven client-id en verzendt het geheim door de <code>[!UICONTROL client_secret_post]</code> methode. Daarom zijn deze parameters automatisch inbegrepen als deel van het symbolische verzoeklichaam. </p> <p>Voor meer informatie over OAuth 2.0 authentificatie, zie <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Refresh token parameters]</p> </td> 
      <td> <p>Voeg om het even welke parameters toe die u in de symbolische vraag wilt omvatten. De volgende standaardparameters worden altijd automatisch opgenomen en hoeven niet te worden toegevoegd.</p> <p>Standaardparameters:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: Het meest recente vernieuwingstoken dat door de dienst wordt verkregen u met verbindt</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: De client-id die u hebt ontvangen bij het maken van de account, wordt automatisch opgenomen in de aanvraaginstantie</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: Het clientgeheim dat u hebt ontvangen bij het maken van de account, wordt automatisch opgenomen in de aanvraaginstantie</p> </li> 
       </ul> <p>Opmerking:  <p>De norm OAuth 2.0 steunt minstens 2 methodes van cliëntauthentificatie tijdens deze stap (<code>[!UICONTROL client_secret_basic]</code> en <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] verzendt automatisch de opgegeven client-id en verzendt het geheim door de <code>[!UICONTROL client_secret_post]</code> methode. Daarom zijn deze parameters automatisch inbegrepen als deel van het symbolische verzoeklichaam. </p> <p>Voor meer informatie over OAuth 2.0 authentificatie, zie <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Custom Headers]</p> </td> 
      <td> <p>Geef aanvullende sleutels en waarden op die u in de koptekst van [!UICONTROL Token] en R[!UICONTROL efresh Token] stappen.</p> <p>Opmerking:  <p>De norm OAuth 2.0 steunt minstens 2 methodes van cliëntauthentificatie tijdens deze stap (<code>[!UICONTROL client_secret_basic]</code> en <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] biedt niet automatisch ondersteuning voor de <code>[!UICONTROL client_secret_basic]</code> methode. Als de dienst die u verbindt om Cliënt te verwachten - identiteitskaart en Geheim om in één enkel koord worden gecombineerd en dan base64 die in de kopbal van de Vergunning wordt gecodeerd, dan zou u die kopbal en zeer belangrijke waarde hier moeten toevoegen.</p> <p> Voor meer informatie over OAuth 2.0 authentificatie, zie <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Geef op of u het token wilt verzenden in het dialoogvenster [!UICONTROL header], [!UICONTROL query string]of in beide gevallen wanneer verbinding wordt gemaakt met de opgegeven URL.</p> <p>Tokens worden meestal verzonden in de verzoekkopbal.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Header token name] </td> 
      <td> <p>Voer de naam van het machtigingstoken in de koptekst in. Standaard: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Query string parameter name] </td> 
      <td> <p>Voer de naam van het verificatietoken in de queryreeks in. Standaard: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Continue]** om verbindingsinstellingen op te slaan.
1. Doorgaan naar [OAuth 2.0 opstelling van de verzoekmodule](#oauth-20-request-module-setup).

### Instructies voor het maken van een verbinding met [!DNL Google] in de [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request module]

In het volgende voorbeeld wordt getoond hoe u de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0] request module to connect to [!DNL Google].

1. Zorg ervoor dat u een project, gevormde montages OAuth hebt gecreeerd, en uw geloofsbrieven zoals die in worden beschreven geproduceerd [Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Open de [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request] module.
1. Klikken **[!UICONTROL Add]** naast het verbindingsvak.
1. Voer de volgende waarden in:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Voer de naam van de verbinding in.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>[!UICONTROL Authorization Code]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Afzonderlijk bereik toevoegen. Zie voor meer informatie over het bereik <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O-bereiken voor [!DNL Google] API's</a> in de [!DNL Google] documentatie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Voer uw [!DNL Google] Client-id. </p> <p>Als u een client-id wilt maken, raadpleegt u <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth-referenties maken</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>Voer uw [!DNL Google] Clientgeheim. </p> <p>Als u een clientgeheim wilt maken, raadpleegt u <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth-referenties maken</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] tot [!DNL Google] Services die een aangepaste OAuth-client gebruiken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>Toevoegen <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>sleutelwaardepaar.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Opmerking: Als u verificatieproblemen ondervindt, bijvoorbeeld bij het vernieuwen van token, kunt u het volgende toevoegen: <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>sleutelwaardepaar.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Continue]** om verbindingsinstellingen op te slaan.
1. Doorgaan naar [OAuth 2.0 opstelling van de verzoekmodule](#oauth-20-request-module-setup).

### Instructies voor verbinding maken met [!DNL Microsoft Graph API] via de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module

Voor instructies over [!DNL Microsoft Graph API], zie [Roep de [!DNL MS Graph REST API] via de [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0 opstelling van de verzoekmodule

Wanneer u een [!DNL Oauth 2].0 verbinding zoals beschreven in [Verbinding maken voor een [!DNL OAuth] verzoek](#creating-a-connection-for-an-oauth-request)zet u de module naar wens in. Alle toestemmingstokens worden automatisch inbegrepen in dit verzoek, en in een ander verzoek dat de zelfde verbinding gebruikt.

Wanneer u vormt [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request] module, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor informatie over het instellen van een verbinding raadpleegt u <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Verbinding maken voor een OAuth-verzoek</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx]) </td> 
   <td> <p>Gebruik deze optie om foutafhandeling in te stellen.</p> <p>Zie voor meer informatie <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Foutafhandeling in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Voer de URL in waarnaar u een aanvraag wilt verzenden, zoals een API-eindpunt, website, enzovoort.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voer de gewenste sleutel-waardeparen voor de query in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>De hoofdtekst van HTTP is de gegevensbytes die in een HTTP- transactiebericht onmiddellijk na de kopballen worden overgebracht als er om het even welk zijn om worden gebruikt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Het type Raw-hoofdtekst is over het algemeen geschikt voor de meeste HTTP-hoofdtekstaanvragen, zelfs in situaties waarin in de documentatie van de ontwikkelaar geen gegevens zijn opgegeven die moeten worden verzonden.</p> <p>Geef een vorm op voor het parseren van de gegevens in het dialoogvenster [!UICONTROL Content type] veld.</p> <p>Ondanks het geselecteerde inhoudstype, worden de gegevens ingevoerd in om het even welk formaat dat door de ontwikkelaarsdocumentatie wordt bepaald of wordt vereist.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Dit lichaamstype is aan POST gegevens gebruikend <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>Voor <code>[!UICONTROL application/x-www-form-urlencoded]</code>, is de hoofdtekst van het HTTP-bericht dat naar de server wordt verzonden, in wezen één queryreeks. De toetsen en waarden worden gecodeerd in sleutelwaardeparen, gescheiden door <code>&amp;</code> en met een <code>=</code> tussen de toets en de waarde. </p> <p>Voor binaire gegevens, <code>use [!UICONTROL multipart/form-data]</code> in plaats daarvan.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Voorbeeld: </b></span></span> 
       <p>Voorbeeld van de resulterende HTTP-aanvraagindeling:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>De [!UICONTROL Multipart/form-data] is een multipart HTTP-aanvraag die wordt gebruikt om bestanden en gegevens te verzenden. Het wordt doorgaans gebruikt om bestanden naar de server te uploaden.</p> <p>Voeg velden toe die in de aanvraag moeten worden verzonden. Elk veld moet een sleutelwaardepaar bevatten.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Voer de sleutel en waarde in die binnen de aanvraaginstantie moeten worden verzonden.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Voer de sleutel in en geef het bronbestand op dat u wilt verzenden in de hoofdtekst van de aanvraag.</p> <p>Wijs het bestand toe dat u uit de vorige module wilt uploaden (bijvoorbeeld [!UICONTROL HTTP] &gt;[!UICONTROL Get a File] of [!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]of voer de bestandsnaam en de bestandsgegevens handmatig in.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Schakel deze optie in om reacties automatisch te parseren en JSON- en XML-reacties om te zetten zodat u deze niet hoeft te gebruiken [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] of [!UICONTROL XML] &gt; [!UICONTROL Parse XML] modules.</p> <p>Voordat u geparseerde JSON- of XML-inhoud kunt gebruiken, voert u de module één keer handmatig uit, zodat de module de inhoud van de reactie herkent en deze in volgende modules kunt toewijzen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Voer de time-out van het verzoek in seconden in (1-300). De standaardwaarde is 40 seconden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Share cookies with other HTTP modules]</td> 
   <td> <p> Schakel deze optie in om cookies van de server te delen met alle HTTP-modules in uw scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> Upload uw certificaat als u TLS wilt gebruiken met uw zelfondertekende certificaat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reject connections that are using unverified (self-signed) certificates] </td> 
   <td> <p>Schakel deze optie in om verbindingen die niet-geverifieerde TLS-certificaten gebruiken, te weigeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> Schakel deze optie in om de URL-omleidingen te volgen met 3xx-reacties.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow all redirects] </td> 
   <td> <p>Schakel deze optie in om de URL-omleidingen te volgen met alle antwoordcodes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disable serialization of multiple same query string keys as arrays]</p> </td> 
   <td> <p>Standaard, [!DNL Workfront Fusion] Verwerkt meerdere waarden voor dezelfde URL-querytekenreeks-parametersleutel als arrays. Bijvoorbeeld: <code>www.test.com?foo=bar&amp;foo=baz</code> wordt omgezet in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Activeer deze optie om deze functie uit te schakelen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> Schakel deze optie in om een gecomprimeerde versie van de website aan te vragen.</p> <p>Hiermee voegt u een <code>[!UICONTROL Accept-Encoding]</code> om gecomprimeerde inhoud aan te vragen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>Schakel deze optie in om Wederzijdse TLS te gebruiken in de HTTP-aanvraag.</p> <p>Voor meer informatie over wederzijdse TLS raadpleegt u <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Wederzijdse TLS gebruiken in HTTP-modules in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
