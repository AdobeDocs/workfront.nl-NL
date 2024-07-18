---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Een gebruiker toevoegen aan een organisatie in Adobe Workfront Fusion
description: U kunt gebruikers toevoegen aan organisaties in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 447ab70566d5f9de3bc368933c9efdb94d2b9e7e
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Een gebruiker toevoegen aan een organisatie in Adobe Workfront Fusion

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet zijn aangemeld bij de [!DNL Adobe Admin Console] . Als uw organisatie is aangemeld bij de [!DNL Adobe Admin Console] , moet u deze handeling uitvoeren via de [!DNL Adobe Admin Console] .
>
>Voor instructies bij het toevoegen van een gebruiker in [!DNL  Adobe Admin Console], zie de sectie &quot;geef gebruikersdetails&quot;in artikel [ individueel gebruikers ](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) uit of contacteer uw [!UICONTROL Adobe Admin Console] Beheerder.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (het Bedrijfs Platform van de Fusie van Adobe Workfront/Adobe) ](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> 
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw organisatie zijn.</p>
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw team zijn.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Gebruikers aan een organisatie toevoegen


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

Als u gebruikers wilt toevoegen aan de organisatie, moet u een beheerder zijn bij de organisatie waaraan u gebruikers wilt toevoegen. Voor informatie over rollen, zie {de rollen van 0} Organisatie in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).[

Een gebruiker toevoegen aan de organisatie:

1. Ga naar **[!UICONTROL Organizations]** in het menu en selecteer de organisatie waaraan u een gebruiker wilt toevoegen.
1. Open de tab **[!UICONTROL Users]** in het dashboard.
1. Klik op **[!UICONTROL Invite a new user]**, vul het formulier in (E-mail, Bericht, Rol) en verzend de uitnodiging door op **[!UICONTROL Send]** te klikken.

>[!NOTE]
>
>   
>Als de knop [!UICONTROL Invite a new user] niet wordt weergegeven, is uw organisatie aangemeld bij de [!DNL Adobe Business Platform.]
>
>  Voor instructies bij het toevoegen van een gebruiker aan een organisatie die aan [!DNL Adobe Business Platform] is bezet, zie [ gebruikers aan  [!DNL Adobe Workfront Fusion]  door  [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md) toevoegen

De gebruiker ontvangt een e-mailuitnodiging waarin hij of zij de uitnodiging kan accepteren.
