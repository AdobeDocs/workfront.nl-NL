---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domeinindeling voor Adobe Workfront API-aanroepen
description: Zoek uw domein voor gebruik in de Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: b9547764abd4f1f61d93da6bc66d9e6776954f4d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Domeinindeling voor Adobe Workfront API-aanroepen

Wanneer u een API-aanroep naar de Workfront API maakt, gebruikt u het domein van uw organisatie in de aanroep. Het formaat voor dit domein URL verschilt gebaseerd op of uw organisatie aan Adobe Verenigde Shell is genegeerd.

Om te weten of uw organisatie op Adobe Verenigde Shell is, onderzoek URL die toont wanneer u een pagina van Workfront bekijkt.

| Workfront URL begint met: | URL voor API-aanroepen: |
|---|---|
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Ga als volgt te werk om uw domein te zoeken:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![ pictogram van de Opstelling ](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem**, dan uitgezochte **Info van de Klant**.

   Uw domein wordt vermeld op het recht van het scherm.

   ![ Domein ](assets/domain.png)

