---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: De gebruikersgeloofsbrieven van Adobe Workfront vs. [!DNL SAML]  gebruikersgeloofsbrieven
description: Na het creëren van de gebruiker, kunt u de gebruiker uitgeven en "slechts toestaan SAML 2.0 Authentificatie"toelaten zodat hun gebruiker en wachtwoord door het systeem van SAML worden gecontroleerd. Als deze optie is ingeschakeld, mag de gebruiker zich alleen aanmelden via SAML. Wanneer zij naar  [!DNL Workfront]  URL gaan, worden zij automatisch opnieuw gericht aan het systeem van SAML en voor hun gebruikersnaam en wachtwoord van SAML ertoe aangezet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Workfront-gebruikersgegevens vs. SAML-gebruikersgegevens

Dit artikel richt zich specifiek op [!DNL Adobe Workfront] en SAML en behandelt geen andere methodes van de authentificatie SSO.

In een database slaat [!DNL Workfront] het e-mailadres van elke gebruiker op als de [!DNL Workfront] gebruikersnaam, samen met het [!DNL Workfront] -wachtwoord. Deze referenties worden herhaald in de sandboxen Voorbeeld en Aangepast vernieuwen.

Als [!DNL Workfront] tijdens het maken van gebruikers detecteert dat SAML 2.0 is geconfigureerd, wordt standaard &quot;Alleen SAML 2.0-verificatie toestaan&quot; voor de gebruiker gebruikt. Als het vak &#39;Een e-mailuitnodiging naar deze persoon verzenden&#39; is ingeschakeld, schakelt [!DNL Workfront] &#39;Alleen SAML 2.0-verificatie toestaan&#39; uit en wordt deze optie verborgen. Als &quot;Een uitnodigings-e-mail verzenden naar deze persoon&quot; is ingeschakeld, wordt de gebruiker een niet-SAML [!DNL Workfront] -gebruiker.

Nadat u de gebruiker hebt gemaakt, kunt u de gebruiker bewerken en **[!UICONTROL Only Allow SAML 2.0 Authentication]** inschakelen, zodat de gebruiker en het wachtwoord worden beheerd door het SAML-systeem.

Op deze manier kan de gebruiker zich alleen via SAML aanmelden. Wanneer ze naar de URL van [!DNL Workfront] gaan, worden ze automatisch doorgestuurd naar het SAML-systeem en gevraagd om hun SAML-gebruikersnaam en -wachtwoord.

De geloofsbrieven van SAML worden opgeslagen in een extern systeem van SAML, zoals Microsoft ADFS, niet in Workfront.
