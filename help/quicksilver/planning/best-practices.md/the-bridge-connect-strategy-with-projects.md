---
title: 'Bridge opbouwen: strategische intentie verbinden met projecten'
description: Leer hoe u een 'strategische thread' maakt tussen uw plannen op hoog niveau in Adobe Workfront Planning en uw dagelijkse uitvoering van workflows in Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# Bouw de brug: verbindend strategische intentie met projecten

{{planning-important-intro}}

Leer hoe u een strategische thread kunt maken tussen uw plannen op hoog niveau in Adobe Workfront Planning en uw dagelijkse uitvoering in Workfront. U kunt een brug tussen strategie en uitvoering bouwen gebruikend verbindingen.

Deze handleiding is bedoeld voor Workfront-beheerders en werkruimtemanagers die Workfront Planning implementeren.

## Overzicht van het uitlijnen van strategie op uitvoering

Door uw strategie aan uw dagelijkse werk te koppelen, wordt visie werkelijkheid. Wanneer de plannen op hoog niveau synchroon met uitvoering zijn, creeert u een strategische draad die elk project en elke taak verzekert beweegt de zaken vooruit.

Om deze afstemming te bereiken, hebt u een reeks technische koppelingen en procesinstructies nodig die de inspanningen in Workfront verbinden met de strategische records in Workfront Planning.

Door de kloof tussen planning en actie te overbruggen, zorgt u ervoor dat de energie van uw team altijd gericht is op uw hoogste-prioritaire doelstellingen.

## Vestig de stichting door een verbinding te creëren

Voordat u planning en uitvoering kunt overbruggen, moet u als werkruimtemanager definiëren welke recordtypen in aanmerking komen voor een verbinding.

### Overzicht van het verbindingsveld

De bridge begint met het maken van een verbindingsveld.

Een verbindingsveld fungeert als de technische handshake tussen recordtypen.

Dit veldtype is de motor achter alle relaties in Workfront Planning. Het is een expressie van intentie, in die zin dat wordt vastgelegd dat een specifiek recordtype (zoals een Kanaaltactiek) mag worden gekoppeld aan andere objecttypen, ongeacht of ze in Planning of Workfront wonen.

