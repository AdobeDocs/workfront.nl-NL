---
title: Recordtypen verwijderen
description: U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn. Als u recordtypen verwijdert, verwijdert u ook alle informatie die is gekoppeld aan de recordtypen, zoals records, velden en weergaven.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 425c3d3afb892ac83a10bbd36efb4c7d9712c4dc
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---


# Recordtypen verwijderen

{{planning-important-intro}}

U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn.

Als u echter recordtypen verwijdert, wordt ook alle informatie verwijderd die aan de recordtypen is gekoppeld. Voor meer informatie, zie de [ Overwegingen wanneer het schrappen van verslagtypes ](#considerations-when-deleting-record-types) sectie in dit artikel.

Voor informatie over verslagtypes, zie [ overzicht van de types van Verslag ](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
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
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p></td> 
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Overwegingen bij het verwijderen van recordtypen

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* U kunt alleen recordtypen verwijderen uit werkruimten waarvoor u beheerdersmachtigingen hebt.
* Als u recordtypen verwijdert, wordt de volgende informatie verwijderd die aan deze recordtypen is gekoppeld:

   * Alle records van dat type.
   * Alle velden die aan het recordtype zijn gekoppeld.
   * Alle weergaven (inclusief filters, groepen en sorteercriteria) van het recordtype.
* Het recordtype wordt verwijderd uit alle gebruikers die de werkruimte openen.
* U kunt verwijderde recordtypen of de bijbehorende gegevens niet herstellen.
* U wordt aangeraden de velden en records die zijn gekoppeld aan het recordtype dat u wilt verwijderen, opnieuw te maken in een ander recordtype voordat u ze verwijdert.

## Recordtypen verwijderen

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt verwijderen.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van het verslagtype, klik **Meer** menu, toen **Schrapping**.
   * Klik de kaart voor het verslagtype dat u, en van de verslagtype pagina wilt schrappen, **Meer** menu ![](assets/more-menu.png) aan het recht van de verslagtype naam klikken, dan **Schrapping** klikken.

   ![](assets/permanently-delete-record-type-confirmation.png)

1. Het type **schrapt** in de bevestigingsdoos, dan klikt **permanent schrapt**. Dit is niet hoofdlettergevoelig.

   Het geselecteerde recordtype en de bijbehorende velden, bijbehorende records en weergaven worden verwijderd en kunnen niet worden hersteld.
