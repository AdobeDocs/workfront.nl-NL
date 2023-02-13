---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Single Sign-On configureren voor [!DNL Workfront Proof] gebruikers
description: Als u het Uitgezochte of Premium plan hebt, kunt u Enige Sign-On (SSO) vermogen verstrekken dat u toestaat om de gebruikersbenaming en het wachtwoord van uw bestaande organisatie te gebruiken om tot uw toegang te hebben [!DNL Workfront Proof] account.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Single Sign-On configureren voor [!DNL Workfront Proof] gebruikers

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als u het Uitgezochte of Premium plan hebt, kunt u Enige Sign-On (SSO) vermogen verstrekken dat u toestaat om de gebruikersbenaming en het wachtwoord van uw bestaande organisatie te gebruiken om tot uw toegang te hebben [!DNL Workfront Proof] account.

Dit betekent dat u tegen uw eigen login systeem, niet tegen het voor authentiek zult verklaren [!DNL Workfront Proof] aanmeldingspagina.

>[!NOTE]
>
>U moet een aangepast subdomein of domein hebben ingesteld op uw [!DNL Workfront Proof] om SAML in te schakelen. U kunt aangepaste subdomeinen gratis instellen. Zie [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) voor meer informatie.U kunt meer lezen over volledig aangepaste domeinen op onze [Merk de [!DNL Workfront Proof] site - geavanceerd](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## SSO inschakelen binnen [!DNL Workfront Proof]

De functie Single Sign-On kan worden ingeschakeld op de [!UICONTROL Single sign-on] tabblad van uw [!UICONTROL Account settings]en wordt toegepast op alle gebruikers op uw [!DNL Workfront Proof] account. Zie [Accountinstellingen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) voor meer informatie .

## Entiteit-id

Als serviceprovider hebben we hier onze entiteit-id gepubliceerd:

[https://yoursubdomain.my.workfront.com/proof/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.my.workfront.com/proof/saml/module.php/saml/sp/metadata.php/phq) (waarbij &#39;uwsubdomein&#39; het subdomein van uw account is)

[!DNL Workfront Proof] vereist het e-mailadres van de gebruiker als unieke id, die kan worden doorgegeven als een van de volgende kenmerken:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* post
* email
* emailAddress

SSO configureren:

1. Open de **[!UICONTROL Single Sign-On]** tab (1).
1. Voer de **SSO-URL** (2)
Dit is de koppeling naar uw SSO-server (bijvoorbeeld **https://sso.mycompany.com/opensso**).

1. Voer de **Aanmeldings-URL** (3)
Dit is de URL die wordt aangeroepen om de gebruikers om te leiden naar uw identiteitsprovider.

1. Dit is geen daadwerkelijke URL u in browser ingaat, maar eerder een eindpunt dat de informatie zal verwerken wij het verzenden om het Login scherm voor te stellen.

Voer de **Afmeldings-URL** (4).
Dit is de URL waarnaar u terugkeert nadat u zich hebt afgemeld, bijvoorbeeld

**https://www.yourcompany.com/services/logout.asp**

1. Voer de **vingerafdruk certificaat** 5.
1. De SHA1-vingerafdruk van het SAML-certificaat dat door uw SAML Identity Provider is verstrekt.
1. Zorg ervoor dat u de toetsinfo opneemt door deze in te stellen op uw identiteitsprovider.
1. Overschakelen **SSO** tot **[!UICONTROL Enabled]** 6.
Zodra SSO wordt toegelaten, zullen u en andere gebruikers op uw rekening login gebruikend uw eigen authentificatiemechanisme. Dit betekent dat wanneer de gebruikers toegang krijgen tot uw [!DNL Workfront Proof] aanmeldingsscherm van de account (bijvoorbeeld **yourcompany.proofhq.com/login**), wordt het overdrachtvenster naar uw eigen aanmeldingspagina voor verificatie gestuurd.

1. (Optioneel) Inschakelen **Gebruikers automatisch voorzien van voorzieningen** (7)
Als deze optie is ingeschakeld, worden gebruikersaccounts automatisch gemaakt voor mensen die hun eigen account niet hebben [!DNL Workfront Proof] profielen, maar u krijgt toegang tot uw [!DNL Workfront Proof] account met hun Single Sign-On aanmeldingsgegevens. Deze actie wordt alleen uitgevoerd als de gebruikerslimiet voor uw account nog niet is bereikt.

1. Nieuwe provisioned gebruikers zullen de het profieltoestemmingen van de Manager door gebrek toegewezen hebben. Voor meer informatie, zie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## SSO inschakelen voor satellietaccounts

Wanneer u satellietrekeningen hebt die met uw hubrekening worden verbonden, kunt u hen van het niveau van de hubrekening beheren.

Single Sign-On is een Select- en Premium-functie, zodat Single Sign-On alleen kan worden ingeschakeld voor satellieten die zich op Select- en Premium-abonnementen bevinden.

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Account settings]** (1)

1. Klik op de satellietaccount in de keuzelijst (2).
1. Open de **[!UICONTROL Single Sign-On]** tab (3).
1. Begin het uitgeven van de configuratie SSO (4).
1. ![enable_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Hier zult u twee methodes (5) van configuratie hebben:

1. **Overgenomen:** SSO met de configuratie die van uw hubrekening wordt genomen.
Als een gebruiker toegang heeft tot [!DNL Workfront Proof] via de **standaardaanmeldingspagina** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) er **twee machtigingsniveaus**: Eerst wordt een gebruiker gevraagd zich aan te melden met [!DNL Workfront Proof] toegangsgegevens (e-mail en wachtwoord); dan wordt de gebruiker overgebracht door een venster SSO naar de SSO login pagina.
Daarom met toegelaten dienst SSO, adviseren wij om binnen door uw te registreren [!DNL Workfront Proof] subdomein/domein.

   >[!NOTE]
   >
   >Op dit moment, wanneer Single Sign-On is ingeschakeld op uw [!DNL Workfront Proof] -account, kunt u zich niet aanmelden bij de iPhone-app met deze gegevens.

   1. **Handmatig** (standaard): SSO met een verschillende configuratie (bijvoorbeeld, wijzend aan een andere Leverancier van de Identiteit).

      >[!NOTE]
      >
      >Als de satellietrekening de configuratie SSO van de hubrekening erft, zal het login scherm dat van de hubrekening zijn. Wanneer de gebruiker van de satellietrekening zijn SSO-aanmeldgegevens op deze pagina invoert, worden deze weer doorgestuurd naar de satellietrekening.

      ![Enabling_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Klikken **[!UICONTROL Save]** 6.

## SSO-instellingen die zijn overgenomen van een Hub-account

Wanneer u verkiest om de montages van uw hubrekening over te nemen zult u merken dat alle gebieden nu met de gegevens van uw hubrekening (7) worden bevolkt en dat Enige Sign-On automatisch wordt Toegelaten/Gehandicapten(8) zoals op uw hoofdrekening. Er zijn ook geen bewerkingskoppelingen meer in de velden, aangezien de gehele SSO-configuratie voor de Satellite Account nu is ingesteld en beheerd vanaf uw hubaccount.

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

In uw hubaccount (9) [!UICONTROL SSO Usage] uit het veld blijkt dat deze configuratie wordt gebruikt via satellietrekeningen ( 10 ) .\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## Handmatig geconfigureerde SSO

Als Handmatige SSO-configuratie is gekozen voor een satellietaccount (1), moet u de gegevens voor Single Sign-On handmatig invoeren.

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Account settings]** (1)

1. Open de **[!UICONTROL Single sign-on]** tab.
1. Klikken **[!UICONTROL Edit],** Vul het veld en klik op **[!UICONTROL Save]** (2)

1. Op de **[!UICONTROL SSO]** rij, klik **[!UICONTROL Enabled]** (3)

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## SSO-aanmelding

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Account settings]** (1)

1. Open de **[!UICONTROL Single sign-on]** tab.
1. Zorg ervoor dat uw [!DNL Workfront Proof] domein/subdomein (1) is ingesteld en dat uw gebruikers toegang hebben tot uw [!DNL Workfront Proof] via dit aangepaste domein/subdomein.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Als Single Sign-On is ingeschakeld, wordt in de URL voor aanmelding bij een subdomein (bijvoorbeeld yourcompany.proofhq.com/login) een transferscherm (2) weergegeven waarmee u rechtstreeks naar de SSO-aanmeldingspagina gaat.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Als een gebruiker toegang heeft tot [!DNL Workfront Proof] via de **standaardaanmeldingspagina** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) er **twee machtigingsniveaus**. Eerst wordt een gebruiker gevraagd zich aan te melden met [!DNL Workfront Proof] toegangsgegevens (e-mail en wachtwoord). Vervolgens wordt de gebruiker overgebracht via een SSO-venster (2) naar de SSO-aanmeldingspagina.\
   Daarom met toegelaten dienst SSO, adviseren wij om binnen door uw te registreren [!DNL Workfront Proof] subdomein/domein.

