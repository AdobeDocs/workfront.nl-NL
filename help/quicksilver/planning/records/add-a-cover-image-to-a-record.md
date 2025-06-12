---
title: Een omslagafbeelding toevoegen aan een record
description: U kunt records personaliseren door een omslagafbeelding toe te voegen aan de recordpagina in Adobe Workfront Planning, wanneer u een record bewerkt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---


# Een omslagafbeelding aan een record toevoegen

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt records personaliseren door een omslagafbeelding toe te voegen aan de recordpagina in Adobe Workfront Planning, wanneer u een record bewerkt.

Voor informatie over het uitgeven van verslagen, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

U moet recordtypen maken voordat u records kunt maken en bewerken.

Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

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
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningspakket wordt opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
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
   <td>   <p>Contribute of hogere toestemmingen aan een werkruimte <span class="preview"> en verslagtype </span>  </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>In het milieu van de Productie, moeten alle gebruikers met inbegrip van de Beheerders van het Systeem aan een lay-outmalplaatje worden toegewezen dat Planning omvat.</p>
<p><span class="preview">In het milieu van de Voorproef, hebben de Standaardgebruikers en de Beheerders van het Systeem Planning die door gebrek wordt toegelaten.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij omslagafbeeldingen van recordpagina&#39;s

U kunt de pagina van een record personaliseren door er een omslagafbeelding aan toe te voegen.

Overweeg het volgende:

* Een omslagafbeelding is uniek voor één record en is niet van toepassing op alle records van hetzelfde type.
* U kunt alleen afbeeldingsbestanden als omslagafbeeldingen toevoegen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* U kunt een omslagafbeelding aan afzonderlijke records toevoegen vanuit de voorvertoning van de record in een willekeurige weergave of vanaf de recordpagina.
* U kunt geen omslagafbeeldingen uit een recordweergave toevoegen.
* Workfront uploadt automatisch een omslagafbeelding wanneer u een record maakt. U kunt deze afbeelding later wijzigen.

## Een omslagafbeelding aan een record toevoegen

U kunt een record personaliseren door een omslagafbeelding boven aan de voorvertoning of pagina van de record toe te voegen.

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt personaliseren,

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op een record

   of

   Van de mening van de lijstlijst, klik **Open details** pictogram ![ Open detailspictogram ](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![ de voorproefdoos van Details ](assets/details-box.png)


1. (Facultatief) klik **Open in nieuw lusje** pictogram ![ Open in nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De recordpagina wordt geopend.

   ![ pagina van Details ](assets/details-page.png)

1. In de verslagvoorproef of detailspagina, houd over de ruimte boven de verslagnaam, dan klik **omslag** toevoegen.

   of

   Beweeg over een bestaand omslagbeeld, klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **uploaden**. <!--check the casing here; I logged a bug for this-->
De **omslag van het Verslag** doos opent in **uploadt** tabel.

   ![ de omslagdoos van het Verslag voor upload ](assets/record-cover-box-for-upload.png)

1. Klik **doorbladert beelden** en doorblader naar een beeld op uw computer om het te selecteren en toe te voegen.

1. (Facultatief) om het beeld te verwijderen alvorens het wordt bewaard, klik **uploadt nieuw beeld** pictogram ![ uploadt nieuw beeldpictogram ](assets/upload-new-image-icon.png), en uploadt een nieuw beeld.

1. (Facultatief) klik de **Galerij** tabel, dan klik een beeld in de galerij van beelden. De galerie met afbeeldingen kan niet worden gewijzigd.

   ![ omslag van het Verslag doos voor galerij ](assets/record-cover-box-for-gallery.png)

1. Klik **beeld van het Gebruik**.

   De afbeelding wordt boven aan de recordvoorvertoning geüpload of de detailpagina wordt automatisch opgeslagen.

   ![ pagina van het Verslag met omslagbeeld ](assets/record-page-with-cover-image.png)

1. (Facultatief) Beweeg over het beeld, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de laag-juiste hoek van het omslag beeld, dan doe één van het volgende:

   * Klik **uploaden** als u het omslagbeeld wilt vervangen en Stap 6 herhalen om een nieuw beeld te uploaden en te bewaren.
   * Klik **Verplaatsing**, en gebruik het **het hulpmiddelpictogram van de Verplaatsing** van het hulpmiddel ![ ](assets/reposition-tool-icon.png) om het omslagbeeld te centreren, dan klik **sparen** wanneer gedaan.
   * Klik **verwijderen** om het omslagbeeld te verwijderen.

   Workfront slaat uw wijzigingen automatisch op.
