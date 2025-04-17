---
title: Records maken
description: Wanneer u Adobe Workfront Planning gebruikt, is een record een instantie van een recordtype. U kunt unieke verslagen voor elk verslagtype in de Planning van Workfront tot stand brengen door hen aan de lijstmening manueel toe te voegen, hen van een lijst in te voeren, hen te dupliceren, of hen te creëren aangezien u hen met andere verslagen verbindt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '2425'
ht-degree: 0%

---


# Records maken

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

In de Planning van Adobe Workfront, is een verslag een geval van een verslagtype.

U kunt records maken door een van de volgende handelingen uit te voeren:

* [Records maken door deze inline toe te voegen vanuit de tabelweergave met recordtype](#create-records-by-adding-them-inline-from-the-record-type-table-view)
* [Records maken met de knop Nieuwe record of Verzoek om record maken vanuit elke recordtypeweergave](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [Een lijst met records uit een externe lijst kopiëren en plakken](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [Records dupliceren vanuit een tabelweergave](#create-records-by-duplicating-them)
* [Records maken terwijl u deze verbindt met andere records](#create-records-as-you-connect-them)
* [Records maken door een aanvraagformulier naar een recordtype te verzenden](#create-records-by-submitting-a-request-form-to-a-record-type)
* [Records maken door gegevens te importeren uit een CSV- of Excel-bestand](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [Records maken met behulp van automatisering](#create-records-by-using-automations)

Raadpleeg de volgende artikelen voor informatie over het beheren van records in de tabel- of tijdlijnweergaven:

* [De tabelweergave beheren](/help/quicksilver/planning/views/manage-the-table-view.md)
* [De tijdlijnweergave beheren](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## Toegangsvereisten

+++ Breid uit om toegangsvereisten te bekijken..

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
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td> Standaard
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p> 
   <p>Bewerk de toegang in Workfront voor de objecttypen die u wilt maken (projecten, programma's en portfolio's) terwijl u de records met deze eigenschappen verbindt. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Draag of hogere toestemmingen aan de werkruimte <span class="preview"> bij en verslagtype </span> waar u verslagen wilt toevoegen. </p>
   <p>De mening of hogere toestemmingen aan de werkruimte <span class="preview"> en verslagtype </span> om verslagen tot stand te brengen gebruikend de het verslagknoop van het Verzoek op de verslagpagina</p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Rechten voor Workfront-objecten (portfolio's) beheren om onderliggende objecten (projecten) toe te voegen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Records maken door deze inline toe te voegen vanuit de tabelweergave met recordtype

U kunt records maken in de tabelweergave van een recordtypepagina terwijl u deze inline toevoegt.

Voor informatie over het uitgeven van verslaginformatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.
Records van het geselecteerde type worden weergegeven in de weergave.

1. (Voorwaardelijk) Voer in de tabelweergave een van de volgende handelingen uit:

   * Klik **Nieuw verslag** in de laatste rij van de lijst

   * Klik **Verschuiving + gaat** op uw toetsenbord van om het even welke kolom of rij van de lijst binnen. Hiermee voegt u een lege rij toe onder de record waaruit u begint.
   * Beweeg over het primaire gebied van een verslag, klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van het gebied, dan klik **verslag van het Tussenvoegsel boven** of **hieronder verslag van het Tussenvoegsel**.

   ![ Toevoegend een nieuwe campagne in lijstrij ](assets/adding-a-new-campaign-in-table-row.png)

   Workfront uploadt automatisch een miniatuur naar elke nieuwe record. U kunt deze afbeeldingen later wijzigen. Voor informatie, zie [ een omslagbeeld aan een verslag ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) toevoegen.

   Er wordt een nieuwe record aan de tabel toegevoegd.

1. Klik op het primaire veld van de nieuwe record

   of

   Klik het **Open detailleert** pictogram ![ Open detailspictogram op het gebied van de lijstnaam ](assets/open-details-icon-in-table-name-field.png) links van de verslagnaam.

   Het voorbeeldvak wordt in de tabel geopend.

1. Typ informatie over de nieuwe record in de velden die u in het voorvertoningsvak ziet.

   >[!NOTE]
   >
   >  * Er zijn geen verplichte velden voor records. Nochtans, adviseren wij dat u informatie voor het primaire gebied van een verslag toevoegt, aangezien het nuttig is om verslagen te identificeren wanneer het verbinden van verslagen aan elkaar. Voor meer informatie over primaire gebieden, zie [ de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) beheren en [ Primair gebiedsoverzicht ](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Velden die naar andere recordtypen of berekende velden verwijzen, zijn alleen-lezen velden.

1. (Voorwaardelijk) wanneer het toevoegen van verslagen in de lijst, alvorens de de voorproefdoos van het verslag te openen, blijft het toevoegen van informatie over elke rij, dan klik **binnengaan** op uw toetsenbord om uw veranderingen te bewaren.

   of

   Klik de naam van het nieuwe verslag of **Open detailleert** pictogram ![ Open detailspictogram op het gebied van de lijstnaam ](assets/open-details-icon-in-table-name-field.png) links van de verslagnaam om de voorproefdoos te openen en de informatie van het verslag op het detailsgebied uit te geven.

   >[!TIP]
   >
   >U kunt tot het **Open detailleert** pictogram slechts van het naamgebied van het verslag toegang hebben wanneer het gebied van de Naam een primair gebied is.

1. (Facultatief) van de voorproefdoos van het verslag, klik **Open in nieuw lusje** pictogram ![ Open details in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek om de pagina van het verslag in een nieuw lusje te openen. Ga door met het bewerken van de record op de recordpagina. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

   Workfront slaat uw wijzigingen automatisch op.

1. (Optioneel) Sluit het voorvertoningsvak of klik op de pijl terug links van de naam van de record als u de pagina van de record hebt geopend.

1. (Optioneel) Gebruik in de tabelweergave de volgende sneltoetsen om nieuwe records of de bijbehorende informatie ongedaan te maken of opnieuw toe te voegen wanneer u deze records toevoegt in de tabelweergave:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren

## Records maken met de knop Nieuwe record of Verzoek om record maken vanuit elke recordtypeweergave

Gebruikers met de machtiging Weergeven in de werkruimte <!--<span class="preview">and record type</span>--> kunnen alleen records maken met de knop Verzoek om record op de pagina met recordtypen.

Gebruikers met de machtigingen Contribute en Manage voor de werkruimte <!--<span class="preview">and record type</span>--> kunnen records maken met de knop New record op de pagina met recordtypen.
<!--did the permissions to record types get released?? if not, take the record type reference here out; AND else-where in this article, including access requirements table-->

>[!IMPORTANT]
>
>Een werkruimtemanager moet een aanvraagformulier voor het recordtype maken, zodat gebruikers met de machtiging Weergeven records kunnen toevoegen met een aanvraagformulier. Anders kunnen gebruikers met de machtiging Weergeven geen records maken.

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.
Alle records van het geselecteerde type worden in de weergave weergegeven.

1. (Voorwaardelijk) Klik vanuit elke weergave op een van de volgende opties in de rechterbovenhoek van het scherm, afhankelijk van de <!--<span class="preview">and record type</span>--> -machtigingen voor de werkruimte:

   * Klik **Nieuw verslag**, als u Contribute of hogere toestemmingen op de werkruimte <!--<span class="preview">and record type</span>--> hebt

     of

   * Klik **verslag van het Verzoek**, als u de toestemmingen van de Mening op de werkruimte <!--<span class="preview">and record type</span>--> hebt.

1. (Voorwaardelijk) als u **Nieuw verslag** klikte, doe het volgende:

   1. Klik één van de volgende manieren om een verslag tot stand te brengen, dan **ga** verder:

      * **voeg manueel** toe. Het voorvertoningsvak van de record wordt geopend.\
        Voeg informatie over het verslag toe, zoals die in [ wordt beschreven creeer verslagen door hen inline van de 1} sectie van de verslagtype lijstmening {in dit artikel toe te voegen, beginnend met stap 6. <!--insure this stays accurate-->](#create-records-by-adding-them-inline-from-the-record-type-table-view)
      * **uploadt van dossier**
Voeg verslagen toe, zoals die in het artikel [ worden beschreven verslagen door informatie van een CSV of dossier van Excel ](/help/quicksilver/planning/records/import-file-to-create-records.md) in te voeren, die met stap 6 beginnen. <!--ensure this stays accurate-->
      * **leg een verzoek** voor
Het aanvraagformulier van het recordtype wordt geopend.

        Een werkruimtebeheerder moet een aanvraagformulier maken om een record te kunnen toevoegen met behulp van een aanvraagformulier.

        >[!TIP]
        >
        >Sommige recordtypen kunnen meerdere formulieren hebben. Klik op een pictogram om het te openen.

        Voeg het verslag, zoals die in het artikel [ wordt beschreven voor:leggen Adobe Workfront planningsverzoeken voor om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen, beginnend met stap 6. <!--ensure this stays accurate-->

      ![ Drie manieren om archiefkeus modaal ](assets/three-ways-to-create-records-choice-modal.png) te creëren

1. (Voorwaardelijk) als u **verslag van het Verzoek** klikte, doe het volgende:

   1. (Voorwaardelijk) Als het recordtype meer dan één aanvraagformulier heeft, klikt u op een formulier om het te kiezen.
   2. Ga verder toevoegend informatie in de vorm om het verslag tot stand te brengen, zoals die in het artikel [ wordt beschreven Voorlegt Adobe Workfront Planningsverzoeken om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen, beginnend met stap 6. <!--ensure this stays accurate-->

1. (Voorwaardelijk) Controleer de nieuwe records.

   Afhankelijk van de manier waarop u ervoor hebt gekozen de record toe te voegen, kunnen enkele van de volgende dingen voorkomen:

   * Er wordt een nieuwe record toegevoegd aan het recordtype, tenzij u ervoor kiest deze toe te voegen met een aanvraagformulier met een goedkeuringsproces. De goedkeuring moet door alle fiatteurs worden verleend voordat de registratie wordt opgesteld.
   * Er worden meerdere records toegevoegd aan het recordtype als u records hebt toegevoegd met een CSV- of Excel-spreadsheet.
   * Er wordt een nieuwe aanvraag toegevoegd op het tabblad Planning van het gebied Workfront Requests als u de aanvraag hebt toegevoegd door een aanvraagformulier in te dienen.

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

## Records maken door deze te kopiëren en te plakken vanuit een externe lijst

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

## Records maken door deze te dupliceren

Voor informatie over het dupliceren van verslagen, zie [ Dubbele verslagen ](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Records maken terwijl u ze verbindt

U kunt de volgende objecttypen maken terwijl u deze verbindt vanuit andere records:

* Workfront-planningsrecords
* Workfront-objecten

In deze sectie wordt beschreven hoe u Workfront Planning-records kunt maken terwijl u deze verbindt vanuit andere records.

>[!NOTE]
>
>Het maken van Workfront-projecten en -portfolio&#39;s wanneer u deze koppelt aan Workfront-planningsrecords, lijkt op het maken van planningsrecords wanneer u deze verbindt met andere records.
>
>Voor informatie over het creëren van de voorwerpen van Workfront van de Planning van Workfront, zie [ de voorwerpen van Workfront van Workfront Planning tot stand brengen aangezien u hen met verslagen ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt.

U moet het volgende hebben voordat u nieuwe records kunt toevoegen door deze te verbinden vanuit bestaande records:

* Verbonden recordtypen. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
* Records.
* De correcte toegang en de toestemmingen in de Planning van Workfront en Workfront, zoals die in de sectie [ vereisten van de Toegang ](#access-requirements) in dit artikel worden beschreven.

Om verslagen tot stand te brengen aangezien u hen van andere verslagen verbindt:

1. Begin verbindend de verslagen van de Planning van Workfront, zoals die in het artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md). U kunt records verbinden vanuit de volgende gebieden:

   * Een verbindingsveld in de volgende gebieden van Workfront Planning:

      * De tabelweergave
      * De detailpagina of het voorvertoningsvak van een record

   * Een verbindingsveld in het gedeelte Planning van een project, portfolio of programma in Workfront.

     Voor informatie, zie [ recordverbindingen van de voorwerpen van Workfront beheren ](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

1. (Voorwaardelijk) Als u geen verslag kunt vinden wanneer het proberen om het aan te sluiten, **+ toevoegen** klikken

   of
Typ een naam en klik vervolgens op **+ Toevoegen** . De knop **+ Toevoegen** wordt gevolgd door de naam van het recordtype waarmee u verbinding maakt. Bijvoorbeeld, &quot;voeg merken&quot;toe wanneer het toevoegen van een merk aan een bestaande campagne. De naam die u hebt getypt, volgt ook de knop Toevoegen.

   ![ voeg knoop toe om verslagen in benadrukte context te creëren ](assets/add-button-to-create-records-in-context-highlighted.png)

   De record wordt gemaakt en toegevoegd aan het verbonden recordveld.

   >[!IMPORTANT]
   >
   >* U kunt alleen projecten, portfolio&#39;s en programma&#39;s maken in Workfront wanneer u deze via een record verbindt.
   >
   >* U kunt geen groepen of bedrijven maken wanneer u deze verbindt vanuit een record in Workfront Planning.
   > 

1. (Optioneel) Ga naar de tabelweergave van het recordtype waarvan u de record hebt gemaakt. Een nieuwe record wordt weergegeven in de laatste rij van de weergave.
1. (Optioneel) Voeg informatie voor de nieuwe record toe in de tabelweergave
of
Klik op de naam van de pagina om de detailpagina te openen en informatie toe te voegen.

## Records maken door een aanvraagformulier naar een recordtype te verzenden

Nadat iemand een aanvraagformulier voor een recordtype heeft gemaakt en er een koppeling naar heeft gedeeld, kunt u een aanvraag indienen waarmee een record voor dat recordtype wordt gemaakt.

Voor informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).

Zowel Workfront-gebruikers als gebruikers buiten uw organisatie kunnen aanvragen indienen bij de planning van recordtypen en records maken als ze een koppeling naar het aanvraagformulier hebben.

Voor informatie, zie [ de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

## Records maken bij het importeren van recordtypen uit een CSV- of Excel-bestand

U kunt records importeren wanneer u recordtypen importeert met een CSV- of Excel-bestand.

Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Records maken door records te importeren uit een CSV- of Excel-bestand

U kunt records voor bestaande recordtypen importeren wanneer u gegevens uit een CSV- of Excel-bestand importeert.

Voor informatie, zie [ verslagen tot stand brengen door informatie van een CSV of dossier van Excel ](/help/quicksilver/planning/records/import-file-to-create-records.md) in te voeren.

## Records maken met behulp van automatisering

U kunt automatiseringen in de Planning van Workfront vormen die, wanneer geactiveerd, verslagen creëren wanneer teweeggebracht van een verslag van de Planning. De gemaakte records worden automatisch verbonden met de records waarvan u de automatisering activeert.

U kunt de automatisering in de verslagpagina in de Planning van Workfront vormen en activeren. De verbonden record die wordt gemaakt, wordt in het verbonden veld van het recordtype geplaatst waaruit u de automatisering uitvoert.

Voor informatie, zie [ voorwerpen creëren gebruikend het verslag van de Planning van Adobe Workfront automatiseringen ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).



