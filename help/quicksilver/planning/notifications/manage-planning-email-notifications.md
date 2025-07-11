---
title: E-mailberichten voor Adobe Workfront-planning beheren
description: Wanneer iemand u of uw teams in een recordcommentaar in de Planning van Adobe Workfront etiketteert, ontvangt u een e-mailbericht voor die markering.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---


# E-mailberichten voor Adobe Workfront Planning beheren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt e-mailmeldingen ontvangen van Workfront Planning wanneer de volgende scenario&#39;s bestaan:

* Iemand tagt u of uw teams in een recordopmerking

  Voor informatie over het etiketteren van anderen in een verslagcommentaar, zie [ recordcommentaren beheren ](/help/quicksilver/planning/records/manage-record-comments.md).
* Iemand vraagt uw toestemming om een mening of een werkruimte te openen
* Iemand bevestigt dat uw toegang is verleend voor een weergave of werkruimte <!--Isk confirmed that there is nno email for denying access but did not test-->
* Je verzendt een aanvraag voor Workfront-planning. Voor informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md)
* Iemand keurt of verwerpt een Workfront-planningsverzoek dat u hebt ingediend goed. Voor informatie, zie [ een verzoek in de Planning van Adobe Workfront goedkeuren ](/help/quicksilver/planning/requests/approve-request.md)
* De status verandert in een Workfront-planningsverzoek dat u hebt verzonden.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

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

1. (Voorwaardelijk en optioneel) Nadat iemand u of uw team tags heeft toegevoegd aan een opmerking in een record, gaat u naar het e-mailbericht dat u op de hoogte brengt van de tag en de opmerking. De afzender van de e-mail is Adobe Experience Cloud.

   ![ E-mail- berichten voorbeeld ](assets/email-notification-example.png)

1. (Facultatief) klik het bericht in het **Workfront** vakje binnen e-mail.

   De pagina met recorddetails wordt geopend in Workfront. U kunt de record bijwerken of op de opmerking reageren.

1. (Voorwaardelijk) als beschikbaar, klik **Mening alle berichten**. <!--check with Lilit - do non-IMS users have this button??-->
De **Berichten** pagina opent in Adobe Experience Cloud. Alle berichten van alle Adobe Experience Cloud-toepassingen worden weergegeven.

## E-mailmeldingen beheren wanneer machtigingen worden aangevraagd en verleend

1. (Voorwaardelijk en optioneel) Nadat iemand u toestemming heeft gevraagd of verleend om toegang te krijgen tot een weergave of werkruimte, gaat u naar de e-mail die u op de hoogte stelt van de aanvraag voor toestemming. De afzender van de e-mail is Adobe Experience Cloud.

1. (Facultatief) klik het bericht in het **Workfront** vakje binnen e-mail.

   De pagina met recorddetails wordt geopend in Workfront. U kunt de record bijwerken of op de opmerking reageren.

1. (Voorwaardelijk) als beschikbaar, klik **Mening alle berichten**.
De **pagina van Meldingen** opent in Adobe Experience Cloud. Alle berichten van alle Adobe Experience Cloud-toepassingen worden weergegeven.


Voor informatie over het verzoeken van, het verlenen van, of het ontkennen van toestemmingen aan een mening of een werkruimte, zie {de toestemmingen van 0} Verzoek aan een mening of een werkruimte [.](/help/quicksilver/planning/access/request-permissions.md)

Voor informatie over het beheren van uw berichten van de Planning van Workfront, zie [ de het berichtvoorkeur van de Planning van Adobe Workfront beheren ](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## E-mailmeldingen beheren over het verzenden, goedkeuren of negeren van Workfront-planningsverzoeken

1. (Optioneel) Ga naar de e-mail die Workfront u stuurt
nadat u een verzoek hebt ingediend of nadat een door u ingediend verzoek is goedgekeurd of afgewezen. De afzender van de e-mail is Adobe Workfornt.

1. (Facultatief) klik **Open verzoek**. Dit opent het verzoek in de Planning van Workfront.

1. Klik het **pictogram van de Meldingen** pictogram van het het gebiedspictogram van ![ in de hoger-juiste hoek van het scherm ](assets/notifications-area-icon-unified-shell.png) **pagina van Meldingen toegang te hebben.**

   Voor informatie over het beheren van uw berichten van de Planning van Workfront, zie [ de het berichtvoorkeur van de Planning van Adobe Workfront beheren ](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
