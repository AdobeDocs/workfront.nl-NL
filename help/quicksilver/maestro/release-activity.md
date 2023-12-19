---
title: Adobe Maestro-releaseactiviteit
description: Adobe Maestro is momenteel beschikbaar voor het selecteren van Workfront-klanten. Lees dit artikel vaak voor meer informatie over de functies die onlangs voor Adobe Maestro zijn uitgebracht.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: bccd29ce284ca247b51971369102b5992061afb0
workflow-type: tm+mt
source-wordcount: '2796'
ht-degree: 0%

---

# Adobe Maestro-releaseactiviteit

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro/maestro-overview.md).

Dit artikel bevat een overzicht van de functies die zijn uitgebracht na de start van het gesloten bètaprogramma van Maestro op 22 mei 2023.

De vrijgegeven functies worden weergegeven in de volgorde van hun release, met de meest recente eerst. Klanten die deelnemen aan het afgesloten bètaprogramma van Maestro hebben toegang tot alle functies in hun voorproef- en productieomgeving.

>[!IMPORTANT]
>
>De documentatie waarnaar in de onderstaande secties wordt verwezen, zal enige tijd beschikbaar zijn nadat de functies naar Production zijn vrijgegeven.

Deze sectie bevat een overzicht van de functies en patches die zijn uitgebracht na de start van het gesloten bètaprogramma van Maestro op 22 mei 2023.

De functies worden wekelijks vrijgegeven en worden weergegeven in de volgorde van hun release, met de meest recente eerst. Klanten die deelnemen aan het afgesloten bètaprogramma van Maestro hebben toegang tot alle functies in hun voorproef- en productieomgeving.

<!--
## Week of November 27, 2023

### Maestro permissions for users and groups

Production: November 28, 2023

>[!IMPORTANT]
>
>This functionality is not yet available in Preview.

You can now share a workspace with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit in a Maestro workspace. After you share permissions to a workspace, users have permissions to the record types, records, and fields in that space.

The following are the permissions levels for Maestro workspaces:  

* None: Users cannot access any workspaces in Maestro, even if the Maestro area is shared with them through a layout template. 

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces ones shared with them.  

* Manage: Users can create, edit, and delete record types, records, and fields in workspaces that are shared with them. They cannot create workspaces.  

Only Workfront administrators can create, edit, or delete workspaces and all information associated with them.  

For more information, see [Grant access to Adobe Maestro](../maestro/access/grant-access.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md). -->

## Week van 18 december 2024

### Opmerkingen toevoegen aan records op de pagina Details

Voorbeeld en productie voor alle klanten: 18 december 2023

