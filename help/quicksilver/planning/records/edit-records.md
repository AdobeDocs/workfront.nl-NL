---
title: Records bewerken
description: U kunt recordgegevens bewerken in Adobe Workfront Planning. U moet recordtypen maken voordat u records kunt maken en bewerken.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '2764'
ht-degree: 0%

---


# Records bewerken

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt recordgegevens bewerken in Adobe Workfront Planning door de waarden te bewerken van de velden die aan de records zijn gekoppeld.

U moet recordtypen maken voordat u records kunt maken en bewerken.

Voor informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

Voor informatie over het creëren van verslagen, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.

&lt;!— vermeld hier dat de velden in de weergave Details hetzelfde zijn als die in de tabelweergave — dit artikel is gekoppeld vanuit de recordweergave Beheren om naar deze informatie te verwijzen.—>

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

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
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
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
   <td> <p>Standard</p> 
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
   <td>  <p>Contribute of hoger machtigingen voor een werkruimte en recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>

</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Overwegingen bij het bewerken van records

* U kunt records bewerken die u hebt gemaakt of records die door anderen zijn gemaakt, als u machtigingen hebt gekregen voor de werkruimte.
* U kunt recordvelden uit de volgende gebieden bewerken:

   * De voorvertoning van de record in een recordweergave
   * De detailpagina van de record
   * Inline, in een lijstmening.
   * <span class="preview"> De kalender en tijdlijnweergave wanneer u de grootte van de records wijzigt in <!--or dragging and dropping--> . Hiermee werkt u de datums van de records bij.</span>

* Wanneer een gebruiker een record bewerkt in een weergave, zijn de wijzigingen direct zichtbaar in alle weergaven en zijn de recordpagina&#39;s voor alle andere gebruikers.

* De volgende typen velden worden automatisch bijgewerkt en u kunt de waarden ervan niet handmatig bewerken:
   * Gekoppelde velden uit andere records
   * Formuliervelden
   * Systeemvelden (Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum van laatste wijziging)
