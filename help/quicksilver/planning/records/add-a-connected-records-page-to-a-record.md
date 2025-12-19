---
title: Een verbonden recordpagina toevoegen aan een record
description: U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag toe te voegen. Hiermee voegt u de verbonden records in een tabelweergave toe aan het tabblad.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '2743'
ht-degree: 0%

---


# Een verbonden recordpagina toevoegen aan een record

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag in de Planning van Adobe Workfront toe te voegen. Hiermee voegt u de verbonden records in een tabelweergave toe aan het tabblad.

Houd rekening met het volgende wanneer u een pagina Verbonden records aan een record toevoegt:

* U kunt een pagina Verbonden records aan een record toevoegen nadat u de record- of objecttypen vanuit de tabelweergave hebt verbonden met het recordtype.

* U kunt een pagina met verbonden records toevoegen vanuit het voorvertoningsgebied van een record of de pagina van de record.

* <span class="preview"> u kunt slechts één verbonden verslagenpagina voor een specifiek verslagtype hebben.</span>

  <span class="preview"> bijvoorbeeld, als u een verbonden registratiepagina voor een campagne creeert en u zijn verbonden Personas wilt tonen, kunt u slechts één verbonden registratiepagina voor Personas hebben.</span>

* Verbonden recordpagina&#39;s geven alleen de verbonden objecten of records van één object of recordtype weer. Op de pagina worden niet alle records van dat type weergegeven.

* Afhankelijk van het object of het recordtype dat u op de pagina met verbonden records weergeeft, kunt u deze weergeven met de volgende weergaven:

   * U kunt verbonden verslagen van de Planning in de volgende meningen tonen:
      * Tabel
      * <span class="preview"> Chronologie </span>
      * <span class="preview"> Kalender </span>
   * U kunt verbonden Workfront-projecten weergeven in de lijstweergave.

* U kunt Verbonden recordpagina&#39;s toevoegen voor de volgende verbonden record- of objecttypen:

   * Workfront Planning-recordtypen
   * Workfront-projecten

     U kunt de verbonden Workfront-projecten ook weergeven als u geen toegangsrechten hebt in Workfront.

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
   <p>Voor informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/get-started"> begonnen worden met Adobe GenStudio for Performance Marketing </a>.</p></li></ul>
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

U moet recordtypes met andere verslagtypes of de projecten van Workfront eerst verbinden alvorens een verbonden verslagenpagina aan een verslag toe te voegen.

