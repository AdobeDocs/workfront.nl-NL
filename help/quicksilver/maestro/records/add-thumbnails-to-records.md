---
title: Een miniatuur toevoegen aan een record
description: U kunt recordgegevens bewerken in Adobe Workfront Planning en elke record koppelen aan afzonderlijke miniaturen, zodat deze gemakkelijk herkenbaar zijn.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Een miniatuur toevoegen aan een record

{{maestro-important-intro}}

U kunt records koppelen aan unieke miniaturen in Adobe Workfront Planning, zodat ze gemakkelijk herkenbaar zijn.

U moet recordtypen maken voordat u records kunt maken en bewerken.
Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

## Toegangsvereisten

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
<p>Uw organisatie moet zijn ingeschreven voor het bètaprogramma Adobe Workfront Planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Contribute of hoger machtigingen voor een werkruimte </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td>  <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> <p>Zie voor meer informatie <a href="/help/quicksilver/maestro/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Overwegingen bij het opnemen van miniaturen

Als u visueel onderscheid wilt maken tussen records in een tabelweergave, kunt u een unieke miniatuurafbeelding aan elke record koppelen.

Overweeg het volgende:

* U kunt alleen afbeeldingsbestanden als miniaturen toevoegen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* U kunt een miniatuurafbeelding toevoegen aan afzonderlijke records in de tabelweergave.
* Miniaturen horen bij de recordgegevens en worden weergegeven in weergaven waar records worden weergegeven. Miniaturen worden bijvoorbeeld naast recordgegevens weergegeven in de volgende gebieden:

   * Het primaire veld van een record in de tabelweergave
   * De recordbalk in de tijdlijnweergave.
* U kunt geen recordminiaturen toevoegen vanaf de pagina van de record of vanuit een ander type weergave.
* Miniaturen worden niet weergegeven op de recordpagina.

## Een miniatuur toevoegen aan een record

{{step1-to-maestro}}

1. Selecteer de werkruimte voor de records waaraan u miniaturen wilt toevoegen en klik op de kaart met recordtype.

   Hierdoor wordt de pagina met recordtypen geopend.
1. Selecteer een tabelweergave in het menu **Weergave** vervolgkeuzelijst. Alle verslagen van het type u selecteerde tonen in een lijst.
1. Klik op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Miniatuur**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Het primaire veld is het veld dat in de eerste kolom van een tabelweergave wordt weergegeven. Het primaire veld is altijd bevroren en kan niet worden verborgen of verplaatst.

   De **Recordminiatuur** wordt geopend.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. In de **Uploaden** slepen en neerzetten van een bestand dat u als miniatuur wilt toevoegen of klikken **Selecteren om te uploaden** Blader vervolgens naar het afbeeldingsbestand dat u wilt toevoegen. Het bestand moet op uw computer worden opgeslagen.
1. (Optioneel) Gebruik het gereedschap Grootte wijzigen om de afbeelding uit te snijden en de grootte ervan te wijzigen.
1. Klikken **Afbeelding gebruiken** om de afbeelding als een miniatuur toe te voegen.
Hiermee sluit u het dialoogvenster **Recordminiatuur** doos.
1. (Voorwaardelijk) Als u ten minste Contribute-machtigingen voor de tabelweergave hebt, klikt u op **Velden** rechtsboven in de tabelweergave.
1. Selecteer de **Miniatuur** schakelen om de miniatuur weer te geven. Deze optie is standaard uitgeschakeld.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   De miniatuur wordt links van de waarde van het primaire veld weergegeven.
1. (Optioneel en voorwaardelijk) Als u geen Contribute- of hogere machtigingen voor de weergave hebt, selecteert u een nieuwe weergave in het menu **Weergave** of maak een weergave.
1. (Optioneel) Als u de miniatuur wilt verwijderen, plaatst u de cursor boven het primaire veld en klikt u op de knop **Meer** menu ![](assets/more-menu.png)> **Miniatuur** > de **Verwijderen** pictogram ![](assets/remove-image-icon.png)en klik vervolgens op **Wijzigingen opslaan**.

<!--
Replace the section above with the following when we release generate thumbnails:

## Add a thumbnail to a record

You can add a thumbnail to a record in the following ways:

* Upload a file from your computer
* Generate an image with a prompt

### Upload a thumbnail to a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Upload** tab, and drag and drop a file to add as a thumbnail
   Or
   Click **Select to upload**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) Use the sizing tool to crop and resize the image.
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
1. (Conditional) If you have at least Contribute permissions to the table view, click **Fields** in the upper-right corner of the table view. 
1. Select the **Thumbnail** toggle to display the thumbnail. This is deselected by default. 

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   The thumbnail displays to the left of the primary field value. 
1. (Optional and conditional) If you do not have Contribute or higher permissions to the view, select a new view from the **View** drop-down menu, or create a view. 
1. (Optional) To remove the thumbnail, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**.

### Generate a thumbnail for a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

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