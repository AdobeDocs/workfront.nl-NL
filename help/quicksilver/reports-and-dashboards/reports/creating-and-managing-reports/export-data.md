---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Gegevens exporteren
description: U kunt Adobe Workfront-gegevens exporteren uit lijsten, rapporten, dashboards en zoekopdrachten.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2252'
ht-degree: 0%

---

# Gegevens exporteren

<!-- Audited: 5/2025 -->

U kunt Adobe Workfront-gegevens exporteren uit lijsten, rapporten, dashboards en zoekopdrachten.

Enkele redenen voor het exporteren van gegevens zijn:

* U wilt een gedrukte kopie van uw gegevens aan iemand buiten Workfront verstrekken.
* U wilt de resultaten van een rapport als gehechtheid naar een externe gebruiker verzenden.
* U wilt een externe back-up van uw Workfront-gegevens maken.
* Er geldt een limiet voor het weergeven van slechts 2.000 resultaten op één pagina in de Workfront-webtoepassing. Als uw rapport meer dan 2.000 produceert, kunt u het rapport naar om het even welke beschikbare formaten uitvoeren en alle resultaten in het rapport in één lijst bekijken.

U kunt of een rapport manueel, van de interface van Workfront uitvoeren, of u kunt een levering voor een rapport plannen en dat rapport zal naar u op een recentere tijd worden verzonden. Voor meer informatie bij het plannen van geleverde rapporten, zie [&#x200B; de leveringsoverzicht van het Rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

De informatie in dit artikel is niet van toepassing op de volgende exporttransacties:

* Gegevens uit grafiekrapporten exporteren.

  Voor meer informatie over het uitvoeren van een grafiekrapport, zie [&#x200B; een grafiek aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

* Informatie exporteren uit het Gantt-diagram.

  Voor meer informatie over het uitvoeren van de grafiek van Gantt, zie [&#x200B; de Grafiek van Gantt naar PDF &#x200B;](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md) uitvoeren.

* Informatie exporteren vanuit de bronnenplanner.

  Voor meer informatie over het uitvoeren van de informatie van de Planner van het Middel, zie &quot;Optie van de Uitvoer&quot;in [&#x200B; het navigatieoverzicht van de Planner van het Middel &#x200B;](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Licht</p>
      <p>Controleren</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Geef rapporten of meer toegang tot rapporten, dashboards en kalenders om rapporten te exporteren</p> <p>Toegang tot de objecten die u in een lijst weergeeft of vergroten om de lijst te exporteren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De mening of hogere toestemmingen aan een rapport of een dashboard om het rapport of het dashboard uit te voeren</p> <p>Geef de objecten die u in een lijst weergeeft of hoger de machtigingen weer om de lijst te exporteren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Het rapport moet worden gemaakt voordat u de gegevens kunt exporteren.

Voor meer informatie bij het creëren van rapporten, zie [&#x200B; een douanerapport &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) of [&#x200B; creëren een exemplaar van een rapport &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Exportindelingen en -beperkingen

### Exportindelingen {#export-formats}

De informatie kan in de volgende formaten worden uitgevoerd:

* PDF (liggend of staand)
* Excel
* Excel (.xlsx)
* Door tabs gescheiden

>[!NOTE]
>
>U kunt dashboards afdrukken of alleen exporteren naar een PDF-bestand.

### Exportlimieten {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Er gelden verschillende beperkingen voor de manier waarop rapporten in Workfront worden weergegeven en voor de manier waarop ze via handmatige export, een geleverd rapport of de API worden geëxporteerd.

* **50.000 cellen:** het maximumaantal cellen die in een rapportuitvoer voor de dossiers van Excel worden toegestaan.
* **50.000 rijen:** het aantal rijen van gegevens toegestaan in een rapportuitvoer voor PDF en het Lusje Gescheiden dossiers.

   * Voor de dossiers van Excel, is deze grens **65.000 rijen**.
   * Voor Excel (.xlsx) dossiers, is deze grens **100.000 rijen**.
   * Deze grenzen sluiten de kolomrubrieken, evenals rijen voor groepen in het rapport uit. Bijvoorbeeld, als u 6 groeperingen in een rapport hebt, en 50.000 rijen van gegevens, zal het uitgevoerde dossier 50.000 rijen hebben.

  >[!IMPORTANT]
  >
  >Het uitvoeren van een rapport dat een inzamelingsverwijzing binnen een kolom omvat kan in een fout resulteren, zelfs als het rapport anders binnen de vermelde uitvoergrenzen is. Als de verzameling waarnaar wordt verwezen te groot is, wordt het exportproces onderbroken en resulteert dit in een fout.
  >
  >U voorkomt deze fout door kolommen die verwijzen naar grote verzamelingen uit te sluiten of de grootte van de verzamelingen waarnaar wordt verwezen, te reduceren voordat u gaat exporteren.

  Als uw rapport meer items bevat dan deze limiet, wordt een fout weergegeven als u wilt dat het exporteren niet is gelukt. Verlaag het aantal items dat u op het scherm ziet tot een getal dat kleiner is dan of gelijk is aan deze limiet om de resultaten te kunnen exporteren.

  Als uw rapport meer dan 50.000/65.000/100.000 rijen heeft en u alle gegevens wilt uitvoeren, adviseren wij dat u filters of herinneringen gebruikt om kleinere ladingen gegevens te verkrijgen, en veelvoudige uitvoeren uit te voeren.

  Voor informatie bij het gebruiken van filters, zie [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Voor informatie over het gebruiken van herinneringen, zie [&#x200B; een herinnering aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

* Deze grenswaarden gelden voor:

   * Een handmatige export van een rapport.
   * Een gepland rapport.
   * Een export via een API-integratie.
   * Gegevens geëxporteerd via een trap-start.

     Voor meer informatie over het uitvoeren van gegevens via schop-begin, zie [&#x200B; Gegevens van de Uitvoer van Adobe Workfront via Kick-Begarts &#x200B;](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >U kunt 50.000 rijen exporteren in een startbestand, hoewel u de gegevens alleen kunt exporteren naar een Excel-bestand.

   * Gebruiksinformatie voor een project exporteren.

     Voor meer informatie over het uitvoeren van gebruiksinformatie voor een project, zie [&#x200B; Overzicht van het rapport van het Gebruik van het Middel &#x200B;](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10MB dossiergrootte:** de groottelimiet van het Dossier voor om het even welk uitgevoerd rapport dat voor levering wordt gepland. Als een geëxporteerd bestand dat is gekoppeld aan een e-mailbericht groter is dan 5 MB, wordt een koppeling waarnaar het bestand kan worden gedownload per e-mail verzonden in plaats van het bijgevoegde geëxporteerde rapport.
* **65.530 hyperlinks:** dit is een grens die door Excel op documenten wordt opgelegd die meer dan 65.530 hyperlinks bevatten. Deze documenten kunnen niet worden geopend wanneer ze handmatig worden geëxporteerd of in een bezorgd rapport worden verzonden. Een Excel-document kan slechts 200 rijen gegevens bevatten, maar als het document meer dan 65.530 koppelingen bevat, wordt het document niet geopend. Deze limiet geldt alleen voor Excel-bestanden en niet voor de andere ondersteunde indelingen.
* **256 kolommen**: Dit is een grens die door Excel op documenten wordt opgelegd die meer dan 256 kolommen bevatten. Deze documenten kunnen niet handmatig worden geëxporteerd of in een bezorgd rapport worden verzonden. Deze limiet geldt alleen voor Excel-bestanden en niet voor de andere ondersteunde indelingen.

  >[!IMPORTANT]
  >
  >Het uitvoeren van een rapport dat een kolom van Rapporten omvat kan in een fout resulteren zelfs als het rapport anders binnen de vermelde uitvoergrenzen is.
  >
  >Als u de de uitvoereigenschap gebruikt om een rapport te delen dat een kolom van Rapporten met anderen bevat, denk na delend het rapport door het openbaar te maken in plaats daarvan. Voor meer informatie bij het maken van een rapport openbaar, zie [&#x200B; een rapport in Adobe Workfront &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md) delen.
  >
  >Als u de exportfunctie gebruikt om gegevens extern te evalueren, raden we u aan in plaats daarvan Workfront Data Connect te gebruiken. Voor meer informatie, zie [&#x200B; de Gegevens van Workfront verbinden overzicht &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Als u probeert gegevens te exporteren die de limiet overschrijden, ontvangt u mogelijk niet alle verwachte gegevens in de exportbewerking. In plaats daarvan wordt een gewijzigd verslag binnen de limiet opgesteld.

Bovendien worden rapporten die langer dan 60 minuten duren, gestopt.

Neem contact op met de technische ondersteuning van Workfront als u problemen hebt met uw limiet.

## Gegevens exporteren

### Gegevens exporteren uit een rapport of lijst {#export-data-from-a-report-or-list}

1. Ga naar het rapport of de lijst die u wilt exporteren.
1. Selecteer de items die u wilt exporteren. Als u afzonderlijke items selecteert, worden alleen de geselecteerde items geëxporteerd.

   Selecteer bijvoorbeeld in een project de taken die u wilt exporteren.

   of

   Laat alle items uitgeschakeld om de volledige lijst te exporteren.

1. Klik **Uitvoer**, dan selecteer een formaat.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![Export dashboard note](assets/nwe-dashboard-export-note-350x271.png)
   -->

   of

   Klik het **pictogram van de Uitvoer** het pictogram van de Uitvoer ![, dan selecteer een formaat.](assets/export-icon-nwe.png)

   Welke opties beschikbaar zijn voor PDF-export, is afhankelijk van de instellingen voor Landinstelling e-mail in uw Workfront-gebruikersinstellingen:

   * Noord-Amerika - Letter - Landscape, Letter - Portrait, Other Sizes

   * Alle locaties buiten Noord-Amerika - A4 - Liggend, A4 - Staand, andere grootten

1. (Voorwaardelijk) Afhankelijk van het besturingssysteem dat u gebruikt, hebt u mogelijk de mogelijkheid om het bestand te openen of op te slaan. Open het bestand met de bijbehorende toepassing of sla het op de vaste schijf op.
1. Om te begrijpen hoe de informatievertoningen in het uitgevoerde dossier, blijven lezend het sectie [&#x200B; gebruiken het uitgevoerde document &#x200B;](#use-the-exported-document) in dit artikel.

### Gegevens exporteren uit een dashboard {#export-data-from-a-dashboard}

U kunt de gegevens van een dashboard afdrukken of exporteren als een PDF-bestand.

Voor meer informatie over het uitvoeren van gegevens van een dashboard, zie [&#x200B; een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md) uitvoeren.

## Het geëxporteerde document gebruiken {#use-the-exported-document}

In de volgende secties wordt beschreven hoe informatie in een geëxporteerd bestand wordt weergegeven:

* [&#x200B; Namen van het Dossier &#x200B;](#file-names)
* [&#x200B; Titels &#x200B;](#titles)
* [&#x200B; Tijdstempels &#x200B;](#timestamps)
* [&#x200B; Formatterend &#x200B;](#formatting)
* [&#x200B; Verbindingen &#x200B;](#links)
* [Branding](#branding)

### Bestandsnamen {#file-names}

Of u nu een lijst met objecten of een rapport exporteert, het geëxporteerde bestand heeft een bestandsnaam en een titel. U kunt het geëxporteerde bestand op uw computer vinden door naar de bestandsnaam te verwijzen. De titel van het rapport geeft gebruikers een indicatie van wat het geëxporteerde bestand vertegenwoordigt wanneer u het met hen deelt.

#### Bestandsnamen voor geëxporteerde lijsten {#file-names-for-exported-lists}

Wanneer u een lijst met objecten exporteert, wordt het objecttype in het geëxporteerde bestand weergegeven in de bestandsnaam en in de titel van de lijst.

Wanneer u een lijst van taak of kwesties uitvoert, kan de **Naam van het Dossier** één van het volgende zijn:

* Wanneer u taak en uitgiftenlijsten in een project uitvoert:

   * *The_project_name_Exported_Tasks* (*in PDF, Excel, Excel (.xlsx), of Door het Lusje afgebakende formaten)*
   * *The_project_name_Exported_Issues* (*in PDF, Excel, Excel (.xlsx), of Door tabs afgebakende formaten)*

* Wanneer u taak en uitgiftenlijsten in een taak (subtaken) uitvoert:

   * **The_project_name_the_task_name_Exported_Tasks** (*in PDF, Excel, Excel (.xlsx), of Door tabs afgebakende formaten)*
   * **The_project_name_the_task_name_Exported_Issues** (*in PDF, Excel, Excel (.xlsx), of Door tabs afgebakende formaten)*

Wanneer u een lijst met andere objecten uit een project naar een PDF-bestand exporteert, geeft de bestandsnaam van het geëxporteerde document het type objecten aan dat u hebt geëxporteerd.\
De bestandsnaam kan bijvoorbeeld als volgt zijn:

* *Exported_Users*, wanneer het uitvoeren van het lusje van Mensen op het project (*in PDF, Excel, Excel (.xlsx), of Door het Lusje afgebakende formaten)*
* *Exported_Risks*, wanneer het uitvoeren van een lijst van Risken op het project (*in PDF, Excel, Excel (.xlsx), of Door tabs afgebakende formaten)*

#### Bestandsnamen voor geëxporteerde rapporten {#file-names-for-exported-reports}

Wanneer u een rapport exporteert, krijgt het geëxporteerde rapport de volgende bestandsnaam:

*The_report_name* (*in PDF, Excel, Excel (.xlsx), of Door het Lusje afgebakende formaten)*

### Titels {#titles}

Wanneer u een lijst met objecten exporteert, heeft alleen het bestand in de PDF-indeling een titel. Als u een lijst of een rapport naar Excel, Excel (.xlsx), of Door tabs gescheiden formaten uitvoert, heeft het dossier geen titel.

#### Titels voor geëxporteerde lijsten {#titles-for-exported-lists}

Wanneer u taak- en uitgavelijsten in een project exporteert naar een PDF-bestand, is de titel van het geëxporteerde document een van de volgende:

* *naam van het Project - de Uitgevoerde Taken*
* *naam van het Project - de Uitgevoerde Kwesties*

Wanneer u taak- en uitgavelijsten in een taak exporteert naar een PDF-bestand, is de tegel van het geëxporteerde document een van de volgende:

* *naam van het Project - de Naam van de Taak - Uitgevoerde Taken*
* *naam van het Project - de Naam van de Taak - Uitgevoerde Kwesties*

Wanneer u een lijst met andere objecten uit een project exporteert naar een PDF-bestand, geeft de titel van het geëxporteerde document het type objecten aan dat u hebt geëxporteerd.\
De titel kan bijvoorbeeld als volgt zijn:

* *Uitgevoerde Gebruikers*, wanneer het uitvoeren van het lusje van Mensen op het project.
* *Uitgevoerde Risken*, wanneer het uitvoeren van een lijst van Risken op het project.

#### Titels voor geëxporteerde rapporten {#titles-for-exported-reports}

Een rapport dat naar een PDF-bestand wordt geëxporteerd, krijgt een titel.

Als het rapport wordt uitgevoerd naar Excel, Excel (.xlsx) of Door tabs gescheiden formaten, zal het uitgevoerde rapport geen titel hebben. De titel van het geëxporteerde bestand is de naam van het rapport zoals deze wordt weergegeven in de Workfront-webtoepassing.

Als het rapport een beschrijving heeft, wordt het opgenomen in het geëxporteerde bestand.

### Tijdstempels {#timestamps}

Er wordt een tijdstempel weergegeven in het geëxporteerde document vanuit de context van de gebruiker die het item heeft geëxporteerd.

De tijdstempel bevat:

* Datum
* Tijd
* Tijdzone waarop het item is geëxporteerd

Afhankelijk van het type document dat u exporteert, worden tijdstempels op verschillende locaties weergegeven:

* **PDF:** Tijdstempels worden getoond op footer van elke pagina en in het dossier - naam.
* **Excel:** Tijdstempels worden getoond in het dossier - naam.

### Opmaak {#formatting}

Wanneer u een project naar PDF uitvoert, worden om het even welke subtaken getoond zoals ingesprongen aan hun oudertaken. Bovenliggende taken worden niet samengevouwen in geëxporteerde lijsten.

U ontvangt altijd het standaardlusje van een rapport wanneer een rapport voor een levering wordt verzonden of gepland, tenzij het rapport een speciale mening heeft.

Als uw rapport een speciale opmaak heeft in de webtoepassing, moet het rapport worden geleverd met de speciale opmaak wanneer de tabbladen Details en Matrix worden geleverd, alleen voor PDF- en Excel-bestanden.

>[!NOTE]
>
>Als de gegevens die u exporteert gedeelde kolommen bevatten en u exporteert naar een indeling die is gescheiden door Excel of Tab, worden deze kolommen gescheiden in het geëxporteerde bestand.

Voor meer informatie over hoe te om het formatteren in een rapport aan te passen, zie [&#x200B; Voorwaardelijke het formatteren van het Gebruik in meningen &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Koppelingen {#links}

Koppelingen kunnen verwijzen naar elk object in Workfront dat koppelingen ondersteunt. Wanneer u een lijst in Workfront naar PDF exporteert, blijven alle ondersteunde koppelingen in het oorspronkelijke document actief in het geëxporteerde document.

>[!TIP]
>
>Als de regel `valueformat=HTML` wordt weergegeven in de tekstmodus voor een aangepaste veldkolom en de koppelingswaarden niet worden weergegeven in een geëxporteerd PDF-bestand, moet u extra coderegels invoeren in de tekstmodus.
>
>Bijvoorbeeld, als u een douanegebied genoemd Open Q1 Projecten hebt die verbindingen bevatten, zou u de volgende code toevoegen:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Wanneer u naar een Excel-indeling exporteert, worden alleen koppelingen naar objecten in Workfront in het geëxporteerde bestand opgenomen. Deze koppelingen worden alleen ondersteund op plaatsen waar u koppelingen in geëxporteerde Excel-documenten kunt toestaan, zoals rapportleveringen.

## Branding {#branding}

>[!IMPORTANT]
>
>Branding is alleen van toepassing op organisaties die nog niet aan boord zijn van Adobe Experience Cloud.
>
>Als uw organisatie is aangemeld bij Adobe Experience Cloud, is branding niet beschikbaar.

Als uw Workfront-beheerder aangepaste branding heeft toegevoegd aan uw Workfront-exemplaar voor de algemene navigatiebalk, bevatten de geëxporteerde PDF-bestanden ook uw persoonlijke logo.

Gegevens die in andere indelingen worden geëxporteerd, kunnen niet worden gepersonaliseerd met uw logo.

Voor meer informatie over branding uw instantie van Workfront en de Globale Bar van de Navigatie, zie [&#x200B; Merk uw instantie van Adobe Workfront &#x200B;](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