* Als de records die u weergeeft, aan andere records zijn gekoppeld, heeft de nieuwe informatie over de records die u bewerkt, betrekking op de gekoppelde records.
* U kunt records niet bulksgewijs bewerken. <!--this will probably change-->
* URL&#39;s worden alleen herkend als koppelingen in tekstveldtypen voor één regel wanneer ze beginnen met: http://, https://, ftp:// of www. .
* U kunt een omslagafbeelding aan elke record toevoegen. De afbeelding is uniek voor elke record en is niet van toepassing op alle records van hetzelfde moment.
* U kunt de volgorde van de velden op een recordpagina bewerken en een omslagafbeelding voor een record toevoegen. Voor meer informatie, zie [&#x200B; de lay-out van de verslagpagina beheren &#x200B;](/help/quicksilver/planning/records/manage-the-record-page.md).

## Records bewerken

U kunt een record uit de volgende gebieden bewerken:

* [De tabelweergave](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [De tijdlijnweergave](#edit-a-record-in-the-timeline-view-of-a-record-type)
* [De kalenderweergave](#edit-a-record-in-the-calendar-view-of-a-record-type)
* [De voorvertoning van de record in een weergave](#edit-a-record-from-the-records-preview-in-a-view)
* [De recordpagina](#edit-a-record-from-the-records-page)
* [Een Workfront-object in het gedeelte Planning](#edit-a-record-from-a-workfront-object-in-the-planning-section)

Ga als volgt te werk om de datums van de records te bewerken:

* [ vergroot of vergroot de bars van de verslagen in de chronologie en kalendermening ]

### Een record inline bewerken in de tabelweergave van een recordtype

Wanneer u records uit de tabelweergave bewerkt, ziet u welk veld wordt bewerkt door andere gebruikers op het moment dat u de record weergeeft.

Voor meer informatie, zie [&#x200B; verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md) leiden.

Wanneer u een nieuwe record toevoegt na de laatste record in een groep of subgroep, werkt Workfront automatisch de velden bij die zijn opgenomen in de groepen voor de nieuwe records. U kunt deze velden desgewenst handmatig bewerken en de records uit de groep verwijderen.

Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt bewerken

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) klik het lusje van een lijstmening of klik **+ Mening** om een lijstmening tot stand te brengen. De tabelweergave moet de standaardweergave zijn, tenzij u het recordtype in een ander type weergave hebt bekeken toen u het voor het laatst opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik in de rij van een record om informatie over de record inline te bewerken.

   ![&#x200B; geef verslagparagraafgebied met het formatteren van lijstmening &#x200B;](assets/edit-record-paragraph-field-with-formatting-table-view.png) uit

   >[!TIP]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. Voor meer informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op datum, Laatst gewijzigd door, Datum Laatst gewijzigd, Formule.

1. (Facultatief en voorwaardelijk) wanneer u een alinea-type gebied uitgeeft, gebruik de volgende **het formatteren opties van de Tekst 0&rbrace; Rich &lbrace;:**

   * Vet
   * Cursief
   * Onderstrepen
   * Een koppeling toevoegen
   * Een lijst met opsommingstekens toevoegen
   * Een genummerde lijst toevoegen

   ![&#x200B; rijke teksttoolbar op paragraafgebied &#x200B;](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Optioneel) Dubbelklik op een verbonden recordveld om gekoppelde records of objecten aan een andere record toe te voegen. Voor meer informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).
1. De pers **gaat** op uw toetsenbord binnen of klikt buiten een rij om uw veranderingen te bewaren. De wijzigingen worden automatisch opgeslagen. A **de Bewaarde** indicatorvertoningen kort in de hoger-juiste hoek van de lijstmening om te tonen dat de veranderingen werden bewaard.


1. (Optioneel) Voer een van de volgende handelingen uit om gegevens van het ene veld naar het andere te kopiëren en te plakken:

   * Kopieer een of meerdere bestaande waarden van een veld en plak deze in een veld van hetzelfde type in een andere record
   * Klik op de kolomkop van een kolom om deze te selecteren en te kopiëren, klik vervolgens op de kolomkop van een andere kolom en plak de inhoud van de gekopieerde kolom. De kolommen moeten gelijkaardige gebiedstypes bevatten.
   * Houd Shift ingedrukt en klik om meerdere rijen in een tabel te selecteren, kopieer de gegevens in de geselecteerde rijen en klik vervolgens op een andere rij en plak de geselecteerde gegevens in de nieuwe rij en de volgende rijen erna.
   * Kopieer de informatie uit één cel en selecteer vervolgens meerdere cellen en plak dezelfde informatie in meerdere cellen. U kunt meerdere cellen selecteren en dezelfde gegevens in meerdere cellen van aangrenzende rijen en kolommen plakken.
   * Selecteer de rechterbenedenhoek van een bestaande cel die de informatie bevat die u wilt kopiëren, en sleep deze vervolgens over de aangrenzende cellen waar u dezelfde informatie wilt plakken. Alle cellen moeten hetzelfde type informatie bevatten.

     ![&#x200B; Dragable laag-juiste hoek voor exemplaardeeg in lijstmening &#x200B;](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)


   * Kopieer een of meerdere cellen van een externe bron (bijvoorbeeld een Excel-bestand) en plak ze in een van de volgende veldtypen:

      * Workfront Planning connection fields.
      * Personenvelden. Alleen velden met één waarde worden ondersteund.

     U kunt geen informatie van een externe bron kopiëren en deze in andere veldtypen plakken, zoals Workfront- of AEM Assets-verbindingsvelden.

   >[!NOTE]
   >
   >Overweeg het volgende:
   >
   >* Gebruik de volgende sneltoetsen voor het kopiëren en plakken van gegevens:
   >   * Kopiëren: CTRL + C (⌘ + C voor Mac)
   >   * Plakken: CTRL + V (⌘ + V voor Mac)
   >
   >* U kunt geen veldwaarden kopiëren en plakken op de recordpagina. Deze functionaliteit wordt alleen ondersteund in de tabelweergave van een recordtype.
   >* U kunt geen veldwaarden kopiëren en plakken voor de volgende veldtypen:
   >
   >    * Velden opzoeken die worden gemaakt bij het verbinden van recordtypen. U kunt gekoppelde recordvelden kopiëren en plakken. Voor meer informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Velden van de volgende typen: Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum Laatst gewijzigd

1. (Optioneel) Gebruik de volgende sneltoetsen om het bewerken of kopiëren en plakken van recordgegevens ongedaan te maken of opnieuw uit te voeren:

   * CTRL + Z (⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z (⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren

   >[!TIP]
   >
   >    U kunt de sneltoetsen meerdere malen achter elkaar gebruiken om meerdere wijzigingen ongedaan te maken.

1. (Optioneel) Voeg een miniatuur toe aan een record. Voor informatie, zie [&#x200B; een duimnagel aan een verslag &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toevoegen.


### Een record bewerken in de tijdlijnweergave van een recordtype

<!--add another step about drag and drop here when that is available-->

1. Open de pagina met recordtypen in een tijdlijnweergave. Voor informatie, zie [&#x200B; de chronologiemening &#x200B;](/help/quicksilver/planning/views/manage-the-timeline-view.md) leiden.

1. <span class="preview"> Beweeg over de einden van de bar van een verslag, klik, sleep en laat vallen zijn marge aan een andere datum. Hiermee werkt u automatisch de begin- of einddatum van de record bij.</span>

   <span class="preview">![&#x200B; Linker-eind bar op chronologiemening resize &#x200B;](assets/left-end-bar-handle-to-resize-timeline-view.png)</span>

1. <span class="preview"> klik en houd een verslagbar, dan belemmering en laat vallen het in een andere positie om zijn chronologie en data bij te werken. De begin- en einddatum van de record worden automatisch bijgewerkt.</span>

1. Klik op de balk van een record om het detailgebied te openen en alle velden te bewerken.

   Voor informatie, zie [&#x200B; een verslag van de voorproef van het verslag in een mening &#x200B;](#edit-a-record-from-the-records-preview-in-a-view) sectie in dit artikel uitgeven.

### Een record bewerken in de kalenderweergave van een recordtype

<!--add another step about drag and drop here when that is available-->

1. Open de pagina met recordtypen in een kalenderweergave. Voor informatie, zie [&#x200B; de kalendermening &#x200B;](/help/quicksilver/planning/views/manage-the-calendar-view.md) leiden.
1. <span class="preview"> (Voorwaardelijk) Houd de muisaanwijzer boven de uiteinden van de balk met records in de kalenderweergave en klik, sleep de marges naar een andere datum. Hiermee werkt u automatisch de begin- of einddatum van de record bij.</span>

   <span class="preview">![&#x200B; Linker-eind bar op kalendermening resize &#x200B;](assets/left-end-bar-handle-to-resize-calendar-monthly-view.png)</span>

1. <span class="preview"> klik en houd een verslagbar, dan belemmering en laat vallen het in een andere positie om zijn chronologie en data bij te werken. De begin- en einddatum van de record worden automatisch bijgewerkt.</span>

1. Klik op de balk van een record om het detailgebied te openen en alle velden te bewerken.

   Voor informatie, zie [&#x200B; een verslag van de voorproef van het verslag in een mening &#x200B;](#edit-a-record-from-the-records-preview-in-a-view) sectie in dit artikel uitgeven.

### Een record uit de voorvertoning van de record bewerken in een weergave

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt bewerken

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de record

   of

   Van de lijstmening, klik het **Open pictogram van details** pictogram ![&#x200B; Open detailspictogram op het gebied van de lijstnaam &#x200B;](assets/open-details-icon-in-table-name-field.png) in de eerste kolom. De voorvertoning van de record wordt in de weergave geopend.

   ![&#x200B; doos van Details &#x200B;](assets/details-box.png)

1. (Facultatief) klik het **Meer** menu rechts van de titel van het verslag, dan klik **anders noemen**. Hiermee werkt u het veld bij dat wordt weergegeven als de titel van de record.

   De titel van de record is het primaire veld van de record bij weergave in een tabelweergave. Voor informatie, zie [&#x200B; Primair gebiedsoverzicht &#x200B;](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Bewerk de veldinformatie in de voorvertoning van de record.

   >[!TIP]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Velden opzoeken van andere records die zijn gemaakt door de recordtypen aan te sluiten. Voor meer informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op datum, Laatst gewijzigd door, Datum Laatst gewijzigd, Formule.

1. (Facultatief) klik **omslag** toevoegen om een omslagbeeld aan het verslag toe te voegen. Voor meer informatie, zie [&#x200B; een omslagbeeld aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) toevoegen.

1. (Facultatief) Beweeg over het duimnagelpictogram, dan klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) > **geef duimnagel** uit om een duimnagelbeeld toe te voegen. Voor informatie, zie [&#x200B; een duimnagel aan een verslag &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toevoegen.

   Workfront slaat uw wijzigingen automatisch op.

1. (Facultatief) klik de **indicator in real time** ![&#x200B; in real time indicatorpictogram &#x200B;](assets/real-time-indicator-icon.png) in de hoger-juiste hoek van de de voorproefdoos van het verslag, dan laat **Medewerkers** het plaatsen toe om de gebieden te benadrukken die door anderen in real time worden uitgegeven.

   De namen en avatars van alle gebruikers die tot het verslag tezelfdertijd toegang hebben tonen in dit gebied.

   Als de instelling is uitgeschakeld, worden de avatars en namen weergegeven in het gebied van de tijdindicator in real time en worden de velden die worden bewerkt niet gemarkeerd.

   ![&#x200B; re-time indicator uitgevouwen verslagvoorproefdoos &#x200B;](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Facultatief) klik het **menu van de Uitvoer** pictogram van de Uitvoer in verslagdetailpagina ![&#x200B; om de details van het verslag uit te voeren. &#x200B;](assets/export-icon-in-record-details-page.png) Voor informatie, zie [&#x200B; de details van een verslag &#x200B;](/help/quicksilver/planning/records/export-the-record-page.md) uitvoeren.

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de voorproef van het verslag om de pagina van het verslag in een nieuw lusje te openen. Ga verder het uitgeven van het verslag zoals die in [&#x200B; wordt beschreven geef een verslag van de pagina van het verslag &#x200B;](#edit-a-record-from-the-records-page) sectie in dit artikel uit.

### Een record op de recordpagina bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt bewerken

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Voer een van de volgende handelingen uit:

   * Van om het even welke mening, toegang tot de voorproef van het verslag, zoals die in [&#x200B; wordt beschreven geef een verslag van de voorproef van het verslag in een mening &#x200B;](#edit-a-record-from-the-records-preview-in-a-view) sectie in dit artikel uit, dan klik **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   * Van de **mening van de Lijst**, houd over de naam van een verslag, dan klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **Mening**

     ![&#x200B; Contextueel menu voor verslagrij &#x200B;](assets/contextual-menu-for-record-row.png)

     De recordpagina wordt geopend.

     ![&#x200B; pagina van Details &#x200B;](assets/details-page.png)

1. (Facultatief) klik het **Meer** menu rechts van de titel van het verslag, dan klik **anders noemen**. Hiermee werkt u het veld bij dat wordt weergegeven als de titel van de record.

   De titel van de record is het primaire veld van de record bij weergave in een tabelweergave. Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

1. Klik op een bewerkbaar veld op de recordpagina om deze te bewerken.

   >[!TIP]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. Voor meer informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op datum, Laatst gewijzigd door, Datum Laatst gewijzigd, Formule.

1. (Optioneel) Klik op het informatiepictogram rechts van een veld dat de beschrijving van een veld weergeeft.
1. (Facultatief) klik **omslag** toevoegen om een omslagbeeld aan het verslag toe te voegen

   of

   Beweeg over het bestaande omslagbeeld, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) > **uploadt** om een nieuw omslagbeeld voor het verslag toe te voegen.

   Voor meer informatie, zie [&#x200B; een omslagbeeld aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) toevoegen.

1. (Facultatief) Beweeg over een bestaande duimnagel, of het **duimnagelpictogram** ![&#x200B; pictogram van het Verslag op detailspagina &#x200B;](assets/record-thumbnail-icon-on-details-page.png), dan klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) > **geeft duimnagel** uit om een duimnagel voor het verslag toe te voegen.

   Voor meer informatie, zie [&#x200B; een duimnagel aan een verslag &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toevoegen.

   Workfront slaat uw wijzigingen automatisch op.

1. (Facultatief) klik de **indicator in real time** ![&#x200B; in real time indicatorpictogram &#x200B;](assets/real-time-indicator-icon.png) in de hoger-juiste hoek van de pagina van het verslag, dan laat **samenwerkers** toe plaatsen tonen om de gebieden te benadrukken die door anderen in real time worden uitgegeven.

   De namen en avatars van alle gebruikers die tot het verslag tezelfdertijd toegang hebben tonen in dit gebied.

   Als de instelling is uitgeschakeld, worden de avatars en namen weergegeven in het gebied van de tijdindicator in real time en worden de velden die worden bewerkt niet gemarkeerd.

   ![&#x200B; Echte - tijdindicator uitgebreide doos van de verslagvoorproef &#x200B;](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Facultatief) klik het **menu van de Uitvoer** pictogram van de Uitvoer in verslagdetailpagina ![&#x200B; om de details van het verslag uit te voeren. &#x200B;](assets/export-icon-in-record-details-page.png) Voor informatie, zie [&#x200B; de details van een verslag &#x200B;](/help/quicksilver/planning/records/export-the-record-page.md) uitvoeren.


## Een record uit een Workfront-object bewerken in de sectie Planning

Nadat u records met Workfront-objecten hebt verbonden, kunt u Workfront Planning-records in Workfront bewerken vanuit de sectie Planning van het object.

Voor meer informatie, zie [&#x200B; recordverbindingen van de voorwerpen van Workfront beheren &#x200B;](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

<div class="preview">

## Veldinstellingen voor één of meerdere selecties bewerken bij het bijwerken van de waarden

<!--some of this information is also available in Edit fields article - update both when necessary-->

Als u informatie in een veld met één of meerdere selecties bijwerkt, kunt u nieuwe opties aan het veld toevoegen zonder dat u het veld hoeft te bewerken.

>[!IMPORTANT]
>
>De in deze sectie beschreven functionaliteit is alleen beschikbaar in de tabelweergave. Deze optie is niet beschikbaar in andere gebieden waar enkelvoudige of meervoudige velden worden weergegeven.

**VOORBEELD**

U hebt mogelijk een veld met de naam Status dat één keuze bevat en de opties Nieuw en Gesloten bevat. U wilt dan een keuze toevoegen voor de status In uitvoering. U kunt de keuze toevoegen door een van de volgende handelingen uit te voeren:

* Het veld bewerken. Voor informatie, zie [&#x200B; gebieden &#x200B;](/help/quicksilver/planning/fields/edit-fields.md) uitgeven
* Een nieuwe optie toevoegen tijdens het bewerken van de record in de tabelweergave, zoals hieronder wordt beschreven.

Een nieuwe keuze toevoegen aan een bestaand selectieveld wanneer u een record bewerkt:

1. Ga naar een pagina met recordtypen en open de tabelweergave.
1. Voeg het veld Eén of Meerdere selecties toe waaraan u een keuze wilt toevoegen in de tabelweergave als een nieuwe kolom. Voor informatie, zie [&#x200B; gebieden &#x200B;](/help/quicksilver/planning/fields/create-fields.md) creëren.
1. U kunt het veld inline bewerken door te dubbelklikken op de cel voor het veld.
1. Typ de naam van de keus u wilt toevoegen, dan klik **kiezen** toevoegen.

   ![&#x200B; voeg keus op enig-uitgezocht gebied in lijstmening toe &#x200B;](assets/add-choice-in-table-view-for-single-select-field.png)

   De nieuwe keuze wordt direct toegevoegd aan het veld Eén keuze.

</div>
