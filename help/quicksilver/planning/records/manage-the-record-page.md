---
title: De lay-out van de pagina Opnemen beheren
description: U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '2395'
ht-degree: 0%

---


# De lay-out van de recordpagina beheren

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt de lay-out van de verslagvoorproef en pagina in de Planning van Adobe Workfront uitgeven.

De recordvoorvertoning is een kleinere weergave van de recordpagina die wordt weergegeven in de weergave van een recordtype.

Wanneer u de indeling van een recordvoorvertoning en pagina wijzigt, hebben de wijzigingen invloed op de voorbeeldvakken en op de detailpagina&#39;s van alle records van hetzelfde type.

In dit artikel wordt beschreven hoe u de lay-out en weergave van een recordvoorvertoningsvak of een recordpagina kunt wijzigen. Voor informatie over het uitgeven van verslagen, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

U moet recordtypen en records maken voordat u kunt beginnen met het bewerken van recordpagina&#39;s.

Raadpleeg de volgende artikelen voor meer informatie:

* [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)

* [Records maken](/help/quicksilver/planning/records/create-records.md)

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
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Willekeurige workflow en planningspakket</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
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


<!--Old:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## Overwegingen bij het bewerken van recordpagina&#39;s

* Standaard worden in de details en de voorvertoningspagina&#39;s van een record alle velden weergegeven die aan de record zijn gekoppeld.

* U kunt geen nieuwe velden toevoegen voor een record in de voorvertoning of op de detailpagina. U moet nieuwe velden toevoegen aan de tabelweergave om deze weer te geven op de pagina&#39;s met voorvertoningen en details.

* U kunt secties toevoegen aan een recordvoorvertoning of detailpagina om de informatie te ordenen op basis van algemene criteria en het gemakkelijker te maken om te zoeken.

* De volgende wijzigingen zijn van invloed op alle records van hetzelfde type en zijn zichtbaar voor alle gebruikers die deze records openen:

   * Velden opnieuw rangschikken
   * Secties toevoegen of verwijderen

* Wijzigingen die u in de voorvertoning van de record aanbrengt, zijn direct zichtbaar op de pagina met recorddetails. Wijzigingen die u aanbrengt in de recordpagina, worden ook weergegeven in het voorvertoningsvak van de record.

