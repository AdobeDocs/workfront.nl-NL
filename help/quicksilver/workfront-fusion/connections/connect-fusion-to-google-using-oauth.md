---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Verbind  [!DNL Adobe Workfront Fusion]  met  [!DNL Google Services]  gebruikend een cliënt van douaneOAuth
description: U kunt  [!DNL Adobe Workfront Fusion]  gebruiken om met  [!DNL Google Services]  te verbinden gebruikend een cliënt van douaneOAuth. Deze procedure vereist een bestaande  [!DNL Google]  rekening.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Verbind [!DNL Adobe Workfront Fusion] met [!DNL Google Services] gebruikend een douaneOAuth cliënt

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

## Vereisten

U hebt een bestaande [!DNL Google] account nodig om deze verbinding te maken.

## Connect Fusion to Google-services met een aangepaste OAuth-client

Als u deze verbinding wilt maken, moet u een project maken en configureren op het Google Cloud-platform en vervolgens de verbinding configureren in Fusion op basis van dat project.

* [Een project maken op  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [ vorm [!UICONTROL OAuth consent] montages ](#configure-oauth-consent-settings)
* [OAuth-referenties maken](#create-oauth-credentials)
* [Verbind met  [!DNL Google]  binnen  [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Deze procedure is bedoeld voor:
>
>* Persoonlijk gebruik ([!DNL `@gmail.com`] en [!DNL `@googlemail.com`] gebruikers)
>* Intern gebruik ([!DNL Google Workspace] gebruikers die verkiezen om een douaneOAuth cliënt te gebruiken)

### Een project maken op [!DNL Google Cloud Platform]

Een project maken op [!DNL Google Cloud] Platform:

1. Teken binnen aan [[!DNL Google Cloud]  Platform ](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) gebruikend uw [!DNL Google] geloofsbrieven.
1. Klik in het linkerdeelvenster op **[!UICONTROL Dashboard]** .
1. Klik op **[!UICONTROL Create project]** in de rechterbovenhoek van het scherm.
1. Voer de **[!UICONTROL Project name]** in en klik op **[!UICONTROL Create]** .

1. Klik op de tab **[!UICONTROL Enable APIs and services]** boven in het scherm.
1. Typ in het veld **[!UICONTROL Search for APIs and Services]** boven in het scherm de naam van de service die u wilt gebruiken (zoals [!DNL Gmail] API of [!DNL Google Drive] API).
1. Wanneer deze wordt weergegeven, klikt u op de API of service waarmee u verbinding wilt maken [!DNL Workfront Fusion] .
1. Klik op **[!UICONTROL Enable]** om de geselecteerde API in te schakelen.
1. Herhaal stap 6-8 voor elke API die u wilt inschakelen.

   >[!NOTE]
   >
   >U moet de API van [!DNL Google Drive] en de API van alle [!DNL Google] -toepassingen die u wilt gebruiken (zoals de API van [!DNL Google Sheets] ) inschakelen.

1. Klik op het scherm dat wordt weergegeven op **[!UICONTROL Create credentials]** in de rechterbovenhoek.
1. Ga aan de sectie [ verder vormen OAuth toestemmingsmontages ](#configure-oauth-consent-settings) in dit artikel.

### [!UICONTROL OAuth consent] -instellingen configureren

1. Klik in het linkerdeelvenster op **[!UICONTROL OAuth consent screen]** .
1. Selecteer **[!UICONTROL External]** en klik op **[!UICONTROL Create]** .

   >[!NOTE]
   >
   >Er wordt geen bedrag in rekening gebracht wanneer u deze optie selecteert. Zie de informatie van [!DNL Google] over uitzonderingen op verificatievereisten voor meer informatie.

1. Vul de vereiste velden als volgt in:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Voer de naam in van de toepassing die om toestemming vraagt.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>Voer een e-mailadres in waarmee gebruikers contact met u kunnen opnemen als ze vragen hebben over hun toestemming wanneer ze verbinding maken met deze app.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email addresses]</td> 
      <td>Voer een of meer e-mailadressen in die Google kan gebruiken om u op de hoogte te stellen van wijzigingen in uw project.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik onder [!UICONTROL Authorized domains] op **[!UICONTROL Add domain]** en voer `workfrontfusion.com` in.

1. Klik op **[!UICONTROL Save and continue]**.
1. Klik op **[!UICONTROL Add or remove scopes]**.
1. Schakel in het rechterdeelvenster het volgende bereik in:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Service/API</th> 
      <th>Vereist bereik</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Mogelijk moet u de lijst uitvouwen of naar de volgende pagina in de lijst gaan om ze allemaal te kunnen zien.

1. Klik op **[!UICONTROL Update]**.
1. Klik op **[!UICONTROL Save and continue]**.
1. (Optioneel) Voeg testgebruikers toe aan het project.
1. Klik op **[!UICONTROL Save and continue]**.
1. Controleer de gegevens op nauwkeurigheid en klik op **[!UICONTROL Back to dashboard]** .

   >[!NOTE]
   >
   >U hoeft niet uw toestemmingsscherm en toepassing voor controle door [!DNL Google] voor te leggen.

1. Ga aan [ creëren OAuth Credentials ](#create-oauth-credentials) verder.

### OAuth-referenties maken

1. Klik in het linkerdeelvenster op **[!UICONTROL Credentials]** .

   >[!NOTE]
   >
   >Als dit niet de eerste API of dienst ([!DNL Gmail] of [!DNL Google Drive]) is u hebt toegelaten, moet u geen nieuwe geloofsbrieven creëren.

1. Klik op **[!UICONTROL Create credentials]** boven aan het scherm en selecteer vervolgens **[!UICONTROL OAuth client ID]** in het keuzemenu.

1. Vul de vereiste velden als volgt in:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Onder [!UICONTROL Authorized redirect URIs], klik **[!UICONTROL Add URI]** en ga **één** van het volgende in:

   * Voor [!DNL Gmail] of [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Voor andere [!DNL Google] -toepassingen: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klik op **[!UICONTROL Create]**.

   De weergave [!UICONTROL Client ID] en [!UICONTROL Client Secret] .

1. Kopieer de [!UICONTROL Client ID] en [!UICONTROL Client Secret] naar een beveiligde locatie. U gebruikt ze om verbinding te maken in [!DNL Workfront Fusion] .
1. Ga aan [  [!DNL Google]   [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion) met verbinden.

### Verbinden met [!DNL Google] in [!DNL Workfront Fusion]

Het maken van een verbinding met [!DNL Google] hangt af van het feit of u een module gebruikt vanuit een [!DNL Google] -service (zoals [!DNL Google Sheets] of [!DNL Google Docs] ) of van het feit of u verbinding maakt met [!DNL Google] via de aanvraagmodule [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0] .

* [Verbind met  [!DNL Google]  in de dienst van a  [!DNL Google] ](#connect-to-google-in-a-google-service)
* [Verbind met  [!DNL Google]  in de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Verbinding maken met [!DNL Google] in een [!DNL Google] -service

1. Zoek in [!DNL Workfront Fusion] de module [!DNL Google] waarvoor u een verbinding moet maken.
1. Klik op **[!UICONTROL Create a connection]** en vervolgens op **[!UICONTROL Show advanced settings]** .

1. Voer in de desbetreffende velden de waarden [!UICONTROL Client ID] en [!UICONTROL Client Secret] die u hebt opgehaald in [[!UICONTROL Create OAuth Credentials]](#create-oauth-credentials) in en klik vervolgens op **[!UICONTROL Continue]** .

1. Meld u aan met uw [!DNL Google] -account.

   Het venster **[!UICONTROL This app isn't verified]** wordt weergegeven. De app die in de venstertitel wordt vermeld, is de OAuth-client die u hierboven hebt gemaakt.

1. Klik op **[!UICONTROL Advanced]** en klik vervolgens op **[!UICONTROL Go to [!DNL Workfront Fusion] (unsafe)]** om toegang toe te staan met behulp van uw aangepaste OAuth-client.

1. Klik op **[!UICONTROL Allow]** om [!DNL Workfront Fusion] toestemming te verlenen.
1. Klik in het venster dat wordt weergegeven nogmaals op **[!UICONTROL Allow]** om uw keuzes te bevestigen.

   De verbinding met de gewenste [!DNL Google] -service met een aangepaste OAuth-client wordt tot stand gebracht.

#### Verbinding maken met [!DNL Google] in de module [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Voor instructies bij het verbinden met [!DNL Google] in [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module, zie [ Instructies voor het creëren van een verbinding aan  [!DNL Google]  in [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module ](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) in [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module ](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Mogelijk foutbericht: [!UICONTROL [403] Access Not Configured]

Als het foutbericht van [!UICONTROL `403 Access Not Configured`] wordt weergegeven, moet u de bijbehorende API inschakelen in uw Google Cloud Platform. Om API toe te laten, volg de stappen in de sectie [ een project op  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in dit artikel creëren.
