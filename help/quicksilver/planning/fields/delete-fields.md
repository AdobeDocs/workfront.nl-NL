---
title: Velden verwijderen
description: In de Planning van Adobe Workfront, kunt u douanegebieden schrappen die niet meer relevant zijn.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---



# Velden verwijderen

{{planning-important-intro}}

In de Planning van Adobe Workfront, kunt u douanevelden tot stand brengen om informatie over verslagen op te slaan.

Voor informatie over het creëren van douanegebieden in de Planning van Workfront, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

U kunt Workfront-planningsvelden verwijderen die niet meer relevant zijn.

## Overwegingen bij het verwijderen van Workfront-planningsvelden:

* U kunt een veld alleen verwijderen in de tabelweergave van het recordtype.
* U kunt het primaire veld van een record niet verwijderen.
* Alle informatie die in het veld is opgeslagen, wordt verwijderd en kan niet worden hersteld.
* Wanneer u een verbonden verslaggebied schrapt, worden alle verbonden raadplegingsgebieden ook geschrapt van het verslagtype u van verbindt. De verbonden recordvelden van de recordtypen waarmee u verbinding maakt, worden ook verwijderd uit de record waarmee u verbinding maakt.

  Wanneer u bijvoorbeeld campagnes verbindt met een ander recordtype genoemd product, en u het Product verbonden gebied en het de raadplegingsgebied van de Status van het Product van de campagne schrapt, worden het volgende geschrapt:

   * Het veld Product-verbinding van de campagne
   * Het veld Product Status opzoeken uit de campagne
   * Het veld Campagne verbonden vanuit het product.

  Voor meer informatie, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
<li>Eerste</li> 
<li>Ultieme</li></ul> 
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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard </p>
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
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Velden verwijderen

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordvelden wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.

1. Klik op de kaart van een recordtype.

1. (Voorwaardelijk) als niet reeds geselecteerd, klik het lusje van de mening van de a **Lijst** op de verslagtype pagina.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.

1. Zoek het veld dat u wilt verwijderen in de kolomkoppen en houd de cursor boven de kolomkop en klik vervolgens op de pijl omlaag na de veldnaam.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klik **Schrapping**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klik **Schrapping** om te bevestigen.

   Het veld wordt verwijderd, kan niet worden hersteld en kan niet meer aan records worden gekoppeld.
