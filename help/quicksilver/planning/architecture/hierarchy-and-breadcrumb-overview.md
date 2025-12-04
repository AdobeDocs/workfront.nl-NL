---
title: Overzicht van Hiërarchie en Breadcrumb
description: U kunt meerdere werkruimtemhiërarchieën maken tussen de recordtypen in een werkruimte.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Overzicht van hiërarchie en broodkruimel

Als werkruimtemanager, kunt u flexibele maar gestructureerde hiërarchieën tussen verslagtypes en andere objecten types in de Planning van Adobe Workfront bepalen.

Hieronder vindt u voordelen van het gebruik van hiërarchieën in uw werkruimten:

* Om het werk te organiseren op een manier die weerspiegelt hoe uw teams eigenlijk plannen, werken, en leveren.
* De gebruikers begrijpen waar zij zijn, hoe de verslagtypes verbinden, en hoe de strategie in uitvoering door naar een reeks broodkruimels te verwijzen die op hun plaats in het systeem wijzen.
* Biedt een betere navigatie en zorgt voor helderheid en continuïteit in alle workflows.
* De hiërarchieën dwingen geen rigide, systeem-bepaalde structuur af, en in plaats daarvan staat u toe om stromen te bepalen die passen hoe uw organisatie werkt, die zowel flexibiliteit als consistentie over alle stadia van het werk steunen.

## Overwegingen bij het werken met hiërarchieën

* Als werkruimtebeheerder kunt u meerdere hiërarchieën maken voor één werkruimte.
* Als er al een verbinding bestaat tussen de geselecteerde recordtypen, gebruikt het systeem de bestaande verbinding opnieuw.
* Als er geen verbinding bestaat, maakt Workfront er automatisch een als onderdeel van de hiërarchische instelling.
* Hieronder vindt u regels voor hiërarchische instellingen:
   * Een recordtype kan slechts één bovenliggend recordtype in een bepaalde werkruimte hebben.

     Een Tactisch recordtype kan bijvoorbeeld niet zowel een campagne- als een Goal-recordtype hebben als een bovenliggend item in dezelfde werkruimte.
   * Een record kan worden verbonden met meerdere bovenliggende records van hetzelfde type, wanneer u een record verbindt met vele of vele records.
Tactic A kan bijvoorbeeld tot zowel Campagne X als Campagne Y behoren.
   * Een recordtype kan verbinding maken met meerdere recordtypen voor onderliggende bestanden.

     Een recordtype voor campagne kan bijvoorbeeld het bovenliggende element zijn van meerdere andere recordtypen, zoals Tactics, Tests en andere recordtypen.
   * De hiërarchieën kunnen zowel de types van het Verslag van de Planning als de objecten van Workfront omvatten.

     U kunt bijvoorbeeld een type Campagnerecord hebben met Planning Tactics en Workfront Projecten als onderliggende items.
   * Algemene recordtypen kunnen voorkomen in meerdere werkruimten binnen meerdere hiërarchieën.
   * Workfront-objecttypen kunnen ook in meerdere hiërarchieën en in verschillende werkruimten worden weergegeven.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * De recordtypen met verbindingen die geen corresponderend veld maken op hun gekoppelde recordtypen, kunnen ook deel uitmaken van hiërarchieën. Nieuwe verbindingen die tijdens hiërarchieopstelling worden gecreeerd zullen altijd tot een overeenkomstig gebied op de verbonden verslagtypes, door gebrek leiden.

## Overwegingen bij het weergeven van broodkruimels