* Het toevoegen van een omslagafbeelding of een miniatuur aan een record maakt geen deel uit van de algemene lay-out van de voorvertoning of pagina van de record. U kunt unieke omslagafbeeldingen of miniaturen aan elke record toevoegen. Voor informatie, zie [&#x200B; een omslagbeeld aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) toevoegen en [&#x200B; voeg een duimnagel aan een verslag &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toe.

## Secties toevoegen aan een recordvoorvertoning of pagina

Houd rekening met het volgende wanneer u secties toevoegt aan een recordpagina:

* Er geldt geen limiet voor het aantal secties dat u op een pagina kunt plaatsen.
* U kunt geen lege sectie hebben. Een sectie moet ten minste één veld bevatten.
* U kunt velden van de ene sectie naar de andere slepen. Voor meer informatie, zie de sectie [&#x200B; gebieden in de verslagvoorproef of detailspagina &#x200B;](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel herschikken.
* Wanneer u alle velden uit een sectie verwijdert, wordt de sectie automatisch verwijderd en kan deze niet worden hersteld.

Een sectie toevoegen aan een recordvoorvertoning of pagina:

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik het **Open pictogram van details** pictogram ![&#x200B; Open detailspictogram op het gebied van de lijstnaam &#x200B;](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![&#x200B; doos van Details &#x200B;](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   De recordpagina wordt geopend. Het tabblad Details wordt standaard geopend.

   ![&#x200B; pagina van Details &#x200B;](assets/details-page.png)

1. In het **lusje van Details** van de verslagvoorproef of de pagina, houd over de witte ruimte links van de gebieden, dan klik **sectie** pictogram ![&#x200B; toevoegen van sectie &#x200B;](assets/add-section-icon.png) om een sectie toe te voegen.
1. Klik binnen de naam van de sectie en vervang **Naamloze sectie** met een naam, dan klik binnengaan. De velden die onder de sectie worden weergegeven, maken automatisch deel uit van de nieuwe sectie.
1. Begin en dalend gebieden aan de nieuwe sectie te slepen, zoals die in de sectie [&#x200B; wordt beschreven herschik gebieden in de verslagvoorproef of detailspagina &#x200B;](#rearrange-fields-in-the-record-preview-or-details-page) in dit artikel.

1. (Facultatief) Beweeg over de naam van een sectie en klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png).

   ![&#x200B; Meer menuopties voor sectie op verslagpagina &#x200B;](assets/more-menu-options-for-section-on-record-page.png)
1. (Optioneel) Voer een van de volgende handelingen uit om de sectie te bewerken:

   * Klik **anders noemen** om de sectie anders te noemen

     >[!TIP]
     >
     > U kunt de naam van een sectie inline wijzigen door op de naam te klikken.

   * Klik **Beweging omhoog** om de sectie omhoog één positie te bewegen

     of

     Klik **Beweging neer** om de sectie neer één positie te bewegen.
Alle velden in de sectie worden met de sectie verplaatst.

   * Klik **Schrapping** om de sectie te schrappen. De sectie wordt verwijderd en kan niet worden hersteld. Alle gebruikers die tot de verslagen van dit type toegang hebben zullen niet meer de geschrapte sectie bekijken.

1. Klik op de pijl omlaag links van een sectienaam om deze samen te vouwen of op de pijl naar rechts om deze uit te vouwen.
Alle secties worden standaard uitgevouwen.

1. (Facultatief) klik het **greep** pictogram ![&#x200B; pictogram van het Grab &#x200B;](assets/grab-icon.png) aan de linkerzijde van een sectienaam, dan belemmering en laat vallen het in een gewenste plaats.

   De nieuwe positie van de sectie wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in secties en de veldvolgorde worden automatisch opgeslagen.

1. (Facultatief) klik het **menu van de Uitvoer** pictogram van de Uitvoer in verslagdetailpagina ![&#x200B; om het lusje van Details naar een Word of een dossier van PDF uit te voeren. &#x200B;](assets/export-icon-in-record-details-page.png) Voor meer informatie, zie [&#x200B; de details van een verslag uitvoeren &#x200B;](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facultatief) klik het **lusje van Verbindingen** naast **Details** tabel. U zou **Meer** kunnen moeten klikken alvorens de **Verbindingen** tabel te klikken.

   Alle records of objecten die zijn verbonden met de geselecteerde record, worden onder de naam van het recordtype weergegeven, of de toepassing waartoe ze behoren.

   ![&#x200B; het lusje van Verbindingen op verslag in de Planning van Workfront &#x200B;](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Facultatief) selecteer **tonen alle verslagen** die in de hoger-juiste hoek van het lusje van Verbindingen plaatsen. Alle verbonden verslagtypes tonen, met inbegrip van degenen die nog geen verbonden verslagen hebben. Standaard is de schakeloptie uitgeschakeld en worden recordtypen zonder gekoppelde records verborgen.

1. (Facultatief) klik **verbinden** om meer verslagen aan de verbonden verslagtypes toe te voegen. Voor meer informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. (Optioneel) Houd de muisaanwijzer boven een opnamekaart en klik op het pictogram voor het verbreken van de verbinding **-** en klik vervolgens op **Verbinding verbreken** . <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ook verwijderd.

## Velden opnieuw rangschikken op het tabblad Details van de record

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Van de mening van de lijstlijst, klik het **Open pictogram van details** pictogram ![&#x200B; Open detailspictogram op het gebied van de lijstnaam &#x200B;](assets/open-details-icon-in-table-name-field.png) in de eerste kolom.

   De voorvertoning van de record wordt in de weergave geopend.

   ![&#x200B; doos van Details &#x200B;](assets/details-box.png)

1. (Facultatief) klik **Open in nieuw lusje** pictogram ![&#x200B; Open detailsdoos in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de hoger-juiste hoek van de verslagvoorproef om de pagina van het verslag in een nieuw lusje te openen.

   Het **lusje van Details** van het verslag opent door gebrek.

   ![&#x200B; pagina van Details &#x200B;](assets/details-page.png)

1. In het verslag **Details** lusje, klik het **greep** pictogram ![&#x200B; pictogram van het Grab &#x200B;](assets/grab-icon.png) aan de linkerzijde van een gebiedsnaam, dan belemmering en laat vallen het op een gewenste plaats.

   >[!TIP]
   >
   >U kunt velden naar een andere sectie slepen.
   >Een sectie moet ten minste één veld bevatten.
   >

   De nieuwe positie van het veld wordt bijgewerkt in zowel de voorvertoning als de pagina van alle records van hetzelfde type voor alle gebruikers die de records bekijken.

   Alle wijzigingen in de lay-out van de recordvoorvertoning of pagina worden automatisch opgeslagen.

## Een verbonden recordpagina toevoegen aan een record

U kunt informatie van verbonden verslagen of voorwerpen bekijken door een lusje voor een Verbonden verslagenpagina aan een verslag toe te voegen.

De gegevens uit de verbonden records kunnen worden bewerkt in de tabelweergave. De gegevens van de objecten die met een andere toepassing zijn verbonden, kunnen niet worden bewerkt in de tabelweergave.

Houd rekening met het volgende wanneer u een pagina Verbonden records aan een record toevoegt:

* U kunt een pagina Verbonden records aan een record toevoegen nadat u de record- of objecttypen hebt verbonden met het recordtype vanuit de tabelweergave van een recordtype.

* In de productieomgeving kunt u geen pagina met verbonden records toevoegen vanuit de voorvertoning van een record.

  <span class="preview"> u kunt een Verbonden verslagenpagina van de voorproef van een verslag in het milieu van de Voorproef toevoegen.</span>

* Verbonden recordpagina&#39;s geven alleen de verbonden objecten of records van één object of recordtype in een tabelweergave weer. Op de pagina worden niet alle records van dat type weergegeven in de tabelweergave.

* Afhankelijk van de omgeving die u gebruikt, kan het volgende opvallen:

   * Nadat u in de productieomgeving een pagina met verbonden records aan een record hebt toegevoegd, is het tabblad Pagina zichtbaar vanuit het voorvertoningsgebied van de record, maar is het leeg. U moet naar de volledige pagina gaan om de lijstmening voor het verbonden verslag te zien.
   * <span class="preview"> in het milieu van de Voorproef, is de Verbonden verslagenpagina zichtbaar van zowel het voorproefgebied van het verslag als van browser tabel.</span>

* U kunt Verbonden recordpagina&#39;s toevoegen voor de volgende verbonden record- of objecttypen:

   * Workfront Planning-recordtypen
   * Workfront-projecten, -programma&#39;s, -portfolio&#39;s, -groepen of -bedrijven. U kunt de verbonden Workfront-objecten ook weergeven als u geen toegangsrechten hebt in Workfront.

  >[!NOTE]
  >
  >   U kunt geen Connect-recordpagina toevoegen voor verbonden AEM Assets-records.

Een pagina voor verbonden records toevoegen:

1. Klik op de naam van de record om deze te openen.
1. Klik **toevoegen pagina** van één van de volgende gebieden:

   * <span class="preview"> het voorproefvenster van het verslag </span>
   * De de detailspagina van het verslag, na het klikken van **Open in nieuw lusje** pictogram ![&#x200B; Open details in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefpagina.

   **creeer pagina** doos opent.

   ![&#x200B; voeg Verbonden verslagen pagina modaal &#x200B;](assets/add-connection-view-page-modal.png) toe

1. Voeg de **naam van de Pagina** toe, klik **Verbonden verslagenpagina**, dan klik **creeer**.

   Er wordt een nieuw tabblad toegevoegd aan de pagina van de record.
1. Zoek of klik op de naam van een verbonden record of objecttype in de lijst.
De tabelweergave van het geselecteerde recordtype wordt weergegeven op de nieuwe pagina en de gekoppelde records worden weergegeven in de tabelweergave.
Alle velden van de verbonden record worden weergegeven in de tabelweergave van het tabblad van de verbonden record.

   De eerste vijf velden van de verbonden recordtabel worden standaard weergegeven. Er worden standaard geen opzoekvelden weergegeven.

   ![&#x200B; Publiek verbonden lijstmening onder campagnedetails &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optioneel) Voer een van de volgende handelingen uit in de tabelweergave van de gekoppelde records:

   * Klik op de naam van een record. Hierdoor wordt de pagina van de record op een nieuw tabblad geopend.

     Hierdoor wordt de voorvertoningspagina van de record geopend. Klik **Open in een nieuw lusje** pictogram ![&#x200B; Open in een nieuw lusjepictogram &#x200B;](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek om de verbonden pagina van het verslag te openen.

   * Klik **verbinden** om meer verslagen te verbinden, dan klik buiten de verbindingsdoos om het te sluiten. De nieuwe records worden automatisch aan de tabel toegevoegd.
   * Bewerk alle gegevens uit de verbonden records in de tabelweergave.

   * Beweeg over de naam van een verbonden verslag, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik één van de volgende opties:
      * Weergave
      * Koppeling kopiëren
      * Miniatuur bewerken
      * Dupliceren
      * Record invoegen boven of onder
      * Verwijderen
   * Selecteer een van de records en klik op een van de volgende opties in de blauwe balk onder aan het scherm:
      * Weergave
      * Koppeling kopiëren
      * Miniatuur bewerken
      * Dupliceren
      * Verwijderen. Verwijderen is de enige beschikbare optie wanneer u meerdere records selecteert.

     Voor informatie over het uitgeven van verslagen in de lijstmening, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

   * Bewerk een van de records in de tabel op de pagina Verbonden records met inline.

     In de productieomgeving worden alle Workfront-objecten weergegeven in een alleen-lezen tabelweergave en kunt u ze niet bewerken.

     <span class="preview"> in het milieu van de Voorproef, kunt u projecten in de verbonden verslagenpagina inline uitgeven.</span>

1. <span class="preview"> (Voorwaardelijk) Wanneer het bekijken van een lijst van verbonden projecten, doe om het even welke volgend:</span>

   * <span class="preview"> klik **verbinden verslagen** in de hoger-juiste hoek van de verbonden verslagpagina om bestaande projecten te verbinden.</span>
   * <span class="preview"> binnen geeft projectinformatie in de lijst uit.</span>
   * <span class="preview"> klik **Nieuwe rij** om een project zonder een malplaatje tot stand te brengen. Het nieuwe project wordt onmiddellijk verbonden met het huidige verslag.</span>

     Voor meer informatie, zie [&#x200B; de voorwerpen van Workfront van de Planning van Workfront creëren aangezien u hen met verslagen &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt
   * <span class="preview"> Hover over een project en klik **Meer** menu [&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik één van het volgende:</span>
      * <span class="preview">**Schrapping** om het project te schrappen. Als u een project verwijdert, wordt de verbinding met het project verbroken en verplaatst naar de prullenbak van Workfront. </span>
      * <span class="preview">**maak** los om het project van het verslag los te maken. Als u een project loskoppelt, verwijdert u het project en alle waarden van de opzoekvelden uit de huidige record. </span>

1. (Optioneel) Dubbelklik op de naam van het tabblad Verbonden recordpagina

   of

   Beweeg over de naam van het lusje, dan klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **anders noemen** om aan nieuw Verbonden meningslusje anders te noemen.
1. (Optioneel) Gebruik een van de volgende weergave-elementen op de werkbalk om de tabelweergave te beheren:

   * Filters
   * Sorteren
   * Groepering
   * Velden om velden weer te geven, te verbergen of opnieuw te rangschikken

   Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

   >[!NOTE]
   >
   >   U kunt geen velden maken, bewerken of verwijderen in de tabelweergave van het tabblad van een verbonden record.
   >

1. (Voorwaardelijk) Als u meer records of objecten wilt verbinden, voert u een van de volgende handelingen uit:

   * Klik **verbinden** bij de bodem van de lijst, om verslagen of om het even welke voorwerpen van Workfront toe te voegen of te verwijderen <span class="preview"> behalve projecten.</span>
   * <span class="preview"> in het milieu van de Voorproef, klik **verbindt verslagen** in de hoger-juiste hoek van de verbonden registratiepagina om bestaande projecten te verbinden of **Nieuwe rij** bij de bodem van de lijst te klikken om projecten tot stand te brengen en hen automatisch met het huidige verslag te verbinden.</span>

   Voor informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).
1. (Facultatief) Hover over de naam van het Verbonden lusje van de verslagenpagina, klik **Meer** ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **Schrapping** om aan tabel te verwijderen.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



