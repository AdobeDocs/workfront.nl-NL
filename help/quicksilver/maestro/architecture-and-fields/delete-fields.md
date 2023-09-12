---
title: Velden verwijderen
description: In Adobe Maestro, kunt u douanevelden schrappen die niet meer relevant zijn.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Velden verwijderen

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

In Adobe Maestro, kunt u douanevelden tot stand brengen om informatie over verslagen op te slaan.

Voor informatie over het maken van aangepaste velden in Maestro raadpleegt u [Velden maken](../architecture-and-fields/create-fields.md).

U kunt Maestro-velden verwijderen die niet meer relevant zijn.

## Overwegingen bij het verwijderen van Maestro-velden:

* U kunt velden verwijderen die u hebt gemaakt of velden die door andere gebruikers zijn gemaakt. <!--this will change with access levels/ permissions-->
* U kunt een veld alleen verwijderen in de tabel met recordtypen.
* Alle informatie die in het veld is opgeslagen, wordt verwijderd en kan niet worden hersteld.
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Velden verwijderen

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   Hiermee opent u de laatst geopende werkruimte in Maestro.
1. Klik op de kaart van een recordtype waarvan u de velden wilt verwijderen.
1. (Voorwaardelijk) Selecteer een **Tabelweergave** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. Zoek het veld dat u wilt verwijderen in de kolomkoppen en houd de cursor boven de kolomkop en klik vervolgens op de pijl omlaag na de veldnaam.
1. Klikken **Verwijderen**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klikken **Verwijderen** ter bevestiging.

   Het veld wordt verwijderd, kan niet worden hersteld en kan niet meer aan records worden gekoppeld.