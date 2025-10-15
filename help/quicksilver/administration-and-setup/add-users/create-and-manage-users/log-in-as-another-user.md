---
title: Aanmelden als andere gebruiker
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder moet u mogelijk Workfront openen namens een andere gebruiker.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Aanmelden als een andere gebruiker

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

Als Adobe Workfront-beheerder moet u mogelijk Workfront openen namens een andere gebruiker. Of, als groepsbeheerder, zou u tot Workfront namens een gebruiker kunnen moeten toegang hebben die een lid van een groep is u beheert.

Als een taak bijvoorbeeld pas kan worden uitgevoerd wanneer een gebruiker op vakantie een bepaalde actie uitvoert, kunt u zich aanmelden als die gebruiker en in plaats daarvan de actie uitvoeren.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Omdat een documentintegratie verbinding kan maken met persoonlijke privébestanden, hebben beheerders geen toegang tot documentintegratie wanneer ze zijn aangemeld als een andere gebruiker.
>
>Voor meer informatie over documentintegratie, zie [&#x200B; documentintegratie &#x200B;](../../../administration-and-setup/configure-integrations/configure-document-integrations.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr>
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. Op deze manier kunt u zich als iedereen aanmelden.</li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. Op deze manier kunt u zich aanmelden als een gebruiker met een lagere licentie. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aanmelden en acties uitvoeren als een andere gebruiker

1. Meld u aan bij Workfront als Workfront-beheerder of groepsbeheerder.

   >[!NOTE]
   >
   >* Als u een groepsbeheerder bent, kunt u zich slechts als gebruikers in de groepen aanmelden u beheert. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten:
   >   
   >  ![&#x200B; Admin gebruiker van de Groep &#x200B;](assets/group-admin-user.png)
   >   
   >  Deze instelling is standaard uitgeschakeld. Voor meer informatie, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
   >   
   >* U kunt het wachtwoord van een Workfront-beheerder niet opnieuw instellen.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Login als**.

1. In het **Begin typend naam...** doos op het **Login als** lusje, begin typend de naam van de gebruiker, dan klik de naam wanneer het in de drop-down lijst verschijnt.


   >[!NOTE]
   >* Voor de gebruiker die u selecteert, moet een toegangsniveau zijn gedefinieerd in Workfront. U kunt zich niet aanmelden bij het Workfront-systeem als een gebruiker die geen rechten heeft om u aan te melden.
   >* De beheerders van de groep kunnen login slechts als gebruikers die lid van de groepen zijn zij leiden. Ze kunnen zich niet aanmelden als Workfront-beheerder.

1. Klik **Login**. U bent aangemeld als een andere gebruiker en een melding wordt boven in het scherm weergegeven om dit aan te geven.

   <!--
   <p> Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->



1. Nadat u de noodzakelijke acties als gebruiker hebt uitgevoerd, klik **Logout** bij de bovenkant van het scherm.

## Traceren en controleren van activiteiten terwijl een beheerder als een andere gebruiker is aangemeld

Workfront biedt mechanismen voor het bijhouden en controleren van activiteiten die plaatsvinden terwijl de beheerder als een andere gebruiker is aangemeld.

Wanneer u zich aanmeldt als een andere gebruiker, wordt de laatste aanmeldingsdatum voor die gebruiker gewijzigd in de datum waarop de systeem- of groepsbeheerder zich aanmeldt als die gebruiker.

* [&#x200B; indicatoren van de Mening over punten &#x200B;](#view-indicators-on-items)
* [Controlegegevens weergeven](#view-audit-information)

### Indicatoren weergeven voor objecten {#view-indicators-on-items}

Wanneer u zich bij Workfront als een andere gebruiker aanmeldt en een actie uitvoert, geeft Workfront duidelijk aan dat u elke actie uitvoert namens de gebruiker die u als gebruiker bent aangemeld.

Bijvoorbeeld, als u op een punt terwijl het programma geopend als een andere gebruiker opmerkt, wijst een verklaring erop dat de commentaar door u namens de gebruiker werd gemaakt toen het bekijken van de sectie van Updates van een voorwerp.

### Controlegegevens weergeven {#view-audit-information}

1. Meld u aan bij Workfront als Workfront-beheerder of groepsbeheerder.
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. In het linkerpaneel, klik **Login als**, dan klik het **Logboek van de Toegang** tabel.

   >[!NOTE]
   >
   >Telkens wanneer een systeem- of groepsbeheerder zich als een andere gebruiker bij Workfront aanmeldt, wordt de gebeurtenis in het audittrail aangemeld. Bovendien worden om het even welke controleerbare acties die plaatsvinden terwijl de beheerder als een andere gebruiker het programma wordt geopend het programma geopend in het auditspoor.

1. (Optioneel) U kunt de resultaten die in het audittrail worden weergegeven, op de volgende manieren filteren:

   * Door gebruiker die zich heeft aangemeld
   * Door gebruiker die is aangemeld als
   * Op datum en tijd