1. Klik op de naam van de record om deze te openen vanuit een willekeurige weergave van een pagina met recordtypen.
1. Klik **toevoegen pagina** van één van de volgende gebieden:

   * Het voorvertoningsvenster van de record
   * De de detailspagina van het verslag, na het klikken van **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefpagina.

   **creeer pagina** doos opent.

   ![&#x200B; voeg Verbonden verslagen pagina modaal &#x200B;](assets/add-connection-view-page-modal.png) toe

1. Voeg de **naam van de Pagina** toe, klik **Verbonden verslagenpagina** voor het **type van Pagina**, dan klik **creeert**.
1. (Optioneel) Klik op de naam van een verbonden record of objecttype in de lijst of zoek ernaar. Klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven om de pagina voor dat record- of objecttype te maken.

   >[!TIP]
   >
   ><span class="preview"> u kunt één verbonden verslagenpagina per verslagtype tot stand brengen. Als een verbonden recordtype reeds een pagina heeft, het niet meer als optie toont.</span>
   >

1. (Facultatief en voorwaardelijk) als meer dan één verbonden gebied van het verslag of objecten type u de pagina voor vertoningen bouwt, klik het gebied waarvan verslagen of voorwerpen u in de verbonden verslagenpagina van de **Uitgezochte verwijzingsgebied** lijst wilt tonen.

   ![&#x200B; Uitgezochte lijst van het verwijzingsgebied &#x200B;](assets/select-reference-field-list-on-connected-records-page.png)

   Een van de volgende pagina&#39;s wordt toegevoegd aan de pagina voor verbonden records:

   * De tabelweergave van een recordtype
   * De lijstmening van een type van projectobjecten

   De verslagen of de projecten die met het huidige verslag worden verbonden tonen in de lijst of lijstmening.

   >[!TIP]
   >
   >U moet verbonden verslagen in de lijst of het gebied van Details van een verslag toevoegen alvorens u hen in een verbonden verslagenpagina kunt tonen. Anders is de tabel of lijst leeg.

   De eerste vijf velden van de verbonden records worden standaard weergegeven. Er worden standaard geen opzoekvelden weergegeven.

   ![&#x200B; Publiek verbonden lijstmening onder campagnedetails &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Voorwaardelijk) Afhankelijk van het type records dat u in de verbonden recordpagina weergeeft, voert u een van de volgende handelingen uit:

   * Planningsrecords beheren
Voor informatie, zie de sectie [&#x200B; de verbonden verslagenpagina voor de Planning verslagen &#x200B;](#manage-the-connected-records-page-for-planning-records) in dit artikel beheren.
   * Workfront-projecten beheren
Voor informatie, zie de sectie [&#x200B; de verbonden verslagenpagina voor de projecten van Workfront &#x200B;](#manage-the-connected-records-page-for-workfront-projects) in dit artikel beheren.

1. (Optioneel) Dubbelklik op de naam van de **Verbonden recordpagina** tab

   of

   Beweeg over de naam van het lusje, dan klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **anders noemen** om aan nieuwe verbonden verslagenpagina tabel anders te noemen.

1. (Facultatief) Beweeg over de naam van de verbonden verslagenpagina tabel, klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **Schrapping** om aan tabel te verwijderen.

### De verbonden recordpagina voor planningsrecords beheren

Het beheren van de verbonden verslagenpagina voor de verslagen van de Planning verschilt afhankelijk van welke milieu u gebruikt.

#### Beheer de verbonden verslagenpagina voor de verslagen van de Planning in het milieu van de Productie

Wanneer u een verbonden verslagenpagina voor verbonden Planningsverslagen in het milieu van de Productie creeert, doe het volgende: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Ga naar een pagina met recordtypen en klik op de naam van een record. Hierdoor wordt de voorvertoningspagina van de record geopend.
1. Klik het lusje voor een verbonden verslagenpagina die de verslagen van de Planning tonen.
De records die zijn verbonden met de record die u hebt geselecteerd, worden weergegeven in de tabelweergave.
1. Klik **verbinden** bij de bodem van de lijstmening om bestaande verslagen te verbinden, hen van de verbindingsdoos te selecteren, dan buiten de doos te klikken om het te sluiten. De records worden automatisch aan de tabel toegevoegd en gekoppeld aan de record die u hebt geselecteerd. De records moeten bestaan voordat u ze kunt toevoegen.

   Voor meer informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. Bewerk alle informatie uit de verbonden records inline in de tabelweergave.
1. Beweeg over de naam van een verbonden verslag, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png)

   of

   Selecteer een van de records en klik op een van de volgende opties in de blauwe balk onder aan de lijst:

   * **Mening** om de verslagpagina in een nieuw lusje te openen
   * **verbinding van het Exemplaar** om een verbinding aan de verslagpagina te kopiëren
   * **geeft duimnagel** uit om de **duimnagel van het Verslag** doos te openen en het duimnagelbeeld van het verslag uit te geven
   * **dupliceer** om het verbonden verslag te dupliceren. De gedupliceerde record wordt ook verbonden met de huidige record.
   * **Verslag van het Tussenvoegsel boven of onder** om nieuwe verslagen aan het verbonden verslagtype toe te voegen. Nieuwe records die u hier toevoegt, worden ook gekoppeld aan de huidige record. Deze optie is niet beschikbaar in de blauwe balk wanneer u een record in de tabel selecteert.
   * **Schrapping** om het verslag te schrappen. Als u een verbonden record verwijdert, wordt deze verwijderd uit het recordtype en van elke locatie waar de record is verbonden. De geschrapte verslagen beweging aan **onlangs schrapte** bak van hun verslagtype.

     Voor informatie over het uitgeven van verslagen in de lijstmening, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

     >[!TIP]
     >
     >U kunt meerdere records of objecten selecteren om deze te verwijderen.
     >

1. Bewerk een van de records in de tabel op de pagina met verbonden records met inline.
1. Gebruik een van de volgende weergave-elementen op de werkbalk van een verbonden recordpagina om de tabelweergave te beheren:

   * **Filters**
   * **Soort**
   * **Groepering**
   * **Gebieden**, om, gebieden te tonen te verbergen of te herschikken
   * **de hoogte van de Rij**
   * **Onderzoek**

   Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

   >[!NOTE]
   >
   >U kunt geen velden maken, bewerken of verwijderen in de tabelweergave van het tabblad van een verbonden record.
   >

<div class="preview">

#### De verbonden recordpagina beheren voor planningsrecords in de voorvertoningsomgeving

Wanneer u een verbonden verslagenpagina voor verbonden verslagen van de Planning in het milieu van de Voorproef creeert, doe het volgende: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Ga naar een pagina met recordtypen en klik op de naam van een record. Hierdoor wordt de voorvertoningspagina van de record geopend.
1. Klik het lusje voor een verbonden verslagenpagina die de verslagen van de Planning tonen.
De records die zijn verbonden met de record die u hebt geselecteerd, worden weergegeven in de tabelweergave.
1. Klik **verbinden verslagen** in de hoger-juiste hoek van de verbonden verslagpagina, om bestaande verslagen te verbinden, hen van de verbindingsdoos te selecteren, dan buiten de doos te klikken om het te sluiten. De records worden automatisch aan de tabel toegevoegd en gekoppeld aan de record die u hebt geselecteerd. De records moeten bestaan voordat u ze kunt toevoegen.

   Voor meer informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. Klik **Nieuwe rij** bij de bodem van de lijst om nieuwe verslagen toe te voegen. De nieuwe records worden automatisch verbonden met de records die u hebt geselecteerd.
1. Bewerk alle informatie uit de verbonden records inline in de tabelweergave.
1. Beweeg over de naam van een verbonden verslag, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png)

   of

   Selecteer een van de records en klik op een van de volgende opties in de blauwe balk onder aan de lijst:

   * **Mening** om de verslagpagina in een nieuw lusje te openen
   * **verbinding van het Exemplaar** om een verbinding aan de verslagpagina te kopiëren
   * **geeft duimnagel** uit om de **duimnagel van het Verslag** doos te openen en het duimnagelbeeld van het verslag uit te geven
   * **dupliceer** om het verbonden verslag te dupliceren. De gedupliceerde record wordt ook verbonden met de huidige record.
   * **Verslag van het Tussenvoegsel boven of onder** om nieuwe verslagen aan het verbonden verslagtype toe te voegen. Nieuwe records die u hier toevoegt, worden ook gekoppeld aan de huidige record. Deze optie is niet beschikbaar in de blauwe balk wanneer u een record in de tabel selecteert.
   * **Schrapping** om het verslag te schrappen. Als u een verbonden record verwijdert, wordt deze verwijderd uit het recordtype en van elke locatie waar de record is verbonden. De geschrapte verslagen beweging aan **onlangs schrapte** bak van hun verslagtype.

     Voor informatie over het uitgeven van verslagen in de lijstmening, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

     >[!TIP]
     >
     >U kunt meerdere records of objecten selecteren om deze te verwijderen.

1. Bewerk een van de records in de tabel op de pagina met verbonden records met inline.
1. Gebruik een van de volgende weergave-elementen op de werkbalk van een verbonden recordpagina om de tabelweergave te beheren:

   * **Filters**
   * **Soort**
   * **Groepering**
   * **Gebieden**, om, gebieden te tonen te verbergen of te herschikken
   * **de hoogte van de Rij**
   * **Onderzoek**

   Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

   >[!NOTE]
   >
   >U kunt geen velden maken, bewerken of verwijderen in de tabelweergave van het tabblad van een verbonden record.
   >

1. Klik het van meningsdropdown menu, en klik **Nieuwe mening** om een nieuwe mening voor de pagina toe te voegen, dan doe het volgende:

   1. Voeg de naam van de a **Mening** toe.
   1. Van het **type van Mening** gebied, selecteer één van de volgende types van meningen:

      * Tabel
Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden
      * Tijdlijn
Voor informatie, zie [&#x200B; de chronologiemening &#x200B;](/help/quicksilver/planning/views/manage-the-timeline-view.md) leiden.
      * Kalender
Voor informatie, zie [&#x200B; de kalendermening &#x200B;](/help/quicksilver/planning/views/manage-the-calendar-view.md) leiden.

        Voor meer informatie, zie de sectie [&#x200B; veelvoudige meningen van de verbonden verslagenpagina &#x200B;](#manage-multiple-views-from-the-connected-records-page) in dit artikel leiden.

   1. Klik **creëren**.
Er wordt een nieuwe weergave toegevoegd aan het vervolgkeuzemenu Weergaven.

   1. (Facultatief) Beweeg over de naam van een mening u creeerde, klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik één van de volgende opties:

      * **noem** anders, om een nieuwe naam voor de mening toe te voegen.
      * **Aandeel**

        Voor meer informatie, zie [&#x200B; meningen van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >U kunt geen systeemweergave delen die door Workfront is gemaakt.

      * **Schrapping**
Voor informatie, zie [&#x200B; verslagmeningen van de Schrapping &#x200B;](/help/quicksilver/planning/views/delete-record-views.md).

        ![](assets/view-more-menu-projects-connected-records-page.png)

</div>

### De pagina met verbonden records voor Workfront-projecten beheren

Wanneer u een verbonden verslagenpagina voor verbonden projecten van Workfront creeert, doe het volgende:

1. Ga naar een pagina met recordtypen en klik op de naam van een record. Hierdoor wordt de voorvertoningspagina van de record geopend.
1. Klik het lusje voor een verbonden verslagenpagina die de projecten van Workfront tonen.
De projecten verbonden met het verslag u selecteerden tonen in de lijstmening.
1. Klik **verbinden verslagen** in de hoger-juiste hoek van de verbonden verslagpagina om bestaande projecten te verbinden.

   Voor informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).
1. Bewerk de projectgegevens in de tabel inline.
1. Klik **Nieuwe rij** om een project zonder een malplaatje tot stand te brengen. Het nieuwe project wordt automatisch verbonden met het huidige verslag.

   Voor meer informatie, zie [&#x200B; de voorwerpen van Workfront van de Planning van Workfront tot stand brengen aangezien u hen met verslagen &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt.

1. Beweeg over een projectnaam in de lijst en klik **Meer** menu [&#x200B; Meer menu &#x200B;](assets/more-menu.png)

   of

   Selecteer een of meer projecten, bekijk de blauwe balk onder aan de lijst en klik op een van de volgende opties:

   * **Schrapping** om het project te schrappen. Als u een project verwijdert, wordt de verbinding met het project verbroken en verplaatst naar de prullenbak van Workfront. Workfront-beheerders kunnen verwijderde projecten herstellen tot 30 dagen nadat ze zijn verwijderd.
   * **maak** los om het project van het verslag los te maken. Als u een project loskoppelt, verwijdert u het project en alle waarden van de opzoekvelden uit de huidige record.

     >[!TIP]
     >
     >U kunt meer dan één project selecteren om hen los te maken of te schrappen.
     >

1. Klik het van meningsdropdown menu, en klik **Nieuwe mening** om een nieuwe mening voor de pagina toe te voegen, dan doe het volgende:

   1. Voeg de naam van de a **Mening** toe.
   1. Selecteer **Lijst** van het **type van Mening** gebied.
   1. Klik **creëren**.
Er wordt een nieuwe lijstweergave toegevoegd aan het vervolgkeuzemenu Weergaven.

      Voor meer informatie, zie de sectie [&#x200B; veelvoudige meningen van de verbonden verslagenpagina &#x200B;](#manage-multiple-views-from-the-connected-records-page) in dit artikel leiden.

   1. (Facultatief) Beweeg over de naam van een mening u creeerde, klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik één van de volgende opties:
      * **noem** anders, om een nieuwe naam voor de mening toe te voegen.
      * <span class="preview">**Aandeel**</span>

        Voor meer informatie, zie [&#x200B; meningen van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >U kunt geen systeemweergave delen die door Workfront is gemaakt.

      * **Schrapping**
Voor informatie, zie [&#x200B; verslagmeningen van de Schrapping &#x200B;](/help/quicksilver/planning/views/delete-record-views.md).

        ![](assets/view-more-menu-projects-connected-records-page.png)

   1. Klik het **pictogram van de Filter** pictogram ![&#x200B; van de Filter &#x200B;](assets/filter-icon.png), en gebruik de filter om specifieke projecten te tonen.

      >[!TIP]
      >
      ><span class="preview"> voor mensen-type gebieden, als **Eigenaar**, of **Sponsor**, kunt u een vervanging gebruiken om projecten te tonen waar de het programma geopende gebruiker aan deze rollen wordt toegewezen.</span>
      >
      >![&#x200B; Filter met gebruikersvervanging voor project verbonden verslagenpagina &#x200B;](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >

   1. Klik het **pictogram van Kolommen** pictogram van Kolommen ![&#x200B; &#x200B;](assets/columns-icon.png) om kolommen in de lijst te verbergen of te tonen.
   1. Klik op het pictogram **+** rechtsboven in de tabelweergave om bestaande velden aan de tabel toe te voegen. Velden moeten bestaan voordat u ze kunt toevoegen.

      De **manager van de Kolom** doos opent. Ga als volgt te werk:

      1. Onderzoek naar een bestaand objecten gebied in de **Beschikbare** kolom, dan klik **+** rechts van het gebied naam het om het aan de **Geselecteerde** kolom toe te voegen.

         De velden die u selecteert, worden toegevoegd aan de tabelweergave op de pagina met verbonden records.
      1. Klik **-** rechts van een gebied in de **Geselecteerde** kolom om het uit de lijstmening te verwijderen.
      1. Klik **sparen** om de verbonden mening van de lijst van de verslagpagina te bewaren.


<div class="preview">

## Meerdere weergaven beheren vanaf de pagina met verbonden records

U kunt meerdere weergavetypen toevoegen en beheren vanaf de verbonden recordpagina van een record.

De meningen u in de Verbonden verslagenpagina van een verslagtype creeert zijn beschikbaar overal in de Planning van Workfront waar die verslagtype pagina toont. Weergaven die voor hetzelfde recordtype ergens anders in Workfront Planning zijn gemaakt, zijn ook toegankelijk in alle verbonden recordpagina&#39;s van dat recordtype.

Meerdere weergaven beheren vanaf de verbonden recordpagina:

1. Van de verbonden verslagenpagina van een verslag, klik het dropdown menu rechts van de meningsnaam, dan klik **Nieuwe mening** om een mening toe te voegen, dan uit de volgende opties te selecteren:

   * **Lijst**. Voor meer informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.
   * **Chronologie**. Voor meer informatie, zie [&#x200B; de chronologiemening &#x200B;](/help/quicksilver/planning/views/manage-the-timeline-view.md) leiden.
   * **Kalender**. Voor meer informatie, zie [&#x200B; de kalendermening &#x200B;](/help/quicksilver/planning/views/manage-the-calendar-view.md) leiden.

1. (Facultatief) Beweeg over de naam van een mening in de Verbonden verslagenpagina, dan klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik één van het volgende:

   * **anders noemen**
   * **Aandeel**. Voor meer informatie, zie [&#x200B; meningen van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Door weergaven te delen van Connected-recordpagina&#39;s, zijn deze toegankelijk voor gebruikers in alle gebieden van Workfront Planning waar de weergave wordt weergegeven.
   >Ook, als een mening van om het even welk ander gebied van de Planning van Workfront wordt gedeeld, is het ook beschikbaar aan de zelfde gebruikers in Verbonden verslagenpagina&#39;s.

   * **Uitvoer**
   * **dupliceer**. Voor meer informatie, zie [&#x200B; Dubbele verslagmeningen &#x200B;](/help/quicksilver/planning/views/duplicate-record-views.md).

     >[!TIP]
     >
     >Als u een weergave dupliceert van Connected-recordpagina&#39;s, is deze beschikbaar op alle andere gebieden van de planning van het personeel, wanneer u dezelfde recordtypen weergeeft.

</div>

<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->