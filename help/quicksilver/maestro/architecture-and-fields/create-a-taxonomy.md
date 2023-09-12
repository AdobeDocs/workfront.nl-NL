---
title: Startrecordtypen voor taxonomie maken
description: Taxonomieën zijn een type herbruikbare recordtypen die kenmerken vastleggen van een operationeel recordtype in Adobe Workfront Maestro.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Startrecordtypen voor taxonomie maken

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

Taxonomieën zijn recordtypen die kenmerken vastleggen over gegevenstypen in Adobe Maestro.

Campagne kan bijvoorbeeld een operationeel recordtype zijn. Hieronder vindt u taxonomieën die kenmerken vastleggen over het type campagnerecord: Regio, Publiek, Land.

Zie voor meer informatie over Maestro-recordtypen [Overzicht van recordtypen en taxonomieën](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
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

## Overwegingen bij het maken van taxonomieën

* U moet een werkruimte maken voordat u taxonomieën in de werkruimte kunt maken.

  Zie voor informatie over werkruimten [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
* U kunt een taxonomie recordtype tot stand brengen door één van het volgende te doen:
   * U kunt deze automatisch maken wanneer u een werkruimte maakt met een sjabloon. Zie voor meer informatie [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
   * Maak ze handmatig, helemaal opnieuw.
   * U kunt ze handmatig maken door gegevens uit een externe lijst te plakken.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* Alle nieuwe taxonomieën worden geleverd met de volgende velden:

   * Naam <!--if there won't be any more fields, consider rephrasing this-->

  Bovendien kunt u aangepaste velden toevoegen aan taxonomieën. Zie voor meer informatie [Velden maken](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    Taxonomieën die worden gemaakt wanneer een werkruimtemalplaatje wordt gebruikt, hebben aanvullende velden.

## Een taxonomie maken

Het maken van taxonomieën lijkt op het maken van een geheel nieuw operationeel recordtype of op basis van een werkruimtemalplaatje.

Zie de sectie Een geheel nieuw recordtype maken in het artikel voor meer informatie. [Recordtypen maken](../architecture-and-fields/create-record-types.md).

Voor informatie over het automatisch creëren van taxonomieën wanneer het creëren van een werkruimte van een malplaatje, zie [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
