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
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet zijn aangemeld bij de [!DNL Adobe Admin Console]. Als uw organisatie is aangemeld bij de [!DNL Adobe Admin Console], moet u deze handeling uitvoeren via de [!DNL Adobe Admin Console].
>
>Voor instructies over het toevoegen van een gebruiker in de[!DNL  Adobe Admin Console], zie de sectie &quot;Gebruikersdetails bewerken&quot; in het artikel [Gebruikers individueel beheren](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) of neem contact op met uw [!UICONTROL Adobe Admin Console] Beheerder.
>
>Ga voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console naar [Platformgebaseerde verschillen in beheer (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> 
     <p>U moet een [!DNL Workfront Fusion] beheerder van uw organisatie.</p>
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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

Als u gebruikers wilt toevoegen aan de organisatie, moet u een beheerder zijn bij de organisatie waaraan u gebruikers wilt toevoegen. Voor informatie over rollen, zie [Organisatiefuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Een gebruiker toevoegen aan de organisatie:

1. Navigeren naar **[!UICONTROL Organizations]** in het menu en selecteer de organisatie waaraan u een gebruiker wilt toevoegen.
1. Open de **[!UICONTROL Users]** in het dashboard.
1. Klikken **[!UICONTROL Invite a new user]**, vult het formulier in (E-mail, Bericht, Rol) en verzendt de uitnodiging door op **[!UICONTROL Send]**.

>[!NOTE]
>
>   
>Als u het geneesmiddel niet ziet [!UICONTROL Invite a new user] -knop, uw organisatie is aangemeld bij de [!DNL Adobe Business Platform.]
>
>  Voor instructies over het toevoegen van een gebruiker aan een organisatie die aan is geregistreerd [!DNL Adobe Business Platform], zie [Gebruikers toevoegen aan [!DNL Adobe Workfront Fusion] via de [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

De gebruiker ontvangt een e-mailuitnodiging waarin hij of zij de uitnodiging kan accepteren.
