---
title: E-mailberichten voor Adobe Workfront-planning beheren
description: Wanneer iemand u in een recordcommentaar in de Planning van Adobe Workfront etiketteert, ontvangt u een e-mailbericht voor die markering.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---


# E-mailberichten voor Adobe Workfront Planning beheren

{{planning-important-intro}}

U kunt e-mailmeldingen ontvangen van Workfront Planning wanneer de volgende scenario&#39;s bestaan:

* Iemand plaatst een tag voor u in een recordopmerking

  Voor informatie over het etiketteren van anderen in een verslagcommentaar, zie [ recordcommentaren beheren ](/help/quicksilver/planning/records/manage-record-comments.md).
* Iemand vraagt uw toestemming om een mening of een werkruimte te openen
* Iemand bevestigt dat uw toegang is verleend voor een weergave of werkruimte <!--Isk confirmed that there is nno email for denying access but did not test-->


## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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


## E-mailmeldingen beheren wanneer iemand u in een opmerking van tags voorziet

1. (Voorwaardelijk) Nadat iemand u in een commentaar op een verslag etiketteert, ga naar het e-mailbericht dat u van de markering en van de commentaar op de hoogte brengt. De afzender van de e-mail is Adobe Experience Cloud.

   ![](assets/email-notification-example.png)

1. Klik het bericht in de **doos van Workfront**.

   De pagina met recorddetails wordt geopend in Workfront. U kunt de record bijwerken of op de opmerking reageren.

1. (Voorwaardelijk) als beschikbaar, klik **Mening alle berichten**. <!--check with Lilit - do non-IMS users have this button??-->
De **Berichten** pagina opent in Adobe Experience Cloud. Alle berichten van alle Adobe Experience Cloud-toepassingen worden weergegeven.

## E-mailmeldingen beheren wanneer machtigingen worden aangevraagd en verleend

U ontvangt e-mailmeldingen wanneer iemand u machtigingen aanvraagt of verleent aan een weergave of werkruimte.

Voor informatie over het verzoeken van, het verlenen van, of het ontkennen van toestemmingen aan een mening of een werkruimte, zie {de toestemmingen van 0} Verzoek aan een mening of een werkruimte ](/help/quicksilver/planning/access/request-permissions.md).[

Voor informatie over het beheren van uw berichten van de Planning van Workfront, zie [ de het berichtvoorkeur van de Planning van Adobe Workfront beheren ](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
