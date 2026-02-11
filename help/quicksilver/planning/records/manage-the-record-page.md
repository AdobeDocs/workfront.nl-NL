---
title: De lay-out van de pagina Opnemen beheren
description: U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 0%

---


# De lay-out van de recordpagina beheren

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.

De recordvoorvertoning is een kleinere weergave van de recordpagina die wordt weergegeven in de weergave van een recordtype.

Wanneer u de indeling van een recordvoorvertoning en pagina wijzigt, hebben de wijzigingen invloed op de voorbeeldvakken en op de detailpagina&#39;s van alle records van hetzelfde type.

In dit artikel wordt beschreven hoe u de lay-out en weergave van een recordvoorvertoningsvak of een recordpagina kunt wijzigen. Voor informatie over het uitgeven van verslagen, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

U moet recordtypen en records maken voordat u kunt beginnen met het bewerken van recordpagina&#39;s.

Raadpleeg de volgende artikelen voor meer informatie:

* [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)

* [Records maken](/help/quicksilver/planning/records/create-records.md)

## Toegangsvereisten

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
<p>Alle Workfront en alle planningspakketten</p>
<p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <p>Contribute of hoger machtigingen voor een werkruimte en recordtype </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>   
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
<p>Any</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## Overwegingen bij het werken met recordpagina&#39;s

* Standaard worden op de detailpagina van een record alle velden weergegeven die aan de record zijn gekoppeld.

* U kunt geen nieuwe velden toevoegen voor een record in de voorvertoning of op de detailpagina. U moet nieuwe velden toevoegen aan de tabelweergave om deze weer te geven op de pagina&#39;s met voorvertoningen en details.

* U kunt secties toevoegen aan een recordvoorvertoning of detailpagina om de informatie te ordenen op basis van algemene criteria en het gemakkelijker te maken om te zoeken.

* De volgende wijzigingen zijn van invloed op alle records van hetzelfde type en zijn zichtbaar voor alle gebruikers die deze records openen:

   * Velden opnieuw rangschikken
   * Secties toevoegen of verwijderen
   * Gekoppelde recordpagina&#39;s toevoegen of verwijderen

* Wijzigingen die u in de voorvertoning van de record aanbrengt, zijn direct zichtbaar op de pagina met recorddetails. Wijzigingen die u aanbrengt in de recordpagina, worden ook weergegeven in het voorvertoningsvak van de record.

