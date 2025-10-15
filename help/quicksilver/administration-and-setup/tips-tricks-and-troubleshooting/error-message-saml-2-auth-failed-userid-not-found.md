---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: SAML 2.0-verificatie mislukt: gebruikersnaam niet gevonden'
description: Als u SAML 2.0 gebruikt, betekent de fout "SAML 2.0 Authentication Failed-User Identifier Not Found" (Niet gevonden voor verificatie van SAML) dat een UID- of NAAM-id niet wordt doorgegeven uit de ADFS-aanvraagregels.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Foutbericht: SAML 2.0-verificatie mislukt: gebruikersnaam niet gevonden

## Probleem

Ik ontvang deze fout wanneer het gebruiken van SAML 2.0: &quot;De Ontbroken Authentificatie van SAML 2.0: Gebruiker - Herkenningsteken niet Gevonden.&quot;

## Oorzaak

Dit gebeurt wanneer a **UID** of **identiteitskaart van de NAAM** niet van de **regels van de Vordering ADFS** wordt overgegaan.

In ADFS moet het **Relying Vertrouwen van de Partij** a **de regel van de Vordering** hebben die of a **UID** of a **waarde van identiteitskaart van de NAAM** overgaat. Wanneer u een **[!DNL Workfront]Verbinding van de Test** in werking stelt, zou het dit moeten tonen als succesvol.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

1. Wanneer het uitgeven van **[!UICONTROL ADFS INFO]**, in **[!UICONTROL Relying Party Trusts]** > Uitgezochte voorwerp > **[!UICONTROL Edit Claim Rules]**.

1. De **[!UICONTROL LDAP Attribute]** (linkerkolom) moet **[!UICONTROL E-Mail Addresses]** (of een andere unieke id) hebben.

1. De **[!UICONTROL Outgoing Claim Type]** (rechterkolom) moet **[!UICONTROL Name ID]** zijn.

   >[!NOTE]
   >
   >Het hoeft niet over de e-mailadressen van LDAP-kenmerken te beschikken. Om het even welk uniek herkenningsteken dat de gebruiker zal identificeren kan worden gebruikt maar het moet in [!DNL Adobe Workfront] als **identiteitskaart van de NAAM** worden overgegaan.
