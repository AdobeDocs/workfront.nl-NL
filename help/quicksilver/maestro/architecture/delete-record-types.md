---
title: Recordtypen verwijderen
description: U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Recordtypen verwijderen

{{maestro-important-intro}}

U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn.

Als u echter recordtypen verwijdert, wordt ook alle informatie verwijderd die aan de recordtypen is gekoppeld. Zie de klasse [Overwegingen bij het verwijderen van recordtypen](#considerations-when-deleting-record-types) in dit artikel.

Zie voor informatie over recordtypen [Overzicht van recordtypen](../architecture/overview-of-record-types-and-taxonomies.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Toegangsvereisten

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het bètaprogramma voor Adobe Workfront-planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de planning van Adobe Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

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

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen en bijbehorende taxonomieën worden weergegeven.
1. Klik op de kaart voor het recordtype dat u wilt verwijderen.

   Hierdoor wordt de pagina van het recordtype geopend.
1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van het recordtype klikt u op **Verwijderen**.
1. Klikken **Verwijderen** ter bevestiging.

   Het geselecteerde recordtype en de bijbehorende velden, bijbehorende records en weergaven worden verwijderd.
