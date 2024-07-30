---
title: Een miniatuur toevoegen aan een record
description: U kunt recordgegevens bewerken in Adobe Workfront Planning en elke record koppelen aan afzonderlijke miniaturen, zodat deze gemakkelijk herkenbaar zijn.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Een miniatuur toevoegen aan een record

{{planning-important-intro}}

U kunt records koppelen aan unieke miniaturen in Adobe Workfront Planning, zodat ze gemakkelijk herkenbaar zijn.

U moet recordtypen maken voordat u records kunt maken en bewerken.
Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Toegangsvereisten

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
<p>Uw organisatie moet zijn ingeschreven in de vroege toegangsfase voor Workfront Planning </p>
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
   <p>Huidig: Plan</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td>  <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> <p>Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van het Werkmiddel ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het opnemen van miniaturen

Als u visueel onderscheid wilt maken tussen records in een tabelweergave, kunt u een unieke miniatuurafbeelding aan elke record koppelen.

Overweeg het volgende:

* Een miniatuur is uniek voor één record en is niet van toepassing op alle records van hetzelfde type.
* U kunt alleen afbeeldingsbestanden als miniaturen toevoegen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* U kunt een miniatuurafbeelding toevoegen aan afzonderlijke records in de tabelweergave of vanaf de pagina of het voorvertoningsvak van de record.
* Workfront uploadt automatisch een miniatuurafbeelding wanneer u een record maakt. U kunt deze afbeelding later wijzigen.
* Miniaturen horen bij de recordgegevens en worden weergegeven in gebieden waar records worden weergegeven. Miniaturen worden bijvoorbeeld naast recordgegevens weergegeven in de volgende gebieden:

   * Het primaire veld van een record in de tabelweergave
   * De recordbalk in de tijdlijnweergave.
   * De detailvoorvertoning en pagina van de record.

## Een miniatuur toevoegen aan een record

U kunt op de volgende manieren een miniatuur toevoegen:

* [Een miniatuur toevoegen aan een record vanuit de tabelweergave](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Een miniatuur toevoegen aan een record via de detailpagina](#add-a-thumbnail-to-a-record-from-the-details-page)

### Een miniatuur toevoegen aan een record vanuit de tabelweergave

{{step1-to-planning}}

1. Klik op de werkruimte voor de records waaraan u miniaturen wilt toevoegen en klik vervolgens op de opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.
1. Selecteer een lijstmening van het **drop-down menu van de Mening**. Alle verslagen van het type u selecteerde tonen in een lijst.
1. Beweeg over de primaire gebiedsinformatie, klik **Meer** menu ![](assets/more-menu.png), dan klik **Duimnagel**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Het primaire veld is het veld dat in de eerste kolom van een tabelweergave wordt weergegeven. Het primaire veld is altijd bevroren en kan niet worden verborgen of verplaatst. De optie Miniatuur is niet beschikbaar in het menu Meer als het primaire veld een formuleringsveld is.

   Het **uploadt** lusje opent door gebrek in de **duimnagel van het Verslag** doos.

   Voor meer informatie over het uploaden van de duimnagel, zie de sectie [ een duimnagel aan een verslag van de detailspagina ](#add-a-thumbnail-to-a-record-from-the-details-page) in dit artikel, beginnend met Stap 6 toevoegen. <!--see if this is accurate-->

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### Een miniatuur toevoegen aan een record via de detailpagina

{{step1-to-planning}}

1. Klik op de werkruimte voor de records waaraan u miniaturen wilt toevoegen en klik vervolgens op de opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.
1. Klik vanuit een willekeurige weergave op een record om deze te openen.

   Het detailvoorbeeld wordt weergegeven.
1. (Facultatief) klik **Open in nieuw lusje** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek.

   De detailpagina van de record wordt geopend.
1. Beweeg over het duimnagelbeeld of pictogram ![](assets/record-thumbnail-icon-on-details-page.png), dan klik **Meer** menu ![](assets/more-menu.png) > **geef duimnagel** uit.

   Het **uploadt** lusje opent door gebrek in de **duimnagel van het Verslag** doos.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Een bestand slepen en neerzetten om als miniatuur toe te voegen

   of

   Klik **doorbladert beelden**, dan doorblader voor een beelddossier om toe te voegen. Het bestand moet op uw computer worden opgeslagen.

1. (Facultatief) na het beeld uploadt in de **duimnagel van het Verslag** doos, gebruik het het rangschikken hulpmiddel om het beeld uit te snijden en resize.
1. (Optioneel) Klik op het pictogram **Nieuwe afbeelding uploaden ![](assets/upload-new-image-icon.png) om een ander beeld te uploaden.**
1. (Facultatief) klik de **Galerij** tabel, dan klik een beeld. De galerie met afbeeldingen kan niet worden gewijzigd.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Facultatief) om de duimnagel te verwijderen alvorens het wordt bewaard, klik **verwijder** pictogram ![](assets/remove-image-icon.png) rechts van het beeld.

1. Klik **beeld van het Gebruik** om het beeld als duimnagel toe te voegen.
Dit sluit de **duimnagel van het Verslag** doos.
De miniatuur wordt weergegeven in gebieden van Workfront Planning waar de record wordt weergegeven.

   >[!TIP]
   >
   >   Als u miniaturen wilt weergeven in deze weergave, moet u het veld Miniatuur in de tabelweergave inschakelen. Deze optie is standaard uitgeschakeld.

1. (Facultatief) om de duimnagel te verwijderen nadat het wordt bewaard, klik een verslag in om het even welke mening om de detailspagina te openen, dan over het duimnagelbeeld te houden en **Meer** menu ![](assets/more-menu.png) te klikken > **verwijdert** pictogram ![](assets/remove-image-icon.png). De miniatuurafbeelding wordt verwijderd.




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->