---
title: Versleuteling
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Versleuteling

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Encryptor ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/encryptor-modules.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

[!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor] -modules kunt u alle tekstgegevens versleutelen. Zij steunen momenteel berichtencryptie via AES256 en PGP ([!UICONTROL OpenPGP]).

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
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het abonnement [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Berichtversleuteling en -ontsleuteling met PGP

Wanneer het coderen en het decrypteren via PGP, is het noodzakelijk om keychain te gebruiken en een privé of openbare sleutel (of allebei) tot stand te brengen.

Voor meer informatie over openbare en privé sleutels, zie [ Basistermijnen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Voor meer informatie over keyketins, zie [ Sleutels in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Encryptor] modules en hun velden

Wanneer u [!UICONTROL Encryptor] modules configureert, worden de volgende velden weergegeven. Een bolde titel in een module wijst op een vereist gebied.

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
