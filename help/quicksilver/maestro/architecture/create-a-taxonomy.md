---
title: Startrecordtypen voor taxonomie maken
description: Taxonomieën zijn een type herbruikbare recordtypen die kenmerken vastleggen van een operationeel recordtype in Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Startrecordtypen voor taxonomie maken

{{maestro-important-intro}}

De types van taxonomieverslag vangen attributen over operationele verslagtypes in Adobe Maestro.

Campagne kan bijvoorbeeld een operationeel recordtype zijn. Hieronder vindt u taxonomieën die kenmerken vastleggen over het type campagnerecord: Regio, Publiek, Land.

Zie voor meer informatie over Maestro-recordtypen [Overzicht van recordtypen en taxonomieën](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt
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

## Overwegingen bij het maken van taxonomieën

* U moet een werkruimte maken voordat u recordtypen voor taxonomieën in de werkruimte kunt maken.

  Zie voor informatie over werkruimten [Werkruimten maken](../architecture/create-workspaces.md).
* U kunt een taxonomie recordtype tot stand brengen door één van het volgende te doen:
   * U kunt deze automatisch maken wanneer u een werkruimte maakt met een sjabloon. Zie voor meer informatie [Werkruimten maken](../architecture/create-workspaces.md).
   * Maak ze handmatig, helemaal opnieuw.

* Alle nieuw gecreëerde types van taxonomiverslag komen met de volgende gebieden:

   * Naam <!--if there won't be any more fields, consider rephrasing this-->

  Bovendien kunt u aangepaste velden toevoegen aan taxonomieën. Zie voor meer informatie [Velden maken](../fields/create-fields.md).

  >[!NOTE]
  >
  >    De recordtypes van taxonomie die worden gecreeerd wanneer het gebruiken van een werkruimtesjabloon hebben extra gebieden.

## Een recordtype voor de taxonomie maken

Het maken van gegevenstypen voor taxonomieën is vergelijkbaar met het maken van geheel nieuwe, operationele recordtypen of een werkruimtemalplaatje.

Zie de sectie Een geheel nieuw recordtype maken in het artikel voor meer informatie. [Recordtypen maken](../architecture/create-record-types.md).

Voor informatie over het automatisch creëren van taxonomieën wanneer het creëren van een werkruimte van een malplaatje, zie [Werkruimten maken](../architecture/create-workspaces.md).
