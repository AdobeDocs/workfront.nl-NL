---
title: Recordtypen verwijderen
description: U kunt gegevenstypen van operationele records of taxonomirecords verwijderen wanneer deze niet meer relevant zijn.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '391'
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

{{maestro-important-intro}}

U kunt gegevenstypen van operationele records of taxonomirecords verwijderen wanneer deze niet meer relevant zijn.

Zie voor informatie over recordtypen en taxonomieën [Overzicht van recordtypen en taxonomieën](../architecture/overview-of-record-types-and-taxonomies.md).

We raden u aan de velden en records die zijn gekoppeld aan het recordtype of de taxonomie die u wilt verwijderen, opnieuw te maken op een ander recordtype voordat u ze verwijdert.

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
   <p> Adobe Workfront</p> <p>Als u Maestro-recordtypen wilt verbinden met Experience Manager Assets, hebt u een Adobe Experience Manager Assets-licentie nodig en moet het Workfront-exemplaar van uw organisatie zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor Maestro</p>  
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
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
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

* U kunt alleen recordtypen of taxonomieën verwijderen uit werkruimten waar u beheerdersmachtigingen hebt.
* Als u recordtypen verwijdert, wordt alle bijbehorende informatie verwijderd, inclusief velden en records van dat type. Het recordtype wordt verwijderd uit alle gebruikers die de werkruimte openen.
* U kunt verwijderde recordtypen of de bijbehorende gegevens niet herstellen.

## Recordtypen verwijderen

Het verwijderen van gegevenstypen in een taxonomie is identiek aan het verwijderen van gegevenstypen in een operationeel record.

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen en bijbehorende taxonomieën worden weergegeven.
1. Klik op de kaart voor het recordtype of de taxonomie die u wilt verwijderen.

   Hierdoor wordt de pagina van het recordtype geopend.
1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van het recordtype klikt u op **Verwijderen**.
1. Klikken **Verwijderen** ter bevestiging.

   Het geselecteerde recordtype of de geselecteerde taxonomie, samen met de velden en bijbehorende records, worden verwijderd.
