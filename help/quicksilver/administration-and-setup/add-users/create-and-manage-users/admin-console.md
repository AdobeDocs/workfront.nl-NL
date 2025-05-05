---
title: Gebruikers in de Adobe Admin Console beheren
description: Als Adobe-beheerder kunt u Adobe Workfront-gebruikers en -systeembeheerders maken met de Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 6e4135fc6f0431c8222ce48c18a0b5c4c6f0dbed
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 0%

---

# Gebruikers beheren in de Adobe Admin Console

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>De functionaliteit in dit artikel is alleen beschikbaar als het exemplaar van Workfront van uw organisatie is aangemeld bij het Adobe Business Platform.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan het Van Bedrijfs Adobe Platform is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) ](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe-beheerder kunt u Adobe Workfront-systeembeheerders maken met de Adobe Admin Console. De console is een centrale locatie voor het beheer van de Adobe-rechten in uw hele organisatie. Voor meer informatie, zie het [ Overzicht van Admin Console ](https://helpx.adobe.com/nl/enterprise/using/admin-console.html).

>[!NOTE]
>
>* **de Beheerders van Workfront moeten in Adobe Admin Console worden gevormd.** voor informatie en instructies, zie [ systeembeheerders in Workfront met Adobe Admin Console ](#create-system-administrators-in-workfront-with-the-adobe-admin-console) in dit artikel creëren.
>* **als uw organisatie Enige Sign-On (SSO)** gebruikt, adviseren wij het creëren van gebruikers en het toewijzen van hen aan Workfront in Adobe Admin Console. Het is mogelijk deze gebruikers te maken in Workfront, maar er kunnen zich problemen voordoen bij het doorgeven van die informatie naar de Adobe Admin Console, op basis van de configuratie van de Admin Console van uw organisatie.
>   Nadat u de gebruiker in de Adobe Admin Console hebt gemaakt, kunt u de gebruikersgegevens in Workfront configureren, zoals het toewijzen van rollen, groepen, teams en toegangsniveaus.
>* **als uw organisatie geen Enige Sign-On (SSO)** gebruikt, kunt u niet-systeembeheerdergebruikers direct in Workfront toevoegen. Het is mogelijk om gebruikers toe te voegen in de Adobe Admin Console, maar als u ze toevoegt in Workfront, kunt u hun toegangsniveau instellen terwijl u ze maakt. Op die manier kunt u tijd besparen.

Wanneer u vanuit de Admin Console wijzigingen aanbrengt in gebruikersprofielen, wordt een update toegevoegd aan het tabblad Systeemactiviteit van de gebruiker in Workfront. De update wordt weergegeven zoals deze door het &quot;Systeem&quot; is gemaakt. Dit verwijst naar de Adobe Admin Console-beheerder en niet naar de Workfront-hoofdbeheerder.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe-beheerdersrechten</td> 
   <td> <p>U moet een beheerder van het Profiel van het Product van Adobe producten voor uw organisatie zijn</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u de Admin Console for Workfront gebruikt, ontvangt u een e-mail waarin u wordt uitgenodigd naar de console.

1. Als u nog geen ervaring hebt met Adobe en u een e-mail hebt ontvangen met de mededeling dat u nu beheerrechten hebt voor Adobe-software en -services voor uw organisatie, klikt u op de knop in de e-mail om een Adobe-account te maken en opent u de Admin Console.

   of

   Als u reeds een rekening van Adobe hebt, ga naar de [ pagina van Adobe Admin Console ](https://adminconsole.adobe.com/).

## Meer informatie over de Adobe Admin Console

* Workfront System Administrators kunnen een Workfront-gebruiker deactiveren vanuit Workfront, maar dit deactiveert de gebruiker niet in de Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* De gebruiker **Groep van het Huis** wordt bepaald gebaseerd op de gebruiker die hen creeerde. Dit kan niet worden aangepast vanuit de Admin Console.
* Het toegangsniveau van de Beheerder van het Systeem van Workfront kan slechts van binnen Adobe Admin Console worden uitgegeven.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* Het veranderen van de toegang van een gebruiker van de Beheerder van het Systeem in een ander toegangsniveau moet eerst door Admin Console worden gedaan.

  <!--
   This is not clear
  -->

* Als u de toegang tot de systeembeheerder van een gebruiker in Workfront wilt verwijderen, moet u de gebruiker met de Adobe Admin Console verwijderen als beheerder van het productprofiel. Hierdoor wordt het Workfront-toegangsniveau van de gebruiker gewijzigd van Systeembeheerder in Aanvrager.

  >[!IMPORTANT]
  >
  >Breng geen wijzigingen aan in het productprofiel zelf.

* Adobe Admin Console-beheerders kunnen automatische toewijzingsregels instellen om het toewijzen van Adobe-producten aan gebruikers in hun organisatie te automatiseren. Uw organisatie moet naar de Verenigde Ervaring van Adobe worden gemigreerd om deze functionaliteit te gebruiken. Voor meer informatie en instructies, zie [ automatische toewijzingsregels beheren ](https://helpx.adobe.com/nl/enterprise/using/automatic-assignment-rules.html) in de documentatie van Adobe.

## Open het gebied voor gebruikers en beheerders van uw Production-instantie van Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Van de [ pagina van Adobe Admin Console ](https://adminconsole.adobe.com/), selecteer het **Producten** lusje in de hoogste navigatiebar, en selecteer dan **Workfront**.

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. Selecteer in de lijst die wordt weergegeven de koppeling bovenaan.

   Dit is uw instantie van de Productie waar uw gebruikers werken.

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >De tweede koppeling in de lijst, uw voorbeeldinstantie, is een testomgeving die een replicatie is van uw live productieomgeving. Voor meer informatie, zie [ het Milieu van Sandbox van de Voorproef van Adobe Workfront ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >In de lijst ziet u mogelijk ook koppelingen naar sandboxomgevingen. Voor meer informatie, zie [ het Milieu van Sandbox van de Voorproef van Adobe Workfront ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. In de lijst die toont, met het **geselecteerde lusje van Profielen van het 0&rbrace; Product &lbrace;, klik de naam van de verbinding van het Profiel van het Product van Workfront.**

   ![ Profielen van het Product ](assets/prod-profile-1.png)

   Deze lijst bevat alle gebruikers die al zijn toegewezen aan uw productie-instantie van Workfront.

   >[!IMPORTANT]
   >
   >Breng geen wijzigingen aan in het productprofiel zelf.

1. Doorgaan naar een van de volgende secties in dit artikel:

   * [ creeer gebruikers in Workfront met Adobe Admin Console ](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Systeembeheerders in Workfront maken met de Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Systeembeheerders in Workfront maken met de Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

Het toegangsniveau van de Beheerder van het Systeem wordt verleend slechts op de Adobe Admin Console. U kunt geen beheerdersrechten verlenen of verwijderen vanuit Workfront.

U moet een gebruiker aan uw instantie van de Productie van Workfront toevoegen alvorens u tot de gebruiker een het systeembeheerder van Workfront kunt maken.

1. Ga naar het gebruiker en admin gebied in Admin Console, zoals die in de sectie [ wordt beschreven toegang tot het gebruiker en het admin gebied voor uw instantie van de Productie van Workfront ](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in dit artikel.
1. Selecteer het **Admins** lusje boven de lijst van gebruikers.
1. Selecteer **Admin** toevoegen.
1. In **voeg de beheerders van het productprofiel** doos toe, ga de e-mailadressen of de namen van de beheerders in u, dan uitgezocht **sparen** wilt toevoegen.

   ![ voeg admin ](assets/add-admin-1.png) toe

   De systeembeheerders worden in Workfront gemaakt.

   >[!IMPORTANT]
   >
   >Breng geen wijzigingen aan in het productprofiel zelf.


## Gebruikers in Workfront maken met de Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>We raden u aan om gebruikers die geen systeembeheerders zijn, rechtstreeks toe te voegen in Workfront. Het is mogelijk om gebruikers toe te voegen in de Adobe Admin Console, maar als u ze toevoegt in Workfront, kunt u hun toegangsniveau instellen terwijl u ze maakt. Op die manier kunt u tijd besparen.

* [Gebruikers rechtstreeks in Workfront maken in de Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Gebruikers maken in Workfront en ze goedkeuren voor de Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Gebruikers rechtstreeks in Workfront maken in de Adobe Admin Console

1. Ga naar het gebruiker en admin gebied in Admin Console, zoals die in de sectie [ wordt beschreven toegang tot het gebruiker en het admin gebied voor uw instantie van de Productie van Workfront ](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in dit artikel.
1. Met het **lusje van Gebruikers** dat boven de lijst wordt geselecteerd, **voegt Gebruiker** toe.
1. In **voeg gebruikers aan dit productprofiel** doos toe, ga het e-mailadres of de naam van een gebruiker in u wilt toevoegen, dan selecteren **sparen**.

   De gebruiker wordt in Workfront gemaakt met het toegangsniveau van de aanvrager.

   >[!IMPORTANT]
   >
   >Breng geen wijzigingen aan in het productprofiel zelf.

1. Wijzig in Workfront het toegangsniveau van de gebruiker.

   Voor instructies op hoe een beheerder van Workfront het de toegangsniveau van de gebruiker kan veranderen, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

1. Herhaal stap 3 en 4 om meer gebruikers toe te voegen.

   >[!NOTE]
   >
   >Voor nieuwe Adobe-gebruikers stuurt de Admin Console een e-mail om hen uit te nodigen het registratieproces te voltooien. Alle gebruikers moeten het registratieproces voltooien om toegang te krijgen tot een Adobe-toepassing.
   >
   >Voor bestaande Adobe-gebruikers kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Deze voorkeur wordt door de Adobe-beheerder voor het product bepaald. Uw Adobe-beheerder kan een andere persoon zijn dan uw Workfront-beheerder.

### Gebruikers maken in Workfront en ze goedkeuren voor de Adobe Admin Console

Op deze manier kunnen groepsbeheerders die geen toegang hebben tot de Adobe Admin Console, gebruikers maken.

Eerst maakt de groepsbeheerder de gebruiker in Workfront. Hierdoor wordt de gebruiker gedeactiveerd en in afwachting van de goedkeuringsstatus.

Vervolgens keurt een Workfront-beheerder de gebruiker goed. Hiermee activeert u de gebruiker in Workfront en voegt u deze toe aan de Adobe Admin Console.

#### De gebruiker in Workfront maken (groepsbeheerder)

Voor instructies bij het creëren van een gebruiker in Workfront, zie [ gebruikers ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

#### De gebruiker goedkeuren (Workfront-beheerder)

Een gebruiker goedkeuren:

{{step-1-to-users}}

1. Selecteer de gebruiker, dan klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png).

1. Om de gebruiker goed te keuren, klik **goedkeuren**, dan klik **voorleggen**.

   of

   Om de gebruiker te verwerpen en hen van Workfront te schrappen, klik **Weigeren**, dan klik **voorleggen**.

   Goedgekeurde gebruikers worden automatisch toegevoegd aan de Adobe Admin Console.

   Geweigerde gebruikers worden automatisch uit Workfront verwijderd.


## Bestaande gebruikers in de Adobe Admin Console bewerken

U kunt de volgende gebruikersgegevens bewerken in de Adobe Admin Console:

* Gebruikersgroepen en producten die aan de gebruiker zijn gekoppeld
* Administratieve rechten
* Land

Voor informatie bij het uitgeven van één enkele gebruiker in Adobe Admin Console, zie [ gebruikersdetails ](https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html#edit-user-details) in het artikel uitgeven individuele gebruikers in de documentatie van Adobe.

Voor informatie over gebruikers van bulkbewerking in de Adobe Admin Console raadpleegt u
[ geef gebruikersdetails ](https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html#edit-user-details) in het artikel uit leidt veelvoudige gebruikers in de documentatie van Adobe.
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/nl/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
