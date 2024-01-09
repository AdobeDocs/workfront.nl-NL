---
title: Werkruimten maken
description: Een werkruimte is een inzameling van operationele verslagtypes en taxonomieën die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Werkruimten maken

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

In Adobe Maestro, zijn de werkruimten gecentraliseerde plaatsen voor teams om het werk te plannen.

Een werkruimte is een inzameling van operationele verslagtypes en taxonomieën die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Maestro.

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
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level*</p></td>
   <td> <p>System Administrator</p>  
   <p>The following license types:</p>
   <ul><li>New: Standard</li>
   <li>Current: Worker or higher </li></ul>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Maestro area to your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver\administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->




<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen over werkruimten

* U kunt werkruimten voor specifieke organisatorische eenheden binnen uw organisatie tot stand brengen, om de unieke manier aan te passen elke eenheid werkt.
* De recordtypen en taxonomieën die een werkruimte bevat, moeten de levenscyclus van het werk van een organisatie weerspiegelen.
* Wanneer u een werkruimte maakt, kan iedereen in uw organisatie deze weergeven, bewerken of verwijderen.  <!--this will change with access levels and permissions-->
* U kunt maximaal 1.000 werkruimten in uw organisatie hebben.
* Werkruimten bevatten recordtypen die uniek zijn voor elke werkruimte. <!--this might change-->

## Een werkruimte maken

1. (Voorwaardelijk) Als u geen werkruimten in uw systeem hebt, klikt u op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront, of in de **Hoofdmenu** pictogram ![](assets/main-menu-shell.png)  in de linkerbovenhoek, indien beschikbaar, klikt u op **Maestro** ![](assets/maestro-icon.png).

   Of klik in een bestaande werkruimte op de knop voor het naar beneden wijzen rechts van de naam van de werkruimte en klik vervolgens op **Werkruimte maken**.

   ![](assets/workspace-drop-down-right-menu.png)

   Hiermee opent u het gedeelte Werkruimten van Maestro.
1. (Optioneel en voorwaardelijk) Klik op **Voorvertoning** binnen een van de volgende vooraf gedefinieerde werkruimtjablonen:

   * Marketing management
   * Verkoopbeheer
   * Productbeheer

   Er is een indicatie van welke operationele recordtypen, taxonomieën en hoeveel velden aan elke sjabloon zijn gekoppeld.

   ![](assets/previewing-a-workspace-template.png)

   Voor informatie over Maestro werkruimtemalplaatjes, zie [Lijst met werkruimtemalplaatjes](../architecture/workspace-templates.md).

1. Klikken **Sjabloon gebruiken** om de werkruimte te maken op basis van de geselecteerde sjabloon

   of

   Klikken **Werkruimte maken** om een werkruimte helemaal opnieuw te maken.

   Er wordt een werkruimte gemaakt voor de volgende typen werkruimten:

   * Een lege werkruimte waarin u recordtypen handmatig kunt toevoegen.
   * Een werkruimte met voorbeeldrecordtypen die u verder kunt aanpassen.

1. Klik binnen de naam van de werkruimte in de koptekst van de nieuwe werkruimte om de naam ervan te wijzigen en druk vervolgens op Enter

   of

   Klik op de knop **Meer** menu ![](assets/more-menu.png)rechts van de naam van de werkruimte in de koptekst klikt u op **Naam wijzigen**.

1. (Optioneel) Klik op **Recordtype toevoegen** om recordtypen toe te voegen aan de werkruimte.

   Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

1. (Optioneel) Klik op **taxonomie toevoegen** om taxonomieën toe te voegen aan de werkruimte.

   Zie voor meer informatie [taxonomieën maken](../architecture/create-a-taxonomy.md).
