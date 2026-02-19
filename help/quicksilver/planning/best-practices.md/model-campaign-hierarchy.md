---
title: 'Uw succes archiveren: uw campagnehiërarchie modelleren'
description: Leer hoe u uw complexe bedrijfsprocessen vertaalt in een schaalbare, beheerde campagnehiërarchie met behulp van 'Graviteitscentra' en een architectuur met meerdere werkruimten.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 0%

---

# Uw succes archiveren: uw campagnehiërarchie modelleren

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Workfront Planning, een extra mogelijkheid van Adobe Workfront.
>
>Uw organisatie moet een Workfront Planning Prime of hoger pakket hebben om de functies te kunnen ondersteunen die in dit artikel worden aanbevolen.
>
>Voor een lijst van vereisten om tot de Planning van Workfront toegang te hebben, zie [&#x200B; het toegangsoverzicht van de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/access/access-overview.md).
> 
>Voor algemene informatie over de Planning van Workfront, zie [&#x200B; begonnen worden met de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/general/planning-overview.md).

Leer hoe u uw complexe bedrijfsprocessen omzet in een schaalbare, beheerde campagnehiërarchie met zwaartepunt en een architectuur met meerdere werkruimten in de Planning van Adobe Workfront.

Deze handleiding is bedoeld voor Workfront-beheerders en Power Users die de architectuur van uw omgeving implementeren en ontwerpen in Workfront Planning.

## Overzicht van de succesarchitectuur

Naarmate uw marketingactiviteiten volwassen worden, neemt ook de complexiteit van uw gegevens toe. Zonder een duidelijke blauwdruk, kan uw Systeem van het Marketing van Verslag snel een junk bak van losgemaakte verslagen, conflicterende terminologie, en rapporteringssilo&#39;s worden.

Wanneer u een architectuur van succes bouwt, vestigt u een kader voor het modelleren van uw campagnehiërarchie in de Planning van Workfront. Het verplaatst u van spreadsheetchaos naar een geregeerd, object-georiënteerd model dat ervoor zorgt dat elk team de zelfde taal spreekt terwijl het handhaven van de behendigheid die zij moeten uitvoeren.

## Bouw een hiërarchie om uw niveaus van intentie te bepalen

Om helderheid en scalability te handhaven, adviseren wij om met een bewezen kernweg te beginnen wanneer het ontwerpen van uw werkschema in de Planning van Workfront.

Vanaf dat punt kunt u uw strategie uitbreiden door meer niveaus aan uw architectuur toe te voegen.

### Het kernpad: hoe van strategie tot actie te komen

Terwijl organisaties deze hiërarchie kunnen uitbreiden aangezien hun operationele behoeften evolueren, beginnend met de drie niveaus die in de hieronder secties worden beschreven een sterke brug tussen strategie en uitvoering verzekeren.

Uit onze bevindingen hebben we kunnen opmaken dat de meeste succesvolle implementaties van Workfront Planning gedijen op een schoon, driedagig model dat zowel Planning als Workfront omvat.

Hieronder vindt u de niveaus van een geslaagde planningimplementatie en de artefacten die u zou kunnen maken om u in het proces te ondersteunen:

* **Niveau 1: Campagnes (de Planning van Workfront)**

   * **Focus:** bepaal de strategische pijlers en de jaarlijkse initiatieven op lange termijn. Definieer bijvoorbeeld een initiatief voor uw organisatie met de naam &quot;FY26 Global Brand Awareness&quot;. Dit is uw focus voor een bepaald tijdkader. Maak campagnes ter ondersteuning van dit initiatief.

   * **Personas:** Belanghebbenden voor dit niveau kunnen de Medewerker van de Marketing, een VP van Marketing, of andere strategische lood zijn.

  Voor informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

* **Niveau 2: De Takken van het Kanaal (de Planning van Workfront)**

   * **Nadruk:** bepaal de operationele instructies die &quot;wat&quot;voor specifieke kanalen schetsen. Dit is de laatste laag met strategische intentie voordat het werk begint. Maak bijvoorbeeld een tactiek &quot;Q1 Social Media Blitz&quot;. U kunt het dan koppelen met uw campagnes.

   * **Personas:** Belangrijkste belanghebbenden zijn een leider van de Verrichtingen van de Marketing, kanaalleiders, of campagnemanagers.

* **Niveau 3: Projecten (Planning en Workfront)**

   * **Nadruk:** voert op de nauwkeurige ervaringen of de activiteiten uit die uiteindelijk uw initiatief zullen verwezenlijken. Een aantal van de te leveren items zijn specifiek, zoals sociale berichten, e-mails en webpagina&#39;s.

   * **Implementatie:** u kunt Tactics in Planning tot stand brengen en hen direct verbinden aan **Projecten** in Workfront, waar de individuele te leveren producten als taken en kwesties worden beheerd.

   * **Persona:** Belangrijkste belanghebbenden hier zijn creatieve personen, individuele contribuanten, iedereen die verantwoordelijk is voor het doen van het werk om het initiatief te steunen.

### Strategische uitbreiding: meer niveaus toevoegen

Zodra u de kernweg vestigt, kunt u verkiezen om extra lagen toe te voegen na zorgvuldige overweging van hun specifieke bedrijfsingewikkeldheid.

Het kan handig zijn om de volgende aanvullende items te maken:

* **Plannen van het Kanaal:** een laag tussen Campagnes en Tactics om dwars-functionele strategieën te groeperen. Bijvoorbeeld, een Plan genoemd &quot;Digitale Strategie&quot;.

* **Activiteiten:** als u in een lager-volume milieu werkt (u zou 5.000 of minder te leveren kunnen hebben per jaar), zouden sommige teams kunnen verkiezen om individuele ervaringen als verslagen van de Planning van Workfront te volgen alvorens zij de projecten van Workfront worden.

>[!IMPORTANT]
>
>Als uw organisatie meer dan 5.000 activiteiten per jaar produceert, zou u individuele te leveren volgen aan Workfront moeten bewegen.
>
>Het beheren van high-volume ervaringsverslagen in Planning kan tot gegevensaccumulatie leiden die uw strategische zicht bedekt.
>Wij bevelen dit algemene richtsnoer voor maximale efficiëntie aan:
>
>* Planning gebruiken voor &quot;waarom&quot; en &quot;wat&quot;
>* Gebruik Workfront voor het hoge volume &#39;how&#39;.

## Begrijp zwaartepunt om uw architectuur te bouwen

Een marketingsysteem van bedrijfsniveau met record is niet in één werkruimte ingebouwd. Het gebruikt een &quot;hub-en-sprekende&quot;architectuur waar verslagtypes in hun natuurlijke centra van zwaartekracht worden beheerd.

Voor meer informatie, zie [&#x200B; uitrollen uw strategisch huis: een 30 dagllanceerpad &#x200B;](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Om uw architectuur te bouwen die de hub-en-sprekende benadering gebruikt, moet u het volgende tot stand brengen:

* Een taxonomihub
* Een werkruimte voor strategische planning
* Functionele woordgroepen

### Bouw de taxonomihub als uw classificaties

U moet eerst één gecentraliseerde werkruimte voor uw globale classificaties tot stand brengen om de belangrijkste concepten te bepalen iedereen in uw organisatie moet begrijpen. Maak bijvoorbeeld de volgende recordtypen in een centrale werkruimte: merken, regio&#39;s, producten, personen.

Voor informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

Stel het volgende in wanneer u uw classificaties maakt:

* **Primaire plaats:** kies een primaire werkruimte. Deze werkruimte moet de bron van de waarheid zijn voor de recordtypen die u maakt.

* **het voordeel:** door deze definities aan de rest van de zaken te synchroniseren, lost u op dat de concepten zoals &quot;Gebied: EMEA&quot;het zelfde ding aan elk team betekent.

### De werkruimte voor strategische planning maken als uitvoerend centrum

Het uitvoerend centrum is waar de campagnes op hoog niveau (en om het even welke plannen van het Kanaal) leven.

* **Primaire plaats:** dit is het uitvoerende zwaartepunt, dat een lawaaivrij milieu voor strategische besluitvorming verstrekt.

* **het voordeel:** leiderschap kan de portefeuille van campagnes beheren zonder het dagelijkse tactische lawaai te luisteren.

### De functionele spaken definiëren als de werkruimten van uw teams

Functionele eenheden (sociaal, Creative, e-mail) hebben hun eigen werkruimte voor het beheren van hun tactiek.

* **Primaire plaats:** Deze werkruimten zijn de individuele centra van zwaartekracht voor lokale teamuitvoering.

* **het voordeel:** de teams verbruiken de globale campagnes en classificaties van de hubs, terwijl het handhaven van hun eigen lokale voorwerpen.

  Bijvoorbeeld, kan het team het type van het verslag van de Campagne van de centrale werkruimte in de werkruimte van hun team toevoegen maar campagnes tot stand brengen relevant slechts voor hun werkruimte. Voorbeelden van campagnes zijn &quot;mediakanalen&quot; of &quot;Gebruiksrechten&quot;.

## Een op zelfstandig bestuur gebaseerde aanpak gebruiken

Om ervoor te zorgen dat uw architectuur onder druk blijft, volgt u het beginsel van zelfstandig bestuur.

We raden het volgende aan bij het maken van uw entiteiten in Workfront Planning:

* **de aannamen van het Gebruik, niet werkwoorden:** noem uw verslagtypes na de dingen u volgt (noem hen &quot;Campagne&quot;of &quot;Tactiek&quot;), niet de te doen acties (noem hen niet &quot;Campaigning&quot;of &quot;Planning&quot;).

* **normaliseer nomenclatuur:** gebruik de zelfde namen over alle werkruimten. Op deze manier kunt u gegevens samenvoegen over de gehele portfolio voor rapportage aan het dagelijks bestuur.

## Hoe zit het met bestaande portfolio&#39;s en programma&#39;s?

Een algemene vraag voor ervaren organisaties is hoe ze de portfolio&#39;s en programma&#39;s die ze al in Workfront hebben gemaakt, moeten verwerken. In het verleden werden deze objecten vaak gebruikt om strategische planning na te bootsen.

Nu raden we u aan om de aanpak van de planning van Workfront te wijzigen, die natuurlijk past bij de strategische aanpak van de planning.

### Portfolio&#39;s en programma&#39;s vervangen door recordtypen

In veel organisaties worden Portfolio&#39;s gebruikt om merken of bedrijfseenheden op hoog niveau weer te geven, terwijl programma&#39;s strategische thema&#39;s zijn.

In de Planning van Workfront, worden deze het best gemodelleerd als Types van Verslag in uw taxonomie hub.

Door een merk of een BedrijfsEenheid als verslagtype te behandelen, kunt u hen met een Campagne of Tactiek over de volledige onderneming verbinden, die veel flexibelere rapportering dan statische Portfolio - de structuur van het Programma verstrekken.

### Een rapportbridge-strategie gebruiken

Hoewel Workfront Planning de toekomst van strategische intentie is, is de native rapportage via Canvas Dashboard nog steeds aan de gang.

Veel organisaties vertrouwen nog steeds op de robuuste rapportagemogelijkheden die verbonden zijn aan hun bestaande Portfolio- en programmastructuren in Workfront.

We raden het volgende aan:

* Verwijder uw portfolio&#39;s en programma&#39;s niet.
* Gebruik de automatisering van de Planning om een brug tussen uw verslagtypes en portefeuilles en programma&#39;s tot stand te brengen.

  Wanneer een Tactic of Campagne in de Planning van Workfront wordt gecreeerd, kan dat verslag een overeenkomstige Portfolio of een Programma in Workfront produceren.

  Voor informatie, zie [&#x200B; voorwerpen creëren gebruikend het verslag van de Planning van Adobe Workfront automatiseringen &#x200B;](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Zo kunt u:

* Geniet van de superieure strategische visualisatie van Workfront Planning met behulp van tijdlijnen en kalenders.

* Behoud uw oudere rapportage in Workfront voor belanghebbenden die nog niet klaar zijn om naar Canvas te gaan.

## Tips en trucs

### Dos

* **Steek aan de kern weg-eerste benadering:** Vestig uw Campagne-aan-Tactic-aan-Project stroom alvorens meer ingewikkeldheid toe te voegen.

* **Wijs primaire werkruimten aan:** verzeker elk verslagtype één huiswerkruimte (denk dat zijn zwaartepunt) heeft die als aggregator voor het melden dienst doet.

* **bevestig verzoekvormen voor het innameproces voorrang:** Gebruik verslagvormen voor groepen met minder verfijning in de Planning van Workfront om meta-gegevensintegriteit te verzekeren.

  >[!CAUTION]
  >
  >Hoewel Power Users baat kan hebben bij het rechtstreeks invoeren van gegevens in tabelweergaven, is voorzichtigheid geboden.
  >Bulkwijzigingen in een tabel kunnen gemakkelijk leiden tot gegevenshoofden voor andere belanghebbenden.

### Don&#39;ts

* **gebruik geen generalisaties:** bijvoorbeeld, in plaats van het spreken over een &quot;kern&quot;milieu, verwijs specifiek naar Workfront en het voorwerp van het Project wanneer het spreken over uitvoering.

* **overcompliceer niet:** Elk extra niveau van hiërarchie voegt een beheersbelasting toe. Voeg alleen niveaus toe die een zakelijke vraag beantwoorden die u momenteel niet kunt beantwoorden.

* **creeer geen silo&#39;s:** zorg ervoor uw verslagtypes over werkruimten worden gedeeld zodat de teams niet de zelfde gegevens opnieuw typen.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->