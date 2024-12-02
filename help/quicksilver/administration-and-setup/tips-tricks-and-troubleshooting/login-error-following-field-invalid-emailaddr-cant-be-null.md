---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Aanmeldingsfout: de volgende velden zijn ongeldig: emailAddr mag niet null zijn'
description: Wanneer ik probeer om in  [!DNL Adobe Workfront]  URL voor mijn domein te registreren, ben ik opnieuw gericht aan het login van SAML portaal en dan terug naar  [!DNL Workfront]  met een fout die zeggen dat het gebied emailAddr niet ongeldig kan zijn.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Aanmeldingsfout: de volgende velden zijn ongeldig: emailAddr mag niet null zijn

## Probleem

Wanneer ik probeer u aan te melden bij [!DNL Adobe Workfront] met mijn URL (https://customerdomain.my.workfront.com), word ik omgeleid naar het SAML-aanmeldingsportaal en vervolgens teruggeleid naar [!DNL Workfront] met de volgende fout:

&quot;Laten we dat opnieuw proberen. De volgende velden zijn ongeldig: emailAddr mag niet null zijn.&quot;

## Oorzaak

Deze fout wordt veroorzaakt door een onjuist punt in het gebied van de Attributen van de Gebruiker van de Kaart van de configuratie SAML 2.0. Voor meer informatie over de attributen van de kaartgebruiker voor SAML 2.0, zie [ Adobe Workfront met SAML 2.0 ](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md) vormen.

## Oplossing

Werk de kenmerktoewijzing voor het e-mailadres bij en klik op **[!UICONTROL Save]** .
