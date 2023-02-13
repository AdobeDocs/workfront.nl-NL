---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Aanmeldingsfout: De volgende velden zijn ongeldig: emailAddr mag niet null zijn'''
description: Wanneer ik probeer in te loggen [!DNL Adobe Workfront] de URL voor mijn domein, wordt ik opnieuw gericht aan het login portal van SAML en dan opnieuw gericht terug naar [!DNL Workfront] met een fout die aangeeft dat het veld emailAddr niet null kan zijn.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---

# Aanmeldingsfout: De volgende velden zijn ongeldig: emailAddr mag niet null zijn

## Probleem

Wanneer ik probeer in te loggen [!DNL Adobe Workfront] met mijn URL (https://customerdomain.my.workfront.com), wordt ik opnieuw gericht aan het login portaal van SAML en dan opnieuw gericht terug naar [!DNL Workfront] met de volgende fout:

&quot;Laten we dat opnieuw proberen. De volgende velden zijn ongeldig: emailAddr mag niet null zijn.&quot;

## Oorzaak

Deze fout wordt veroorzaakt door een onjuist punt in het gebied van de Attributen van de Gebruiker van de Kaart van de configuratie SAML 2.0. Voor meer informatie over het in kaart brengen van gebruikersattributen voor SAML 2.0, zie [Adobe Workfront configureren met SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Oplossing

Werk de afbeelding van kenmerken voor het e-mailadres bij en klik op **[!UICONTROL Save]**.
