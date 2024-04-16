---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken
description: U kunt [!DNL Adobe Workfront Fusion] verbinding maken met [!DNL Google Services] een aangepaste OAuth-client gebruiken. Deze procedure vereist een bestaande [!DNL Google] account.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 7d2b4a9940cb21de1b8b5f2955f53b3d88040e44
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken

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

## Vereisten

U hebt een bestaande [!DNL Google] om deze verbinding te maken.

## Connect Fusion to Google-services met een aangepaste OAuth-client

Als u deze verbinding wilt maken, moet u een project maken en configureren op het Google Cloud-platform en vervolgens de verbinding configureren in Fusion op basis van dat project.

* [Een project maken op [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Configureren [!UICONTROL OAuth consent] instellingen](#configure-oauth-consent-settings)
* [OAuth-referenties maken](#create-oauth-credentials)
* [Verbinden met [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Deze procedure is bedoeld voor:
>
>* Persoonlijk gebruik ([!DNL `@gmail.com`] en [!DNL `@googlemail.com`] gebruikers)
>* Intern gebruik ([!DNL G Suite] gebruikers die liever een aangepaste OAuth-client gebruiken)

### Een project maken op [!DNL Google Cloud Platform]

Een project maken op [!DNL Google Cloud] Platform:

1. Aanmelden bij [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) met uw [!DNL Google] referenties.
1. Klik in het linkerdeelvenster op **[!UICONTROL Dashboard]**.
1. Klikken **[!UICONTROL Create project]** rechtsboven in het scherm.
1. Voer de **[!UICONTROL Project name]** en klik vervolgens op **[!UICONTROL Create]**.

1. Klik op de knop **[!UICONTROL Enable APIs and services]** aan de bovenkant van het scherm.
1. In de **[!UICONTROL Search for APIs and Services]** veld boven aan het scherm typt u de naam van de service die u wilt gebruiken (bijvoorbeeld [!DNL Gmail] API of [!DNL Google Drive] API).
1. Klik op de API of service waarmee u verbinding wilt maken wanneer deze wordt weergegeven [!DNL Workfront Fusion].
1. Klikken **[!UICONTROL Enable]** om de geselecteerde API in te schakelen.
1. Herhaal stap 6-8 voor elke API die u wilt inschakelen.

   >[!NOTE]
   >
   >U moet inschakelen [!DNL Google Drive] API en de API van alle [!DNL Google] apps die u wilt gebruiken (zoals [!DNL Google Sheets] API).

1. Klik op het scherm dat wordt weergegeven op **[!UICONTROL Create credentials]** in de rechterbovenhoek.
1. Doorgaan naar de sectie [Instellingen voor OAuth-toestemming configureren](#configure-oauth-consent-settings) in dit artikel.

### Configureren [!UICONTROL OAuth consent] instellingen

1. Klik in het linkerdeelvenster op **[!UICONTROL OAuth consent screen]**.
1. Selecteren **[!UICONTROL External]** en klik vervolgens op **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >Er wordt geen bedrag in rekening gebracht wanneer u deze optie selecteert. Zie voor meer informatie [!DNL Google]Informatie over uitzonderingen op verificatievereisten.

1. Vul de vereiste velden als volgt in:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Voer de naam in van de toepassing die om toestemming vraagt.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
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

1. Onder [!UICONTROL Authorized domains], klikt u op **[!UICONTROL Add domain]** en voert u `workfrontfusion.com`.

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
1. Controleer uw gegevens op nauwkeurigheid en klik vervolgens op **[!UICONTROL Back to dashboard]**.

   >[!NOTE]
   >
   >U hoeft het toestemmingsscherm en de aanvraag voor verificatie niet in te dienen door [!DNL Google].

1. Doorgaan naar [OAuth-referenties maken](#create-oauth-credentials).

### OAuth-referenties maken

1. Klik in het linkerdeelvenster op **[!UICONTROL Credentials]**.

   >[!NOTE]
   >
   >Als dit niet de eerste API of service is ([!DNL Gmail] of [!DNL Google Drive]) die u hebt ingeschakeld, hoeft u geen nieuwe referenties te maken.

1. Klikken **[!UICONTROL Create credentials]** aan de bovenkant van het scherm, dan selecteer **[!UICONTROL OAuth client ID]** in het keuzemenu.

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

1. Onder [!UICONTROL Authorized redirect URIs], klikt u op **[!UICONTROL Add URI]** en betreden **één** van het volgende:

   * Voor [!DNL Gmail] of [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Voor andere [!DNL Google] apps: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klik op **[!UICONTROL Create]**.

   De [!UICONTROL Client ID] en [!UICONTROL Client Secret] weergeven.

1. De [!UICONTROL Client ID] en [!UICONTROL Client Secret] naar een beveiligde locatie. U gebruikt deze voor het maken van een verbinding in [!DNL Workfront Fusion].
1. Doorgaan naar [Verbinden met [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Verbinden met [!DNL Google] in [!DNL Workfront Fusion]

Het maken van een verbinding met [!DNL Google] verschilt afhankelijk van of u een module gebruikt van een [!DNL Google] diensten (zoals [!DNL Google Sheets] of [!DNL Google Docs]), of als u verbinding maakt met [!DNL Google] via de [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0] aanvraagmodule.

* [Verbinden met [!DNL Google] in een [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Verbinden met [!DNL Google] in de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Verbinden met [!DNL Google] in een [!DNL Google] service

1. In [!DNL Workfront Fusion], zoekt u de [!DNL Google] die u een verbinding voor moet maken.
1. Klikken **[!UICONTROL Create a connection]** en klik vervolgens op **[!UICONTROL Show advanced settings]**.

1. Voer de [!UICONTROL Client ID] en [!UICONTROL Client Secret] u hebt opgehaald in [[!UICONTROL Create OAuth Credentials]](#create-oauth-credentials) in de respectieve gebieden, dan klik **[!UICONTROL Continue]**.

1. Meld u aan met uw [!DNL Google] account.

   De **[!UICONTROL This app isn't verified]** wordt weergegeven. De app die in de venstertitel wordt vermeld, is de OAuth-client die u hierboven hebt gemaakt.

1. Klikken **[!UICONTROL Advanced]** en klik vervolgens op **[!UICONTROL Go to [!DNL Workfront Fusion] (unsafe)]** om toegang toe te staan gebruikend uw douaneOAuth cliënt.

1. Klikken **[!UICONTROL Allow]** verlenen [!DNL Workfront Fusion] toestemming.
1. Klik in het venster dat wordt weergegeven op **[!UICONTROL Allow]** nogmaals ter bevestiging van uw keuze.

   De verbinding met het gewenste [!DNL Google] de dienst die een douaneOAuth cliënt gebruikt wordt gevestigd.

#### Verbinden met [!DNL Google] in de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Voor instructies voor het verbinden met [!DNL Google] in de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module, zie [Instructies voor het maken van een verbinding met [!DNL Google] in de [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) in [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Mogelijk foutbericht:[!UICONTROL [403] Access Not Configured]

Als de [!UICONTROL `403 Access Not Configured`] weergegeven foutberichten: u moet de bijbehorende API inschakelen in uw Google Cloud Platform. Volg de stappen in de sectie om de API in te schakelen [Een project maken op [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in dit artikel.
