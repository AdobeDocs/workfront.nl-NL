---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler-instellingen kunnen leiden tot verminderde prestaties
description: Na het creëren van de gebruiker, kunt u de gebruiker uitgeven en "slechts toestaan SAML 2.0 Authentificatie"toelaten zodat hun gebruiker en wachtwoord door het systeem van SAML worden gecontroleerd. Als deze optie is ingeschakeld, mag de gebruiker zich alleen aanmelden via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: ZScaler-instellingen kunnen leiden tot verminderde prestaties

>[!NOTE]
>
>Dit is een probleem met ZScaler en wordt niet door Workfront opgelost.

De webservice van ZScaler maakt standaard gebruik van `http/1.1` , wat kan leiden tot verminderde prestaties in Workfront.

Om dit probleem te controleren en op te lossen, configureert u de ZScaler-software voor gebruik van `http/2` . Dit kan niet worden geconfigureerd in Workfront.

U vindt informatie over `http/2` in de ZScaler-documentatie.
