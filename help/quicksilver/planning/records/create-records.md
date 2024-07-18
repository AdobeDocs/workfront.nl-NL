---
title: Records maken
description: Wanneer u Adobe Workfront Planning gebruikt, is een record een instantie van een recordtype.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Records maken

{{planning-important-intro}}

In de Planning van Adobe Workfront, is een verslag een geval van een verslagtype.

U kunt records maken door een van de volgende handelingen uit te voeren:

* Deze handmatig maken voor recordtypen
* Maak records door gegevens uit een externe lijst te kopiëren en te plakken.

In dit artikel wordt beschreven hoe u records kunt maken. Raadpleeg de volgende artikelen voor informatie over het beheren van records in de tabel- of tijdlijnweergaven:

* [De tabelweergave beheren](/help/quicksilver/planning/views/manage-the-table-view.md)
* [De tijdlijnweergave beheren](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
   <p>Nieuw: Standaard</p>
   <p>Huidig: Plan</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Adobe Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Contribute of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang voor de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/planning/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Records maken door deze handmatig aan een recordtype toe te voegen <!--in a record type table (I don't think you can create them elsewhere right now)-->

U kunt records maken in de tabelweergave van een pagina met recordtypen.

Voor informatie over het uitgeven van verslaginformatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.
Alle records van het geselecteerde type worden in de weergave weergegeven.

1. (Voorwaardelijk) Afhankelijk van de weergave die u weergeeft, voert u een van de volgende handelingen uit:

   * In de tabelweergave:

      * Klik **Nieuw verslag** in de laatste rij van de lijst

      * Klik **Verschuiving + gaat** op uw toetsenbord van om het even welke kolom of rij van de lijst binnen. Hiermee voegt u een lege rij toe.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Vanuit elke weergave:

      * Klik **Nieuw verslag** in de hoger-juiste hoek van de pagina. Het voorvertoningsvak voor records wordt geopend.

     Workfront uploadt automatisch een miniatuur en een omslagafbeelding naar elke nieuwe record. U kunt deze afbeeldingen later wijzigen. Raadpleeg de volgende artikelen voor meer informatie:

      * [Een omslagafbeelding aan een record toevoegen](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Een miniatuur toevoegen aan een record](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Typ informatie over de nieuwe record in de velden die u in het voorvertoningsvak ziet.

   >[!NOTE]
   >
   >  * Er zijn geen verplichte velden voor records. Nochtans, adviseren wij dat u informatie voor het primaire gebied van een verslag toevoegt, aangezien het nuttig is om verslagen te identificeren wanneer het verbinden van verslagen aan elkaar. Voor meer informatie over primaire gebieden, zie [ de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) beheren en [ Primair gebiedsoverzicht ](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Velden die naar andere recordtypen of berekende velden verwijzen, zijn alleen-lezen velden.

1. (Voorwaardelijk) wanneer het toevoegen van verslagen in de lijst, blijft het toevoegen van informatie over elke rij, dan klik **gaat** op uw toetsenbord binnen om uw veranderingen te bewaren.

   of

   Klik de naam van het nieuwe verslag of **Open details** pictogram ![](assets/open-details-icon-in-table-name-field.png) links van de verslagnaam. In de tabel wordt een voorvertoning geopend met de gedetailleerde informatie van de record.

   >[!TIP]
   >
   >U kunt tot het **Open pictogram van Details** slechts van het naamgebied van het verslag toegang hebben wanneer het gebied van de Naam een primair gebied is.

1. Bewerk de recordgegevens in de voorvertoning van de record. Workfront slaat uw wijzigingen automatisch op.
1. (Facultatief) klik **Open in nieuw lusje** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproef van het verslag om de pagina van het verslag in een nieuw lusje te openen. Ga door met het bewerken van de record op de recordpagina. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

1. (Optioneel) Gebruik de volgende sneltoetsen om nieuwe records of de bijbehorende informatie ongedaan te maken of opnieuw toe te voegen wanneer u deze in de tabelweergave toevoegt:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Records maken door gegevens uit een externe lijst te kopiëren en te plakken

1. Begin creërend verslagen in de mening van de Lijst, zoals die in sectie [ wordt beschreven creeer verslagen door hen aan een verslagtype ](#create-records-by-manually-adding-them-to-a-record-type) in dit artikel manueel toe te voegen.

   Zorg ervoor dat de tabelweergave de kolommen (of de velden) bevat die u wilt vullen met de nieuwe recordgegevens.

1. Klik **Nieuw &lt; het type van Verslag naam >** in de laatste rij van de lijst om zo vele nieuwe rijen aan de lijst toe te voegen aangezien u uw nieuwe verslagen wilt zijn.

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

   De volgende informatie wordt geïmporteerd in het planningsgebied van Workfront:

   * De rijen bevatten de nieuwe records
   * De kolommen vullen informatie voor de gebieden van de verslagen.
