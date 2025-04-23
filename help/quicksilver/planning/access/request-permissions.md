---
title: Machtigingen aanvragen voor een weergave of een Workspace
description: Wanneer iemand een koppeling deelt naar een weergave of werkruimte waartoe u geen toegang hebt, kunt u machtigingen aanvragen om de koppeling te kunnen openen. In dit artikel worden de stappen beschreven die u moet uitvoeren om toegang te vragen tot een weergave of werkruimte wanneer u een gedeelde koppeling tegenkomt die u niet kunt openen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '625'
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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p> 
<p><b>BELANGRIJK</b></p>
<p>De gebruikers in uw organisatie kunnen om toestemmingen voor meningen en werkruimten slechts verzoeken wanneer uw organisatie aan de Adobe Verenigde Ervaring wordt betreden. </p>
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
   <td>  <p>Nadat uw verzoek om toestemming wordt verleend, kon u de volgende toestemmingen verkrijgen:</p>
   <ul><li><p>Weergeven of Beheren voor een weergave</p></li>
   <li><p>Een werkruimte weergeven, Contribute of Beheren</p></li></ul>  
   <p>Alleen gebruikers met de machtiging Beheren in een werkruimte en een weergave kunnen een weergave openbaar delen.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

-->

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
