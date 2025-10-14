---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domeinindeling voor Adobe Workfront API-aanroepen
description: Zoek uw domein voor gebruik in de Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Domeinindeling voor Adobe Workfront API-aanroepen

Wanneer u een API-aanroep naar de Workfront API maakt, gebruikt u het domein van uw organisatie in de aanroep. Het formaat voor dit domein URL verschilt gebaseerd op of uw organisatie aan de Adobe Verenigde Shell is genegeerd.

Om te weten of uw organisatie op de Adobe Verenigde Shell is, onderzoek URL die toont wanneer u een pagina van Workfront bekijkt.

| Workfront URL begint met: | URL voor API-aanroepen: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Ga als volgt te werk om uw domein te zoeken:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem**, dan uitgezochte **Info van de Klant**.

   Uw domein wordt vermeld op het recht van het scherm.

   ![&#x200B; Domein &#x200B;](assets/domain.png)

