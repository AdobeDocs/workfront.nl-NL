---
title: De lay-out van de pagina Opnemen beheren
description: U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: f171db8474df703fddbf63a673f9bfbd2ab2db27
workflow-type: tm+mt
source-wordcount: '2034'
ht-degree: 0%

---


# De lay-out van de recordpagina beheren

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.

De recordvoorvertoning is een kleinere weergave van de recordpagina die wordt weergegeven in de weergave van een recordtype.

Wanneer u de indeling van een recordvoorvertoning en pagina wijzigt, hebben de wijzigingen invloed op de voorbeeldvakken en op de detailpagina&#39;s van alle records van hetzelfde type.

In dit artikel wordt beschreven hoe u de lay-out en weergave van een recordvoorvertoningsvak of een recordpagina kunt wijzigen. Voor informatie over het uitgeven van verslagen, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

U moet recordtypen en records maken voordat u kunt beginnen met het bewerken van recordpagina&#39;s.

Raadpleeg de volgende artikelen voor meer informatie:

* [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)

* [Records maken](/help/quicksilver/planning/records/create-records.md)

## Toegangsvereisten

+++ Breid uit om toegangsvereisten te bekijken..

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
   <p> Producten</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td>
   <td>
<p>Een van de volgende Workfront-plannen:</p>
<ul><li>Selecteren</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td>
   <td>
<p>Alle</p>
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-platform</p></td>
   <td>
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <p>Contribute of hogere toestemmingen aan een werkruimte <span class="preview"> en verslagtype </span> </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Alle gebruikers, met inbegrip van de beheerders van Workfront, moeten een lay-outmalplaatje worden toegewezen dat het Gebied van de Planning in het Belangrijkste Menu en het Gebied van de Planning voor projecten, portefeuilles, en programma's omvat. </p> Voor meer informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> Adobe die toegangsoverzicht van de Planning </a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 

<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Overwegingen bij het bewerken van recordpagina&#39;s

* Standaard worden in de details en de voorvertoningspagina&#39;s van een record alle velden weergegeven die aan de record zijn gekoppeld.

* U kunt geen nieuwe velden toevoegen voor een record in de voorvertoning of op de detailpagina. U moet nieuwe velden toevoegen aan de tabelweergave om deze weer te geven op de pagina&#39;s met voorvertoningen en details.

* U kunt secties toevoegen aan een recordvoorvertoning of detailpagina om de informatie te ordenen op basis van algemene criteria en het gemakkelijker te maken om te zoeken.

* De volgende wijzigingen zijn van invloed op alle records van hetzelfde type en zijn zichtbaar voor alle gebruikers die deze records openen:

   * Velden opnieuw rangschikken
   * Secties toevoegen of verwijderen

* Wijzigingen die u in de voorvertoning van de record aanbrengt, zijn direct zichtbaar op de pagina met recorddetails. Wijzigingen die u aanbrengt in de recordpagina, worden ook weergegeven in het voorvertoningsvak van de record.

