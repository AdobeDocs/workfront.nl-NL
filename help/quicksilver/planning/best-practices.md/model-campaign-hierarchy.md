---
title: 'De blauwdruk van Succes: Uw campagnehiërarchie modelleren'
description: Leer hoe u uw complexe bedrijfsprocessen vertaalt in een schaalbare, beheerde campagnehiërarchie met behulp van 'Graviteitscentra' en een architectuur met meerdere werkruimten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 77ef50ebd583f0a46324e5cbdc4feea9d21f4280
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 0%

---


# De blauwdruk van Succes: Uw campagnehiërarchie modelleren



## Goal

Leer hoe u uw complexe bedrijfsprocessen vertaalt in een schaalbare, beheerde campagnehiërarchie met behulp van &#39;Graviteitscentra&#39; en een architectuur met meerdere werkruimten.



## Overzicht

Naarmate uw marketingactiviteiten worden geschaald, wordt ook de complexiteit van uw gegevens vergroot. Zonder een duidelijke blauwdruk, kan uw Systeem van het Verslag van de Marketing (MSOR) snel een &quot;junk bak&quot;van losgemaakte verslagen, conflicterende terminologie, en rapporteringssilo&#39;s worden.



De &quot;blauwdruk van Succes&quot;is een kader voor het modelleren van uw campagnehiërarchie in de Planning van Workfront (WFP). Het verplaatst u van &quot;spreadsheetchaos&quot;naar een geregeerd, object-georiënteerd model dat ervoor zorgt dat elk team de zelfde taal spreekt terwijl het handhaven van de behendigheid zij moeten uitvoeren.



## De hiërarchie: uw niveaus van intentie zoeken

Om duidelijkheid en scalability te handhaven, adviseren wij aanvang met een bewezen **Weg van de Kern**. Terwijl organisaties deze hiërarchie kunnen uitbreiden aangezien hun operationele behoeften evolueren, om te beginnen met deze drie niveaus een sterke brug tussen strategie en uitvoering verzekert.



### Het kernpad: strategie voor actie

De meeste succesvolle implementaties bloeien op een schoon, drielagenmodel dat zowel Planning als Workflow omvat:



1. **Niveau 1: Campagnes (de Module van de Planning)**

   * **Focus:** strategische pijlers op lange termijn en jaarlijkse initiatieven (b.v., &quot;FY26 Global Brand Awareness&quot;).

   * **Persona:** CMO, VP van Marketing, Strategische Leads.

2. **Niveau 2: De Takken van het Kanaal (de Module van de Planning)**

   * **Nadruk:** de operationele instructies die &quot;wat&quot;voor specifieke kanalen (b.v., &quot;Q1 Sociale Blitz van Media bepalen&quot;). Dit is de laatste laag met strategische intentie voordat het werk begint.

   * **Persona:** de Marketing Ops, de Leidingen van het Kanaal, de Managers van de Campagne.

