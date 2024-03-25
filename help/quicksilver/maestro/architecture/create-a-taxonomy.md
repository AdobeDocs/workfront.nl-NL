---
title: Startrecordtypen voor taxonomie maken
description: Wanneer u een sjabloon gebruikt om een werkruimte te maken, worden recordtypen gemaakt in de secties Operationele records en Belastingen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Startrecordtypen voor taxonomie maken

{{maestro-important-intro}}

Wanneer u een sjabloon gebruikt om een werkruimte te maken, worden recordtypen gemaakt in de volgende secties:

* Operationele recordtypen
* Taxonomieën

De recordtypen in de sectie Taxonomies van een werkruimte leggen kenmerken vast over recordtypen in de sectie Typen operationele records van dezelfde werkruimte.

Campagne kan bijvoorbeeld een operationeel recordtype zijn. Hieronder vindt u taxonomieën die kenmerken vastleggen over het type campagnerecord: Regio, Publiek, Land.

Zie voor meer informatie over recordtypen [Overzicht van recordtypen](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Als u recordtypen wilt verbinden met Experience Manager Assets, hebt u een Adobe Experience Manager Assets-licentie nodig en moet het Workfront-exemplaar van uw organisatie zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma voor Adobe Workfront-planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
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

* U moet een werkruimte maken met behulp van een sjabloon voordat u recordtypen kunt maken in de sectie Taxonomies van de werkruimte.

  Zie voor informatie over werkruimten [Werkruimten maken](../architecture/create-workspaces.md).
* U kunt een recordtype maken in de sectie Taxonomies van een werkruimte door een van de volgende handelingen uit te voeren:
   * U kunt deze automatisch maken wanneer u een werkruimte maakt met een sjabloon. Zie voor meer informatie [Werkruimten maken](../architecture/create-workspaces.md).
   * U kunt ze handmatig maken in de sectie Taxonomies van een werkruimte.

* Alle nieuwe taxonomieën hebben standaard de volgende velden:

   * Naam
   * Beschrijving
   * Begindatum
   * Einddatum
   * Status

  Bovendien kunt u aangepaste velden toevoegen aan taxonomieën. Zie voor meer informatie [Velden maken](../fields/create-fields.md).

  >[!NOTE]
  >
  >    De recordtypes van taxonomie die worden gecreeerd wanneer het gebruiken van een werkruimtesjabloon hebben extra gebieden.

## Een recordtype voor de taxonomie maken

Het maken van taxonomie-recordtypen lijkt op het maken van recordtypen.

Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).
