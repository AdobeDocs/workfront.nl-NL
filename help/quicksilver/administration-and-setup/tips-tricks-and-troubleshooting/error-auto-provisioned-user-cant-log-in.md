---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Fout: gebruiker met automatische provisioning kan zich niet aanmelden"
description: Als een gebruiker met automatische provisioning zich voor het eerst aanmeldt en een fout ontvangt die aangeeft dat het systeem hun geen toegangsniveau toewijst, kan dit zijn omdat uw systeem geen toegangsniveaus heeft die zijn gekoppeld aan de Request-licentie. De auto-levering gebruikt het de vergunningstype van het Verzoek, zodat kunt u dit probleem oplossen door een toegangsniveau te creëren dat met een vergunning van het Verzoek wordt geassocieerd.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Fout: gebruiker met automatische provisioning kan zich niet aanmelden

Wanneer een gebruiker met automatische provisioning zich voor het eerst aanmeldt, wordt de volgende fout gegenereerd:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Probleem

Het systeem wijst de nieuwe gebruiker geen toegangsniveau toe.

Standaard wordt voor automatische provisioning het licentietype Verzoek gebruikt. Als er geen toegangsniveaus met een aanvraaglicentie bestaan, kan het systeem de gebruiker geen toegangsniveau toewijzen.

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

Creeer een basistoegangsniveau met een vergunning van het Verzoek:

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Access Levels]** .

1. Klik op **[!UICONTROL New Access Level]**.
1. Voer een **[!UICONTROL Name]** in.
1. Selecteer Verzoek in de vervolgkeuzelijst **[!UICONTROL License Type]** .
1. Klik op **[!UICONTROL Save Changes]**.

Nadat u een toegangsniveau met een vergunning van het Verzoek creeert, heb het gebruikerslogin met hun geloofsbrieven SSO.


