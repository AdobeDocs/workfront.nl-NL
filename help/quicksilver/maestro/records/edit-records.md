---
title: Records bewerken
description: U kunt recordgegevens bewerken in Adobe Workfront Planning. U moet recordtypen maken voordat u records kunt maken en bewerken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Records bewerken

{{planning-important-intro}}

U kunt recordgegevens bewerken in Adobe Workfront Planning door de waarden te bewerken van de velden die aan de records zijn gekoppeld.

U moet recordtypen maken voordat u records kunt maken en bewerken.

Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

Zie voor informatie over het maken van records [Records maken](/help/quicksilver/maestro/records/create-records.md).

&lt;!— vermeld hier dat de velden in de weergave Details hetzelfde zijn als die in de tabelweergave — dit artikel is gekoppeld vanuit de recordweergave Beheren om naar deze informatie te verwijzen.—>

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
   <td> <p>Contribute of hoger machtigingen voor een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het bewerken van records

* U kunt records bewerken die u hebt gemaakt of records die door anderen zijn gemaakt, als u machtigingen hebt gekregen voor de werkruimte.
* U kunt recordvelden uit de volgende gebieden bewerken:

   * De voorvertoning van de record in een recordweergave
   * De recordpagina
   * Inline, in een lijstmening.

* Wanneer een gebruiker een record bewerkt in een weergave, zijn de wijzigingen direct zichtbaar in alle weergaven en zijn de recordpagina&#39;s voor alle andere gebruikers.

* De volgende typen velden worden automatisch bijgewerkt en u kunt de waarden ervan niet handmatig bewerken:
   * Gekoppelde velden uit andere records
   * Formuliervelden
   * Systeemvelden (Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum van laatste wijziging)
* Als de records die u weergeeft, aan andere records zijn gekoppeld, heeft de nieuwe informatie over de records die u bewerkt, betrekking op de gekoppelde records.
* U kunt records niet bulksgewijs bewerken. <!--this will probably change-->
* URL&#39;s worden alleen herkend als koppelingen in tekstveldtypen voor één regel wanneer ze beginnen met: http://, https://, ftp:// of www. .
* U kunt een omslagafbeelding aan elke record toevoegen. De afbeelding is uniek voor elke record en is niet van toepassing op alle records van hetzelfde moment.
* U kunt de volgorde van de velden op een recordpagina bewerken en een omslagafbeelding voor een record toevoegen. Zie voor meer informatie [De recordpagina beheren](/help/quicksilver/maestro/records/manage-the-record-page.md).

## Records bewerken

U kunt een record uit de volgende gebieden bewerken:

