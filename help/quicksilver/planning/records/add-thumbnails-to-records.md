---
title: Een miniatuur toevoegen aan een record
description: U kunt recordgegevens bewerken in Adobe Workfront Planning en elke record koppelen aan afzonderlijke miniaturen, zodat deze gemakkelijk herkenbaar zijn.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# Een miniatuur toevoegen aan een record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

U kunt records koppelen aan unieke miniaturen in Adobe Workfront Planning, zodat ze gemakkelijk herkenbaar zijn.

U moet recordtypen maken voordat u records kunt maken en bewerken.
Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Toegangsvereisten

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Alle workflows en planningspakketten</li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Contribute of hoger machtigingen voor een werkruimte en recordtype  </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr>   
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


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
1. Beweeg over de primaire gebiedsinformatie, klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **Duimnagel**.

   ![ Verslag meer uitgevouwen menu ](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Het primaire veld is het veld dat in de eerste kolom van een tabelweergave wordt weergegeven. Het primaire veld is altijd bevroren en kan niet worden verborgen of verplaatst. De optie Miniatuur is niet beschikbaar in het menu Meer als het primaire veld een formuleringsveld is.

   Het **uploadt** lusje opent door gebrek in de **duimnagel van het Verslag** doos.

   Voor meer informatie over het uploaden van de duimnagel, zie de sectie [ een duimnagel aan een verslag van de detailspagina ](#add-a-thumbnail-to-a-record-from-the-details-page) in dit artikel, beginnend met Stap 6 toevoegen. <!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### Een miniatuur toevoegen aan een record via de detailpagina

{{step1-to-planning}}

1. Klik op de werkruimte voor de records waaraan u miniaturen wilt toevoegen en klik vervolgens op de opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.
1. Klik vanuit een willekeurige weergave op een record om deze te openen.

   Het detailvoorbeeld wordt weergegeven.
1. (Facultatief) klik **Open in nieuw lusje** pictogram ![ Open details in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek.

   De detailpagina van de record wordt geopend.

1. (Voorwaardelijk) in de verslagvoorproef of detailspagina, houd over het duimnagelbeeld of pictogram van het pictogram ![ duimnagel van het Verslag op detailspagina ](assets/record-thumbnail-icon-on-details-page.png), dan klap over de ruimte boven de verslagnaam, dan klik **duimnagel** toevoegen of **geeft duimnagel** uit.

   Het **uploadt** lusje opent door gebrek in de **duimnagel van het Verslag** doos.

   ![ de duimnageldoos van het Verslag voor upload ](assets/record-thumbnail-box-for-upload.png)

1. Een bestand slepen en neerzetten om als miniatuur toe te voegen

   of

   Klik **doorbladert beelden**, dan doorblader voor een beelddossier om toe te voegen. Het bestand moet op uw computer worden opgeslagen.

1. (Facultatief) na het beeld uploadt in de **duimnagel van het Verslag** doos, gebruik het het rangschikken hulpmiddel om het beeld uit te snijden en resize.
1. (Optioneel) Klik op het pictogram **Nieuwe afbeelding uploaden** ![ om een ander beeld te uploaden.](assets/upload-new-image-icon.png)
1. (Facultatief) klik de **Galerij** tabel, dan klik een beeld. De galerie met afbeeldingen kan niet worden gewijzigd.

   ![ de duimnageldoos van het Verslag voor galerij ](assets/record-thumbnail-box-for-gallery.png)

1. (Facultatief) om de duimnagel te verwijderen alvorens het wordt bewaard, **verwijder** pictogram ![ verwijder beeldpictogram ](assets/remove-image-icon.png) rechts van het beeld.

1. Klik **beeld van het Gebruik** om het beeld als duimnagel toe te voegen.
Dit sluit de **duimnagel van het Verslag** doos.
De miniatuur wordt weergegeven in gebieden van Workfront Planning waar de record wordt weergegeven.

   >[!TIP]
   >
   >   Als u miniaturen wilt weergeven in deze weergave, moet u het veld Miniatuur in de tabelweergave inschakelen. Deze optie is standaard uitgeschakeld.

1. (Facultatief) om de duimnagel te verwijderen nadat het wordt bewaard, klik een verslag in om het even welke mening om de detailspagina te openen, dan te bewegen over het duimnagelbeeld en **Meer** menu ![ Meer menupictogram ](assets/more-menu.png) > **verwijder** pictogram ![ verwijder pictogram ](assets/remove-image-icon.png). De miniatuurafbeelding wordt verwijderd.


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
