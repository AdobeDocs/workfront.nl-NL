---
title: Records maken
description: Wanneer u de planningsmogelijkheden van Adobe Workfront gebruikt, is een record een instantie van een recordtype. U moet recordtypen maken voordat u afzonderlijke records kunt maken. Het maken van taxonomieverslagen is identiek aan het maken van operationele verslagen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Records maken

{{maestro-important-intro}}

In Adobe Workfront-planningsmogelijkheden is een record een instantie van een recordtype.

U kunt de volgende typen records hebben:

* **Operationele gegevens**: Deze vertegenwoordigen werkgerelateerde objecten. Voor een operationeel record met de naam &#39;Campagne&#39; kunt u bijvoorbeeld records met een naam als &#39;Maandelijkse nieuwsbrief&#39; of &#39;Zomerverkoop&#39; hebben genoemd.
* **Taxonomische gegevens**: Ze vertegenwoordigen kenmerken die aan operationele records kunnen worden gekoppeld. Voor een taxonomie-recordtype met de naam &#39;Kanaal&#39; kunt u bijvoorbeeld taxonomieën als &#39;E-mail&#39;, &#39;Sociale media&#39; of &#39;Advertising&#39; een naam geven.

Het maken van operationele records is hetzelfde als het maken van taxonomierecords.

U kunt records maken door een van de volgende handelingen uit te voeren:

* Deze handmatig maken voor recordtypen
  <!-- not possible anymore: * Connect them to records from other applications-->
* Maak records door gegevens uit een externe lijst te kopiëren en te plakken.

In dit artikel wordt beschreven hoe u records kunt maken. Raadpleeg de volgende artikelen voor informatie over het beheren van records in de tabel- of tijdlijnweergaven:

* [De tabelweergave beheren](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [De tijdlijnweergave beheren](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Records maken door deze handmatig toe te voegen aan een recordtype <!--in a record type table (I don't think you can create them elsewhere right now)-->

U kunt records maken in de tabelweergave van een pagina met recordtypen.

Zie voor informatie over het bewerken van recordgegevens [Records bewerken](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture/create-workspaces.md).
1. Klik op een opnametype. Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture/create-record-types.md).

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.
Alle records van het geselecteerde type worden weergegeven in de tabelweergave.

1. (Voorwaardelijk) Als de pagina met recordtypen niet wordt geopend in de tabelweergave, klikt u op de knop **Weergave** en selecteert u een bestaande **Tabelweergave** ![](assets/table-view-icon.png) of klik op **Weergave maken > Tabel** een tabelweergave maken.

<!--Replace the above with this when we release the tabbed views: 
1. (Conditional) If the record type page does not open in the table view, click the tab of a table view, or click **+ View** to create a table view. -->

1. Klik op **Nieuwe record** in de laatste rij van de tabel

   of

   Klikken **Shift + Enter** op uw toetsenbord vanuit een willekeurige kolom of rij van de tabel. Hiermee voegt u een lege rij toe.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Typ informatie in de nieuwe rij over de nieuwe record.

   >[!NOTE]
   >
   >  * Er zijn geen verplichte velden voor records. Nochtans, adviseren wij dat u een Naam voor het verslag toevoegt aangezien het nuttig is om verslagen te identificeren wanneer het verbinden van verslagen aan elkaar.
   >
   >  * Velden die naar andere recordtypen of berekende velden verwijzen, zijn alleen-lezen velden.

1. Ga door met het toevoegen van informatie over elke rij en klik vervolgens op **Enter** op uw toetsenbord om uw wijzigingen op te slaan.

<!--Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. The **Details** box opens in the table. 

      >[!TIP]
      >
      >    You can access the Details box only from the name field of the record when the Name field is a primary field. 

  1. Start editing the record's information in the Details box. Workfront automatically saves your changes. 
  1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record on the Details page.
    -->

1. (Optioneel) Gebruik de volgende sneltoetsen om nieuwe records ongedaan te maken of opnieuw toe te voegen:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Records maken door gegevens uit een externe lijst te kopiëren en te plakken

1. Beginnen met het maken van records in de tabelweergave, zoals beschreven in de sectie [Records maken door deze handmatig toe te voegen aan een recordtype](#create-records-by-manually-adding-them-to-a-record-type) in dit artikel.

   Zorg ervoor dat de tabelweergave de kolommen (of de velden) bevat die u wilt vullen met de nieuwe recordgegevens.

1. Klikken **Nieuw &lt; Naam recordtype >** in de laatste rij van de tabel om zoveel nieuwe rijen aan de tabel toe te voegen als u wilt dat de nieuwe records worden gemaakt.

   Voeg bijvoorbeeld 10 rijen toe aan de tabelweergave als u de gegevens voor 10 nieuwe records uit een andere toepassing wilt plakken.

1. Maak in een andere toepassing een lijst met records die u wilt importeren.

   U kunt bijvoorbeeld een Excel-werkblad gebruiken om uw lijst te maken.

   De lijst moet informatie in tabelvorm bevatten.

   >[!TIP]
   >
   > De kolommen in de lijst moeten informatie bevatten voor de bestaande velden die u in Workfront hebt.
   >
   > Zorg ervoor dat de gewenste velden al in Workfront zijn gemaakt en dat de gegevens op uw blad in de juiste indeling worden weergegeven die overeenkomt met die van elk veld in Workfront.

1. In een andere toepassing selecteert u meerdere rijen en kolommen en plakt u de gegevens in de tabelweergave van het recordtype, te beginnen met de eerste nieuwe record.

   De volgende informatie wordt geïmporteerd in het gedeelte Workfront-planningsmogelijkheden:

   * De rijen bevatten de nieuwe records
   * De kolommen vullen informatie voor de gebieden van de verslagen.
