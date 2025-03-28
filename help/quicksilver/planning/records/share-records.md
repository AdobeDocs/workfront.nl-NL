---
title: Records delen
description: U kunt records met anderen delen om de samenwerking te verbeteren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Records delen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<!--take out preview and production references at release-->

{{planning-important-intro}}

Als u met andere gebruikers wilt samenwerken, kunt u records met anderen delen.

U kunt een Adobe Workfront-planningsrecord op de volgende manieren delen:

* Kopieer de koppeling van de recordpagina vanuit uw browser wanneer de pagina is geopend.

* Kopieer een koppeling naar de pagina van de record wanneer u records bekijkt in de tabelweergave van het recordtype.

* U kunt alle records in een werkruimte delen met andere gebruikers door de werkruimte <!--<span class="preview">and record type</span>--> te delen. Voor meer informatie, zie [ een werkruimte ](/help/quicksilver/planning/access/share-workspaces.md) delen.

<!-- replace the last sentence above with this: 

For more information see the following articles:

* [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md)


<div class="preview">

* [Share a record type](/help/quicksilver/planning/access/share-record-types.md)

</div>

-->

In dit artikel wordt beschreven hoe u een koppeling naar de pagina van een record kunt kopiëren vanuit de tabelweergave van een recordtype.

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
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Medewerker, licht of standaard </p>
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
   <td>  <p>Machtigingen voor het delen van een record via een koppeling weergeven of hoger in een werkruimte<!--<span class="preview">and record type</span>--> </p>
   <p>Rechten voor een werkruimte beheren <!--<span class="preview">and record type</span>--> om de records in de werkruimte te delen </p>
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


<!--OLD:

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
   <p> Adobe Workfront</p> </td>
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
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
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

## Recordkoppelingen delen vanuit de tabelweergave van het recordtype

{{step1-to-planning}}

De werkruimte die u het laatst hebt geopend.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) van **Mening** drop-down menu in de hoger-juiste hoek van de lijst, selecteer een lijstmening. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik met de rechtermuisknop op een recordrij

   of

   Beweeg over de naam van een verslag, klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **verbinding van het Exemplaar**.

   ![ Contextueel menu voor verslagrij ](assets/contextual-menu-for-record-row.png)

   De koppeling wordt naar het klembord gekopieerd.

1. Plak de koppeling in een e-mail- of chatvenster om deze met andere gebruikers te delen. Wanneer gebruikers de koppeling ontvangen, wordt de recordpagina geopend.

   >[!TIP]
   >
   >De velden op de recordpagina zijn dezelfde velden die beschikbaar zijn in de tabelweergave van de record.


   <!--add there when it will be available: if they have access to this record-->

## Alle records in een werkruimte delen door de werkruimte te delen

U kunt alle records in een werkruimte delen wanneer u de werkruimte deelt met anderen.

Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen deze delen met anderen.

Voor meer informatie, zie [ een werkruimte ](/help/quicksilver/planning/access/share-workspaces.md) delen.


<!--
<div class="preview">

## Share all records in a record type by sharing the record type

In the Production environment, records inherit permissions from the workspace. 

In the Preview environment, records inherit permissions from the record type. 

By default, record types inherit permissions from the workspace. 

However, you can do any of the following:

* Turn off inherited permissions from the workspace on a record type. This removes permissions from the records. 
* Manually grant permissions to users to a record type, even when they have no permissions to the workspace. This automatically gives them View permissions to the workspace. This grants permissions to users to the records. 

Only users with Manage permissions to a workspace can share its record types and records with others. 

For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>

-->