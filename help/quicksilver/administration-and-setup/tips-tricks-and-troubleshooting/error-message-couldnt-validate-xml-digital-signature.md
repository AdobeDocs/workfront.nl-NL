---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Foutbericht: Kan digitale XML-handtekening niet valideren"
description: U kunt geen verbinding maken met ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Foutbericht: Kan digitale XML-handtekening niet valideren

## Probleem

U kunt geen verbinding maken met ADFS.

![error_message.png](assets/error-message.png)

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

## Oorzaak 1: Het certificaat is onjuist

### Oplossing

Haal het ondertekeningscertificaat handmatig op van de ADFS-server:

1. In [!DNL Windows], klikt u op **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Het dialoogvenster ADFS 2.0-beheer wordt weergegeven.

1. Selecteren **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in het linkerdeelvenster.

1. Klikken met rechtermuisknop aan op **[!UICONTROL Relying Party Trust]** en selecteert u **[!UICONTROL Properties]**.

1. Klik op de knop **[!UICONTROL Signature]** tab.
1. Klik op de naam van het ondertekenende certificaat en klik op **[!UICONTROL View]**.
1. Klik op Kopiëren naar **[!UICONTROL File]**... en selecteer **[!UICONTROL Next]**.

1. Selecteren **[!UICONTROL Base-64 encoded x.509 (CER)]** en klik op **[!UICONTROL Next]**.

1. Geef een bestandsnaam op en klik op **[!UICONTROL Next]**.
1. Klik op **[!UICONTROL Finish]**.
1. In [!DNL Adobe Workfront], navigeer naar **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** en uploadt u het ondertekenende certificaat handmatig.

## Oorzaak 2: Het certificaat wordt ondertekend met behulp van DSA wanneer [!DNL Workfront] verwacht een RSA-handtekening

### Oplossing

Maak het certificaat opnieuw en gebruik de handtekening van RSA in plaats van DSA.

## Oorzaak 3: XML-gegevens zijn onjuist

### Oplossing

Exporteer en importeer de XML-metagegevens opnieuw vanuit het ADFS-beheersysteem.

## Oorzaak 4: Het verzoek kon niet worden uitgevoerd wegens een fout aan de kant van SAML

### Oplossing

Neem contact op met uw SAML-provider.
