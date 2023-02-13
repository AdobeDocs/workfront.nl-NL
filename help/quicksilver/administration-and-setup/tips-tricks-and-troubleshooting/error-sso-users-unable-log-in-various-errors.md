---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fout: SSO-gebruikers kunnen zich niet aanmelden bij [!DNL Adobe Workfront] Door diverse fouten"'
description: Wanneer u een login fout over gefederaliseerde enige sign-on ontvangt, uw gebruikersbenaming/wachtwoordcombinatie, of uw toegang tot [!DNL Workfront], the problem might be that your [!DNL Workfront] -instantie gebruikt SSO en u probeert u aan te melden met een onjuiste URL. Zorg ervoor dat u zich aanmeldt met de juiste URL zonder dat dit gebeurt na ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Fout: SSO-gebruikers kunnen zich niet aanmelden bij [!DNL Adobe Workfront] Door diverse fouten

## Probleem

Ik kan me niet aanmelden bij [!DNL Workfront] en heeft een van de volgende fouten ontvangen:

* U hebt geen toegang [!DNL Workfront] via dit aanmeldingsscherm. [!DNL Workfront] is ingesteld voor Federated Single Sign-On met SAML 2.0. Neem contact op met uw [!DNL Workfront] beheerder.
* Die combinatie van gebruikersnaam en wachtwoord was niet helemaal juist. Zorg ervoor dat de vergrendeling van de caps niet is ingeschakeld en probeer het opnieuw.
* U hebt geen toegang tot [!DNL Workfront]. Neem contact op met uw [!DNL Workfront] beheerder om een gebruikersnaam en wachtwoord te krijgen.

## Oplossing

Uw [!DNL Workfront] -instantie gebruikt SSO en u probeert u aan te melden via een onjuiste URL. Zorg ervoor dat u zich aanmeldt met de juiste URL zonder dat er iets is gebeurd na &quot;.com&quot;

>[!TIP]
>
>Verwijder bestaande bladwijzers met ongeldige URL&#39;s.
