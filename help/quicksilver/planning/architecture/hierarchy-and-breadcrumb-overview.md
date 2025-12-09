---
title: Overzicht van Hiërarchie en Breadcrumb
description: U kunt meerdere werkruimtemhiërarchieën maken tussen de recordtypen in een werkruimte.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
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

Hiërarchieën zijn verbindingen tussen recordtypen. U kunt maximaal vier record- en objecttypen in één hiërarchie laten verbinden.

Voor informatie over het creëren van hiërarchieën, zie [&#x200B; werkruimtescheidingen &#x200B;](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) creëren.

Hieronder vindt u voordelen van het gebruik van hiërarchieën in uw werkruimten:

* Om het werk te organiseren op een manier die weerspiegelt hoe uw teams eigenlijk plannen, werken, en leveren.
* Gebruikers kunnen zien waar ze zich bevinden, hoe recordtypen verbinding maken en hoe strategie in uitvoering stroomt door te verwijzen naar een set broodkruimels die hun plaats in het systeem aangeven.
* Een betere navigatie bieden en zorgen voor helderheid en continuïteit in alle workflows.
* Om stromen te bepalen die passen hoe uw organisatie werkt, ondersteunend zowel flexibiliteit als consistentie over alle stadia van het werk.

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

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * Algemene recordtypen kunnen voorkomen in meerdere werkruimten binnen meerdere hiërarchieën. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Workfront-objecttypen kunnen ook in meerdere hiërarchieën en in verschillende werkruimten worden weergegeven.
   * Algemene recordtypen kunnen geen deel uitmaken van hiërarchieën in verschillende werkruimten.

     Als een campagne bijvoorbeeld een algemeen recordtype is en deel uitmaakt van een hiërarchie in Workspace 1, kan deze worden toegevoegd als een bestaand recordtype aan Workspace 2, maar kan deze daar geen deel uitmaken van een hiërarchie. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * De recordtypen met verbindingen die geen corresponderend veld maken op hun gekoppelde recordtypen, kunnen ook deel uitmaken van hiërarchieën. Nieuwe verbindingen die tijdens hiërarchieopstelling worden gecreeerd zullen altijd tot een overeenkomstig gebied op de verbonden verslagtypes, door gebrek leiden.

## Overwegingen bij het weergeven van broodkruimels

Wanneer u hiërarchieën tussen recordtypes creeert, produceren zij broodkruimels voor verslagen die tot die verslagtypes behoren.

Bijvoorbeeld, als u een hiërarchie creeert en Campagnes met Tactics met Programma&#39;s en toen Projecten verbindt, wanneer u aan een verslag van om het even welke die types navigeert in de hiërarchie worden verbonden, kunt u bekijken waar in de hiërarchie het verslag wordt geplaatst.

Overweeg het volgende:

* Als een recordtype deel van veelvoudige hiërarchieën in veelvoudige werkruimten uitmaakt, kunt u tussen hiërarchieën van de broodkruimel van het verslag op de pagina van het verslag schakelen.
* Broodkruimels werken in Workfront en Planning.

  Wanneer u bijvoorbeeld een project bekijkt dat is verbonden met planningscampagnes en tactieken, maar ook met Workfront-portfolio&#39;s en -programma&#39;s, kunt u vanuit de breadcrumb schakelen tussen de hiërarchieën van zowel de Planning als de Workfront.

  Voor meer informatie, zie [&#x200B; de hiërarchieën van de werkruimte &#x200B;](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) creëren.


