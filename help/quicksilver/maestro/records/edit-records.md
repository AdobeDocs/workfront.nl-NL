---
title: Records bewerken
description: U kunt recordgegevens bewerken in Adobe Maestro. U moet recordtypen maken voordat u records kunt maken en bewerken.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Records bewerken

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt recordgegevens bewerken in Adobe Maestro. U moet recordtypen maken voordat u records kunt maken en bewerken.
Zie voor meer informatie [Recordtypen maken](../architecture-and-fields/create-record-types.md).

&lt;!— vermeld hier dat de velden in de weergave Details hetzelfde zijn als die in de tabelweergave — dit artikel is gekoppeld vanuit de recordweergave Beheren om naar deze informatie te verwijzen.—>

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
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
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen bij het bewerken van records

* U kunt records bewerken die u of een andere gebruiker heeft gemaakt. <!--will change with access levels-->
* Als de bewerkte records zijn gekoppeld aan andere records, heeft de nieuwe informatie over de records die u bewerkt, betrekking op de gekoppelde records.
* U kunt records niet bulksgewijs bewerken. <!--this will probably change-->

## Records bewerken

U kunt een record uit de volgende gebieden bewerken:

* [Via de pagina Details van een record](#edit-a-record-from-the-records-details-page)
* [Vanuit de tabelweergave van een recordtype](#edit-a-record-from-the-record-type-table-view)

### Een record bewerken vanaf de pagina Details van de record

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek, of de **Hoofdmenu** ![](assets/main-menu-shell.png) in de linkerbovenhoek, als deze beschikbaar is, klikt u op Maestro.

   De werkruimte die u als laatste opent.
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

   >[!NOTE]
   >
   >    Gekoppelde velden of velden die berekeningen bevatten of door het systeem worden gegenereerd, kunnen niet worden bewerkt.


1. Klikken **Wijzigingen opslaan**. <!--logged a bug for this - this needs to be "Save"-->

### Een record bewerken vanuit de tabelweergave van het recordtype

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De werkruimte die u het laatst hebt geopend.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) Van de **Weergave** Selecteer een tabelweergave in de rechterbovenhoek van de tabel. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik in de rij van een record om informatie over de record inline te bewerken en druk vervolgens op **Enter** op uw toetsenbord om uw wijzigingen op te slaan. De wijzigingen worden automatisch opgeslagen.

   >[!TIP]
   >
   >Gekoppelde velden kunnen niet worden bewerkt. De gegevens voor deze velden worden automatisch ingevuld via de gekoppelde records. Zie voor meer informatie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).



