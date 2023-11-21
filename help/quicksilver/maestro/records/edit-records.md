---
title: Records bewerken
description: U kunt recordgegevens bewerken in Adobe Maestro. U moet recordtypen maken voordat u records kunt maken en bewerken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Records bewerken

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt recordgegevens bewerken in Adobe Maestro. U moet recordtypen maken voordat u records kunt maken en bewerken.
Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

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

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


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
* [Vanuit de tabelweergave van een recordtype](#edit-a-record-from-the-record-type-table-view)

### Een record bewerken vanaf de pagina Details van de record

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek, of de **Hoofdmenu** ![](assets/main-menu-shell.png) in de linkerbovenhoek, als deze beschikbaar is, klikt u op **Maestro**.

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

### Een record bewerken vanuit de tabelweergave van het recordtype

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De werkruimte die u het laatst hebt geopend.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) Van de **Weergave** Selecteer een tabelweergave in de rechterbovenhoek van de tabel. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik in de rij van een record om informatie over de record inline te bewerken.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Druk **Enter** op uw toetsenbord of klik buiten een rij om uw wijzigingen op te slaan. De wijzigingen worden automatisch opgeslagen. Een opgeslagen indicator wordt kort in de rechterbovenhoek van de tabelweergave weergegeven om aan te geven dat de wijzigingen zijn opgeslagen.