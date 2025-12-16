---
title: Een verbonden recordpagina toevoegen aan een record
description: U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag toe te voegen. Hiermee voegt u de verbonden records in een tabelweergave toe aan het tabblad.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 0%

---


# Een verbonden recordpagina toevoegen aan een record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag toe te voegen. Hiermee voegt u de verbonden records in een tabelweergave toe aan het tabblad.

Houd rekening met het volgende wanneer u een pagina Verbonden records aan een record toevoegt:

* U kunt een pagina Verbonden records aan een record toevoegen nadat u de record- of objecttypen hebt verbonden met het recordtype vanuit de tabelweergave van een recordtype.

* U kunt een pagina met verbonden records toevoegen vanuit het voorvertoningsgebied van een record of de pagina van de record.

* Verbonden recordpagina&#39;s geven alleen de verbonden objecten of records van één object of recordtype weer. Op de pagina worden niet alle records van dat type weergegeven.

* U kunt de objecten weergeven op een pagina met verbonden records in de tabelweergave.

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>
-->

* U kunt Verbonden recordpagina&#39;s toevoegen voor de volgende verbonden record- of objecttypen:

   * Workfront Planning-recordtypen
   * Workfront-projecten, -programma&#39;s, -portfolio&#39;s, -groepen of -bedrijven. U kunt de verbonden Workfront-objecten ook weergeven als u geen toegangsrechten hebt in Workfront.

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront en alle planningspakketten</p>
<p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
<tr>
<td> 
   <p> Aanvullende producten</p> </td> 
   <td> 
   <p> Als u een verbonden recordpagina wilt toevoegen voor objecten uit de volgende toepassingen, moet u niet alleen over Adobe Workfront beschikken, maar ook over de volgende opties:</p>
   <ul><li><p>Een Adobe Experience Manager Assets-licentie en integratie tussen AEM Assets en Workfront om AEM-middelen te verbinden met planningsrecordtypen.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md"> Adobe Workfront voor Experience Manager Assets en de Hoofdzaak van Activa: artikelindex </a>. </p></li>
   <li><p> Een Adobe GenStudio for Performance Marketing-licentie om recordtypen te verbinden met GenStudio Brands</p>
   <p>Voor informatie, zie <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started"> begonnen worden met Adobe GenStudio for Performance Marketing </a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <p>Contribute of hoger machtigingen voor een werkruimte en recordtype </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>   
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Een verbonden recordpagina toevoegen aan een record

U moet eerst recordtypen verbinden met andere record- of objecttypen voordat u een gekoppelde recordpagina aan een record toevoegt.

1. Klik op de naam van de record om deze te openen vanuit een willekeurige weergave van een pagina met recordtypen.
1. Klik **toevoegen pagina** van één van de volgende gebieden:

   * Het voorvertoningsvenster van de record
   * De de detailspagina van het verslag, na het klikken van **Open in nieuw lusje** pictogram ![ Open details in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefpagina.

   **creeer pagina** doos opent.

   ![ voeg Verbonden verslagen pagina modaal ](assets/add-connection-view-page-modal.png) toe

1. Voeg de **naam van de Pagina** toe, klik **Verbonden verslagenpagina**, dan klik **creeer**.

   Een nieuwe gekoppelde recordpagina wordt als een nieuw tabblad toegevoegd aan de recordpagina.

   De records die zijn verbonden met de huidige record, worden in de tabelweergave weergegeven.

   >[!TIP]
   >
   >U moet verbonden verslagen in de lijst of het gebied van Details van een verslag toevoegen alvorens u hen in een verbonden verslagenpagina kunt tonen.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   De eerste vijf velden van de verbonden records worden standaard weergegeven. <!--No lookup fields display by default.-->

   ![ Publiek verbonden lijstmening onder campagnedetails ](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optioneel) Klik op de naam van een verbonden record of objecttype in de lijst of zoek ernaar en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.

1. (Optioneel en voorwaardelijk) Als u meer dan één verbonden veld hebt dat wordt weergegeven in de tabelweergave of de detailpagina van de record, klikt u op het veld waarvan u de records wilt weergeven op de pagina met verbonden records.

   De tabelweergave van het geselecteerde verbonden recordtype wordt toegevoegd aan de verbonden recordpagina.

1. (Optioneel en voorwaardelijk) Wanneer u een gekoppelde recordpagina maakt voor verbonden planningsrecords, voert u een van de volgende handelingen uit: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Klik op de naam van een record. Hierdoor wordt de pagina van de record op een nieuw tabblad geopend.
   * Klik **verbinden** bij de bodem van de lijstmening om bestaande verslagen te verbinden, hen van de verbindingsdoos te selecteren, dan buiten de doos te klikken om het te sluiten. De records worden automatisch aan de tabel toegevoegd. De records moeten bestaan voordat u ze kunt toevoegen.

   Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).
   * Bewerk alle informatie uit de verbonden records inline in de tabelweergave.

   * Beweeg over de naam van een verbonden verslag, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png)

     of

     Selecteer een van de records en klik op een van de volgende opties in de blauwe balk onder aan de lijst:

      * **Mening** om de verslagpagina in een nieuw lusje te openen
      * **verbinding van het Exemplaar** om een verbinding aan de verslagpagina te kopiëren
      * **geeft duimnagel** uit om de **duimnagel van het Verslag** doos te openen en het duimnagelbeeld van het verslag uit te geven
      * **dupliceer** om het verbonden verslag te dupliceren. De gedupliceerde record wordt ook verbonden met de huidige record.
      * **Verslag van het Tussenvoegsel boven of onder** om nieuwe verslagen aan het verbonden verslagtype toe te voegen. Nieuwe records die u hier toevoegt, worden ook gekoppeld aan de huidige record. Deze optie is niet beschikbaar in de blauwe balk wanneer u een record in de tabel selecteert.
      * **Schrapping** om het verslag te schrappen. Als u een verbonden record verwijdert, wordt deze verwijderd uit het recordtype en van elke locatie waar de record is verbonden.

        Voor informatie over het uitgeven van verslagen in de lijstmening, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

        >[!TIP]
        >
        >U kunt meerdere records of objecten selecteren om deze te verwijderen.

   * Bewerk de inline records in de tabel op de pagina Verbonden records.

