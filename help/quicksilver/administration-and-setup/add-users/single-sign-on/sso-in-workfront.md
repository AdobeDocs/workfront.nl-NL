---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Overzicht van Single Sign-On in Adobe Workfront
description: Workfront biedt een centraal beheerde SSO-configuratie (Single Sign-On) die Workfront eenvoudig kan integreren met uw bestaande SSO-oplossing. Deze configuratie is eenvoudig in te stellen en te beheren en is beschikbaar voor zowel OnDemand- als OnPremise Enterprise-klanten.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Overzicht van Single Sign-On in Adobe Workfront

{{important-admin-console-onboard}}


Workfront biedt een centraal beheerde SSO-configuratie (Single Sign-On) die Workfront eenvoudig kan integreren met uw bestaande SSO-oplossing. Deze configuratie is eenvoudig in te stellen en te beheren en is beschikbaar voor zowel OnDemand- als OnPremise Enterprise-klanten.

Als u de SSO-functionaliteit in Workfront wilt gebruiken, moet uw organisatie een SSO-toepassing instellen. Vervolgens kunt u Workfront zo configureren dat deze kan communiceren met uw SSO-oplossing.

Met federatieve oplossingen kunnen gebruikers zich aanmelden bij al hun toepassingen door hun gebruikersnaam en wachtwoord in te voeren in een gecentraliseerd aanmeldingsportal.

![](assets/overview-sso-wf.png)


## Uw firewall configureren

Wanneer Workfront een SSO-oplossing gebruikt, wordt een verbinding met de server op de opgegeven poort tot stand gebracht.

Als u zich op verzoek abonneert op Workfront en als u uw firewall- of mailserver zodanig hebt geconfigureerd dat alleen bepaalde leveranciers toegang krijgen, moet u bepaalde Workfront IP-adressen toevoegen aan de lijst van gewenste personen van uw firewall. Zie voor meer informatie [De lijst van gewenste personen van uw firewall configureren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Single Sign-On configureren

Workfront integreert met de volgende SSO-oplossingen:

* Federale oplossingen die SAML 2.0 ondersteunen

   Voor informatie over het integreren van Workfront met SAML 2.0 raadpleegt u [Adobe Workfront configureren met SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Federale oplossingen die SAML 2.0 ondersteunen met ADFS

   Voor informatie over het integreren van Workfront met SAML 2.0 met behulp van ADFS raadpleegt u [Adobe Workfront configureren met SAML 2.0 met behulp van ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
