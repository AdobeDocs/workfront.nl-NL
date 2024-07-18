---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: SAML 2.0-fout: gebruikersnaam niet gevonden'
description: U kunt geen verbinding maken met ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '201'
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

Claims op de ADFS-server zijn onjuist

## Toegangsvereisten

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn. Voor meer informatie, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

Controleer of er op de ADFS-server een claim voor naam-id is:

1. Klik in Windows op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]** .\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteer **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op het vertrouwen van de betrouwbare partij dat betrekking heeft op Adobe Workfront en selecteer **[!UICONTROL Edit Claim Rules]** .
1. Controleer of de claim een **[!UICONTROL Outgoing Claim Type]** van **[!UICONTROL Name ID]** heeft.

![ 1.png ](assets/1-350x287.png)