1. (Optioneel en voorwaardelijk) Wanneer u een pagina met verbonden records maakt voor de volgende Workfront-objecttypen:

   * Portfolio&#39;s
   * Programma&#39;s
   * Groepen
   * Bedrijven

   Voer een van de volgende handelingen uit in de tabelweergave van de pagina met verbonden records:

   * Klik op de naam van een object. Hierdoor wordt de objectpagina op een nieuw tabblad geopend.
   * Klik **verbinden** bij de bodem van de lijstmening om bestaande voorwerpen te verbinden, hen van de verbindingsdoos te selecteren, dan buiten de doos te klikken om het te sluiten. De objecten worden automatisch aan de tabel toegevoegd. De objecten moeten bestaan voordat u ze kunt toevoegen.

   Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

   * Selecteer een van de objecten in de tabelweergave en klik op een van de volgende opties in de blauwe balk onder aan de lijst:

   * **Mening** om de verslagpagina in een nieuw lusje te openen
   * **verbinding van het Exemplaar** om een verbinding aan de verslagpagina te kopiëren
   * **maak** los om het voorwerp van het verslag los te maken u bekijkt.

   >[!TIP]
   >
   >U kunt meerdere records of objecten selecteren om de verbinding te verbreken.

1. (Optioneel en voorwaardelijk) Wanneer u een pagina voor verbonden records maakt voor verbonden Workfront-projecten:

   * Klik **verbinden verslagen** in de hoger-juiste hoek van de verbonden verslagpagina om bestaande projecten te verbinden.

   Voor informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).
   * Bewerk de projectgegevens in de tabel inline.
   * Klik **Nieuwe rij** om een project zonder een malplaatje tot stand te brengen. Het nieuwe project wordt onmiddellijk verbonden met het huidige verslag.

     Voor meer informatie, zie [ de voorwerpen van Workfront van de Planning van Workfront creëren aangezien u hen met verslagen ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt
   * Beweeg over een project en klik **Meer** menu [ Meer menu ](assets/more-menu.png)

     of

     Selecteer een of meer projecten, bekijk de blauwe balk onder aan de lijst en klik op een van de volgende opties:

      * **Schrapping** om het project te schrappen. Als u een project verwijdert, wordt de verbinding met het project verbroken en verplaatst naar de prullenbak van Workfront.
      * **maak** los om het project van het verslag los te maken. Als u een project loskoppelt, verwijdert u het project en alle waarden van de opzoekvelden uit de huidige record.

     >[!TIP]
     >
     >U kunt meer dan één project selecteren om hen los te maken of te schrappen.
   * Klik op het pictogram **+** rechtsboven in de tabelweergave om bestaande velden aan de tabel toe te voegen. Velden moeten bestaan voordat u ze kunt toevoegen.

     De **manager van de Kolom** doos opent. Ga als volgt te werk:

      1. Onderzoek naar een bestaand objecten gebied in de **Beschikbare** kolom, dan klik **+** rechts van het gebied naam het om het aan de **Geselecteerde** kolom toe te voegen.

         De velden die u selecteert, worden toegevoegd aan de tabelweergave op de pagina met verbonden records.
      1. Klik **-** rechts van een gebied in de **Geselecteerde** kolom om het uit de lijstmening te verwijderen.
      1. Klik **sparen** om de verbonden mening van de lijst van de verslagpagina te bewaren.

1. (Optioneel) Dubbelklik op de naam van de **Verbonden recordpagina** tab

   of

   Beweeg over de naam van het lusje, dan klik **Meer** ![ Meer menu ](assets/more-menu.png), dan klik **anders noemen** om aan nieuw Verbonden meningslusje anders te noemen.
1. (Optioneel) Gebruik een van de volgende weergave-elementen op de werkbalk van een verbonden recordpagina om de tabelweergave te beheren:

   * Filters
   * Sorteren. Niet beschikbaar voor projecten.
   * Groeperen. Niet beschikbaar voor projecten.
   * Kolommen om velden weer te geven, te verbergen of opnieuw te rangschikken
   * Rijhoogte. Niet beschikbaar voor projecten.
   * Zoeken

   Voor informatie, zie [ de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

   >[!NOTE]
   >
   >U kunt geen velden maken, bewerken of verwijderen in de tabelweergave van het tabblad van een verbonden record.

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Facultatief) Hover over de naam van het Verbonden lusje van de verslagenpagina, klik **Meer** ![ Meer menu ](assets/more-menu.png), dan klik **Schrapping** om aan tabel te verwijderen.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->