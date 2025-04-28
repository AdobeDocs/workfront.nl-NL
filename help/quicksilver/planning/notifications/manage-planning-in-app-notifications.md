---
title: In-app-berichten voor Adobe Workfront-planning beheren
description: Wanneer iemand u in een recordcommentaar etiketteert, ontvangt u een e-mailbericht voor die markering.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---


# In-app-berichten voor Adobe Workfront-planning beheren

{{planning-important-intro}}

U kunt in-app berichten van de Planning van Workfront ontvangen wanneer de volgende scenario&#39;s bestaan:

* Iemand plaatst een tag voor u in een recordopmerking

  Voor informatie over het etiketteren van anderen in een verslagcommentaar, zie [ recordcommentaren beheren ](/help/quicksilver/planning/records/manage-record-comments.md).
* Iemand vraagt uw toestemming om een mening of een werkruimte te openen
* Iemand bevestigt dat uw toegang is verleend voor een weergave of werkruimte <!--Isk confirmed there is no notification for denying permissions - did not test-->

## Toegangsvereisten

+++ Breid uit om toegangsvereisten te bekijken..

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd.</p> 
<p>De gebruikers in uw organisatie ontvangen berichten van de Planning van Workfront slechts wanneer uw organisatie aan de Adobe Verenigde Ervaring wordt betreden. </p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard, licht of contribuant</p>
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
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

+++ Expand to view access requirements.. 

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
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

+++
-->

## Meldingen in de app beheren wanneer iemand u in een opmerking van tags voorziet

1. (Voorwaardelijk) na iemand etiketteert u in een commentaar op een verslag, ga naar het in-app **pictogram van Meldingen** pictogram ![ de wolkenberichten van de Ervaring ](assets/experience-cloud-notifications-icon.png) in Adobe Experience Cloud.

   ![ In-app meldingsvoorbeeld ](assets/in-app-notification-example.png)

1. Klik op het bericht.

   De pagina met recorddetails wordt geopend in Workfront Planning. U kunt de record bijwerken of op de opmerking reageren.

1. (Facultatief) klik **Teken allen als gelezen** om erop te wijzen dat u alle berichten hebt gelezen.
1. (Facultatief) klik **Mening allen** om naar de **pagina van Meldingen** in Adobe Experience Cloud te gaan.

## Meldingen in apps beheren bij het aanvragen en verlenen van machtigingen

U ontvangt meldingen in de app wanneer iemand u om toestemming vraagt of verleent aan een weergave of werkruimte.

Voor informatie over het verzoeken van, het verlenen van, of het ontkennen van toestemmingen aan een mening of een werkruimte, zie {de toestemmingen van 0} Verzoek aan een mening of een werkruimte ](/help/quicksilver/planning/access/request-permissions.md).[

Voor informatie over het beheren van uw berichten van de Planning van Workfront, zie [ de het berichtvoorkeur van de Planning van Adobe Workfront beheren ](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
