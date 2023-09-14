---
title: Adobe Maestro-releaseactiviteit
description: Gebruik Maestro om aangepaste objecten, velden en werkruimten te maken.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 0%

---


# Adobe Maestro-releaseactiviteit

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
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

   * [Verbind recordtypen](../maestro/architecture-and-fields/connect-record-types.md)
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