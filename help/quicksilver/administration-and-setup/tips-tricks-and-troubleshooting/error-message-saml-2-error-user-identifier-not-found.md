---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Foutbericht: SAML 2.0-fout: gebruikersnaam niet gevonden"
description: U kunt geen verbinding maken met ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Foutbericht: SAML 2.0-fout: gebruikersnaam niet gevonden

## Probleem

U kunt geen verbinding maken met ADFS.

![ identifier_not_found.png ](assets/identifier-not-found.png)

>[!NOTE]
>
>Als u een geslaagde testverbinding tot stand brengt en er zich nog steeds problemen voordoen, hebt u mogelijk onjuiste kenmerktoewijzingen of problemen met de federatie-id&#39;s. Neem contact op met de klantenondersteuning voor vragen.

## Oorzaak:

Claims op de ADFS-server zijn onjuist.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een [!DNL Workfront] beheerder zijn. </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

Controleer of er op de ADFS-server een claim voor naam-id is:

1. Klik in Windows op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]** .\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteer **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op het vertrouwen van de betrouwbare partij dat betrekking heeft op Adobe Workfront en selecteer **[!UICONTROL Edit Claim Rules]** .
1. Controleer of de claim een **[!UICONTROL Outgoing Claim Type]** van **[!UICONTROL Name ID]** heeft.

![ 1.png ](assets/1-350x287.png)
