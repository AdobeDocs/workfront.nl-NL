---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domeinindeling voor Adobe Workfront API-aanroepen
description: Zoek uw domein voor gebruik in de Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 1f45298f6bff0b633ce2cd5f3bedd098904eba9d
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

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **Systeem** selecteert u vervolgens **Klantgegevens**.

   Uw domein wordt vermeld op het recht van het scherm.

   ![Domein](assets/domain.png)

