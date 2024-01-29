---
title: Miniaturen toevoegen aan records
description: U kunt recordgegevens bewerken in Adobe Maestro en elke record koppelen aan afzonderlijke miniaturen, zodat deze gemakkelijk herkenbaar zijn.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7448f6b8a622bc814604e59d4654644b3d7a1e12
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Miniaturen toevoegen aan records

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt records koppelen aan unieke miniaturen in Adobe Maestro, zodat ze gemakkelijk herkenbaar zijn.

U moet recordtypen maken voordat u records kunt maken en bewerken.
Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

## Toegangsvereisten

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td> <p>Machtigingen voor een werkruimte weergeven of vergroten </p>  
   <p>Machtigingen voor de tabelweergave weergeven of vergroten </p> 
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


## Overwegingen bij het opnemen van miniaturen

Als u visueel onderscheid wilt maken tussen records in een tabelweergave, kunt u een unieke miniatuurafbeelding aan elke record koppelen.

Overweeg het volgende:

* U kunt alleen afbeeldingsbestanden als miniaturen toevoegen.
* U kunt een miniatuurafbeelding toevoegen aan afzonderlijke records in de tabelweergave.
* U kunt geen recordminiaturen toevoegen vanaf de pagina Details van de record of in de tijdlijnweergave.
* De miniatuurafbeelding wordt altijd links van het primaire veld van elke record weergegeven, ongeacht het veldtype.

  Velden met één regel tekst, cijfers of formules kunnen worden aangewezen als primaire velden.
Zie voor meer informatie [De tabelweergave beheren](/help/quicksilver/maestro/views/manage-the-table-view.md).

<!--above: when you know exactly what type of files are allowed, add the exact extensions above-->

## Een miniatuur toevoegen aan een record

{{step1-to-maestro}}

1. Selecteer de werkruimte voor de records waaraan u miniaturen wilt toevoegen en klik op de kaart met recordtype.

   Hierdoor wordt de pagina met recordtypen geopend.
1. Selecteer een tabelweergave in het menu **Weergave** vervolgkeuzelijst. Alle verslagen van het type u selecteerde tonen in een lijst.
1. Klik op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Miniatuur**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Het primaire veld is het veld dat in de eerste kolom van een tabelweergave wordt weergegeven. Het primaire veld is altijd bevroren en kan niet worden verborgen of verplaatst.

   De **Recordminiatuur** wordt geopend.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. In de **Uploaden** slepen en neerzetten van een bestand dat u als miniatuur wilt toevoegen of klikken **Selecteren om te uploaden** Blader vervolgens naar het afbeeldingsbestand dat u wilt toevoegen. Het bestand moet op uw computer worden opgeslagen.
1. (Optioneel) Gebruik het gereedschap Grootte wijzigen om de afbeelding uit te snijden en de grootte ervan te wijzigen.
1. Klikken **Afbeelding gebruiken** om de afbeelding als een miniatuur toe te voegen.
Hiermee sluit u het dialoogvenster **Recordminiatuur** doos.
1. Klik op Velden in de rechterbovenhoek van de tabelweergave.
1. Selecteer de **Miniatuur** schakelen om de miniatuur weer te geven. Deze optie is standaard uitgeschakeld.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   De miniatuur wordt links van de waarde van het primaire veld weergegeven.
1. (Optioneel) Als u de miniatuur wilt verwijderen, plaatst u de cursor boven het primaire veld en klikt u op de knop **Meer** menu ![](assets/more-menu.png)> **Miniatuur** > de **Verwijderen** pictogram ![](assets/remove-image-icon.png)en klik vervolgens op **Wijzigingen opslaan**.