* Het toevoegen van een omslagafbeelding of een miniatuur aan een record maakt geen deel uit van de algemene lay-out van de voorvertoning of pagina van de record. U kunt unieke omslagafbeeldingen of miniaturen aan elke record toevoegen. Voor informatie, zie [&#x200B; een omslagbeeld aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) toevoegen en [&#x200B; voeg een duimnagel aan een verslag &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toe.

* U kunt extra pagina&#39;s van de volgende typen toevoegen aan de pagina van een record:

   * Verbonden recordpagina

     Voor informatie, zie de sectie [&#x200B; een Verbonden verslagenpagina aan een verslag &#x200B;](#add-a-connected-records-page-to-a-record) toevoegen.

## Secties toevoegen aan een recordvoorvertoning of pagina

Houd rekening met het volgende wanneer u secties toevoegt aan een recordpagina:

* Er geldt geen limiet voor het aantal secties dat u op een pagina kunt plaatsen.
* U kunt geen lege sectie hebben. Een sectie moet ten minste één veld bevatten.
* U kunt velden van de ene sectie naar de andere slepen. Voor meer informatie, zie de sectie [&#x200B; gebieden in de verslagvoorproef of detailspagina &#x200B;](#manage-fields-in-the-records-details-tab) in dit artikel leiden.
* Wanneer u alle velden uit een sectie verwijdert, wordt de sectie automatisch verwijderd en kan deze niet worden hersteld.

Een sectie toevoegen aan een recordvoorvertoning of pagina:

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik het **Open pictogram van details** pictogram ![&#x200B; Open detailspictogram op het gebied van de lijstnaam &#x200B;](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   <span class="preview"> de voorproef van het verslag opent in de mening.</span>

   ![&#x200B; doos van Details &#x200B;](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De recordpagina wordt geopend. Het tabblad Details wordt standaard geopend.

   ![&#x200B; pagina van Details &#x200B;](assets/details-page.png)

1. In het **lusje van Details** van de verslagvoorproef of de pagina, houd over de witte ruimte links van de gebieden, dan klik **sectie** pictogram ![&#x200B; toevoegen van sectie &#x200B;](assets/add-section-icon.png) om een sectie toe te voegen.
1. Klik binnen de naam van de sectie en vervang **Naamloze sectie** met een naam, dan klik binnengaan. De velden die onder de sectie worden weergegeven, maken automatisch deel uit van de nieuwe sectie.
1. Begin en dalend gebieden aan de nieuwe sectie te slepen, zoals die in de sectie [&#x200B; wordt beschreven leidt gebieden in de verslagvoorproef of detailspagina &#x200B;](#manage-fields-in-the-records-details-tab) in dit artikel.

1. (Facultatief) Beweeg over de naam van een sectie en klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png).

   ![&#x200B; Meer menuopties voor sectie op verslagpagina &#x200B;](assets/more-menu-options-for-section-on-record-page.png)
1. (Optioneel) Voer een van de volgende handelingen uit om de sectie te bewerken:

   * Klik **anders noemen** om de sectie anders te noemen

     >[!TIP]
     >
     > U kunt de naam van een sectie inline wijzigen door op de naam te klikken.

   * Klik **Beweging omhoog** om de sectie omhoog één positie te bewegen

     of

     Klik **Beweging neer** om de sectie neer één positie te bewegen.
Alle velden in de sectie worden met de sectie verplaatst.

   * Klik **Schrapping** om de sectie te schrappen. De sectie wordt verwijderd en kan niet worden hersteld. Alle gebruikers die tot de verslagen van dit type toegang hebben zullen niet meer de geschrapte sectie bekijken.

1. Klik op de pijl omlaag links van een sectienaam om deze samen te vouwen of op de pijl naar rechts om deze uit te vouwen.
Alle secties worden standaard uitgevouwen.

1. (Facultatief) klik het **greep** pictogram ![&#x200B; pictogram van het Grab &#x200B;](assets/grab-icon.png) aan de linkerzijde van een sectienaam, dan belemmering en laat vallen het in een gewenste plaats.

   De nieuwe positie van de sectie wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in secties en de veldvolgorde worden automatisch opgeslagen.

1. (Facultatief) klik het **menu van de Uitvoer** pictogram van de Uitvoer in verslagdetailpagina ![&#x200B; om het lusje van Details naar een Word of een dossier van PDF uit te voeren. &#x200B;](assets/export-icon-in-record-details-page.png) Voor meer informatie, zie [&#x200B; de details van een verslag uitvoeren &#x200B;](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facultatief) klik het **lusje van Verbindingen** naast **Details** tabel. U zou **Meer** kunnen moeten klikken alvorens de **Verbindingen** tabel te klikken.

   Alle records of objecten die zijn verbonden met de geselecteerde record, worden onder de naam van het recordtype weergegeven, of de toepassing waartoe ze behoren.

   ![&#x200B; het lusje van Verbindingen op verslag in de Planning van Workfront &#x200B;](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Facultatief) selecteer **tonen alle verslagen** die in de hoger-juiste hoek van het lusje van Verbindingen plaatsen. Alle verbonden verslagtypes tonen, met inbegrip van degenen die nog geen verbonden verslagen hebben. De schakeloptie is standaard uitgeschakeld en recordtypen zonder verbonden records worden verborgen.

1. (Facultatief) klik **verbinden** om meer verslagen aan de verbonden verslagtypes toe te voegen. Voor meer informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. (Optioneel) Houd de muisaanwijzer boven een opnamekaart en klik op het pictogram voor het verbreken van de verbinding **-** en klik vervolgens op **Verbinding verbreken** . <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ook verwijderd.

## Velden beheren op het tabblad Details van de record

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik het **Open pictogram van details** pictogram ![&#x200B; Open detailspictogram op het gebied van de lijstnaam &#x200B;](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   <span class="preview"> de voorproef van het verslag opent in de mening.</span>

   ![&#x200B; doos van Details &#x200B;](assets/details-box.png)

1. <span class="preview"> (Optioneel en voorwaardelijk) Afhankelijk van de velden die u wilt weergeven op de pagina Details voert u een van de volgende handelingen uit: </span>

   <div class="preview">

   * Selecteer **tonen alle gebieden** het plaatsen om alle gebieden van de de lijstmening van het verslag, met inbegrip van de verborgen degenen te bekijken.
   * Deselecteer **tonen alle gebieden** plaatsen om slechts gebieden te bekijken die niet verborgen in de de lijstmening van het verslag zijn. Dit is de standaardinstelling

   </div>

   >[!TIP]
   >
   ><span class="preview"> **toon alle gebieden** het plaatsen is beschikbaar slechts in de de voorproefdoos van Details van het verslag. Het is niet beschikbaar in de pagina van de Details van het verslag.</span>


   <!--replace with this when they fix the UI text:
   * Select the **Show all fields** setting to include all the record's fields in the **Details** page. This is the default setting. 
   * Deselect the **Show all fields** setting to exclude the record's fields that are hidden in the table view of the record from the **Details** page.
   -->

   </div>

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![&#x200B; Open detailsdoos in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De verslag **Details** pagina opent in een nieuw lusje.

   ![&#x200B; pagina van Details &#x200B;](assets/details-page.png)

1. In het verslag **Details** lusje, klik het **greep** pictogram ![&#x200B; pictogram van het Grab &#x200B;](assets/grab-icon.png) aan de linkerzijde van een gebiedsnaam, dan belemmering en laat vallen het op een gewenste plaats.

   >[!TIP]
   >
   >U kunt velden naar een andere sectie slepen.
   >Een sectie moet ten minste één veld bevatten.
   >

   De nieuwe positie van het veld wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in de lay-out van de recordvoorvertoning of pagina worden automatisch opgeslagen.

## Een verbonden recordpagina toevoegen aan een record

U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan het de detailsgebied van een verslag toe te voegen. Hiermee voegt u de verbonden records in een tabel- of lijstweergave toe aan het tabblad.

Voor meer informatie, zie [&#x200B; een Verbonden verslagenpagina aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) toevoegen.

<!--this content has been moved to the page linked above
Consider the following when adding a Connected records page to a record: 

* You can add a Connected records page to a record after you connected record or object types to the record type from the table view of a record type.

* You can add a Connected records page from a record's preview area or the record's page.

* Connected records pages display only the connected objects or records from one object or record type in a table view. The page does not display all records of that type. 

* You can add Connected records pages for the following connected record or object types:

   * Workfront Planning record types
   * Workfront projects, programs, portfolios, groups, or companies. You can view the connected Workfront objects even when you do not have permissions to access them in Workfront. 

To add a Connected records page:

1. Click the name of the record to open it from any view of a record type page. 
1. Click **Add page** from one of the following areas: 

   * The record's preview window
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

   The **Create page** box opens.

   ![Add Connected records page modal](assets/add-connection-view-page-modal.png) 

1. Add the **Page name**, click **Connected records page**, then click **Create**.

   A new connected records page is added as a new tab to the record's page.
   
   The records that are connected to the current record display in the table view.  

      >[!TIP]
      >
      >You must add connected records in the table or Details area of a record before you can display them in a connected records page.

   (^^^^^^All fields of the connected record display in the table view of the connected record's tab.^^^^^^^^)
   
   The first five fields of the connected records display by default. (^^^^No lookup fields display by default.^^^^^^^)

   ![Audience connected table view under campaign details](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) Search for or click the name of a connected record or object type in the list.

1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Planning records or any Workfront objects except for projects: 

   * Click the name of a record. This opens the record's page in a new tab. 

   * Click **Connect** at the bottom of the table view to connect more records, then click outside the connection box to close it. The new records are automatically added to the table. 

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
   * Edit any information from the connected records inline in the table view. 

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)
   
      Or 
      
      Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
      * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
      * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
      * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.

   * Inline edit any of the Planning records in the table on the Connected records page. 
   
      All other Workfront objects display in a read-only table view and you cannot edit them. 
   
1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Workfront projects:

     * Click **Connect records** in the upper-right corner of the connected record page to connect existing projects.

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
     * Inline edit project information in the table.
     * Click **New row** to create a project without a template. The new project is connected to the current record immediately.

         For more information, see [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
     * Hover over a project and click the **More** menu [More menu](assets/more-menu.png)
     
         Or

         Select one or more projects, and notice the blue bar at the bottom of the list, then click one of the following:
         
         * **Delete** to delete the project. Deleting a project disconnects it from the record and moves it to the Workfront's Recycle Bin. 
         * **Disconnect** to disconnect the project from the record. Disconnecting a project removes it and all the values of its lookup fields from the current record.
      
1. (Optional) Double-click the name of the **Connected records page** tab

   Or

   Hover over the name of the tab, then click **More** ![More menu](assets/more-menu.png), then click **Rename** to rename to new Connected view tab.
1. (Optional) Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * Filters
   * Sort
   * Grouping
   * Fields, to display, hide, or rearrange fields
   * Row height
   * Search

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   
1. (Optional)  Hover over the name of the Connected records page tab, click **More** ![More menu](assets/more-menu.png), then click **Delete** to remove to tab.-->


<!--
## Add a Brief page to a record

(^^^^^^^^^^move this content to its own article, like you did above - leave the header here with a link^^^^^^^^^^^^)

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



