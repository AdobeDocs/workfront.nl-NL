---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fout: De gebruikers SSO zijn Onbekwaam aan login aan  [!DNL Adobe Workfront]  toe te schrijven aan Diverse Fouten'
description: Wanneer u een login fout over gefederaliseerde enige sign-on ontvangt, uw gebruikersbenaming/wachtwoordcombinatie, of uw toegang tot  [!DNL Workfront], the problem might be that your [!DNL Workfront]  instantiengebruikt SSO en u probeert om binnen het gebruiken van onjuiste URL te registreren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Fout: SSO-gebruikers kunnen zich niet aanmelden bij [!DNL Adobe Workfront] vanwege verschillende fouten

## Probleem

Ik kan me niet aanmelden bij [!DNL Workfront] en een van de volgende fouten hebben ontvangen:

* U kunt [!DNL Workfront] helaas niet openen via dit aanmeldingsscherm. [!DNL Workfront] is ingesteld voor Single Sign-On met SAML 2.0. Neem contact op met uw [!DNL Workfront] -beheerder.
* Die combinatie van gebruikersnaam en wachtwoord was niet helemaal juist. Zorg ervoor dat de vergrendeling van de caps niet is ingeschakeld en probeer het opnieuw.
* U hebt geen toegang tot [!DNL Workfront] . Neem contact op met uw [!DNL Workfront] -beheerder voor een gebruikersnaam en wachtwoord.

## Oplossing

Uw [!DNL Workfront] -instantie gebruikt SSO en u probeert u aan te melden via een onjuiste URL. Zorg ervoor dat u zich aanmeldt met de juiste URL zonder dat dit gebeurt na &quot;.com&quot;

>[!TIP]
>
>Verwijder bestaande bladwijzers met ongeldige URL&#39;s.