>[!NOTE]
>
>De volgende mogelijkheden zijn beschikbaar in Production met de release van januari 2024:
>
>* Zoeken naar opmerkingen
>
>* Afbeeldingen kopiëren en plakken
>
>* Afbeeldingen slepen en neerzetten
>
>Zie voor meer informatie [Overzicht eerste release 2024, kwartaal 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

U kunt nu met anderen samenwerken aan individuele verslagen door commentaren toe te voegen of anderen te antwoorden terwijl het bekijken van een verslag in de pagina van Details.

De opmerkingervaring voor Maestro-records komt overeen met de nieuwe opmerkingervaring voor Workfront-objecten.

Zie voor meer informatie [Opnameopmerkingen beheren](/help/quicksilver/maestro/records/manage-record-comments.md).

## Week van 11 december 2023

### Het primaire veld bijwerken in een tabelweergave van een recordtype

Voorbeeld en productie: 14 december 2023

U kunt nu het veld kiezen dat u wilt weergeven in de eerste kolom van een Maestro-tabelweergave. Dit veld wordt nu een primair veld genoemd.

Vóór deze verbetering, het gebied van de Naam van een verslag altijd getoond in de eerste kolom van de lijstmening en het kon niet in een andere positie worden geplaatst.

Met deze verbetering, merk het volgende op:

* De kolom of het veld Naam is standaard nog steeds de eerste kolom van een tabel.

* U kunt elk veld van de volgende typen als primair veld kiezen en het veld Naam in de eerste kolom vervangen:

   * Tekst met één regel

   * Getal

   * Formule

     >[!NOTE]
     >
     >Formule-tekstvelden worden later vrijgegeven.

* Het primaire veld van een tabelweergave wordt altijd bevroren en kan alleen worden verplaatst als u een ander veld instelt als primair veld.

* U kunt het primaire veld wijzigen in een niet-primaire kolomkop.

* Alle tabelweergaven van een recordtype hebben hetzelfde primaire veld dat u selecteert.

Zie voor meer informatie [Tabelweergave beheren](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Connect Maestro-records met Adobe Experience Manager Assets

Voorvertoningsrelease: 14 december 2023

Productie: gepland voor 15 december 2023

>[!IMPORTANT]
>
>Het exemplaar van Workfront van uw organisatie moet aan het Adobe Bedrijfsplatform of Adobe Admin Console worden bezet om Maestro- verslagen aan Adobe Experience Manager Assets te kunnen verbinden.
>
>Als u vragen hebt over instaptoegang tot de Adobe Admin Console, raadpleegt u de [Veelgestelde vragen over Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


U kunt nu een verbinding tot stand brengen tussen Maestro-recordtypen en Adobe Experience Manager Assets.

Nadat u de verbinding tot stand hebt gebracht, is de volgende functionaliteit beschikbaar bij deze update:

* U kunt Experience Managers en mappen koppelen aan een Maestro-record vanuit een specifieke opslagplaats in Experience Manager Assets waartoe ze toegang hebben. In dit proces kunt u elementvelden verbinden met Maestro-velden.

* Maestro-gebruikers kunnen de naam van de verbonden elementen en de waarden van de verbonden velden in Maestro weergeven

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* U kunt op de elementnaam in de tabelweergave van de Maestro-record klikken vanuit het verbonden recordveld en een pop-upvenster weergeven met de elementminiatuur en verschillende toetsvelden. Vanuit het pop-upvenster kunt u naar de viewer voor middelen in Experience Manager navigeren en alle gegevens erover weergeven.

Zie voor meer informatie [Verbind recordtypen](/help/quicksilver/maestro/architecture/connect-record-types.md).

## Week van 4 december 2023

### Informatie van het ene veld naar het andere kopiëren en plakken in de tabelweergave van Maestro voor recordvelden van het type Mensen en gekoppelde recordvelden

Voorbeeld en productie: 5 december 2023

U kunt nu informatie van het ene veld naar een ander veld van hetzelfde type kopiëren en plakken in een tabelweergave van het type Maestro-record. Deze functionaliteit wordt nu ondersteund voor de volgende typen velden:

* Mensen
* Gekoppelde recordvelden

Overweeg het volgende:

* Het kopiëren en plakken van veldwaarden van het ene veld naar het andere wordt ondersteund voor velden die meerdere waarden weergeven.

* U kunt geen informatie kopiëren van een andere bron, behalve een Maestro-veld van hetzelfde type als het veld waarin u de informatie plakt.

* U kunt geen veldwaarden kopiëren en plakken voor velden die worden weergegeven in het gebied Details van een record.

Zie voor meer informatie [Records bewerken](../maestro/records/edit-records.md).

Zie voor informatie over gekoppelde velden [Verbind recordtypen](../maestro/architecture/connect-record-types.md).

## Week van 27 november 2023

### Informatie van het ene veld naar het andere kopiëren en plakken in de tabel Maestro-weergave

Voorbeeld en productie: 28 november 2023

U kunt nu informatie van het ene veld naar een ander veld van hetzelfde type kopiëren en plakken in een tabelweergave van het type Maestro-record.

Overweeg het volgende:

* U kunt geen informatie kopiëren van een andere bron, behalve een Maestro-veld van hetzelfde type als het veld waarin u de informatie plakt.

* U kunt geen veldwaarden kopiëren en plakken voor velden die worden weergegeven in het gebied Details van een record.

* U kunt geen veldwaarden kopiëren en plakken voor de volgende veldtypen:

   * Mensen

   * Systeemvelden

   * Gekoppelde velden die zijn gemaakt als gevolg van het verbinden van records

Zie voor meer informatie [Records bewerken](../maestro/records/edit-records.md).

## Week van 6 november 2023

### Groeperen voor de tabelweergave

Voorbeeld en productie: 7 november 2023

U kunt nu records groeperen in de tabelweergave van een recordtypepagina. U kunt groeperen door drie unieke gebieden in de interface van Maestro <!--checking into this for now: and by four fields when using the API-->.

Zie voor meer informatie [De tabelweergave beheren](../maestro/views/manage-the-table-view.md).

## Week van 30 oktober 2023

### Nieuwe veldtypen voor gebruikers- en datumvelden die moeten vastleggen wie een record heeft gemaakt of voor het laatst een record heeft gewijzigd of op welke datum

Voorbeeld en productie: 30 oktober 2023

De volgende veldtypen zijn geïntroduceerd voor Maestro-records:

* Gemaakt door

* Aanmaakdatum

* Laatst gewijzigd door

* Laatst gewijzigd

De veldwaarden van de velden die van deze veldtypen zijn gemaakt, zijn alleen-lezen en leggen de naam vast van de gebruiker die een record heeft gemaakt of voor het laatst heeft gewijzigd, of de datum waarop de record is gemaakt of voor het laatst is gewijzigd.

Zie voor meer informatie [Velden maken](../maestro/fields/create-fields.md).

### Navigeren naar Workfront-objecten vanuit een Maestro-record

Voorbeeld en productie: 31 oktober 2023

U kunt nu de Workfront-objectpagina&#39;s openen vanuit de volgende gebieden in Maestro:

* De alleen-lezen gekoppelde Workfront-objectrecordtabelweergave

* De alleen-lezen Workfront-objectrecordpagina Details

Zie voor meer informatie [Connect-records](../maestro/records/connect-records.md).

### Verbeterde navigatie in de tabelweergave

Voorbeeld en productie: 2 november 2023

De navigatie in de tabelweergave van een recordtype is verbeterd.

Hieronder volgen enkele verbeteringen:

* Gebruik de tabtoets op het toetsenbord om door de kolommen en rijen van de tabel te navigeren

* Voeg een nieuwe record toe vanaf een willekeurige kolompositie. Vóór deze verbetering kon u een verslag slechts van de eerste kolom toevoegen.

* Gebruik de toetsenbordcombinatie Shift + Enter om een nieuwe record (of rij) aan de tabel toe te voegen.

Zie voor meer informatie [Records maken](../maestro/records/connect-records.md).

## Week van 16 oktober 2023

### Het veldtype New People

Voorbeeld en productie: 16 oktober 2023

U kunt nu een veld van het type Mensen toevoegen aan Maestro-recordtypen. U kunt velden van het type Mensen gebruiken om bestaande gebruikers aan een record te koppelen. Zie voor meer informatie [Velden maken](../maestro/fields/create-fields.md).

### RTF-indeling voor alineasvelden

Voorbeeld en productie: 16 oktober 2023

We hebben besturingselementen voor RTF-opmaak toegevoegd voor velden van het type Alinea. U kunt de alineasvelden opmaken met RTF-tekst in de tabelweergave van een recordtype of op de pagina Details van een record. Zie voor meer informatie [Records bewerken](../maestro/records/edit-records.md).


### Kleurcodering opnemen en groeperen voor de tijdlijnweergave

Voorbeeld en productie: 19 oktober 2023

U kunt nu de recordbalken en de groepen in de tijdlijnweergave in kleur coderen.

Hier volgen opties voor de kleuren die u kunt weergeven voor recordbalken en groepen in de tijdlijnweergave:

* Groepen kunnen overeenkomen met de volgende kleuren:

   * Grijs (standaard)

   * De kleur van het veld waarop u groepeert

* Balken kunnen overeenkomen met de volgende kleuren:

   * De kleur van het recordtype

   * De kleur van een veld dat u selecteert

   * De kleur van de groep

   * Geen kleur (standaard)

Wanneer u kleuren afstemt op een bepaald veld, kunt u alleen velden met opties voor kleurcodes selecteren.

Zie voor meer informatie [De tijdlijnweergave beheren](../maestro/views/manage-the-timeline-view.md).

## Week van 9 oktober 2023

### Zoeken in tabelweergave

Voorbeeld en productie: 9 oktober 2023

U kunt nu naar een trefwoord zoeken om snel een record te zoeken in de tabelweergave. U kunt trefwoorden en speciale tekens gebruiken in alle velden die zichtbaar zijn op het scherm om een record te zoeken. Zie voor meer informatie [De tabelweergave beheren](../maestro/views/manage-the-table-view.md).

## Week van 18 september 2023

### Rijen opnieuw ordenen

Voorbeeld en productie: 20 september 2023

U kunt nu een of meerdere rijen (of records) opnieuw rangschikken in de tabelweergave van een recordtypepagina. Zie voor meer informatie [De tabelweergave beheren](../maestro/views/manage-the-table-view.md).

## Week van 4 september 2023

### Connect Maestro-records met Workfront-bedrijven en -groepen

Voorbeeld en productie: 5 september 2023

U kunt nu een Maestro-record verbinden met Workfront-bedrijven en -groepen. U moet eerst een verbinding maken tussen een Maestro-recordtype en de objecttypen van Workfront-bedrijven en -groepen. Vervolgens kunt u één Maestro-record van het geselecteerde recordtype verbinden met afzonderlijke Workfront-bedrijven en -groepen.

Overweeg het volgende:

* U moet een verbinding tussen Maestro- verslagtypes en het de objecten van het Bedrijf van Workfront en van de Groep types voor elke Werkruimte tot stand brengen.

* U kunt geen gegevenstypen voor taxonomie verbinden met Workfront-objecttypen.

* U kunt meerdere Maestro-records verbinden met hetzelfde Workfront-bedrijf of dezelfde-groep en meerdere bedrijven of groepen koppelen aan hetzelfde Maestro-record.

* U kunt bedrijven of groepen niet bewerken in Maestro. Alle wijzigingen van het bedrijf of de groep die in Workfront zijn uitgevoerd, zijn zichtbaar in Maestro, wanneer de aan Maestro gekoppelde records worden gecontroleerd.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Verbind recordtypen](../maestro/architecture/connect-record-types.md)
   * [Connect-records](../maestro/records/connect-records.md)

### URL-ondersteuning voor tekstvelden met één regel

Voorbeeld en productie: 7 september 2023

Voor een betere zichtbaarheid bij het werken met koppelingen in de tabelweergave hebben we ondersteuning toegevoegd voor URL&#39;s in tekstvelden van één regel. Wanneer u URL&#39;s gebruikt naar andere websites of externe stations bij het bijwerken van een tekstveld met één regel, worden deze nu geïdentificeerd als koppelingen en kunt u erop klikken in de tabel. Vóór deze verbetering, verbindingen die als tekst worden getoond.

## Week van 28 augustus 2023

### Menu Veldzichtbaarheid voor de werkbalk Tabelweergave

Voorbeeld en productie: 31 augustus 2023

Als u de juiste informatie wilt weergeven op een bepaalde set records, met name als u de weergave wilt delen met anderen die sommige maar niet alle velden van een recordtype moeten zien, kunt u nu selecteren welke velden (of kolommen) u wilt weergeven en welke u wilt verbergen in de tabelweergave.

U kunt afzonderlijke velden verbergen of weergeven voor elke koptekst van de veldkolommen, of u kunt alle velden van het recordtype beheren vanuit een instelling op de werkbalk van de tabelweergave.

Zie voor meer informatie [De tabelweergave beheren](../maestro/views/manage-the-table-view.md).

## Week van 21 augustus 2023

### Connect Maestro-records koppelen aan programma&#39;s en portfolio&#39;s

Voorbeeld en productie: 24 augustus 2023

U kunt nu een Maestro-record verbinden met Workfront-programma&#39;s en -portfolio&#39;s. U moet een verbinding maken tussen een Maestro-recordtype en een programma of portfolio waarmee een verbonden veld wordt gemaakt. Vervolgens kunt u alle Maestro-records van alle andere recordtypen in dezelfde werkruimte verbinden met specifieke programma&#39;s en portfolio&#39;s die een recordtype Workfront Program (alleen-lezen) of Workfront Portfolio maken in dezelfde werkruimte. Overweeg het volgende:

* Workfront-connectorrecordtypen zijn uniek voor elke werkruimte.
* U kunt meerdere Maestro-records verbinden met hetzelfde Workfront-programma of -portfolio en meerdere programma&#39;s en portfolio&#39;s koppelen aan hetzelfde Maestro-record.
* U kunt geen programma&#39;s en portfolio&#39;s bewerken in Maestro. Alle programma- en portfoliowijzigingen die in Workfront zijn uitgevoerd, zijn zichtbaar in Maestro bij het controleren van de gekoppelde records.

### Nieuwe sorteerfunctionaliteit voor de tabelweergave

Voorbeeld en productie: 24 augustus 2023

U kunt records nu sorteren in de tabelweergave van een recordtypepagina.
De volgende mogelijkheden zijn nu beschikbaar:

* Sorteren op tabelniveau, waarbij u meerdere velden tegelijk kunt sorteren.
* Sorteren op kolom- of veldniveau, waar u kunt sorteren op een afzonderlijk veld tegelijk.

### Verbeteringen in de tijdlijnweergave: nieuwe look-and-feel voor groepen en de compacte/standaardweergavekiezer

Voorbeeld en productie: 24 augustus 2023

De tijdlijnweergave is als volgt verbeterd:

* U kunt de tijdlijnweergave nu in de volgende modi weergeven:

   * Standaard - Hiermee worden records in afzonderlijke regels weergegeven.
   * Compact: de records weergeven waarvan de datums elkaar niet op dezelfde regel snijden.

* We hebben de vormgeving van de groeperingslijnen in de tijdlijnweergave gewijzigd, zodat deze boven de tijdlijn van de records die ze bevatten, worden weergegeven. Vóór deze verbetering worden de groeperingslijnen weergegeven over de volledige lengte van de tijdlijn.

## Week van 14 augustus 2023

### Kolommen opnieuw ordenen in de tabelweergave

U kunt de kolommen nu opnieuw ordenen in de tabelweergave Maestro. Houd rekening met het volgende wanneer u de kolommen opnieuw ordent:

* Het veld Naam is altijd het eerste veld in de tabelweergave van een pagina met recordtypen

* U kunt het veld Naam niet naar een andere positie verplaatsen

* Het veld Naam is bevroren en maakt geen deel uit van de horizontale schuifbalk.

### Horizontaal schuiven voor tijdlijnweergave

U kunt nu horizontaal schuiven in de tijdlijnweergave van een recordtype.

## Week van 7 augustus 2023

### Recordtypen importeren uit een Excel-bestand

Voorbeeld en productie: 10 augustus 2023

U kunt nu een Excel-bestand importeren om recordtypen in een werkruimte te maken. De bladen van het dossier worden de verslagtypes, en de kolommen van het dossier worden hun respectieve gebieden.

### Verbeterde ervaring voor het verbinden van recordtypen en projecten

Voorbeeld en productie: 10 augustus 2023

We hebben de manier verbeterd waarop u recordtypen met elkaar verbindt, zoals verbinding maken met Workfront-projecten. Als onderdeel van deze verbetering hebben we de volgende wijzigingen aangebracht bij het toevoegen van een veld voor een recordtype in de tabelweergave:

* Het veld Relatie-type is verwijderd uit het tabblad &quot;Nieuw veld&quot;.

* Voeg een tabblad &quot;Nieuwe verbinding&quot; toe waar u rechtstreeks het record- of objecttype kunt selecteren waarmee u verbinding wilt maken, zodat er geen veld van het type relatie meer nodig is.

## Week van 10 juli 2023

### De weergave van een recordtype bijwerken

Voorbeeld en productie: 13 juli 2023

U kunt nu een aangepast pictogram selecteren voor een recordtype en een aangepaste kleur voor het pictogram voor het recordtype.

### Nieuw veldtype selectievakje

Voorbeeld en productie: 13 juli 2023

U kunt nu een veldtype van het Selectievakje aan de recordtypes van Maestro toevoegen. U kunt een veld van het type Selectievakje gebruiken om één optie voor het selectievakje aan een record toe te voegen. U kunt dit veld gebruiken om een specifiek kenmerk of een specifieke status voor die specifieke record aan te geven. U kunt deze bijvoorbeeld gebruiken als vlag voor het bijhouden van voltooiing, goedkeuring of een ander binair kenmerk voor elke record.

## Week van 26 juni 2023

### Snelle activering van het contextmenu in een tabel

Voorbeeld en productie: 28 juni 2023

We hebben de mogelijkheid ingeschakeld om het contextafhankelijke menu te activeren door met de rechtermuisknop ergens in een recordrij te klikken wanneer de records in de tabelweergave of een recordtype worden weergegeven. U kunt nu snel een koppeling naar de pagina Details van de record weergeven, verwijderen of kopiëren wanneer u het contextmenu opent vanuit een willekeurige locatie in de tabelweergave van een recordtype. Voorafgaand aan deze verbetering, was het contextafhankelijke menu toegankelijk slechts van het Meer menu in de kolom van de Naam van een verslag.

## Week van 19 juni 2023

### Recordveldnamen zijn uniek

We hebben nu de eis ingevoerd dat de veldnamen van een Maestro-recordtype unieke namen moeten hebben. Velden die tot verschillende recordtypen behoren, hoeven geen unieke naam te hebben.

## Week van 5 juni 2023

### Connect Maestro-records met Workfront-projecten

Voorbeeld en productie: 5 juni 2023

U kunt nu een Maestro-record verbinden met Workfront-projecten. U moet een verbindingstype van Maestro tot stand brengen verslag om de verbinding tussen Maestro verslagen en de projecten van Workfront te vestigen. Dan, kunt u om het even welke verslagen Maestro van alle andere verslagtypes met het schakelaarverslag verbinden gebruikend het gebied van de Verhouding. Overweeg het volgende:

* U moet een type van schakelaarverslag voor Workfront voor elke Werkruimte hebben.
* U kunt veelvoudige verslagen Maestro met het zelfde project van Workfront verbinden, en veelvoudige projecten aan het zelfde verslag Maestro.
* U kunt geen projecten bewerken in Maestro. Alle projectwijzigingen die in Workfront worden uitgevoerd, zijn zichtbaar in Maestro wanneer de gekoppelde records worden gecontroleerd.

## Week van 29 mei 2023

### Vereiste voor het maken van een tijdlijnweergave met twee datums

Voorbeeld en productie: 31 mei 2023

Er moeten ten minste twee datumvelden zijn gekoppeld aan een recordtype om een tijdlijnweergave te maken.