* [Vanuit de tabelweergave van een recordtype](#edit-a-record-from-the-table-view-of-a-record-type)
* [Uit de voorvertoning van de record in een weergave](#edit-a-record-from-the-records-box-in-a-view)
* [Van de recordpagina](#edit-a-record-from-the-records-page)

### Een record inline bewerken in de tabelweergave van een recordtype

{#step1-to-maestro}

De werkruimte die u het laatst hebt geopend.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) klik het lusje van een lijstmening of klik **+ Weergave** een tabelweergave maken. De tabelweergave moet de standaardweergave zijn, tenzij u het recordtype in een ander type weergave hebt bekeken toen u het voor het laatst opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik in de rij van een record om informatie over de record inline te bewerken.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op datum, Laatst gewijzigd door, Datum Laatst gewijzigd, Formule.

1. (Optioneel en voorwaardelijk) Als u een veld van het type Alinea bewerkt, gebruikt u het volgende **RTF** opmaakopties:

   * Vet
   * Cursief
   * Onderstrepen
   * Een koppeling toevoegen
   * Een lijst met opsommingstekens toevoegen
   * Een genummerde lijst toevoegen

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Optioneel) Dubbelklik op een verbonden recordveld om gekoppelde records of objecten aan een andere record toe te voegen. Zie voor meer informatie [Connect-records](/help/quicksilver/maestro/records/connect-records.md).
1. Druk **Enter** op uw toetsenbord of klik buiten een rij om uw wijzigingen op te slaan. De wijzigingen worden automatisch opgeslagen. A **Opgeslagen** de indicator wordt kort weergegeven in de rechterbovenhoek van de tabelweergave om aan te geven dat de wijzigingen zijn opgeslagen.


1. (Optioneel) Voer een van de volgende handelingen uit om gegevens van het ene veld naar het andere te kopiëren en te plakken:

   * Kopieer een of meerdere bestaande waarden van een veld en plak deze in een veld van hetzelfde type in een andere record
   * Klik op de kolomkop van een kolom om deze te selecteren en te kopiëren, klik vervolgens op de kolomkop van een andere kolom en plak de inhoud van de gekopieerde kolom. De kolommen moeten gelijkaardige gebiedstypes bevatten.
   * Houd Shift ingedrukt en klik om meerdere rijen in een tabel te selecteren, kopieer de gegevens in de geselecteerde rijen en klik vervolgens op een andere rij en plak de geselecteerde gegevens in de nieuwe rij en de volgende rijen erna.
   * Kopieer de informatie uit één cel en selecteer vervolgens meerdere cellen en plak dezelfde informatie in meerdere cellen. U kunt meerdere cellen selecteren en dezelfde gegevens in meerdere cellen van aangrenzende rijen en kolommen plakken.

   >[!NOTE]
   >
   >Overweeg het volgende:
   >
   >* Gebruik de volgende sneltoetsen voor het kopiëren en plakken van gegevens:
   >   * Kopie: CTRL + C ( ⌘ + C voor Mac)
   >   * Plakken: CTRL + V ( ⌘ + V voor Mac)
   >
   >* U kunt geen veldwaarden kopiëren en plakken op de recordpagina. Deze functionaliteit wordt alleen ondersteund in de tabelweergave van een recordtype.
   >* U kunt geen veldwaarden kopiëren en plakken voor de volgende veldtypen:
   >
   >
   >    * Gekoppelde velden (of opzoekvelden) die worden gemaakt door het verbinden van recordtypen. U kunt gekoppelde recordvelden kopiëren en plakken. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
   >    * Velden van de volgende typen: Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum Laatst gewijzigd

1. (Optioneel) Gebruik de volgende sneltoetsen om het bewerken of kopiëren en plakken van recordgegevens ongedaan te maken of opnieuw uit te voeren:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren

   >[!TIP]
   >
   >    U kunt de sneltoetsen meerdere malen achter elkaar gebruiken om meerdere wijzigingen ongedaan te maken.

1. (Optioneel) Voeg een miniatuur toe aan een record. Zie voor meer informatie [Een miniatuur toevoegen aan een record](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Een record uit de voorvertoning van de record bewerken in een weergave

{{step1-to-maestro}}

De werkruimte die u als laatste opent.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Klik in de tabelweergave op de knop **Details openen** pictogram ![](assets/open-details-icon-in-table-name-field.png) links van een recordnaam. De voorvertoning van de record wordt in de weergave geopend.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >U kunt de **Details openen** pictogram links van het veld Naam van een record alleen in een tabelweergave als het veld Naam een primair veld is.

1. Bewerk de veldinformatie in de voorvertoning van de record.

   >[!TIP]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op datum, Laatst gewijzigd door, Datum Laatst gewijzigd, Formule.

1. (Optioneel) Klik op **omslag toevoegen** om een omslagafbeelding aan de record toe te voegen. Zie voor meer informatie [Een omslagafbeelding aan een record toevoegen](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

   Workfront slaat uw wijzigingen automatisch op.

1. (Optioneel) Klik op de knop **Openen op nieuw tabblad** pictogram ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de rechterbovenhoek van de voorvertoning van de record om de pagina van de record in een nieuw tabblad te openen. Doorgaan met het bewerken van de record zoals beschreven in [Een record op de recordpagina bewerken](#edit-a-record-from-the-records-page) in dit artikel.

### Een record op de recordpagina bewerken

{{step1-to-maestro}}

De werkruimte die u als laatste opent.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Voer een van de volgende handelingen uit:

   * Vanuit een willekeurige weergave toegang tot de voorvertoning van de record, zoals beschreven in het dialoogvenster [Een record uit de voorvertoning van de record bewerken in een weergave](#edit-a-record-from-the-records-preview-in-a-view) in dit artikel en klik vervolgens op de knop **Openen op nieuw tabblad** pictogram ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de rechterbovenhoek van de recordvoorvertoning om de pagina van de record op een nieuw tabblad te openen.

   * Van de **Tabel** weergegeven, plaatst u de muisaanwijzer op de naam van een record en klikt u op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Weergave**

     ![](assets/contextual-menu-for-record-row.png)

     De recordpagina wordt geopend.

     ![](assets/details-page.png)

1. Klik op een bewerkbaar veld op de recordpagina om deze te bewerken.

   >[!TIP]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op datum, Laatst gewijzigd door, Datum Laatst gewijzigd, Formule.

1. (Optioneel) Klik op **omslag toevoegen** om een omslagafbeelding aan de record toe te voegen. Zie voor meer informatie [Een omslagafbeelding aan een record toevoegen](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

   Workfront slaat uw wijzigingen automatisch op.

