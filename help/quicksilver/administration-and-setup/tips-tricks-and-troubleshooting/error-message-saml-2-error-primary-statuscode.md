---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: SAML 2.0-fout: Primaire statuscode'
description: U kunt geen verbinding maken met ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Foutbericht: SAML 2.0-fout: Primaire statuscode

## Probleem

U kunt geen verbinding maken met ADFS.

![&#x200B; SAML_2.0_Error_Primary_Status_Code.png &#x200B;](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Als u een geslaagde testverbinding tot stand brengt en er zich nog steeds problemen voordoen, hebt u mogelijk onjuiste kenmerktoewijzingen of problemen met de federatie-id&#39;s. Neem contact op met de klantenondersteuning voor vragen.

## Toegangsvereisten

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

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oorzaak 1: Veilig hash-algoritme is ingesteld op SHA-256

### Oplossing

1. Klik in Windows op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]** .\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteer **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op het vertrouwen van de betrouwbare partij dat betrekking heeft op [!DNL Adobe Workfront] en selecteer vervolgens **[!UICONTROL Properties]** .
1. Klik op de tab **[!UICONTROL Advanced]** en selecteer vervolgens **[!UICONTROL SHA-1]** in de vervolgkeuzelijst **[!UICONTROL Secure hash algorithm]** .
   ![&#x200B; SHA-1 &#x200B;](assets/1-350x287.png)

## Oorzaak 2: ADFS-ondertekeningscertificaat verloopt binnenkort en is vervangen door een nieuw certificaat met overlappende datums

### Oplossing

De [!DNL Workfront] pagina van de Opstelling van SSO maakt een lijst van de certificaatvervaldatum. Als het certificaat bijna verlopen is, moet u het Nieuwe het Ondertekenen Certificaat van de Server van ADFS manueel trekken:

1. Klik in Windows op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]** .\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteer **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op het vertrouwen van de betrouwbare partij dat betrekking heeft op [!DNL Workfront] en selecteer **[!UICONTROL Properties]** .
1. Klik op de tab **[!UICONTROL Signature]** .
1. Klik op de naam van het ondertekenende certificaat en klik op **[!UICONTROL View]** .
1. Klik op Kopiëren naar **[!UICONTROL File]** ... en selecteer **[!UICONTROL Next]** .

1. Selecteer **[!UICONTROL Base-64 encoded x.509 (CER)]** en klik op **[!UICONTROL Next]** .

1. Geef de bestandsnaam op en klik op **[!UICONTROL Next]** .
1. Klik op **[!UICONTROL Finish]**.
1. Navigeer in [!DNL Workfront] naar **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** en upload het handtekeningcertificaat handmatig.

## Oorzaak 3: controle op intrekking certificaat mislukt

De oplossing hiervoor is afhankelijk van de versie van [!DNL Microsoft] ADFS die u gebruikt. Raadpleeg de documentatie van [!DNL Microsoft] voor de juiste opdrachten voor uw versie.