3. **Niveau 3: De Projecten van het werkschema (de Module van het Werkschema)**

   * **Nadruk:** de daadwerkelijke uitvoering van &quot;Ervaringen&quot;of &quot;Activiteiten&quot; (b.v., specifieke sociale posten, e-mails, Web-pagina&#39;s).

   * **Uitvoering:** Takken in de Planning verbinding direct aan **Projecten** in de module van het Werkschema, waar de individuele te leveren producten als taken en kwesties worden beheerd.

   * **Persona:** Creatieve personen, Individuele Medewerkers.



### Strategische uitbreiding: meer niveaus toevoegen

Zodra de kernweg wordt gevestigd, kunnen de organisaties verkiezen om extra lagen toe te voegen na zorgvuldig onderzoek van hun specifieke bedrijfsingewikkeldheid:



* **Plannen van het Kanaal:** Een laag tussen *Campagnes* en *Tactics* aan groep de dwars-functionele strategieën (bijvoorbeeld, &quot;Digitale Strategie&quot;).

* **Activiteiten WFP:** in laag-volume milieu&#39;s (typisch &lt;5.000 te leveren producten/jaar), verkiezen sommige teams om individuele &quot;Ervaringen&quot;als verslagen te volgen WFP alvorens zij projecten worden.


>[!TIP]
>
>**Cruciale Uiteinde: De 5.000 Geleverbare Drempel**
>
>Als uw organisatie meer dan 5.000 activiteiten per jaar produceert, zou u **&#x200B;**&#x200B;altijd individueel het te leveren volgen aan de **module van het Werkschema** moeten ontladen. Het beheren van high-volume &quot;Ervaring&quot;verslagen in Planning kan tot gegevensaccumulatie leiden die uw strategische zicht verbergt. De Planning van het gebruik voor &quot;waarom&quot;en &quot;wat,&quot;en de module van het Werkschema voor het hoge volume &quot;hoe.&quot;



## Architectuur: zwaartepunt

Een MSOR van ondernemingsniveau wordt niet gebouwd in één enkele werkruimte. Het gebruikt een &quot;hub-en-Spoke&quot;architectuur waar de verslagtypes in hun natuurlijke **Centers van Zwaartekracht** worden beheerd.



### &#x200B;1. De Taxonomy Hub (classificaties)

Stel één gecentraliseerde werkruimte in voor uw &quot;Global Classifications&quot; (bijvoorbeeld Merken, Regio&#39;s, Producten, Personas).

* **Primaire Plaats:** Deze werkruimte is &quot;Source van Waarheid&quot;voor deze voorwerpen.

* **Het Voordeel:** door deze definities aan de rest van de zaken te synchroniseren, lost u &quot;Semantische Drijf op&quot;het verzekeren dat &quot;Gebied: EMEA&quot;het zelfde ding aan elk team betekent.



### &#x200B;2. De Workspace voor strategische planning (Uitvoerend Centrum)

Dit is waar hoog-niveau **campagnes** (en om het even welke **Plannen van het Kanaal**) levend.

* **Primaire Plaats:** dit is het uitvoerende zwaartepunt, dat een lawaaivrij milieu voor strategische besluitvorming verstrekt.

* **het Voordeel:** de LEIDING kan de portefeuille beheren zonder de dagelijkse tactische rotzooi te zien.



### &#x200B;3. Functionele penselen (teamwerkruimten)

De functionele eenheden (Sociaal, Creative, E-mail) hebben hun eigen werkruimten om hun **Tactiek** te beheren.

* **Primaire Plaats:** Deze werkruimten zijn het centrum van zwaartekracht voor lokale teamuitvoering.

* **het Voordeel:** de Teams &quot;verbruiken&quot;de globale campagnes en classificaties van de hubs, terwijl het handhaven van hun eigen lokale voorwerpen (als *Uitgangen van Media* of *Rechten van het Gebruik*).



## Governance in Noun: Spreek één taal

Om uw blauwdruk te verzekeren houdt omhoog onder druk, volg het beginsel van **Noun-Gebaseerd Bestuur**.



* **Nouns van het Gebruik, niet Verbs:** noem uw verslagtypes na de &quot;dingen&quot;u volgt (`Campaign`, `Tactic`), niet de &quot;acties&quot; (`Campaigning`, `Planning`).

* **normaliseer Nomenclatuur:** gebruik de zelfde namen over alle werkruimten. Op deze manier kunt u gegevens samenvoegen over de gehele portfolio voor rapportage aan het dagelijks bestuur.



## Hoe zit het met bestaande portfolio&#39;s en programma&#39;s?

Een gemeenschappelijke vraag voor volwassen organisaties is hoe te om de Portfolio&#39;s en Programma&#39;s te behandelen zij reeds in de **module van het Werkschema** hebben gebouwd. In het verleden werden deze objecten vaak gebruikt om strategische planning na te bootsen.



### &#x200B;1. Portfolio&#39;s en programma&#39;s → Typen records

In vele organisaties, **Portfolio&#39;s** worden gebruikt om merken op hoog niveau of BedrijfsEenheden (BUs) te vertegenwoordigen, terwijl **Programma&#39;s** strategische thema&#39;s vertegenwoordigen.

* **Verschuiving:** deze zijn best gemodelleerd als **Types van Verslag** in uw **Hub van de Taxonomie**. Door &quot;merk&quot;of &quot;BedrijfsEenheid&quot;als verslagtype te behandelen, kunt u hen met om het even welke campagne of tactiek over de volledige onderneming verbinden, die veel flexibelere rapportering dan een statische structuur van Portfolio/van het Programma verstrekken.



### &#x200B;2. De &quot;Reporting Bridge&quot;-strategie

Terwijl de Planning van Workfront de toekomst van strategische intentie is, is zijn inheemse rapportering via **Dashboards van het Canvas** nog rijpend. Veel organisaties vertrouwen nog steeds op de robuuste rapportagemogelijkheden die gekoppeld zijn aan hun bestaande Portfolio- en programmastructuren in de workflowmodule.

* **de Aanbeveling:** schrapt nog niet uw Portfolio&#39;s en Programma&#39;s. In plaats daarvan, gebruik **automatiseringen van de Fusie** om een brug tot stand te brengen.

* **hoe het werkt:** wanneer een Tactische of Campagne in WFP wordt gecreeerd, kan de Fusie die verslag in een overeenkomstige Portfolio of Programma in de module van het Werkschema automatisch weerspiegelen. Zo kunt u:

   1. Geniet van superieure **strategische visualisatie van WFP** (Chronologie/Kalenders).

   2. Handhaaf uw **erfenis die** in de module van het Werkschema voor bewaarders rapporteert die nog niet klaar zijn om naar Canvas te bewegen.

## Tips en trucs

### Doe:

* **kruis aan de Weg van de Kern eerst.** Stel uw campagne-aan-tactiek-aan-project stroom vast alvorens meer ingewikkeldheid toe te voegen.

* **wijs Primaire Werkruimten aan.** Zorg ervoor dat elk recordtype één thuiswerkruimte (zwaartepunt) heeft die als aggregator voor rapportage fungeert.

* **Prioritize Forms for Intake.** Gebruik recordformulieren voor groepen met minder geavanceerde WFP om de integriteit van metagegevens te garanderen. Terwijl de Gebruikers van de Macht van directe gegevensingang in de meningen van de Lijst kunnen profiteren, zou dit met voorzichtigheid moeten worden benaderd: bulkveranderingen in een lijst kunnen tot gegevenskopzorgen voor andere belanghebbenden gemakkelijk leiden.


### Niet doen:

* **zeg niet &quot;Kern&quot;.** verwijs specifiek naar de **module van het Werkschema** en de **4&rbrace; voorwerpen van het Project &lbrace;wanneer het spreken over uitvoering.**

* **niet overcompliceer.** Elk extra hiërarchisch niveau voegt een &quot;beheerbelasting&quot; toe. Voeg alleen niveaus toe die een zakelijke vraag beantwoorden die u momenteel niet kunt beantwoorden.

* **creeer geen silo&#39;s.** Zorg ervoor dat uw recordtypen worden gedeeld in de verschillende werkruimten, zodat teams niet dezelfde gegevens opnieuw typen.




