---
title: Aanmelden als een andere gebruiker
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder moet u mogelijk Workfront openen namens een andere gebruiker.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 0%

---

# Aanmelden als een andere gebruiker

<!--Audited: April, 2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Adobe Admin Console zijn. Als uw organisatie is aangemeld bij de Adobe Admin Console, is deze actie niet beschikbaar.
>
>Ga voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console naar [Platformgebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-beheerder moet u mogelijk Workfront openen namens een andere gebruiker.

Of, als groepsbeheerder, zou u tot Workfront namens een gebruiker kunnen moeten toegang hebben die een lid van een groep is u beheert.

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
>Zie voor meer informatie over documentintegratie [Documentintegratie configureren](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Met het de toegangsniveau van de Beheerder van het Systeem, kunt u login als iedereen. Voor informatie over dit toegangsniveau raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> <p>Met een toegangsniveau van de Planner, kunt u login als gebruiker met een lager vergunningsniveau als <b>Gebruikers</b> het plaatsen in het toegangsniveau wordt gevormd om <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste één van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>OPMERKING</b>: Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> 
   <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aanmelden en acties uitvoeren als een andere gebruiker

1. Meld u aan bij Workfront als Workfront-beheerder of groepsbeheerder.

   >[!NOTE]
   >
   >* Als u een groepsbeheerder bent, kunt u zich slechts als gebruikers in de groepen aanmelden u beheert. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Deze instelling is standaard uitgeschakeld. Zie voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* U kunt het wachtwoord van een Workfront-beheerder niet opnieuw instellen.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aanmelden als**.

1. In de **Gebruikers** op de **Aanmelden als** begint u de naam van de gebruiker te typen en klikt u vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   De gebruiker moet een toegangsniveau hebben dat in Workfront wordt bepaald. U kunt zich niet aanmelden bij het Workfront-systeem als een gebruiker die geen rechten heeft om u aan te melden.

   >[!NOTE]
   >
   >De beheerders van de groep kunnen login slechts als gebruikers die lid van de groepen zijn zij leiden. Ze kunnen zich niet aanmelden als Workfront-beheerder.

1. Klikken **Log in.**

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

   Wanneer u als een andere gebruiker het programma wordt geopend, toont een bericht bij de bovenkant van het scherm om op dit te wijzen.

1. Nadat u de noodzakelijke acties als gebruiker hebt uitgevoerd, klik **Afmelden.**

## Traceren en controleren van activiteiten terwijl een beheerder als een andere gebruiker is aangemeld

Workfront biedt mechanismen voor het bijhouden en controleren van activiteiten die plaatsvinden terwijl de beheerder als een andere gebruiker is aangemeld.

Wanneer u zich aanmeldt als een andere gebruiker, wordt de laatste aanmeldingsdatum voor die gebruiker gewijzigd tot de datum waarop de systeem- of groepsbeheerder zich aanmeldt als die gebruiker.

* [Indicatoren weergeven voor objecten](#view-indicators-on-items)
* [Controlegegevens weergeven](#view-audit-information)

### Indicatoren weergeven voor objecten {#view-indicators-on-items}

Wanneer u zich bij Workfront als een andere gebruiker aanmeldt en een actie uitvoert, geeft Workfront duidelijk aan dat u elke actie uitvoert namens de gebruiker die u als gebruiker bent aangemeld.

Bijvoorbeeld, als u op een punt terwijl het programma geopend als een andere gebruiker opmerkt, wijst een verklaring erop dat de commentaar door u namens de gebruiker werd gemaakt toen het bekijken van de sectie van Updates van een voorwerp.

### Controlegegevens weergeven {#view-audit-information}

1. Meld u aan bij Workfront als Workfront-beheerder of groepsbeheerder.
1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aanmelden als,** Klik vervolgens op de knop **Toegangslogboek** tab.

   Telkens wanneer een systeem- of groepsbeheerder zich als een andere gebruiker bij Workfront aanmeldt, wordt de gebeurtenis in het audittrail aangemeld. Bovendien worden om het even welke controleerbare acties die plaatsvinden terwijl de beheerder als een andere gebruiker het programma wordt geopend het programma geopend in het auditspoor.

1. (Optioneel) U kunt de resultaten die in het audittrail worden weergegeven, op de volgende manieren filteren:

   * Door gebruiker die zich heeft aangemeld
   * Door gebruiker die is aangemeld als
   * Op datum
