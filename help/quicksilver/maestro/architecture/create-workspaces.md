---
title: Werkruimten maken
description: Een werkruimte is een inzameling van operationele verslagtypes en taxonomieën die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '561'
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
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   <p>Huidig: Werk of hoger</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor Maestro</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>U ontvangt beheermachtigingen voor de werkruimten die u maakt. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>U moet het gebied Maestro aan uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Voor meer informatie over toegangsvereisten, zie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
* Wanneer u een werkruimte maakt, hebt u alleen de toestemming om de werkruimte te openen en te beheren. U moet het met andere gebruikers delen opdat zij met u in de zelfde ruimte kunnen samenwerken. Zie voor meer informatie [Een werkruimte delen](/help/quicksilver/maestro/access/share-workspaces.md).
* U kunt maximaal 1.000 werkruimten in uw organisatie hebben.
* Werkruimten bevatten recordtypen die uniek zijn voor elke werkruimte. <!--this might change-->

## Een werkruimte maken

{{step1-to-maestro}}

1. (Voorwaardelijk) Als u geen werkruimten in uw omgeving hebt, klikt u op **Werkruimte maken**

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
