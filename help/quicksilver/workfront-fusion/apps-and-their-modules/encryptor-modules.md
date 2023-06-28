---
title: Versleuteling
description: Met Adobe Workfront Fusion Encryptor-modules kunt u alle tekstgegevens versleutelen. Ze ondersteunen momenteel berichtversleuteling via AES256 en PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Versleuteling

[!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor] kunt u alle tekstgegevens coderen. Ze ondersteunen momenteel berichtversleuteling via AES256 en PGP ([!UICONTROL OpenPGP]).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Berichtversleuteling en -ontsleuteling met PGP

Wanneer het coderen en het decrypteren via PGP, is het noodzakelijk om keychain te gebruiken en een privé of openbare sleutel (of allebei) tot stand te brengen.

Zie voor meer informatie over openbare en persoonlijke sleutels [Basistermen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Voor meer informatie over keyketins, zie [Toetsen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Encryptor] modules en hun velden

Wanneer u vormt [!UICONTROL Encryptor] -modules, worden de volgende velden weergegeven. Een bolde titel in een module wijst op een vereist gebied.

### Een PGP-bericht versleutelen

Met deze module kunt u een bericht versleutelen met openbare en persoonlijke sleutels.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Voer de persoonlijke sleutel van de afzender in. Hierdoor kan de identiteit van de afzender worden geverifieerd.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Voer de openbare sleutel van de ontvanger in.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Voer het bericht in dat u wilt versleutelen.</td>
    </tr>

### Een PGP-bericht decoderen

Deze module staat u toe om een bericht te decrypteren gebruikend openbare en privé sleutels.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Voer de persoonlijke sleutel van de ontvanger in.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Voer de openbare sleutel van de ontvanger in. Hierdoor kan de identiteit van de afzender worden geverifieerd.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Wijs het bericht toe dat u wilt decoderen.</td>
    </tr>
</table>
