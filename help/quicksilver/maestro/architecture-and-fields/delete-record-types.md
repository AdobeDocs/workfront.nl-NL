---
title: Recordtypen verwijderen
description: U kunt gegevenstypen van operationele records of taxonomirecords verwijderen wanneer deze niet meer relevant zijn.
hidefromtoc: true
hide: true
source-git-commit: 14b456f32dd2c8735e0a5252387f25305efc7610
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Recordtypen verwijderen

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt gegevenstypen van operationele records of taxonomirecords verwijderen wanneer deze niet meer relevant zijn.

Zie voor informatie over recordtypen en taxonomieën [Overzicht van recordtypen en taxonomieën](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

We raden u aan de velden en records die zijn gekoppeld aan het recordtype of de taxonomie die u wilt verwijderen, opnieuw te maken op een ander recordtype voordat u ze verwijdert.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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

## Overwegingen bij het verwijderen van recordtypen

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* U kunt elk recordtype of elke taxonomie verwijderen die u of iemand in uw organisatie heeft gemaakt. <!--this will change with access levels and permissions-->
* Als u recordtypen verwijdert, wordt alle bijbehorende informatie verwijderd, inclusief velden en records van dat type.
* U kunt verwijderde recordtypen of de bijbehorende gegevens niet herstellen.

## Recordtypen verwijderen

Het verwijderen van gegevenstypen in een taxonomie is identiek aan het verwijderen van gegevenstypen in een operationeel record.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen en bijbehorende taxonomieën worden weergegeven.
1. Klik op de kaart voor het recordtype of de taxonomie die u wilt verwijderen.

   Hierdoor wordt de pagina van het recordtype geopend.
1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van het recordtype klikt u op **Verwijderen**.
1. Klikken **Verwijderen** ter bevestiging.

   Het geselecteerde recordtype of de geselecteerde taxonomie, samen met de velden en bijbehorende records, worden verwijderd.