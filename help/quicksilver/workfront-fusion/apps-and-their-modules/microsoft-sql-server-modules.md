---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server-modules
description: U kunt [!DNL Adobe Workfront Fusion] om verbinding te maken met Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] modules

U kunt [!DNL Adobe Workfront Fusion] om verbinding te maken met [!UICONTROL Microsoft SQL Server].

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
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
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

## Gebruiken [!DNL Microsoft SQL Server] modules

U kunt uw aangepaste logica rechtstreeks op uw databaseserver uitvoeren via opgeslagen procedures. [!DNL Adobe Workfront Fusion] laadt de interface van invoer-/uitvoerparameters en recordset dynamisch, zodat elke parameter of waarde afzonderlijk kan worden toegewezen. Voordat u uw scenario gaat configureren, moet u ervoor zorgen dat de account die u gebruikt om verbinding te maken met uw database, leestoegang heeft tot `INFORMATION_SCHEMA.ROUTINES` en `INFORMATION_SCHEMA.PARAMETERS` weergaven.

Wanneer [!DNL Fusion] stelt de verbinding met de [!DNL SQL server] doel, de [!DNL Fusion] de gebruiker identificeert de Gastheer (de domeinnaam of IP adres waar de server wordt ontvangen) en de haven. [!DNL Fusion] kan verbinding maken met elke beschikbare host en poort.

Voor informatie over specifieke IP adressen die door worden gebruikt [!DNL Workfront Fusion], zie [IP Adressen voor de toegang tot [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Voor meer informatie over het creëren van een opgeslagen procedure, zie [!DNL Microsoft SQL Server] documentatie.

>[!NOTE]
>
>[!DNL Workfront Fusion] biedt geen ondersteuning voor meerdere recordsets. Alleen de eerste wordt verwerkt.

## Probleemoplossing [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Lock wait timeout exceeded; try restarting transaction]

Deze fout treedt op wanneer u dezelfde gegevens wijzigt met behulp van meerdere modules. Dit wordt veroorzaakt door SQL-transacties.

Wanneer een SQL-module wordt uitgevoerd, wordt een transactie gestart. De transactie wordt gebeëindigd nadat het scenario volledig wordt uitgevoerd.

Als een andere module probeert om tot de zelfde gegevens toegang te hebben, moet het wachten tot de vorige transactie wordt gebeëindigd. Aangezien de eerste transactie zal worden gebeëindigd nadat het scenario wordt gebeëindigd, kan de tweede transactie nooit beginnen.

### Oplossing:

Schakel Automatisch vastleggen in. Automatisch vastleggen voltooit (legt) elke transactie direct nadat de module is uitgevoerd.

1. Klik op de knop [!UICONTROL Scenario settings] pictogram ![](assets/scenario-settings-icon.png)onder aan het scherm.
1. Klik op de knop **[!UICONTROL Auto commit]** selectievakje.
1. Klikken **[!UICONTROL OK]** om de scenario-instellingen op te slaan.
