---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: SAML 2.0-verificatie mislukt: gebruikersnaam niet gevonden'
description: Als u SAML 2.0 gebruikt, betekent de fout "SAML 2.0-verificatie Niet gevonden-gebruikersnaam niet" dat een UID- of NAAM-id niet wordt doorgegeven uit de ADFS-aanvraagregels. In ADFS moet het Relying Party Trust een Claim-regel hebben die een UID- of een NAAM-id-waarde doorgeeft. Wanneer u de Verbinding van de Test van de a [!DNL Workfront]  in werking stelt, zou het dit moeten tonen als succesvol.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Foutbericht: SAML 2.0-verificatie mislukt: gebruikersnaam niet gevonden

## Probleem

Ik ontvang deze fout wanneer het gebruiken van SAML 2.0: &quot;De Ontbroken Authentificatie van SAML 2.0: Gebruiker - Herkenningsteken niet Gevonden.&quot;

## Oorzaak

Dit gebeurt wanneer a **UID** of **identiteitskaart van de NAAM** niet van de **regels van de Vordering ADFS** wordt overgegaan.

In ADFS moet het **Relying Vertrouwen van de Partij** a **de regel van de Vordering** hebben die of a **UID** of a **waarde van identiteitskaart van de NAAM** overgaat. Wanneer u een **[!DNL Workfront]Verbinding van de Test** in werking stelt, zou het dit moeten tonen als succesvol.

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

1. Wanneer het uitgeven van **[!UICONTROL ADFS INFO]**, in **[!UICONTROL Relying Party Trusts]** > Uitgezochte voorwerp > **[!UICONTROL Edit Claim Rules]**.

1. De **[!UICONTROL LDAP Attribute]** (linkerkolom) moet **[!UICONTROL E-Mail Addresses]** (of een andere unieke id) hebben.

1. De **[!UICONTROL Outgoing Claim Type]** (rechterkolom) moet **[!UICONTROL Name ID]** zijn.

   >[!NOTE]
   >
   >Het hoeft niet over de e-mailadressen van LDAP-kenmerken te beschikken. Om het even welk uniek herkenningsteken dat de gebruiker zal identificeren kan worden gebruikt maar het moet in [!DNL Adobe Workfront] als **identiteitskaart van de NAAM** worden overgegaan.
