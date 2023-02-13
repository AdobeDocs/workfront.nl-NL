---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront gebruikersgegevens vs. [!DNL SAML] gebruikersgegevens
description: Na het creëren van de gebruiker, kunt u de gebruiker uitgeven en "slechts toestaan SAML 2.0 Authentificatie"toelaten zodat hun gebruiker en wachtwoord door het systeem van SAML worden gecontroleerd. Als deze optie is ingeschakeld, mag de gebruiker zich alleen aanmelden via SAML. Als ze naar de [!DNL Workfront] URL, worden zij automatisch opnieuw gericht aan het systeem van SAML en veroorzaakt voor hun gebruikersnaam en wachtwoord van SAML.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Adobe Workfront-gebruikersgegevens versus SAML-gebruikersgegevens

Dit artikel richt zich specifiek op [!DNL Adobe Workfront] en SAML en heeft geen betrekking op andere SSO-verificatiemethoden.

In een database: [!DNL Workfront] slaat het e-mailadres van elke gebruiker op als hun [!DNL Workfront] gebruikersnaam, samen met hun [!DNL Workfront] wachtwoord. Deze referenties worden herhaald in de sandboxen Voorbeeld en Aangepast vernieuwen.

Tijdens het maken van de gebruiker, als [!DNL Workfront] ontdekt dat SAML 2.0 wordt gevormd, blijft het aan &quot;slechts toestaan SAML 2.0 Authentificatie&quot;voor de gebruiker in gebreke. Als het vak &quot;Een uitnodigingse-mail naar deze persoon verzenden&quot; is ingeschakeld, [!DNL Workfront] Hiermee schakelt u &#39;Alleen SAML 2.0-verificatie toestaan&#39; uit en verbergt u deze optie. Zodra &quot;verzend een uitnodigingsE-mail naar deze persoon&quot;wordt toegelaten, wordt de gebruiker een niet-SAML [!DNL Workfront] gebruiker.

Nadat u de gebruiker hebt gemaakt, kunt u de gebruiker bewerken en inschakelen **[!UICONTROL Only Allow SAML 2.0 Authentication]** zodat hun gebruiker en wachtwoord door het SAML systeem worden gecontroleerd.

Op deze manier kan de gebruiker zich alleen via SAML aanmelden. Als ze naar de [!DNL Workfront] URL, worden zij automatisch opnieuw gericht aan het systeem van SAML en veroorzaakt voor hun gebruikersnaam en wachtwoord van SAML.

De geloofsbrieven van SAML worden opgeslagen in een extern systeem van SAML, zoals Microsoft ADFS, niet in Workfront.
