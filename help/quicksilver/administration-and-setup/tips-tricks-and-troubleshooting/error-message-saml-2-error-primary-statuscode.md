---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: SAML 2.0-fout: Primaire statuscode'''
description: U kunt geen verbinding maken met ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Foutbericht: SAML 2.0-fout: Primaire statuscode

## Probleem

U kunt geen verbinding maken met ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Als u een geslaagde testverbinding tot stand brengt en er zich nog steeds problemen voordoen, hebt u mogelijk onjuiste kenmerktoewijzingen of problemen met de federatie-id&#39;s. Neem contact op met de klantenondersteuning voor vragen.

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
   <td> <p>U moet een [!DNL Workfront] beheerder. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oorzaak 1: Beveiligd hash-algoritme is ingesteld op SHA-256

### Oplossing

1. Klik in Windows op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteren **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op het vertrouwen van de betrouwbare partij dat betrekking heeft op [!DNL Adobe Workfront]selecteert u vervolgens **[!UICONTROL Properties]**.
1. Klik op de knop **[!UICONTROL Advanced]** tab, dan selecteren **[!UICONTROL SHA-1]** van de **[!UICONTROL Secure hash algorithm]** vervolgkeuzemenu.\
   ![](assets/1-350x287.png)

## Oorzaak 2: ADFS-ondertekeningscertificaat verloopt bijna en is vervangen door een nieuw certificaat met overlappende datums

### Oplossing

De [!DNL Workfront] De pagina van de Opstelling SSO maakt een lijst van de certificaatvervaldatum. Als het certificaat bijna verlopen is, moet u het Nieuwe het Ondertekenen Certificaat van de Server van ADFS manueel trekken:

1. Klik in Windows op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteren **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klik met de rechtermuisknop op het vertrouwen van de betrouwbare partij dat betrekking heeft op [!DNL Workfront]en selecteert u **[!UICONTROL Properties]**.
1. Klik op de knop **[!UICONTROL Signature]** tab.
1. Klik op de naam van het ondertekenende certificaat en klik op **[!UICONTROL View]**.
1. Klik op Kopiëren naar **[!UICONTROL File]**... en selecteer **[!UICONTROL Next]**.

1. Selecteren **[!UICONTROL Base-64 encoded x.509 (CER)]** en klik op **[!UICONTROL Next]**.

1. Geef een bestandsnaam op en klik op **[!UICONTROL Next]**.
1. Klik op **[!UICONTROL Finish]**.
1. In [!DNL Workfront], navigeer naar **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** en uploadt u het ondertekenende certificaat handmatig.

## Oorzaak 3: Certificaatintrekkingscontrole mislukt

De oplossing hiervoor is afhankelijk van de versie van [!DNL Microsoft] ADFS die u gebruikt. Consult [!DNL Microsoft]Documentatie voor het verkrijgen van de juiste opdrachten voor uw versie.
