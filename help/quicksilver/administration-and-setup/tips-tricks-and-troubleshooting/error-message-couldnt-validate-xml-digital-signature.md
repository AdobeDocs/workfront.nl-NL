---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: kan de digitale XML-handtekening niet valideren'
description: U kunt geen verbinding maken met ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Foutbericht: kan de digitale XML-handtekening niet valideren

## Probleem

U kunt geen verbinding maken met ADFS.

![ error_message.png ](assets/error-message.png)

>[!NOTE]
>
>Als u een geslaagde testverbinding tot stand brengt en er zich nog steeds problemen voordoen, hebt u mogelijk onjuiste kenmerktoewijzingen of problemen met de federatie-id&#39;s. Neem contact op met de klantenondersteuning voor vragen.

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
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oorzaak 1: Het certificaat is onjuist

### Oplossing

Haal het ondertekeningscertificaat handmatig op van de ADFS-server:

1. Klik in [!DNL Windows] op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]** .\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteer **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op **[!UICONTROL Relying Party Trust]** en selecteer **[!UICONTROL Properties]** .

1. Klik op de tab **[!UICONTROL Signature]** .
1. Klik op de naam van het ondertekenende certificaat en klik op **[!UICONTROL View]** .
1. Klik op Kopiëren naar **[!UICONTROL File]** ... en selecteer **[!UICONTROL Next]** .

1. Selecteer **[!UICONTROL Base-64 encoded x.509 (CER)]** en klik op **[!UICONTROL Next]** .

1. Geef de bestandsnaam op en klik op **[!UICONTROL Next]** .
1. Klik op **[!UICONTROL Finish]**.
1. Navigeer in [!DNL Adobe Workfront] naar **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** en upload het handtekeningcertificaat handmatig.

## Oorzaak 2: Het certificaat wordt ondertekend met behulp van DSA wanneer [!DNL Workfront] een RSA-handtekening verwacht

### Oplossing

Maak het certificaat opnieuw en gebruik de handtekening van RSA in plaats van DSA.

## Oorzaak 3: XML-gegevens zijn onjuist

### Oplossing

Exporteer en importeer de XML-metagegevens opnieuw vanuit het ADFS-beheersysteem.

## Oorzaak 4: De aanvraag kon niet worden uitgevoerd vanwege een fout aan de SAML zijde

### Oplossing

Neem contact op met uw SAML-provider.
