---
title: De lay-out van de recordpagina beheren
description: U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# De lay-out van de recordpagina beheren

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
   of
   <p>Huidig: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   Van de mening van de lijstlijst, klik **Open details** pictogram ![](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De recordpagina wordt geopend. <!--The Details tab opens by default. -->

   ![](assets/details-page.png)

1. In de <!--**Details** tab of the--> verslagvoorproef of pagina, houd over de witte ruimte links van de gebieden, dan klik **sectie** pictogram ![](assets/add-section-icon.png) toevoegen om een sectie toe te voegen.
1. Klik binnen de naam van de sectie en vervang **Naamloze sectie** met een naam, dan klik binnengaan. De velden die onder de sectie worden weergegeven, maken automatisch deel uit van de nieuwe sectie.
1. Begin en dalend gebieden aan de nieuwe sectie te slepen, zoals die in de sectie [ wordt beschreven herschik gebieden in de verslagvoorproef of detailspagina ](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel.

1. (Facultatief) Beweeg over de naam van een sectie en klik **Meer** menu ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
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

1. (Facultatief) klik de **greep** pictogram ![](assets/grab-icon.png) links van een sectienaam, dan belemmering en laat vallen het in een gewenste plaats.

   De nieuwe positie van de sectie wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in secties en de veldvolgorde worden automatisch opgeslagen.

<!--1. (Optional) Click the **Connections** tab. All records or objects that are connected to the selected record display under the names of the record type, or the application they belong to. 

      ![](assets/connections-tab-on-record-in-workfront-planning.png)

      For information about connecting records from the Connections tab, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->

## Velden in de voorvertoning of pagina van de record opnieuw rangschikken

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik **Open details** pictogram ![](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De recordpagina wordt geopend.

   ![](assets/details-page.png)

1. In de verslagvoorproef of de pagina, klik **greep** pictogram ![](assets/grab-icon.png) links van een gebiedsnaam, dan belemmering en laat vallen het in een gewenste plaats. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   De nieuwe positie van het veld wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in de lay-out van de recordvoorvertoning of pagina worden automatisch opgeslagen.

