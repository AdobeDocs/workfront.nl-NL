---
title: Records bewerken
description: U kunt recordgegevens bewerken in de planningsmogelijkheden van Adobe Workfront. U moet recordtypen maken voordat u records kunt maken en bewerken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Records bewerken

{{maestro-important-intro}}

U kunt recordgegevens in Adobe Workfront-planningsmogelijkheden bewerken door de waarden te bewerken van de velden die aan de records zijn gekoppeld.

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
<p>Uw organisatie moet zijn ingeschreven voor het gesloten bètaprogramma voor Adobe Workfront-planningsmogelijkheden. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td> <p>Er zijn geen toegangsbesturingselementen voor Adobe Workfront-planningsmogelijkheden </p>  
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
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het bewerken van records

* U kunt records bewerken die u hebt gemaakt of records die door anderen zijn gemaakt, als u machtigingen hebt gekregen voor de werkruimte.
* U kunt recordvelden bewerken vanaf de pagina Details van een record of vanuit de tabelweergave van een recordtype.
* U kunt recordgegevens uit de tijdlijnweergave niet bewerken.
* De volgende typen velden worden automatisch bijgewerkt en u kunt de waarden ervan niet handmatig bewerken:
   * Gekoppelde velden uit andere records
   * Formuliervelden
   * Systeemvelden (Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum van laatste wijziging)
* Als de records die u weergeeft, aan andere records zijn gekoppeld, heeft de nieuwe informatie over de records die u bewerkt, betrekking op de gekoppelde records.
* U kunt records niet bulksgewijs bewerken. <!--this will probably change-->
* URL&#39;s worden alleen herkend als koppelingen in tekstveldtypen voor één regel wanneer ze beginnen met: http://, https://, ftp:// of www. .

## Records bewerken

U kunt een record uit de volgende gebieden bewerken:

* [Vanuit de tabelweergave van een recordtype](#edit-a-record-from-the-table-view-of-a-record-type)
* [Via de pagina Details van een record](#edit-a-record-from-the-records-details-page)

### Een record bewerken vanuit de tabelweergave van een recordtype

{#step1-to-maestro}

De werkruimte die u het laatst hebt geopend.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) Van de **Weergave** in de linkerbovenhoek van de tabel selecteert u een **Tabel** weergeven. Dit moet de standaardweergave zijn, tenzij u het recordtype in een ander type weergave hebt bekeken toen u het als laatste opende.

<!--replace above with this when we release view redesign: (Conditional) Click the tab of a table view or click **+ View** to create a table view. The table view should be the default view, unless you viewed the record type in another type of view when you accessed it last. -->

    De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik in de rij van een record om informatie over de record inline te bewerken.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!NOTE]
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


   <!--
    1. (Optional) Click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of a record name, or click a record name. The **Details** box opens in the table. 
        >[!TIP]
        >
        >    You can view the Open details icon to the left of the Name field of a record only when the Name field is a primary field. 
    1. Start editing the field information in the Details box. Workfront automatically saves your changes. 
    1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) (*********check the icon; they are changing it***********) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record as described in [Edit a record from the record's Details page](#edit-a-record-from-the-records-details-page) section in this article. 
    -->

1. (Optioneel) Voer een van de volgende handelingen uit om gegevens van het ene veld naar het andere te kopiëren en te plakken:

   * Kopieer een of meerdere bestaande waarden van een veld en plak ze in een veld van hetzelfde type in een andere record
   * Klik op de kolomkop van een kolom om deze te selecteren en te kopiëren, klik vervolgens op de kolomkop van een andere kolom en plak de inhoud van de gekopieerde kolom. De kolommen moeten gelijkaardige gebiedstypes bevatten.
   * Houd Shift ingedrukt en klik om meerdere rijen in een tabel te selecteren, kopieer de gegevens in de geselecteerde rijen en klik vervolgens op een andere rij en plak de geselecteerde gegevens in de nieuwe rij en de volgende rijen erna.

   >[!NOTE]
   >
   >Overweeg het volgende:
   >
   >* Gebruik de volgende sneltoetsen voor het kopiëren en plakken van gegevens:
   >   * Kopie: CTRL + C ( ⌘ + C voor Mac)
   >   * Plakken: CTRL + V ( ⌘ + V voor Mac)
   >* U kunt geen informatie uit een andere bron kopiëren, behalve een recordveld van hetzelfde type als het veld waarin u de informatie plakt.
   >
   >* U kunt geen veldwaarden kopiëren en plakken in het gebied Details van een record. Deze functionaliteit wordt alleen ondersteund in de tabelweergave van een recordtype.
   >* U kunt geen veldwaarden kopiëren en plakken voor de volgende veldtypen:
   >
   >
   >    * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. U kunt gekoppelde recordvelden kopiëren en plakken. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
   >    * Velden van de volgende typen: Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum Laatst gewijzigd

1. (Optioneel) Gebruik de volgende sneltoetsen om het bewerken of kopiëren en plakken van recordgegevens ongedaan te maken of opnieuw uit te voeren:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren

   >[!TIP]
   >
   >    U kunt de sneltoetsen meerdere malen achter elkaar gebruiken om meerdere wijzigingen ongedaan te maken.

1. (Optioneel) Voeg een miniatuur toe aan een record. Zie voor meer informatie [Een miniatuur toevoegen aan een record](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).


### Een record bewerken vanaf de pagina Details van de record

<!--You can edit a record from the Details box in a table view, or from the Details page. For information about editing records in the Details box, see the [Edit a record from the table view of a record type](#edit-a-record-from-the-table-view-of-a-record-type) section in this article.-->

{{step1-to-maestro}}

De werkruimte die u als laatste opent.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.
1. Voer een van de volgende handelingen uit:

   * Van een **Tabel** Klik op de naam van een record.
   * Van de **Tabel** weergegeven, plaatst u de muisaanwijzer op de naam van een record en klikt u op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Weergave**

     ![](assets/contextual-menu-for-record-row.png)
   * Klik in een tijdlijnweergave op een recordbalk.

   De record **Details** pagina wordt geopend.

1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van de record klikt u op **Bewerken**

   of

   Klik in een bewerkbaar veld op de pagina Details om de gegevens te bewerken. <!--Your changes are saved automatically.-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Klikken **Wijzigingen opslaan**. <!--Eliminate this step when we release the new Details box in the table with the Details page. Add above that the saves are automatic-->