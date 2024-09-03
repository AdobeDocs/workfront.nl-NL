---
title: Voorkeuren voor Adobe Workfront-planningsberichten beheren
description: Je kunt je berichtgevingsvoorkeuren voor Adobe Workfront Planning mogelijk beheren. In dit artikel wordt beschreven hoe u uw voorkeuren voor meldingen kunt configureren.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 1e62d5c7eff86432b4914793d75cdf4f835f3d5d
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---


# Voorkeuren voor Adobe Workfront-planningsberichten beheren

{{planning-important-intro}}

U kunt meldingen in de app of per e-mail ontvangen wanneer de volgende acties plaatsvinden in Workfront Planning:

* Iemand voegt u toe aan een opmerking op de recordpagina
* Iemand vraagt om toestemming om een weergave of werkruimte te openen
* Iemand geeft u toestemming om een weergave of werkruimte te openen <!--I could not test this but Isk confirmed-->

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

U moet het volgende hebben om tot de Planning van Workfront toegang te hebben:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Eerste</li> 
<li>Ultieme</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td> 
   <td> 
<p>Alle </p> 
<p>Voor meer informatie over wat in elk Plan van de Planning van Workfront inbegrepen is, zie <a href="https://business.adobe.com/products/workfront/pricing.html"> Adobe Workfront tarifering en verpakking </a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>De instantie van uw organisatie van Workfront moet aan de Adobe Verenigde Ervaring worden genegeerd.</p> 
<p>De gebruikers in uw organisatie ontvangen berichten van de Planning van Workfront slechts wanneer uw organisatie aan de Adobe Verenigde Ervaring wordt bezet. </p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p><p>Standaard, licht of contribuant
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>De mening of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Raadpleeg ook de volgende artikelen voor meer informatie over berichten over Workfront Planning:

* Voor informatie over commentaren op verslagen, zie [ recordcommentaren beheren ](/help/quicksilver/planning/records/manage-record-comments.md).
* Voor informatie over in-app berichten van de Planning van Workfront, zie [ binnen-app berichten voor de Planning van Adobe Workfront beheren ](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Voor informatie over e-mailberichten van de Planning van Workfront, zie [ e-mailberichten voor de Planning van Adobe Workfront beheren ](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).
<!--

OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive in-app notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

## Meldingsvoorkeuren beheren

1. Meld u aan bij Workfront met uw Adobe Experience Cloud-referenties.
1. Klik het **pictogram van het 0} rekeningsmenu ![](assets/account-menu-icon-on-experience-cloud.png) in het hoger-recht van het scherm, dan klik** Voorkeur **.**
1. Onder de **sectie van Meldingen**, klik **Workfront**.
1. Selecteer de meldingen die u wilt ontvangen.
of
Schakel de meldingen uit die u niet meer wilt ontvangen.

   ![](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. De volgende berichten zijn beschikbaar voor Workfront:

   * **Vermeldingen**: U ontvangt een bericht wanneer iemand u in een commentaar in de Planning van Workfront etiketteert
   * **Verzoeken**: U ontvangt een bericht wanneer iemand om u verzoekt of toestemming verleent aan een voorwerp van de Planning van Workfront

   Voor meer informatie over het beheren van berichten, zie [ voorkeur en berichten van de Rekening ](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