* Het toevoegen van een omslagafbeelding of een miniatuur aan een record maakt geen deel uit van de algemene lay-out van de voorvertoning of pagina van de record. U kunt unieke omslagafbeeldingen of miniaturen aan elke record toevoegen. Voor informatie, zie [ een omslagbeeld aan een verslag ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) toevoegen en [ voeg een duimnagel aan een verslag ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toe.

## Secties toevoegen aan een recordvoorvertoning of pagina

Houd rekening met het volgende wanneer u secties toevoegt aan een recordpagina:

* Er geldt geen limiet voor het aantal secties dat u op een pagina kunt plaatsen.
* U kunt geen lege sectie hebben. Een sectie moet ten minste één veld bevatten.
* U kunt velden van de ene sectie naar de andere slepen. Voor meer informatie, zie de sectie [ gebieden in de verslagvoorproef of detailspagina ](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel herschikken.
* Wanneer u alle velden uit een sectie verwijdert, wordt de sectie automatisch verwijderd en kan deze niet worden hersteld.

Een sectie toevoegen aan een recordvoorvertoning of pagina:

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik het **Open pictogram van details** pictogram ![ Open detailspictogram op het gebied van de lijstnaam ](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![ doos van Details ](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![ Open details in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De recordpagina wordt geopend. Het tabblad Details wordt standaard geopend.

   ![ pagina van Details ](assets/details-page.png)

1. In het **lusje van Details** van de verslagvoorproef of de pagina, houd over de witte ruimte links van de gebieden, dan klik **sectie** pictogram ![ toevoegen van sectie ](assets/add-section-icon.png) om een sectie toe te voegen.
1. Klik binnen de naam van de sectie en vervang **Naamloze sectie** met een naam, dan klik binnengaan. De velden die onder de sectie worden weergegeven, maken automatisch deel uit van de nieuwe sectie.
1. Begin en dalend gebieden aan de nieuwe sectie te slepen, zoals die in de sectie [ wordt beschreven herschik gebieden in de verslagvoorproef of detailspagina ](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel.

1. (Facultatief) Beweeg over de naam van een sectie en klik **Meer** menu ![ Meer menu ](assets/more-menu.png).

   ![ Meer menuopties voor sectie op verslagpagina ](assets/more-menu-options-for-section-on-record-page.png)
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

1. (Facultatief) klik het **greep** pictogram ![ pictogram van het Grab ](assets/grab-icon.png) aan de linkerzijde van een sectienaam, dan belemmering en laat vallen het in een gewenste plaats.

   De nieuwe positie van de sectie wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in secties en de veldvolgorde worden automatisch opgeslagen.

1. (Facultatief) klik het **menu van de Uitvoer ![ pictogram van de Uitvoer in verslagdetailpagina ](assets/export-icon-in-record-details-page.png) om het lusje van Details naar een Word of een dossier van PDF uit te voeren.** Voor meer informatie, zie [ de details van een verslag uitvoeren ](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facultatief) klik het **lusje van Verbindingen** naast **Details** tabel. U zou **Meer** kunnen moeten klikken alvorens de **Verbindingen** tabel te klikken.

   Alle records of objecten die zijn verbonden met de geselecteerde record, worden onder de naam van het recordtype weergegeven, of de toepassing waartoe ze behoren.

   ![ het lusje van Verbindingen op verslag in de Planning van Workfront ](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Facultatief) selecteer **tonen alle verslagen** die in de hoger-juiste hoek van het lusje van Verbindingen plaatsen. Alle verbonden verslagtypes tonen, met inbegrip van degenen die nog geen verbonden verslagen hebben. Standaard is de schakeloptie uitgeschakeld en worden recordtypen zonder gekoppelde records verborgen.

1. (Facultatief) klik **verbinden** om meer verslagen aan de verbonden verslagtypes toe te voegen. Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

1. (Optioneel) Houd de muisaanwijzer boven een opnamekaart en klik op het pictogram voor het verbreken van de verbinding **-** en klik vervolgens op **Verbinding verbreken** . <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ook verwijderd.

## Velden opnieuw rangschikken op het tabblad Details van de record

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik het **Open pictogram van details** pictogram ![ Open detailspictogram op het gebied van de lijstnaam ](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![ doos van Details ](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![ Open detailsdoos in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   Het **lusje van Details** van het verslag opent door gebrek.

   ![ pagina van Details ](assets/details-page.png)

1. In het verslag **Details** lusje, klik het **greep** pictogram ![ pictogram van het Grab ](assets/grab-icon.png) aan de linkerzijde van een gebiedsnaam, dan belemmering en laat vallen het op een gewenste plaats.

   >[!TIP]
   >
   >U kunt velden naar een andere sectie slepen.
   >Een sectie moet ten minste één veld bevatten.
   >

   De nieuwe positie van het veld wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in de lay-out van de recordvoorvertoning of pagina worden automatisch opgeslagen.

## Een tabblad van de verbindingsweergave toevoegen aan de pagina van een record

<!--suggested a new name for this type of page: "Connected records page" - check to see if this changed, and update this everywhere in this section-->

U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een type van de meningspagina van de Verbinding aan een verslag toe te voegen. De informatie van de verbonden verslagen toont in een read-only lijstmening.

&lt;!-vervang de laatste zin hierboven door deze bij vrijgave:

In de productieomgeving wordt de informatie van de verbonden records of objecten weergegeven in een tabelweergave met het kenmerk Alleen-lezen.

<Span class="preview"> in het milieu van de Voorproef, kan de informatie van de verbonden verslagen in de lijstmening worden uitgegeven. De informatie van de voorwerpen die van een andere toepassing worden verbonden is niet editable in de lijstmening.</span> —>

Houd rekening met het volgende wanneer u een verbindingsweergave toevoegt aan de pagina van een record:

* U kunt een pagina van de mening van de Verbinding aan de pagina van een verslag toevoegen nadat u verslag of objecten types aan het verslagtype verbond.

* U kunt geen pagina van de mening van de Verbinding aan het voorproefgebied van een verslag toevoegen.

* Op pagina&#39;s in de verbindingsweergave wordt een verbonden recordtype of een verbonden objecttype uit een andere toepassing in een tabelweergave weergegeven.

* Nadat u een pagina van de de meningsmening van de Verbinding aan de pagina van een verslag toevoegt, is het paginatabusje zichtbaar van het voorproefgebied van het verslag. U moet naar de volledige pagina gaan om de lijstmening voor het verbonden verslag te zien. <!--this might have changed? check and take disclaimer out-->

Een pagina van de verbindingsweergave toevoegen:

1. Van een mening van de verslagpagina, klik de naam van een verslag om het te openen, dan klik **Open in nieuw lusje** pictogram ![ Open details in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefpagina.
1. Klik **toevoegen pagina**.

   ![ voeg modaal de pagina van de verbindingsmening ](assets/add-connection-view-page-modal.png) toe
1. Voeg de **naam van de Pagina** toe, klik **mening van de Verbinding**, dan klik **creeer**.

   Er wordt een nieuw tabblad toegevoegd aan de pagina van de record.
1. Zoek of klik op de naam van een verbonden record of objecttype in de lijst.
De tabelweergave van het geselecteerde recordtype wordt weergegeven op de nieuwe pagina en de gekoppelde records worden weergegeven in de tabelweergave.
Alle velden van de verbonden record worden weergegeven in de tabelweergave van het tabblad van de verbonden record.

   De eerste vijf velden van de verbonden recordtabel worden standaard weergegeven. Er worden standaard geen opzoekvelden weergegeven.

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   ![ Publiek verbonden lijstmening onder campagnedetails ](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optioneel) Voer een van de volgende handelingen uit in de tabelweergave van de gekoppelde records:

   * Klik op de naam van een record. Hierdoor wordt de pagina van de record op een nieuw tabblad geopend. <!--<span class="preview">In the Preview environment, this opens the record's preview page.</span>-->
   * Klik **verbinden** om meer verslagen te verbinden, dan klik buiten de verbindingsdoos om het te sluiten. De nieuwe records worden automatisch aan de tabel toegevoegd.
     <!--* <span class="preview">Edit any information from the connected records inside the table view. </span>-->

   <!--<div class="preview">

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following options: 
      * View 
      * Copy link
      * Edit thumbnail
      * Duplicate
      * Insert record above or below
      * Delete 
   * Select one of the records, then click one of the following options in the blue bar at the bottom of the screen: 
      * View
      * Copy link
      * Edit thumbnail
      * Duplicate
      * Delete. Delete is the only option available when you select more than one record. 

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

   </div>-->


1. (Optioneel) Dubbelklik op de naam van het tabblad Verbinding.

   of

   Beweeg over de naam van het lusje, dan klik **Meer** ![ Meer menu ](assets/more-menu.png), dan klik **anders noemen** om aan nieuw Verbonden meningslusje anders te noemen.
1. (Optioneel) Gebruik een van de volgende weergave-elementen op de werkbalk om de tabelweergave te beheren:

   * Filters
   * Sorteren
   * Groepering
   * Velden om velden weer te geven, te verbergen of opnieuw te rangschikken

   Voor informatie, zie [ de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

   >[!NOTE]
   >
   >   U kunt geen velden maken, bewerken of verwijderen in de tabelweergave van het tabblad van een verbonden record.
   >

1. Klik **verbinden** om verslagen toe te voegen of te verwijderen. Voor informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md)
1. (Facultatief) Beweeg over de naam van het lusje van de mening van de Verbinding, klik **Meer** ![ Meer menu ](assets/more-menu.png), dan klik **Schrapping** om aan tabel te verwijderen.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



