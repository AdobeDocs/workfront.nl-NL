---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fout: gebruiker met automatische provisioning kan zich niet aanmelden'
description: Als een gebruiker met automatische provisioning zich voor het eerst aanmeldt en een fout ontvangt die aangeeft dat het systeem hun geen toegangsniveau toewijst, kan dit zijn omdat uw systeem geen toegangsniveaus heeft die zijn gekoppeld aan de Request-licentie.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Fout: gebruiker met automatische provisioning kan zich niet aanmelden

Wanneer een gebruiker met automatische provisioning zich voor het eerst aanmeldt, wordt de volgende fout gegenereerd:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Probleem

Het systeem wijst de nieuwe gebruiker geen toegangsniveau toe.

Standaard wordt voor automatische provisioning het licentietype Verzoek gebruikt. Als er geen toegangsniveaus met een aanvraaglicentie bestaan, kan het systeem de gebruiker geen toegangsniveau toewijzen.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

Creeer een basistoegangsniveau met een vergunning van het Verzoek:

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Access Levels]** .

1. Klik op **[!UICONTROL New Access Level]**.
1. Voer een **[!UICONTROL Name]** in.
1. Selecteer Verzoek in de vervolgkeuzelijst **[!UICONTROL License Type]** .
1. Klik op **[!UICONTROL Save Changes]**.

Nadat u een toegangsniveau met een vergunning van het Verzoek creeert, heb het gebruikerslogin met hun geloofsbrieven SSO.


