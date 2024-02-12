---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Platformgebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)
description: Als uw organisatie is aangemeld bij het Adobe Business Platform, gebruiken uw gebruikers het Adobe Business Platform om toegang te krijgen tot Adobe Workfront. Dit betekent dat gebruikersbeheer grotendeels via de Adobe Admin Console wordt uitgevoerd en dat Single Sign-On (SSO) wordt afgehandeld via het Adobe Business Platform in plaats van via Workfront. Als Adobe Workfront-beheerder verschillen uw beheerverantwoordelijkheden en -procedures afhankelijk van het feit of uw organisatie is aangemeld bij het Adobe Business Platform. Dit artikel bevat een lijst met de procedures die verschillend moeten worden afgehandeld en koppelingen naar instructies voor zowel Workfront als Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Platformgebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)

Als uw organisatie is aangemeld bij het Adobe Business Platform, gebruiken uw gebruikers het Adobe Business Platform om toegang te krijgen tot Adobe Workfront. Dit betekent dat:

* Systeembeheerders worden gemaakt via de Adobe Admin Console
* Single Sign-On (SSO) wordt afgehandeld via het Adobe Business Platform in plaats van via Workfront

Als Adobe Workfront-beheerder verschillen uw beheerverantwoordelijkheden en -procedures afhankelijk van het feit of uw organisatie is aangemeld bij het Adobe Business Platform. Dit artikel bevat een overzicht van de procedures die verschillend worden afgehandeld en koppelingen naar instructies voor zowel Workfront als Adobe Admin Console.

## Gebruikers



>[!NOTE]
>
>We raden u aan om gebruikers die geen systeembeheerders zijn, rechtstreeks toe te voegen in Workfront. Het is mogelijk om gebruikers toe te voegen in de Adobe Admin Console, maar als u ze toevoegt in Workfront, kunt u hun toegangsniveau instellen terwijl u ze maakt. Op die manier kunt u tijd besparen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Handeling</th> 
   <th>Zie voor instructies in Workfront</th> 
   <th>Voor instructies in de Adobe Admin console, zie</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Gebruikerbeheertoegang verlenen</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "Gebruikersgegevens bewerken" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gebruikers individueel beheren</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een gebruiker toevoegen aan Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Gebruikers toevoegen</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Gebruikers beheren in de Adobe Admin Console</a> </p> </li> 
     <li> <p>De sectie "Gebruikers toevoegen" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gebruikers individueel beheren</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Een gebruiker deactiveren</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "Gebruikers verwijderen" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gebruikers individueel beheren</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een gebruiker verwijderen</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Gebruikers verwijderen</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "Gebruikers definitief verwijderen" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Mapgebruikers beheren</a>
     </p><p>Opmerking: een gebruiker verwijderen uit het dialoogvenster [!DNL Adobe Admin Console] deactiveert de gebruiker in [!DNL Workfront], maar ze worden niet verwijderd [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een gebruikersprofiel bewerken</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "Gebruikersgegevens bewerken" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gebruikers individueel beheren</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gebruikersprofielen voor bulkbewerking</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Gebruikersprofielen bulksgewijs bewerken</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "Gebruikersgegevens bewerken" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk-CSV-upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gebruikers importeren </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Gebruikers importeren</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "Gebruikers toevoegen" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk-CSV-upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aanmelden als een andere gebruiker</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Aanmelden als een andere gebruiker</a> </p> </li> 
    </ul> </td> 
   <td>Niet beschikbaar</td> 
  </tr> 
  <tr> 
   <td role="rowheader">SAML-certificaat verlengen</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Het Adobe Workfront SAML 2.0-metagegevenscertificaat verlengen</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>De sectie "De digitale handtekening in de SAML-respons heeft niet gevalideerd..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Probleemoplossing Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (eenmalige aanmelding)

Omdat het Bedrijfs Platform van de Adobe Enige Sign-On (SSO) voor gebruikers controleert, worden de volgende acties en de functionaliteit automatisch behandeld door het Bedrijfs Platform van de Adobe. Als uw organisatie nog niet is aangemeld bij het Adobe Business Platform, moet u deze handelingen uitvoeren in Workfront.


* [Adobe Workfront configureren met SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Adobe Workfront configureren met SAML 2.0 met behulp van ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Single Sign-On in Adobe Workfront deactiveren](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [SAML 2.0-metagegevens bijwerken in uw identiteitsprovider](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Gebruikers bijwerken voor eenmalige aanmelding](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Wachtwoordbeleid voor verificatie configureren](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Systeembeveiligingsvoorkeuren configureren](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
