---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Aan de slag met rapporten
description: Rapporten geven inzicht in wat er met gebruikers en het werk gebeurt. Met rapporten kunt u informatie over objecten weergeven in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '3294'
ht-degree: 0%

---

# Aan de slag met rapporten

<!-- Audited: 12/2023 -->

Rapporten geven inzicht in wat er met gebruikers en het werk gebeurt. Met rapporten kunt u informatie over objecten weergeven in Adobe Workfront.

Ga voor meer informatie over objecten en hoe deze kunnen worden gerapporteerd in de Workfront-toepassing naar [Overzicht van Adobe Workfront-objecten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Rapportelementen

Rapporten zijn een combinatie van de volgende drie elementen in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Weergave</td> 
   <td> <li>Bepaalt de kolommen in uw rapport en welke informatie u in elke kolom kunt omvatten.</li> <li>Zie voor informatie over weergaven <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Overzicht van weergaven in Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groepering</td> 
   <td> <li>Hiermee categoriseert u informatie op basis van een gemeenschappelijke informatie en geeft u de resultaten van het rapport onder koppen weer.</li> <li>Zie voor informatie over groepen <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Overzicht van groepen in Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <li>Bepaalt de hoeveelheid informatie die in een rapport wordt weergegeven.</li> <li>Zie voor informatie over filters <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Overzicht van filters</a>.</li> <li>Voor informatie over filtermodifiers, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- en voorwaardenmodificatoren</a>.</li> <li>U kunt filteren door vervangingen te gebruiken, om uw filters algemener te maken en hen meer flexibiliteit van gebruik te geven.</li> <li>Voor informatie over het gebruiken van vervangingskaarten in filters, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variabelen van jokerfilter</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wanneer u een nieuw filter, een nieuwe weergave of een nieuwe groepering in een lijst selecteert, blijft die selectie behouden, zelfs als u zich afmeldt bij Workfront of uw browser sluit.

Voor informatie over rapportelementen, zie [Elementen rapporteren: filters, weergaven en groepen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Om uw rapporten te verbeteren, kunt u de volgende elementen toevoegen:

* Een grafiek: een visuele weergave van de resultaten in uw rapport.\
  Voor informatie over grafiekrapporten, zie [Een diagram toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Een matrixgroepering: vat de informatie van het rapport in een bijeengevoegde lijstformaat samen.\
  Zie voor informatie over matrixrapporten [Een matrixrapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Een vraag: een open filter dat u kunt aanpassen en toepassen verschillend telkens als u het rapport in werking stelt.\
  Voor informatie over herinneringen, zie [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

Wanneer het bouwen van een rapport, kunt u om het even welk van deze elementen individueel in de rapportbouwer wijzigen.

Een andere manier om de relevantie van de informatie in uw rapporten te verbeteren, is door voorwaardelijke opmaak toe te passen op uw weergaven.\
Zie voor informatie over het gebruik van voorwaardelijke opmaak [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Systeemrapporten

Workfront biedt verschillende systeemrapporten die standaard in uw systeem worden geladen.\
Na het invoeren van informatie in uw systeem kunt u deze rapporten gebruiken om de informatie visueel weer te geven.

Voor meer informatie over hoe te om tot systeemrapporten toegang te hebben en welke systeemrapporten beschikbaar zijn, zie [Ingebouwde Adobe Workfront-rapporten gebruiken](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Rapporten maken

Naast de systeemrapporten die Workfront levert, kunt u ook uw eigen aangepaste rapporten maken die voldoen aan de behoeften van uw organisatie.

Als u een rapport wilt maken, kunt u een van de volgende handelingen uitvoeren:

* Maak een volledig nieuw rapport.
* Kopieer een bestaand rapport.\
  U moet minstens toestemming van de Mening hebben om een rapport te kopiëren dat door iemand anders wordt gecreeerd. Voor meer informatie over het kopiëren van een rapport raadpleegt u [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Voor informatie over het maken van rapporten raadpleegt u [Overzicht van kalenderrapporten](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

### Vereisten voor het maken van rapporten {#prerequisites-for-creating-reports}

* U moet een licentie voor abonnementen (huidige licenties) of een standaardlicentie (nieuwe licenties) hebben om uw eigen rapporten te maken.\
  Voor informatie over de Workfront-licentietypen raadpleegt u [Overzicht van licenties](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) voor de huidige vergunningen, en [Overzicht van nieuwe licenties](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) voor de nieuwe vergunningen.

* Uw Workfront-beheerder moet u toegang geven tot Rapporten bewerken op uw Toegangsniveau.\
  Voor informatie over het verlenen van toegang tot Edit rapporten, zie [Toegang verlenen tot rapporten, dashboards en kalenders](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Uw Workfront-beheerder moet u toegang geven tot Filters, Weergaven en Groepen bewerken in uw toegangsniveau.

  Voor informatie over het verlenen van toegang tot Edit filters, meningen, en groeperingen, zie [Toegang verlenen tot filters, weergaven en groepen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* U moet één object definiëren waarover u wilt rapporteren. Rapporten zijn objectspecifiek in Workfront en u moet eerst een objecttype selecteren voordat u het rapport kunt gaan samenstellen. U kunt alleen rapporteren over objecten die beschikbaar zijn in de Workfront-interface.

### Eigendom rapporteren {#report-ownership}

Wanneer u een rapport in Workfront creeert, wordt u de standaardeigenaar van het rapport en het toont in uw Mijn sectie van Rapporten. U kunt de eigenaar van een rapport niet wijzigen.

Wanneer u een rapport kopieert, wordt u automatisch de eigenaar van het gekopieerde rapport.
Voor informatie over het kopiëren van rapporten raadpleegt u [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

U kunt zien wie eigenaar is van een rapport door de **Ingevoerd door** veld.

![Ingevoerd op veld](assets/nwe-entered-by-350x218.png)

### Rapporten maken in de builderinterface {#create-reports-in-the-builder-interface}

Wij adviseren dat u de interface van het rapportgebouw eerst gebruikt om een nieuw rapport te bouwen. De interface biedt een gestroomlijnde reeks hulpmiddelen aan die u door het samenstellen van elementen lopen om het gewenste rapport tot stand te brengen. U hebt objecten en velden die u kunt selecteren in lijsten en toevoegen aan alle rapportelementen.\
Voor meer informatie over het creëren van rapporten in de interface van het rapportgebouw, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Voor een lijst met objecten die u kunt melden, raadpleegt u de [Objecten rapporteren](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects) in het artikel [Overzicht van Adobe Workfront-objecten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Voor meer informatie over de gebieden die u in rapporten kunt tonen, zie [Woordenlijst met Adobe Workfront-terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Rapporten maken in de tekstmodus {#create-reports-in-text-mode}

Mogelijk kunt u bepaalde velden in de builderinterface niet vinden, maar deze zijn wel beschikbaar in de API.\
Zie het artikel voor informatie over welke velden beschikbaar zijn in de API [API Explorer](../../../wf-api/general/api-explorer.md).

Zie het artikel voor informatie over het gebruik van de API Explorer [De API Explorer gebruiken](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>U kunt niet in de interface van Workfront op voorwerpen rapporteren die niet beschikbaar in de rapportbouwer zijn. Nochtans, kunt u over gebieden rapporteren verbonden aan de voorwerpen in de rapportbouwer als die gebieden door API beschikbaar zijn. Hiervoor moet u de interface Tekstmodus gebruiken.

Met de Tekstmodus kunt u complexere weergaven, filters, groepen en aanwijzingen maken door het mogelijk te maken velden te gebruiken die niet beschikbaar zijn in de standaardmodusinterface.

#### terminologie voor tekstmodus {#text-mode-terminology}

U moet een specifieke syntaxis gebruiken om de interface van de Wijze van de Tekst van Workfront te gebruiken.

Zie voor meer informatie over de Workfront-syntaxis voor de tekstmodus [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Berekende kolommen, voorwaardelijke opmaak en andere toepassingen van de tekstmodus {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Buiten de rapportage over velden die niet beschikbaar zijn in de builderinterface, kunt u de Tekstmodus gebruiken om berekeningen of vergelijkingen tussen bepaalde velden weer te geven.

Voor een lijst van de gemeenschappelijkste toepassingen van de Wijze van de Tekst in een rapport, zie [Overzicht van veelvoorkomende toepassingen voor de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Zie voor informatie over het opnemen van berekende aangepaste gegevens in rapporten [Berekende aangepaste gegevens in rapporten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Zie voor informatie over het vergelijken van velden in voorwaardelijke opmaak [Velden in voorwaardelijke opmaak vergelijken](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

In rapporten kunt u ook naar verzamelingsvelden verwijzen met de tekstmodus.\
Voor informatie over het gebruiken van de Wijze van de Tekst om inzamelingsinformatie in een rapport te tonen, zie [Referentieverzamelingen in een rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Voorbeelden van tekstmodi {#text-mode-samples}

We hebben een bibliotheek met voorbeelden van de meest gebruikte weergaven, filters en groepen die u kunt maken met de tekstmodus.

Raadpleeg het artikel als u door deze bibliotheek wilt bladeren en enkele voorbeelden wilt gebruiken die we aanbieden [Voorbeelden van aangepaste weergaven, filters en groepen: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## De tabbladen van een verslag

Een rapport kan verscheidene lusjes bevatten wanneer u het rapport in de interface in werking stelt.

Zie het artikel voor informatie over het uitvoeren van een rapport [Een rapport uitvoeren](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Op elk lusje, toont de informatie u in het rapport in lichtjes verschillende formaten omvat. Kies de indeling die het best aansluit bij de behoeften van uw organisatie.

U kunt om het even welk lusje tot het standaardlusje van het rapport maken. Het standaardlusje is het eerste lusje dat toont wanneer u de naam van een rapport klikt om het te openen, en het is het lusje dat toont wanneer u het rapport op een dashboard plaatst.

### Tabblad Details {#details-tab}

Het lusje van Details van een rapport toont het voorwerp van de rapporten en de attributen die u voor dat voorwerp in een lijstvorm kiest. Elk rapport heeft een tabblad Details.

>[!IMPORTANT]
>
>De informatie in het lusje van Details kan verschillend van het lusje van de Grafiek tonen dat op uw tijdzone wordt gebaseerd.\
>Bijvoorbeeld, voltooide een gebruiker in Californië een taak om 9:30 pm PST op 12 Februari. Wanneer een gebruiker in New York een rapport bekijkt dat deze taakvoltooiing omvat, toont de Ware Datum van de Voltooiing als Februari 13 in zowel het lusje van Details als de details van de Grafiek omdat het om 12:30 UUR EST op 13 Februari werd voltooid. Nochtans, in de grafiek, is het inbegrepen in de 12 van Februari groepering tot u het grafiekelement uitbreidt.

### Tabblad Samenvatting {#summary-tab}

Rapporten die een groepering bevatten, hebben een tabblad Overzicht.

Dezelfde informatie die wordt weergegeven in de vorm van een lijst op het tabblad Details, wordt samengevat en samengevoegd op basis van de groepen in het rapport op het tabblad Overzicht.

Zie voor informatie over groepen [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Het tabblad Matrix {#matrix-tab}

Rapporten die een Matrixgroepering bevatten, hebben een tabblad Matrix.

Dezelfde informatie die op het tabblad Details in de lijstindeling wordt weergegeven, wordt weergegeven in een tabelindeling, gegroepeerd op de groepen in het rapport op het tabblad Matrix.

Wanneer u een Matrix-groepering toevoegt aan een rapport, wordt het tabblad Samenvatting vervangen door het tabblad Matrix.

Raadpleeg het artikel voor informatie over het samenstellen van een Matrixgroep [Een matrixrapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Tabblad Diagram {#chart-tab}

Rapporten met een diagram hebben een tabblad Diagram.

Overweeg een grafiek in uw rapporten op te nemen voor onechte dashboards voor uw managers. Grafieken zijn een beknopte manier om de informatie in een rapport weer te geven. U kunt een grafiekelement uitbreiden door het te klikken om de punten te tonen inbegrepen in dat element.

>[!IMPORTANT]
>
>Wanneer u een grafiekelement klikt, kan de uitgebreide informatie verschillend van de grafiek tonen die op uw tijdzone wordt gebaseerd.\
>Bijvoorbeeld, voltooide een gebruiker in Californië een taak om 9:30 pm PST op 12 Februari. Wanneer een gebruiker in New York een rapport bekijkt dat deze taakvoltooiing omvat, toont de Ware Datum van de Voltooiing als Februari 13 in zowel het lusje van Details als de details van de Grafiek omdat het om 12:30 UUR EST op 13 Februari werd voltooid. Nochtans, in de grafiek, is het inbegrepen in de 12 van Februari groepering tot u het grafiekelement uitbreidt.

Zie het artikel voor informatie over het samenstellen van een rapport met een grafiek [Een diagram toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Tabblad Vragen {#prompts-tab}

Rapporten met een vraag hebben een tabblad Vragen.

Een herinnering staat u toe om een filter aan een rapport toe te voegen telkens als u het rapport in werking stelt. Wanneer u een herinnering aan het rapport toevoegt, wordt het lusje van Vragen automatisch het standaardlusje van het rapport. Dit kan niet worden gewijzigd in een ander tabblad.

Voor informatie over het bouwen van een herinnering voor een rapport, zie het artikel [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Rapporten delen

Nadat u een rapport hebt gemaakt, kunt u het rapport delen met andere gebruikers.

### Het delen toestemmingen aan een rapport geven {#give-sharing-permissions-to-a-report}

U kunt een andere gebruiker toestemming geven om een rapport dat u maakt, weer te geven of te beheren. U kunt een andere gebruiker een machtigingsniveau geven dat gelijk is aan of lager is dan dat van u. U kunt een rapport ook openbaar maken gebruikend het delen toestemmingen. Voor informatie over het delen van een rapport raadpleegt u [Een rapport delen in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Een rapportlevering plannen {#schedule-a-report-delivery}

U kunt een rapport voor levering plannen. De gebruikers u het rapport met deelt ontvangen een e-mail met een gehechtheid van de rapportresultaten. De bijlage kan de volgende notaties hebben:

* HTML
* PDF
* Excel
* .TSV

Voor informatie over het plannen van een rapportlevering, zie [Overzicht van levering rapporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### De resultaten van een rapport exporteren {#export-the-results-of-a-report}

U kunt de resultaten van een rapport exporteren naar de volgende bestandsindelingen:

* PDF
* Excel (.xls en .xlsx formaten)
* Door tabs gescheiden

Voor informatie over het exporteren van de resultaten van een rapport raadpleegt u [Gegevens exporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Nadat het rapport naar een van deze indelingen is geëxporteerd, kunt u het rapport delen met andere gebruikers door het als bijlage te e-mailen of af te drukken.

### Een rapport toevoegen aan een dashboard {#add-a-report-to-a-dashboard}

U kunt een rapport aan een dashboard toevoegen en het dashboard met andere gebruikers delen. Voor informatie over het toevoegen van rapporten aan een dashboard, zie [Een rapport toevoegen aan een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Kalenders maken

Als u de gegevens in een kalenderindeling wilt weergeven, kunt u kalenders maken in plaats van rapporten.

Voor informatie over bouw en het gebruiken van kalenders, zie [Overzicht van kalenderrapporten](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Rapportgebruik

Nadat u rapporten hebt gemaakt en deze met andere gebruikers hebt gedeeld, kunt u bijhouden hoe vaak deze rapporten worden gebruikt.
Raadpleeg het artikel voor informatie over het gebruik van rapporten, zoals hoe vaak ze worden weergegeven, door welke gebruiker en op welke dashboards ze worden weergegeven [Overzicht van rapportgebruik](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Algemene termen die worden gebruikt in verband met rapporten

De volgende termen worden gebruikt voor Workfront-rapporten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Term of woordgroep</strong> </th> 
   <th><strong>Definitie</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Geavanceerde opties</td> 
   <td> <p>Verwijst naar de verbinding op het lusje van Kolommen (Mening) van de rapportbouwer die de capaciteit verstrekt om het volgende te doen:</p> 
    <ul> 
     <li>Stel de voorwaardelijke opmaak van de kolommen voor tekst en afbeeldingen in op basis van criteria die u selecteert.</li> 
     <li>Geef de kolom een nieuwe naam.</li> 
     <li>Maak de waarden in uw kolom op.</li> 
    </ul> <p>U kunt bijvoorbeeld alle bovenliggende taken vet weergeven of de Geplande voltooiingsdatum rood weergeven als de taak te laat is.</p> </td> 
  </tr> 
  <tr> 
   <td>Kenmerk</td> 
   <td> Het veld van een object zoals gedefinieerd in de database. Deze wordt gebruikt in een tekstmodusexpressie. <br>Het veld Status wordt bijvoorbeeld weergegeven als <em>status</em> bij gebruik in een tekstmodusexpressie. </td> 
  </tr> 
  <tr> 
   <td>Bean of JavaBean</td> 
   <td>Een Bean vertegenwoordigt een herbruikbaar-programmeringselement. De term Bean identificeert relaties tussen verschillende objecten in de Workfront-toepassing. Het is belangrijk dat u vertrouwd bent met deze relaties wanneer u aanvullende kenmerken van een object probeert weer te geven die niet beschikbaar zijn in de standaard rapportagegereedschappen.</td> 
  </tr> 
  <tr> 
   <td>Builder-interface of -Report Builder</td> 
   <td>De interface van de Bouwer is de reeks drop-down menu's die gebieden bevatten die in de lusjes van Kolommen (Mening), van de Filter, en van de Groepering worden getoond. Het verstrekt een intuïtieve afbeelding van de verhoudingen van Bean helpen in het identificeren van de kolommen in een mening, de criteria van een filter, en de gemeenschappelijke attributen van een groepering.</td> 
  </tr> 
  <tr> 
   <td>Camel Case</td> 
   <td> <p>Camel Case verwijst naar een specifieke manier om programmeringselementen aan koord samen te schrijven multi-word attributen. Wanneer u een kenmerk in Camel Case typt, is de eerste letter van het eerste woord in kleine letters geschreven, is er geen ruimte tussen de woorden en is de eerste letter van elk volgend woord in hoofdletters.</p> <p>Thuisgroep wordt bijvoorbeeld geschreven zoals <em>homeGroup</em>, bronnenpool <em>resourcePool</em>en de werkelijke begindatum <em>actualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Diagram</td> 
   <td> <p>Een lusje binnen de rapportaannemer, een rapportlusje, nadat u het rapport, evenals een facultatief element van een rapport opslaat dat u toestaat om een grafiek aan om het even welk rapport toe te voegen. U moet een Groepering in het rapport bepalen alvorens u een grafiek kunt tot stand brengen.</p> <p>Hier volgt een overzicht van typen grafieken die aan elk rapport kunnen worden toegevoegd:<br></p> 
    <ul> 
     <li>Kolom</li> 
     <li>Balk</li> 
     <li>Schijf</li> 
     <li>Lijn</li> 
     <li>Gage</li> 
     <li>Bubble</li> 
    </ul> <p>Zie het artikel voor meer informatie over het toevoegen van grafieken aan rapporten <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Een diagram toevoegen aan een rapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Details</td> 
   <td>Dit is één van de lusjes van een rapport, nadat u sparen het rapport. Het toont de bevindingen van uw rapport, dat in de mening en de groepering van uw keus wordt getoond.</td> 
  </tr> 
  <tr> 
   <td>Uitdrukking</td> 
   <td>Een uitdrukking is een geschreven formule in de Wijze van de Tekst om informatie over te brengen die moet worden gezocht of worden getoond wanneer het gebruiken van de interface van de Wijze van de Tekst. Het is doorgaans één regel in een grotere instructie Tekstmodus.</td> 
  </tr> 
  <tr> 
   <td>Velden</td> 
   <td> <p>Verwijst naar de kenmerken van uw objecten. De status is bijvoorbeeld een veld voor projecten, taken of problemen. 'Portfolio Manager' is een veld voor het object Portfolio.</p> <p>U kunt ook aangepaste velden hebben die u zelf maakt en aan aangepaste formulieren toevoegt.<br>Zie het artikel voor informatie over het maken van aangepaste formulieren <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Veldnaam </td> 
   <td>De waarde van een attribuut dat in een mening wordt getoond, of in de voorwaarde van een filter, of als gemeenschappelijk element van een groepering wordt gebruikt. De opties voor Veldnaam zijn afhankelijk van de optie Veldbron.</td> 
  </tr> 
  <tr> 
   <td>Veldbron </td> 
   <td>De waarde van een object dat wordt weergegeven in een weergave, of wordt gebruikt in de voorwaarde van een filter, of als het gemeenschappelijke element van een groep. De opties in de Bron van het Gebied zijn afhankelijk van het objecten type van het element UI dat wordt gecreeerd. Met de veldbron kunt u verwijzen naar kenmerken van andere objecten dan het objecttype van het interface-element.</td> 
  </tr> 
  <tr> 
   <td>Filter</td> 
   <td>A main report element that determines which results display in the report.</td> 
  </tr> 
  <tr> 
   <td>Formulier </td> 
   <td>Wordt door elkaar gebruikt met "Aangepast formulier". Velden en secties worden toegevoegd aan formulieren. Deze worden vervolgens gekoppeld aan een object om het aantal velden dat u aan een object kunt koppelen, uit te breiden.</td> 
  </tr> 
  <tr> 
   <td>Groepering </td> 
   <td>Een hoofdrapportelement dat aangeeft hoe een lijst met resultaten wordt georganiseerd. De groepering leidt tot horizontale bars door het rapport om de resultaten te groeperen door gemeenschappelijke die attributen worden bepaald wanneer het creëren van het. Groepen worden gebruikt in Matrixrapporten om gegevens samen te voegen, evenals in grafieken, om de assen van grafieken te bepalen.</td> 
  </tr> 
  <tr> 
   <td>Object- of objecttype</td> 
   <td> Een object is een Workfront-toepassingselement (bijvoorbeeld Project, Task, Group, Company, Filter). Het Type van Objecten wordt gebruikt wanneer het creëren van een nieuw rapport, een mening, een filter, of het groeperen om te identificeren welk voorwerp de nadruk van het rapport is. Rapporten kunnen slechts één objecttype hebben, dat het belangrijkste object van het rapport is.<br>In hetzelfde rapport kan naar bovenliggende objecten worden verwezen.<br>Zie voor meer informatie over de hiërarchie van objecten de sectie 'De onderlinge afhankelijkheid en hiërarchie van objecten begrijpen' in het artikel <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Overzicht van Adobe Workfront-objecten</a>.</td> 
  </tr> 
  <tr> 
   <td>Vragen</td> 
   <td> <p>Een facultatief rapportelement dat aan een rapport kan worden toegevoegd wanneer u een verschillende filter moet gebruiken telkens als u het rapport in werking stelt.</p> <p>Voor informatie over herinneringen, zie <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Een vraag toevoegen aan een rapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Voorwaarde- of kwalificatiebepalingen</td> 
   <td> <p>Dit gebied verschijnt op de volgende gebieden van een rapport:</p> 
    <ul> 
     <li>Op het tabblad Filter</li> 
     <li>Het scherm Geavanceerde opties voor de kolom in de Kolommen (Mening) tabel. Als u een kwalificatie definieert, kunt u de veldnaam vergelijken met een ander veld of een andere waarde.</li> 
     <li> In een aangepaste prompt<br><p>Voor informatie over herinneringen, zie <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Een vraag toevoegen aan een rapport</a>.</p>.</li> 
    </ul> <p>Wanneer u bijvoorbeeld een filter maakt voor taken met een geplande voltooiingsdatum van vandaag, selecteert u <strong>Gelijk</strong> in uw gebied van de Kwalificatie, en de datum van vandaag op het gebied van de Datum:</p> <p><em>Taak &gt; Geplande Voltooiingsdatum&gt;Gelijk&gt; (huidige datum)</em> </p> <p>In dit scenario is de kwalificatie <strong>Gelijk</strong>.<br>Raadpleeg het artikel voor meer informatie over kwalificatietoetsen <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- en voorwaardenmodificatoren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Rapport </td> 
   <td>De combinatie van een weergave, een filter en (soms) een groep. Het doel van een rapport is gegevens over de interface constant te tonen, informatie te verdelen, en de behoefte te elimineren om het zelfde onderzoek of de vraag op een regelmatige basis in werking te stellen.</td> 
  </tr> 
  <tr> 
   <td>Instructie</td> 
   <td>Bestaat uit verscheidene uitdrukkingen die worden samengesteld om te bepalen welke informatie in een rapport wanneer het gebruiken van de Wijze van de Tekst toont. Een verklaring kan voor een mening, filter, groepering, of voor een Herinnering van de Douane in een rapport worden gecreeerd.</td> 
  </tr> 
  <tr> 
   <td>Samenvatting</td> 
   <td>Dit is één van de lusjes van een rapport, nadat u sparen het rapport. Dit lusje wordt gecreeerd slechts wanneer u het groeperen voor het rapport bepaalt. Het vat informatie samen die op de groepering wordt gebaseerd die tijdens rapportverwezenlijking wordt bepaald en geeft een snel overzicht van de bijeengevoegde voorwerpen van het rapport. Het toont niet elk voorwerp in het rapport, enkel die die worden bijeengevoegd.</td> 
  </tr> 
  <tr> 
   <td>Interface voor tekstmodus</td> 
   <td>Verstrekt de capaciteit om de code van douanemeningen, filters, groeperingen, en herinneringen tot stand te brengen of te wijzigen die oorspronkelijk door de Interface van de Bouwer worden gecreeerd. Voorgesteld wordt dat rapportelementen eerst worden gemaakt via de Builder-interface en vervolgens worden omgezet in de tekstmodus nadat ze zijn opgeslagen om de codering van geavanceerde weergaven, filters, groepen of aanwijzingen te vereenvoudigen.</td> 
  </tr> 
  <tr> 
   <td>Gebruikersinterface (UI)</td> 
   <td>Verwijst naar de componenten of bouwstenen van wat op het scherm van een gebruiker op om het even welk bepaald ogenblik toont.</td> 
  </tr> 
  <tr> 
   <td>Weergave (of kolommen)</td> 
   <td>Een van de belangrijkste elementen van een verslag. Het identificeert de kolomkopballen die in de lijst van een rapport zullen worden getoond.</td> 
  </tr> 
 </tbody> 
</table>