Voor informatie, zie [&#x200B; Verbonden overzicht van recordtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

### Definiëren wanneer verbinding moet worden gemaakt

In het ideale geval moet u bepalen of u verbindingen moet maken voordat u een werk maakt.

Door een verbindingsgebied toe te voegen, bouwt u uw milieu aan steun een strategische draad, ongeacht hoe de individuele verslagen uiteindelijk worden gecreeerd.

## Strategie en uitvoering synchroon instellen

Om uw strategische laag geconcentreerd te houden, adviseren wij uw planningsverslagen op hoog niveau intent te concentreren terwijl het gebruiken van Workfront voor tactische uitvoering.

Deze benadering gebruikt de unieke sterke punten van beide modules op de volgende manieren:

* **Planning van Workfront (de strategische laag):** blijft high-level. Het volgt de Campagne, de Tactiek van het Kanaal, en de Begroting. Het is lawaaivrij en bestuurbaar.

* **Workfront (de uitvoeringslaag):** beheert de tactische details. U kunt individuele ervaringen of activiteiten als projecten, taken, en kwesties beheren. U kunt ze toewijzen voor eigendom en goedkeuring voor uitvoering inbouwen.

## Ga van intent aan actie door de brug te activeren

Nadat de verbinding wordt gevormd, moet u beslissen hoe te om het verband tussen een specifiek strategisch verslag en een uitvoeringsproject te activeren.

### Een pad met tabelkoppen gebruiken

De strategen en de machtsgebruikers gebruiken vaak de lijstmening als hun werkbank om plannen in tijd te verfijnen.

Als u een record in een tabel maakt, wordt standaard geen koppeling naar Workfront tot stand gebracht.

De verbinding met een uitvoeringsproject wordt gevestigd wanneer een gebruiker besluit om de verbinding te activeren.

Dit kan op de volgende manieren worden gedaan:

* Creëer manueel een stroomafwaarts verbonden project direct van het verbindingsgebied in de Planning van Workfront of van een facultatieve pagina van Verbindingen in de de detailmening van het verslag.

  Handmatig maken resulteert in een leeg project zonder specifieke aangepaste formulieren.

  Voor informatie, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

* Automatisch, door de automatisering van de Planning van Workfront te gebruiken, voor complexere behoeften.

  Deze automatiseringen zijn beschikbaar als knoppen op de actiebalk wanneer u een rij in een tabel selecteert.

  Dit staat voor menselijk toezicht of placeholder verwezenlijking toe, die ervoor zorgen dat de projecten slechts in uw werkschemamilieu worden geproduceerd wanneer zij echt nodig zijn.

  Voor informatie, zie [&#x200B; voorwerpen creëren gebruikend het verslag van de Planning van Adobe Workfront automatiseringen &#x200B;](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### Automatische activering maken

Voor organisaties met hoge volumeverzoeken of geavanceerde automatiseringsbehoeften, kan de brug automatisch worden geactiveerd gebaseerd op specifieke gebeurtenissen of op gebiedswaarden die in een verzoekvorm worden gevormd.

Voor deze aanpak hebt u een licentie voor Adobe Workfront Fusion nodig.

Voor meer informatie zie [&#x200B; Opstelling en beheer Workfront Fusion: artikelindex &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc).

* **de voorleggingstrekkers van het Gebruik:** Omdat de vormen één enkele, schone voorleggingsgebeurtenis verstrekken, kunnen zij als trekkers voor de automatisering van de Fusie worden gebruikt. Een Fusion-scenario kan een formulierverzending detecteren en direct een gekoppeld project genereren in Workfront.

* **gebied-waarde trekkers van het Gebruik:** voor diepere automatisering, kunt u Fusie vormen om specifieke gebieden te controleren. Een eenvoudig selectievakje met de naam &quot;Gereed voor uitvoering&quot; kan bijvoorbeeld als katalysator fungeren en automatisch de bridge bepalen zodra deze wordt gecontroleerd.

## Opzoekvelden toevoegen aan zichtbaarheid oppervlak

Zodra een project wordt verbonden, kunt u gegevens in real time van Workfront direct binnen het verslag van de Planning oppervlakte oppervlakte door raadplegingsgebieden van het project toe te voegen.

Als werkruimtemanager, kunt u opzoekgebieden opstelling om het even welk systeem of douanegebied van het verbonden project (zoals de Ware Datum van de Voltooiing of Lead van Creative) in het het verslagtype van de Planning te trekken. Als deze gegevens eenmaal zijn vastgelegd, kunnen ze op meerdere niveaus van uw strategische hiërarchie worden opgerold, tot op het campagnereniveau. Dit zorgt voor krachtige gezamenlijke rapportage voor belanghebbenden gedurende de hele marketinglevenscyclus, waarbij ze op de hoogte worden gehouden zonder dat ze de planningsomgeving hoeven te verlaten.

## Zichtbaarheid bereiken door strategie aan actie aan te sluiten

De ultieme waarde van de bridge is realtime zichtbaarheid.

Door intent met actie te verbinden, kunt u kritieke bedrijfsvragen in een oogopslag beantwoorden. Hieronder volgen voorbeelden van deze vragen:

* Geeft onze campagne &quot;FY26 Brand Awareness&quot; nu actief resultaten?

* Waar hebben onze strategische tactieken meer creatieve steun nodig om op schema te blijven?

* Hoe brengen we onze middelen in overeenstemming met onze strategische pijlers met de hoogste prioriteit?

## Tips en trucs

### Dos:

* **gebruik de &quot;strategische draad&quot;metafoor:** herinnert teams dat elk project een &quot;hoofd&quot;op een strategisch koord zou moeten zijn.

* **automatiseer de handoff:** de automatiseringen van het Gebruik om projectverwezenlijking teweeg te brengen om tijd en inspanning te besparen terwijl ook het verbeteren van gegevensconnectiviteit en bestuur.

* **Verbinding, dupliceer niet:** de raadplegingsgebieden van het gebruik aan oppervlakte in real time uitvoeringsgegevens (als status of voltooiingsdata) in uw strategische verslagen. Dit zorgt ervoor dat uw strategische weergaven altijd accuraat zijn zonder dat uw team handmatig moet worden bijgewerkt.

### Don&#39;t:

* **behandelt planningsverslagen niet als taaklijsten:** de brug wordt ontworpen om strategische intentie met uitvoeringsprojecten te verbinden. Houd uw planningsverslagen geconcentreerd op &quot;wat&quot;en &quot;waarom,&quot;en laat de werkschemamodule de korrelige &quot;hoe&quot;door taken en kwesties behandelen.

* **niet over-synchronisatie:** u te hoeven niet om elk project-vlakke detail terug naar Planning te synchroniseren. Houd de strategische laag hoog en ruisvrij.

* **negeert niet de brug:** als het werk in de module van het Werkschema zonder een verbinding aan Planning begint, hebt u een &quot;Plan van de Schaduw&quot;gecreeerd dat aan leiderschap onzichtbaar is.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



