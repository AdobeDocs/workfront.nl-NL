---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domeinindeling voor Adobe Workfront API-aanroepen
description: Zoek uw domein voor gebruik in de Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: 480f40d77cfc494ac28a2332c0e15bd1f0f00a6b
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Domeinindeling voor Adobe Workfront API-aanroepen

Wanneer u een API-aanroep naar de Workfront API maakt, gebruikt u het domein van uw organisatie in de aanroep.

De URL die u maakt voor de API-aanroep is afhankelijk van de URL die u gebruikt om verbinding te maken met Workfront.

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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Ga als volgt te werk om uw domein te zoeken:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem**, dan uitgezochte **Info van de Klant**.

   Uw domein wordt vermeld op het recht van het scherm.

   ![&#x200B; Domein &#x200B;](assets/domain.png)

