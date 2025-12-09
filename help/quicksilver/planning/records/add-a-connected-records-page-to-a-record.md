---
title: Een verbonden recordpagina toevoegen aan een record
description: U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag toe te voegen. Hiermee voegt u de verbonden records in een tabelweergave toe aan het tabblad.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---


# Een verbonden recordpagina toevoegen aan een record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag toe te voegen. Hiermee voegt u de verbonden records in een tabelweergave toe aan het tabblad.

Houd rekening met het volgende wanneer u een pagina Verbonden records aan een record toevoegt:

* U kunt een pagina Verbonden records aan een record toevoegen nadat u de record- of objecttypen hebt verbonden met het recordtype vanuit de tabelweergave van een recordtype.

* U kunt een pagina met verbonden records toevoegen vanuit het voorvertoningsgebied van een record of de pagina van de record.

* Verbonden recordpagina&#39;s geven alleen de verbonden objecten of records van één object of recordtype in een tabelweergave weer. Op de pagina worden niet alle records van dat type weergegeven.

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

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Een verbonden recordpagina toevoegen aan een record

1. Klik op de naam van de record om deze te openen vanuit een willekeurige weergave van een pagina met recordtypen.
1. Klik **toevoegen pagina** van één van de volgende gebieden:

   * Het voorvertoningsvenster van de record
   * De de detailspagina van het verslag, na het klikken van **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefpagina.

   **creeer pagina** doos opent.

   ![&#x200B; voeg Verbonden verslagen pagina modaal &#x200B;](assets/add-connection-view-page-modal.png) toe

1. Voeg de **naam van de Pagina** toe, klik **Verbonden verslagenpagina**, dan klik **creeer**.

   Een nieuwe gekoppelde recordpagina wordt als een nieuw tabblad toegevoegd aan de recordpagina.

   De records die zijn verbonden met de huidige record, worden in de tabelweergave weergegeven.

   >[!TIP]
   >
   >U moet verbonden verslagen in de lijst of het gebied van Details van een verslag toevoegen alvorens u hen in een verbonden verslagenpagina kunt tonen.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   De eerste vijf velden van de verbonden records worden standaard weergegeven. <!--No lookup fields display by default.-->

   ![&#x200B; Publiek verbonden lijstmening onder campagnedetails &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optioneel) Zoek of klik op de naam van een verbonden record of objecttype in de lijst.

1. (Optioneel en voorwaardelijk) Voer in de tabelweergave van de pagina met verbonden records een van de volgende handelingen uit wanneer u verbonden planningsrecords of Workfront-objecten bekijkt, behalve projecten: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Klik op de naam van een record. Hierdoor wordt de pagina van de record op een nieuw tabblad geopend.

   * Klik **verbinden** bij de bodem van de lijstmening om meer verslagen te verbinden, dan klik buiten de verbindingsdoos om het te sluiten. De nieuwe records worden automatisch aan de tabel toegevoegd.

     Voor informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).
   * Bewerk alle informatie uit de verbonden records inline in de tabelweergave.

   * Beweeg over de naam van een verbonden verslag, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png)

     of

     Selecteer een van de records en klik op een van de volgende opties in de blauwe balk onder aan de lijst:

      * **Mening** om de verslagpagina in een nieuw lusje te openen
      * **verbinding van het Exemplaar** om een verbinding aan de verslagpagina te kopiëren
      * **geeft duimnagel** uit om de **duimnagel van het Verslag** doos te openen en het duimnagelbeeld van het verslag uit te geven
      * **dupliceer** om het verbonden verslag te dupliceren. De gedupliceerde record wordt ook verbonden met de huidige record.
      * **Verslag van het Tussenvoegsel boven of onder** om nieuwe verslagen aan het verbonden verslagtype toe te voegen. Nieuwe records die u hier toevoegt, worden ook gekoppeld aan de huidige record. Deze optie is niet beschikbaar in de blauwe balk wanneer u een record in de tabel selecteert.
      * **Schrapping** om het verslag te schrappen. Als u een verbonden record verwijdert, wordt deze verwijderd uit het recordtype en van elke locatie waar de record is verbonden.

     Voor informatie over het uitgeven van verslagen in de lijstmening, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

     >[!TIP]
     >
     >U kunt meerdere records of objecten selecteren om deze te verwijderen.

   * Bewerk de inline records in de tabel op de pagina Verbonden records.

     Alle andere Workfront-objecten worden weergegeven in een tabelweergave (alleen-lezen) en u kunt ze niet bewerken.

1. (Optioneel en voorwaardelijk) Voer in de tabelweergave van de pagina met verbonden records een van de volgende handelingen uit wanneer u verbonden Workfront-projecten weergeeft:

   * Klik **verbinden verslagen** in de hoger-juiste hoek van de verbonden verslagpagina om bestaande projecten te verbinden.

   Voor informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).
   * Bewerk de projectgegevens in de tabel inline.
   * Klik **Nieuwe rij** om een project zonder een malplaatje tot stand te brengen. Het nieuwe project wordt onmiddellijk verbonden met het huidige verslag.

     Voor meer informatie, zie [&#x200B; de voorwerpen van Workfront van de Planning van Workfront creëren aangezien u hen met verslagen &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt
   * Beweeg over een project en klik **Meer** menu [&#x200B; Meer menu &#x200B;](assets/more-menu.png)

     of

     Selecteer een of meer projecten, bekijk de blauwe balk onder aan de lijst en klik op een van de volgende opties:

      * **Schrapping** om het project te schrappen. Als u een project verwijdert, wordt de verbinding met het project verbroken en verplaatst naar de prullenbak van Workfront.
      * **maak** los om het project van het verslag los te maken. Als u een project loskoppelt, verwijdert u het project en alle waarden van de opzoekvelden uit de huidige record.

1. (Optioneel) Dubbelklik op de naam van de **Verbonden recordpagina** tab

   of

   Beweeg over de naam van het lusje, dan klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **anders noemen** om aan nieuw Verbonden meningslusje anders te noemen.
1. (Optioneel) Gebruik een van de volgende weergave-elementen op de werkbalk van een verbonden recordpagina om de tabelweergave te beheren:

   * Filters
   * Sorteren
   * Groepering
   * Velden om velden weer te geven, te verbergen of opnieuw te rangschikken
   * Rijhoogte
   * Zoeken

   Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

   >[!NOTE]
   >
   >U kunt geen velden maken, bewerken of verwijderen in de tabelweergave van het tabblad van een verbonden record.

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Facultatief) Hover over de naam van het Verbonden lusje van de verslagenpagina, klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **Schrapping** om aan tabel te verwijderen.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage views from the connected records page of a record. 

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