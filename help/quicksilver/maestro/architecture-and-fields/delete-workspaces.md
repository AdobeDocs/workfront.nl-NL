---
title: Werkruimten verwijderen
description: U kunt werkruimten verwijderen als deze niet meer relevant zijn.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Werkruimten verwijderen

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

In Adobe Maestro, zijn de werkruimten gecentraliseerde plaatsen voor teams om het werk te plannen. Zie voor meer informatie [Werkruimten maken](../architecture-and-fields/create-workspaces.md).

U kunt werkruimten verwijderen die niet meer relevant zijn.

We raden u aan enkele of alle recordtypen en taxonomieën die aan de werkruimte zijn gekoppeld, opnieuw te maken die u in een andere werkruimte wilt verwijderen voordat u deze verwijdert.

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

## Overwegingen bij het verwijderen van werkruimten

* U kunt elke werkruimte verwijderen die u of iemand in uw organisatie heeft gemaakt. <!--this will change with access levels and permissions-->
* Wanneer u werkruimten verwijdert, worden ook alle recordtypen, taxonomieën en de bijbehorende velden verwijderd. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* Verwijderde werkruimten en de gegevens in deze werkruimten kunnen niet worden hersteld.

## Een werkruimte verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   Hierdoor wordt de laatste werkruimte geopend die u hebt geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte die u wilt verwijderen.
1. Klik op de knop **Meer** menu ![](assets/more-menu.png) naast de naam van de werkruimte klikt u op **Verwijderen**.
1. Klikken **Verwijderen** ter bevestiging.

   De werkruimte wordt verwijderd en kan niet worden hersteld. Alle recordtypen, taxonomieën, de bijbehorende records en de bijbehorende velden worden ook verwijderd. <!--ensure this is right after closed beta-->