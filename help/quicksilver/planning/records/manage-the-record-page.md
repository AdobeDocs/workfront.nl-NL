---
title: De lay-out van de recordpagina beheren
description: U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# De lay-out van de recordpagina beheren

{{planning-important-intro}}

U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.

De recordvoorvertoning is een kleinere weergave van de recordpagina die wordt weergegeven in de weergave van een recordtype.

Wanneer u de indeling van een recordvoorvertoning en pagina wijzigt, hebben de wijzigingen invloed op de voorbeeldvakken en op de detailpagina&#39;s van alle records van hetzelfde type.

In dit artikel wordt beschreven hoe u de lay-out en weergave van een recordvoorvertoningsvak of een recordpagina kunt wijzigen. Voor informatie over het bewerken van records raadpleegt u [Records bewerken](/help/quicksilver/planning/records/edit-records.md).

U moet recordtypen en records maken voordat u kunt beginnen met het bewerken van recordpagina&#39;s.

Raadpleeg de volgende artikelen voor meer informatie:

* [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)

* [Records maken](/help/quicksilver/planning/records/create-records.md)

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
   <p>Nieuw: Licht of hoger</p>
   of
   <p>Huidig: Werk of hoger</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen voor een werkruimte beheren of hoger</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="/help/quicksilver/planning/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het bewerken van recordpagina&#39;s

* Standaard worden in de details en de voorvertoningspagina&#39;s van een record alle velden weergegeven die aan de record zijn gekoppeld.

* U kunt geen nieuwe velden toevoegen voor een record in de voorvertoning of op de detailpagina. U moet nieuwe velden toevoegen aan de tabelweergave om deze weer te geven op de pagina&#39;s met voorvertoningen en details.

* U kunt secties toevoegen aan een recordvoorvertoning of detailpagina om de informatie te ordenen op basis van algemene criteria en het gemakkelijker te maken om te zoeken.

* De volgende wijzigingen zijn van invloed op alle records van hetzelfde type en zijn zichtbaar voor alle gebruikers die deze records openen:

   * Velden opnieuw rangschikken
   * Secties toevoegen of verwijderen

* Wijzigingen die u in de voorvertoning van de record aanbrengt, zijn direct zichtbaar op de pagina met recorddetails. Wijzigingen die u aanbrengt in de recordpagina, worden ook weergegeven in het voorvertoningsvak van de record.

* Het toevoegen van een omslagafbeelding of een miniatuur aan een record maakt geen deel uit van de algemene lay-out van de voorvertoning of pagina van de record. U kunt unieke omslagafbeeldingen of miniaturen aan elke record toevoegen. Zie voor meer informatie [Een omslagafbeelding aan een record toevoegen](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) en [Een miniatuur toevoegen aan een record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Secties toevoegen aan een recordvoorvertoning of pagina

Houd rekening met het volgende wanneer u secties toevoegt aan een recordpagina:

* Er geldt geen limiet voor het aantal secties dat u op een pagina kunt plaatsen.
* U kunt geen lege sectie hebben. Een sectie moet ten minste één veld bevatten.
* U kunt velden van de ene sectie naar de andere slepen. Zie de sectie voor meer informatie [De volgorde van velden in de recordvoorvertoning of op de detailpagina wijzigen](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel.
* Wanneer u alle velden uit een sectie verwijdert, wordt de sectie automatisch verwijderd en kan deze niet worden hersteld.

Een sectie toevoegen aan een recordvoorvertoning of pagina:

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Klik in de tabelweergave op de knop **Details openen** pictogram ![](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![](assets/details-box.png)

1. (Optioneel) Klik op de knop **Openen op nieuw tabblad** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de rechterbovenhoek van de recordvoorvertoning om de pagina van de record op een nieuw tabblad te openen.

   De recordpagina wordt geopend.

   ![](assets/details-page.png)

1. Houd de aanwijzer in de voorvertoning of pagina van de record boven de witruimte links van de velden en klik vervolgens op de knop **Sectie toevoegen** pictogram ![](assets/add-section-icon.png) een sectie toevoegen.
1. Klik binnen de naam van de sectie en vervang **Naamloze sectie** met een naam, en klik dan binnengaan. De velden die onder de sectie worden weergegeven, maken automatisch deel uit van de nieuwe sectie.
1. Velden naar de nieuwe sectie slepen en neerzetten, zoals beschreven in de sectie [De volgorde van velden in de recordvoorvertoning of op de detailpagina wijzigen](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel.

1. (Optioneel) Houd de muisaanwijzer boven de naam van een sectie en klik op de knop **Meer** menu ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Optioneel) Voer een van de volgende handelingen uit om de sectie te bewerken:

   * Klikken **Naam wijzigen** om de naam van de sectie te wijzigen

     >[!TIP]
     >
     > U kunt de naam van een sectie inline wijzigen door op de naam te klikken.

   * Klikken **Omhoog verplaatsen** om de sectie één positie omhoog te verplaatsen

     of

     Klikken **Omlaag verplaatsen** om de sectie één positie omlaag te verplaatsen.
Alle velden in de sectie worden met de sectie verplaatst.

   * Klikken **Verwijderen** om de sectie te verwijderen. De sectie wordt verwijderd en kan niet worden hersteld. Alle gebruikers die tot de verslagen van dit type toegang hebben zullen niet meer de geschrapte sectie bekijken.

1. Klik op de pijl omlaag links van een sectienaam om deze samen te vouwen of op de pijl naar rechts om deze uit te vouwen.
Alle secties worden standaard uitgevouwen.

1. (Optioneel) Klik op de knop **grijpen** pictogram ![](assets/grab-icon.png) links van een sectienaam, en sleep het en zet het op een gewenste plaats neer.

   De nieuwe positie van de sectie wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in secties en de veldvolgorde worden automatisch opgeslagen.

## De volgorde van velden in de recordvoorvertoning of op de detailpagina wijzigen

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Klik in de tabelweergave op de knop **Details openen** pictogram ![](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![](assets/details-box.png)

1. (Optioneel) Klik op de knop **Openen op nieuw tabblad** pictogram ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de rechterbovenhoek van de recordvoorvertoning om de pagina van de record op een nieuw tabblad te openen.

   De recordpagina wordt geopend.

   ![](assets/details-page.png)

1. Klik in de voorvertoning of pagina van de record op de knop **grijpen** pictogram ![](assets/grab-icon.png) links van een veldnaam, en sleep het op een gewenste plaats. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   De nieuwe positie van het veld wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in de lay-out van de recordvoorvertoning of pagina worden automatisch opgeslagen.

