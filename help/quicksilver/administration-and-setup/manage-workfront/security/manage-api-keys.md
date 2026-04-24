---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API-toetsen beheren
description: Adobe Workfront-beheerders kunnen de API-sleutels beheren die worden gebruikt om toepassingen in staat te stellen om namens een gebruiker toegang te krijgen tot Workfront, om zo kwetsbaarheden op het gebied van API-beveiliging tot een minimum te beperken.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# API-sleutels beheren

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront raadt niet langer het gebruik van de `/login` eindpunt- of API-toetsen aan. Gebruik in plaats daarvan een van de volgende verificatiemethoden:
>
>* Serververificatie met JWT
>* Gebruikersverificatie met OAuth2
>
>Voor instructies bij vestiging deze authentificatiemethodes, zie [&#x200B; tot toepassingen OAuth2 voor de integratie van Workfront leiden &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Voor instructies bij het gebruiken van serverauthentificatie in Workfront, zie [&#x200B; vormen en gebruiken de douaneOAuth 2 van uw organisatie toepassingen gebruikend stroom JWT &#x200B;](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)
>
>Voor instructies bij het gebruiken van gebruikersauthentificatie in Workfront, zie [&#x200B; vormen en gebruiken de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van de vergunningscode &#x200B;](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)

Adobe Workfront-beheerders kunnen de API-sleutels beheren die worden gebruikt om toepassingen in staat te stellen om namens een gebruiker toegang te krijgen tot Workfront, om zo kwetsbaarheden op het gebied van API-beveiliging tot een minimum te beperken.

U kunt de huidige API-sleutel voor beheerders opnieuw instellen of verwijderen, API-sleutels configureren voor verlopen en de API-sleutels voor alle gebruikers verwijderen.

Voorbeelden van toepassingen die gebruikmaken van de Workfront API zijn:

* Documentintegratie zoals Dropbox, Google Drive en Workfront DAM
* Workfront mobiele toepassingen

>[!IMPORTANT]
>
>Wanneer u een API-sleutel opnieuw instelt of verwijdert, moet elke toepassing die gebruikmaakt van de Workfront API en die via deze API-sleutel voor verificatie bij Workfront zorgt, opnieuw worden geconfigureerd om toegang tot Workfront te herstellen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standaard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Workfront API-toetsen

Elke gebruiker in Workfront heeft een unieke API-sleutel. Deze sleutel wordt per gebruiker gegenereerd op het moment dat de gebruiker toegang krijgt tot een integratie die gebruikmaakt van de Workfront API (zoals de mobiele Workfront-app of documentintegratie).

>[!NOTE]
>
> API-sleutels die u genereert in de productieomgeving, worden tijdens de wekelijkse vernieuwing gekopieerd naar de voorbeeldomgeving. Alle API-sleutels die u genereert in de voorvertoningsomgeving, worden tijdens de wekelijkse vernieuwing overschreven met uw productie-API-sleutels.

Workfront-beheerders hebben ook een unieke API-sleutel. Wanneer een toepassing een beheerder-API-sleutel gebruikt om toegang te krijgen tot Workfront, heeft de toepassing beheerderstoegang tot Workfront.

## De API-sleutel voor beheerders beheren

U kunt de API-sleutel voor uw beheerdersgebruikersaccount genereren, opnieuw instellen of verwijderen.

{{step-1-to-setup}}

1. Klik **Systeem >** **Info van de Klant.**
1. (Voorwaardelijk) Voer een van de volgende handelingen uit:

   Om een API Sleutel te produceren: In de **API Zeer belangrijke sectie van Montages**, klik **produceert API Sleutel**.

   of\
   Om een API Sleutel terug te stellen: In de **API Zeer belangrijke sectie van Montages**, klik **Terugstellen**, dan **Teruggesteld.**

   of

   Om de API Sleutel te verwijderen: In de **API Zeer belangrijke sectie van Montages**, **verwijdert**, dan **verwijdert**.

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## Configureren wanneer API-sleutels verlopen

U kunt API Toetsen vormen om voor alle gebruikers in uw systeem te verlopen. Wanneer de API-sleutel van een gebruiker vervalt, moet de gebruiker opnieuw worden geverifieerd voor toepassingen die de Workfront API gebruiken om toegang te krijgen tot Workfront. U kunt de frequentie wijzigen waarmee de API-toetsen verlopen. U kunt ook configureren of API-sleutels verlopen wanneer het wachtwoord van een gebruiker verloopt.

{{step-1-to-setup}}

1. Klik **Systeem** > **Info van de Klant**.
1. In het **Belangrijkste gebied van Montages API**, in **na verwezenlijking**, **API sleutels verlopen in** drop-down lijst, selecteer timeframe wanneer u de API sleutels wilt verlopen.

   Wanneer u deze optie wijzigt, begint de nieuwe tijdlijn vanaf het moment dat u de wijziging aanbracht. Bijvoorbeeld, als u deze optie van *1 maand* in *6 maanden* verandert, verlopen de API Sleutels 6 maanden vanaf de tijd u de verandering aanbrengt.

   API-sleutels verlopen standaard elke maand.

1. Om API Sleutels te vormen om in de tijd te verlopen de wachtwoorden van de gebruikers verlopen, laat **toe verwijder API sleutel wanneer het wachtwoord van een gebruiker** verloopt.

   Deze optie is standaard niet ingeschakeld.

   Voor informatie over hoe te om gebruikerswachtwoorden te vormen om te verlopen, zie [&#x200B; de voorkeur van de systeemveiligheid &#x200B;](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) vormen.

1. Klik **sparen**.

## De API-sleutels voor alle gebruikers verwijderen

Als u zich zorgen maakt over een bepaalde inbreuk op de beveiliging van uw Workfront-systeem, kunt u de API-sleutels voor alle gebruikers tegelijk verwijderen.

>[!IMPORTANT]
>
>Als u API-sleutels verwijdert voor alle gebruikers, worden ALLE API-sleutels voor alle gebruikers in het systeem ongeldig. Hierdoor zullen al uw integraties in Workfront mislukken totdat u een nieuwe API-sleutel genereert in Workfront en al uw integraties bijwerkt.

{{step-1-to-setup}}

1. Breid **Systeem** uit, dan klik **Info van de Klant**.

1. In het **Belangrijkste gebied van Montages API**, verwijdert de klik **alle API sleutels**, dan klikt **verwijdert** **allen**.

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Administration differences between Adobe Workfront and Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
