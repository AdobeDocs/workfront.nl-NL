---
title: Records bewerken
description: U kunt recordgegevens bewerken in Adobe Maestro. U moet recordtypen maken voordat u records kunt maken en bewerken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 83b4aa974fe0d9ba2ace797b52198b15fc55f5d8
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Records bewerken

{{maestro-important-intro}}

U kunt recordgegevens bewerken in Adobe Maestro. U moet recordtypen maken voordat u records kunt maken en bewerken.
Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

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
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td> <p>Er zijn geen toegangscontroles voor Maestro </p>  
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

## Overwegingen bij het bewerken van records

* U kunt records bewerken die u of een andere gebruiker heeft gemaakt. <!--will change with access levels-->
* U kunt geen velden bewerken die zijn gekoppeld vanuit andere records of velden die berekeningen bevatten.
* Als de records die u weergeeft, aan andere records zijn gekoppeld, heeft de nieuwe informatie over de records die u bewerkt, betrekking op de gekoppelde records.
* U kunt records niet bulksgewijs bewerken. <!--this will probably change-->
* URL&#39;s worden alleen herkend als koppelingen in tekstveldtypen voor één regel wanneer ze beginnen met: http://, https://, ftp:// of www. .
* U kunt de volgende opmaakopties voor RTF-tekst gebruiken bij het bewerken van een veld voor alineatekst:

   * Vet
   * Cursief
   * Onderstrepen
   * Een koppeling toevoegen
   * Een lijst met opsommingstekens toevoegen
   * Een genummerde lijst toevoegen

## Records bewerken

U kunt een record uit de volgende gebieden bewerken:

* [Via de pagina Details van een record](#edit-a-record-from-the-records-details-page)
* [Vanuit de tabelweergave van een recordtype](#edit-a-record-from-the-table-view-of-a-record-type)

### Een record bewerken vanaf de pagina Details van de record

{{step1-to-maestro}}

De werkruimte die u als laatste opent.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.
1. Voer een van de volgende handelingen uit:

   * Klik in een tabelweergave op de naam van een record.
   * Houd de muisaanwijzer in de tabelweergave boven de naam van een record en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Weergave**

     ![](assets/contextual-menu-for-record-row.png)
   * Klik in een tijdlijnweergave op een recordbalk.

   De record **Details** pagina wordt geopend.

1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van de record klikt u op **Bewerken**

   of

   Klik in een bewerkbaar veld op de pagina Details om de gegevens te bewerken.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Klikken **Wijzigingen opslaan**. <!--logged a bug for this - this needs to be "Save"-->

### Een record bewerken vanuit de tabelweergave van een recordtype

{#step1-to-maestro}

De werkruimte die u het laatst hebt geopend.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) Van de **Weergave** in de rechterbovenhoek van de tabel selecteert u een **Tabel** weergeven. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik in de rij van een record om informatie over de record inline te bewerken.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Druk **Enter** op uw toetsenbord of klik buiten een rij om uw wijzigingen op te slaan. De wijzigingen worden automatisch opgeslagen. Een opgeslagen indicator wordt kort in de rechterbovenhoek van de tabelweergave weergegeven om aan te geven dat de wijzigingen zijn opgeslagen.

   >[!NOTE]
   >
   >  U kunt de gegevens voor de volgende velden niet bewerken, omdat het alleen-lezen is en Workfront deze automatisch bijwerkt:
   >  
   >  * Gekoppelde velden die worden gemaakt door het verbinden van recordtypen. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
   >  * Velden van de volgende typen: Gemaakt door, Gemaakt op, Laatst gewijzigd door, Datum Laatst gewijzigd


1. (Optioneel) Kopieer een of meerdere bestaande waarden van een veld en plak deze in een veld van hetzelfde type in een andere record. Klik vervolgens op **Enter** op uw toetsenbord om uw wijzigingen op te slaan.

   >[!NOTE]
   >
   >Overweeg het volgende:
   >
   >* U kunt geen informatie kopiëren van een andere bron, behalve een Maestro-veld van hetzelfde type als het veld waarin u de informatie plakt.
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
1. (Optioneel) Voeg een miniatuur toe aan een record. Zie voor meer informatie [Een miniatuur toevoegen aan een record](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).
