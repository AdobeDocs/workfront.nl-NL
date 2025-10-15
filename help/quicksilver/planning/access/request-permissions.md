---
title: Machtigingen aanvragen voor een weergave of een Workspace
description: Wanneer iemand een koppeling deelt naar een weergave of werkruimte waartoe u geen toegang hebt, kunt u machtigingen aanvragen om de koppeling te kunnen openen. In dit artikel worden de stappen beschreven die u moet uitvoeren om toegang te vragen tot een weergave of werkruimte wanneer u een gedeelde koppeling tegenkomt die u niet kunt openen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Machtigingen aanvragen voor een weergave of werkruimte

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>De functionaliteit die in dit artikel wordt beschreven is beschikbaar slechts wanneer uw organisatie aan de Adobe Verenigde Ervaring is genegeerd.
>
>Voor meer informatie, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


U kunt machtigingen aanvragen voor een weergave of werkruimte wanneer iemand een koppeling deelt met u naar de weergave of werkruimte waartoe u geen toegang hebt.

Het aanvragen van machtigingen voor een weergave lijkt op het aanvragen van machtigingen voor een werkruimte.

In dit artikel wordt beschreven hoe u toegang tot een weergave of werkruimte kunt aanvragen wanneer iemand een koppeling met u deelt en u geen toegang hebt tot de gedeelde pagina.

Zie de volgende artikelen voor informatie over het verlenen van machtigingen aan weergaven en werkruimten:

* [Weergaven delen](/help/quicksilver/planning/access/share-views.md)
* [Werkruimten delen](/help/quicksilver/planning/access/share-workspaces.md)


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront- en planningspakketten</p> 
of
<p>Willekeurig workflowpakket en planningspakket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Alle</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  <p>Nadat uw verzoek om toestemming wordt verleend, kon u de volgende toestemmingen verkrijgen:</p>
   <ul><li><p>Weergeven of Beheren voor een weergave</p></li>
   <li><p>Een werkruimte weergeven, Contribute of Beheren</p></li></ul>  
   <p>Alleen gebruikers met de machtiging Beheren in een werkruimte en een weergave kunnen een weergave openbaar delen.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## Machtigingen aanvragen voor een weergave of werkruimte

Het aanvragen van machtigingen voor een weergave is vergelijkbaar met het aanvragen van machtigingen voor een werkruimte.

Wanneer iemand met u een koppeling deelt naar een werkruimte of een weergave waartoe u geen toegang hebt:

1. Klik op de koppeling die met u wordt gedeeld voor de weergave of de werkruimte.

   A **u hebt geen toegang** paginagtoningen om u mee te delen dat u geen toegang tot de mening of de werkruimte hebt.

   ![ toegang van het Verzoek tot mening ](assets/request-access-to-view.png)

1. (Voorwaardelijk) als de gedeelde verbinding voor een mening voor een werkruimte is waar u toegang hebt, klik **Open met bestaande mening**. Als u toegang hebt tot de werkruimte, wordt de pagina met recordtypen geopend in de standaardweergave.

1. (Facultatief en voorwaardelijk) als u geen toestemmingen hebt om de werkruimte te bekijken, voeg een gepersonaliseerd bericht in de beschikbare doos toe, dan klik **de toegang van het Verzoek**.

   Alle gebruikers met de machtiging Beheren voor de weergave of werkruimte ontvangen de volgende meldingen voor de toegangsaanvraag:
   * Een melding in de app
     ![ In-app bericht voor toegangsverzoek ](assets/in-app-notification-for-access-request.png)
   * Een e-mailmelding
     ![ E-mailbericht voor toegangsverzoek ](assets/email-notification-for-access-request.png)

1. (Voorwaardelijk) Wanneer de weergave of werkruimtenmanager u machtigingen verleent aan de weergave of werkruimte, ontvangt u een e-mailmelding en een melding in de app met een bevestiging dat de machtiging is verleend. <!--check this - I was not able to test this, but Isk confirmed.-->
