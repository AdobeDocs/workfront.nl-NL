---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Verschillen in beheer op basis van platforms (Adobe Workfront/Adobe Business Platform)
description: Als uw organisatie is aangemeld bij het Adobe Business Platform, gebruiken uw gebruikers het Adobe Business Platform om toegang te krijgen tot Adobe Workfront. Dit betekent dat gebruikersbeheer grotendeels via de Adobe Admin Console wordt uitgevoerd en dat Single Sign-On (SSO) wordt afgehandeld via het Adobe Business Platform in plaats van via Workfront. Als Adobe Workfront-beheerder verschillen uw beheerverantwoordelijkheden en -procedures afhankelijk van het feit of uw organisatie is aangemeld bij het Adobe Business Platform. Dit artikel bevat een lijst met de procedures die verschillend moeten worden afgehandeld en koppelingen naar instructies voor zowel Workfront als Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Platformgebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)

Als Adobe Workfront-beheerder kunnen uw beheerverantwoordelijkheden en -procedures afwijken, afhankelijk van het feit of uw organisatie is aangemeld bij het Adobe Business Platform. Dit artikel bevat een overzicht van de procedures die verschillend worden afgehandeld en koppelingen naar instructies voor zowel Workfront als Adobe Admin Console.

Als uw organisatie is aangemeld bij het Adobe Business Platform, gebruiken uw gebruikers het Adobe Business Platform om toegang te krijgen tot Adobe Workfront. Dit betekent dat:

* Systeembeheerders worden gemaakt via de Adobe Admin Console
* Het vernieuwen van een SAML-certificaat wordt afgehandeld via de Adobe Admin Console.
* Single Sign-On (SSO) wordt afgehandeld via het Adobe Business Platform in plaats van via Workfront

## Workfront-systeembeheerders maken in de Adobe Admin Console

>[!NOTE]
>
>We raden u aan om gebruikers die geen systeembeheerders zijn, rechtstreeks toe te voegen in Workfront. Het is mogelijk om gebruikers toe te voegen in de Adobe Admin Console, maar als u ze toevoegt in Workfront, kunt u hun toegangsniveau instellen terwijl u ze maakt. Op die manier kunt u tijd besparen.

Voor instructie bij het creëren van het systeembeheerders van Workfront, zie [&#x200B; gebruikers in Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## Het SAML-certificaat verlengen

Voor instructies bij het vernieuwen van het certificaat van SAML op Adobe Admin Console, zie de sectie &quot;De digitale handtekening in de reactie van SAML ongeldig maakte...&quot;in [&#x200B; het Oplossen van problemen Federated ID &#x200B;](https://helpx.adobe.com/nl/enterprise/kb/tshoot-fed-id.html).

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/nl/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO (eenmalige aanmelding)

Omdat het Adobe Business Platform Single Sign-On (SSO) voor gebruikers beheert, worden de volgende acties en functies automatisch afgehandeld via het Adobe Business Platform. Als uw organisatie nog niet is aangemeld bij het Adobe Business Platform, moet u deze handelingen uitvoeren in Workfront.


* [&#x200B; vorm Adobe Workfront met SAML 2.0 &#x200B;](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [&#x200B; vorm Adobe Workfront met SAML 2.0 gebruikend ADFS &#x200B;](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [&#x200B; deactivate enig teken-op in Adobe Workfront &#x200B;](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [&#x200B; de meta-gegevens van SAML 2.0 van de Update in uw identiteitsleverancier &#x200B;](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [&#x200B; de gebruikers van de Update voor enig teken-op &#x200B;](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [&#x200B; vorm wachtwoordbeleid voor authentificatie &#x200B;](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [&#x200B; vorm de voorkeur van de systeemveiligheid &#x200B;](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