1. Op dit moment, wanneer Single Sign-On is ingeschakeld op uw Workfront Proof-account, kunt u zich niet met deze gegevens aanmelden bij de iPhone-app.

## Informatie over het toevoegen van een nieuwe gebruiker

Wanneer de Single Sign-On-functionaliteit is ingeschakeld op uw [!DNL Workfront Proof] nieuwe gebruikers ontvangen geen bevestigingse-mails omdat hun accounts automatisch worden geactiveerd en klaar zijn voor gebruik.

Van uw [!DNL Workfront Proof] aanmeldpagina, nadat u op de knop [!UICONTROL Login] gebruikers worden doorgestuurd naar uw aanmeldingspagina voor SSO en wordt gevraagd uw aanmeldingsgegevens voor Single Sign-On in te voeren.

>[!IMPORTANT]
>
>Gebruikers worden tijdens het verificatieproces geïdentificeerd aan de hand van een e-mailadres. Dit houdt in dat het e-mailaccount dat wordt gebruikt voor uw aanmelding bij een SSO, het e-mailadres moet zijn van de gebruiker die is geregistreerd in uw account.

## Active Directory Federation Services (AD FS)

De Actieve Diensten van de Federatie van de Folder (AD FS) is a [!DNL Microsoft] softwarecomponent die op de werkende systemen van de Server van Vensters kan worden geïnstalleerd om gebruikers van Enige Sign-On toegang tot systemen en toepassingen te verlenen die over organisatorische grenzen worden gevestigd. Voor meer informatie, zie de &quot;Actieve Diensten van de Federatie van de Folder&quot;op de website van het Netwerk van de Ontwikkelaar van Microsoft.

De [!DNL Workfront Proof] Het systeem steunt SAML 2.0 en is slechts compatibel met versie 2.0 van de ADVERTENTIE of groter.

Zie [Single Sign-On [!DNL Workfront Proof]: AD FS-configuratie](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) voor gedetailleerde instructies.
