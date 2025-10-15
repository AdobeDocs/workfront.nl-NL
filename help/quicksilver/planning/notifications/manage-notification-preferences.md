---
title: Voorkeuren voor Adobe Workfront-planningsberichten beheren
description: Je kunt je berichtgevingsvoorkeuren voor Adobe Workfront Planning mogelijk beheren. In dit artikel wordt beschreven hoe u uw voorkeuren voor meldingen kunt configureren.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: f2fe6ef78b3032f7a89d4c816cb11b525634c067
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Voorkeuren voor Adobe Workfront-planningsberichten beheren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt meldingen in de app of per e-mail ontvangen wanneer de volgende acties plaatsvinden in Workfront Planning:

* Iemand voegt u of uw teams toe aan een opmerking op de recordpagina
* Iemand vraagt om toestemming om een weergave of werkruimte te openen
* Iemand geeft u toestemming om een weergave of werkruimte te openen <!--I could not test this but Isk confirmed-->
* Je verzendt een aanvraag voor Workfront-planning.
* Iemand keurt of verwerpt een Workfront-planningsverzoek dat u hebt ingediend goed.
* De status verandert in een Workfront-planningsverzoek dat u hebt verzonden.

## Toegangsvereisten


+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Alle workflows en planningspakketten</li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Licht of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>De mening of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p><p>Standard, Light, or Contributor
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table> -->

Raadpleeg ook de volgende artikelen voor meer informatie over berichten over Workfront Planning:

* Voor informatie over commentaren op verslagen, zie [&#x200B; recordcommentaren beheren &#x200B;](/help/quicksilver/planning/records/manage-record-comments.md).
* Voor informatie over in-app berichten van de Planning van Workfront, zie [&#x200B; binnen-app berichten voor de Planning van Adobe Workfront beheren &#x200B;](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Voor informatie over e-mailberichten van de Planning van Workfront, zie [&#x200B; e-mailberichten voor de Planning van Adobe Workfront beheren &#x200B;](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Meldingsvoorkeuren beheren

1. Meld u aan bij Workfront met uw Adobe Experience Cloud-referenties.
1. Klik het **pictogram** het menupictogram van de Rekening op Experience Cloud ![&#x200B; in het hoger-recht van het scherm, dan klik &#x200B;](assets/account-menu-icon-on-experience-cloud.png) Voorkeur **.**
1. Onder de **sectie van Meldingen**, klik **Workfront**.
1. Selecteer de meldingen die u wilt ontvangen.
of
Schakel de meldingen uit die u niet meer wilt ontvangen.

   ![&#x200B; Adobe Experience Cloud berichten paneel voor de Planning van Workfront &#x200B;](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. De volgende berichten zijn beschikbaar voor Workfront:

   * **Vermeldingen**: U ontvangt een bericht wanneer iemand u of uw team in een commentaar in de Planning van Workfront etiketteert
   * **Verzoeken**: U ontvangt een bericht wanneer iemand één van het volgende deed:

      * Verzoekt of verleent u toestemming aan een voorwerp van de Planning van Workfront
      * Je hebt een aanvraag voor een Workfront-planning verzonden
      * De status van een Workfront-planningsverzoek dat u hebt ingediend
      * Aanvragen, subsidies of afwijzing van een aanvraag voor een Workfront-planning

   Voor meer informatie over het beheren van berichten, zie [&#x200B; voorkeur en berichten van de Rekening &#x200B;](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
