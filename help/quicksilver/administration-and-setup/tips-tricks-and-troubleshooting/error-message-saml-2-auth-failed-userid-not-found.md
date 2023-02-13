---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: SAML 2.0-verificatie mislukt: Gebruiker-id niet gevonden"'
description: Als u SAML 2.0 gebruikt, betekent de fout "SAML 2.0-verificatie Niet gevonden-gebruikersnaam niet" dat een UID- of NAAM-id niet wordt doorgegeven uit de ADFS-aanvraagregels. In ADFS moet het Relying Party Trust een Claim-regel hebben die een UID- of een NAAM-id-waarde doorgeeft. Wanneer u een [!DNL Workfront] Test Connection, it should show this if success.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Foutbericht: SAML 2.0-verificatie mislukt: Gebruiker-id niet gevonden

## Probleem

Ik ontvang deze fout wanneer het gebruiken van SAML 2.0: &quot;SAML 2.0-verificatie mislukt: Gebruiker-id niet gevonden.&quot;

## Oorzaak

Dit gebeurt wanneer een **UID** of **NAAM-ID** wordt niet doorgegeven uit de **ADFS-aanvraagregels**.

In ADFS worden de **Betrouwbaarheid partij** moet een **Claimregel** die een **UID** of **NAAM-ID** waarde. Wanneer u een **[!DNL Workfront]Verbinding testen**, moet zij dit laten zien als het succesvol is.

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

## Oplossing

1. Bij het bewerken van de **[!UICONTROL ADFS INFO]** in de **[!UICONTROL Relying Party Trusts]** > Object selecteren >**[!UICONTROL Edit Claim Rules]**.

1. De **[!UICONTROL LDAP Attribute]** (linkerkolom) moet **[!UICONTROL E-Mail Addresses]** (of een unieke id).

1. De **[!UICONTROL Outgoing Claim Type]** (rechterkolom) moet **[!UICONTROL Name ID]**.

   >[!NOTE]
   >
   >Het hoeft niet over de e-mailadressen van LDAP-kenmerken te beschikken. Om het even welke unieke herkenningsteken die de gebruiker zal identificeren kan worden gebruikt maar het moet worden overgegaan in [!DNL Adobe Workfront] als de **NAAM-ID**.
