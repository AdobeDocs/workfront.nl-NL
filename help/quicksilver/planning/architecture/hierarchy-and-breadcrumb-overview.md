---
title: Overzicht van Hiërarchie en Breadcrumb
description: U kunt meerdere werkruimtemhiërarchieën maken tussen de recordtypen in een werkruimte.
hide: true
hidefromtoc: true
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '887'
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

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Als werkruimtemanager, kunt u flexibele maar gestructureerde hiërarchieën tussen verslagtypes en andere objecten types in de Planning van Adobe Workfront bepalen.

Hiërarchieën zijn verbindingen tussen recordtypen, of tussen recordtypen en een Workfront-project.

Voor informatie over het creëren van hiërarchieën, zie [ werkruimtescheidingen ](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) creëren.

Hieronder vindt u voordelen van het gebruik van hiërarchieën in uw werkruimten:

* Om het werk te organiseren op een manier die weerspiegelt hoe uw teams eigenlijk plannen, werken, en leveren.
* Gebruikers kunnen zien waar ze zich bevinden, hoe recordtypen verbinding maken en hoe strategie in uitvoering stroomt door te verwijzen naar een set broodkruimels die hun plaats in het systeem aangeven.
* Een betere navigatie bieden en zorgen voor helderheid en continuïteit in alle workflows.
* Om stromen te bepalen die passen hoe uw organisatie werkt, ondersteunend zowel flexibiliteit als consistentie over alle stadia van het werk.

## Overwegingen bij het werken met hiërarchieën

* U kunt meerdere hiërarchieën maken voor één werkruimte.
* U kunt maximaal vier record- en objecttypen in één hiërarchie laten verbinden.
* U kunt alleen de volgende objecttypen verbinden in een werkruimtehiërarchie:
   * De types van verslag die tot de werkruimte behoren u de hiërarchieën binnen bouwt.
   * Workfront-projecten. Workfront-projecten kunnen niet worden toegevoegd als bovenliggende bestanden van andere recordtypen. Ze zijn altijd het laatste objecttype in een hiërarchie.
* U kunt de volgende objecttypen niet toevoegen in een hiërarchie:
   * De types van verslag van andere werkruimten, zelfs wanneer zij als verbindbare of globale verslagtypes worden geplaatst. U kunt algemene recordtypen alleen aan hiërarchieën toevoegen wanneer ze zijn toegevoegd aan de werkruimte waaruit u de hiërarchie maakt.
   * Alle andere Workfront-objecten.
   * AEM Assets.
* De hiërarchieën kunnen zowel de types van het Verslag van de Planning als de projecten van Workfront tezelfdertijd omvatten.

       bijvoorbeeld, kunt u een het verslagtype van de Campagne met de Projecten van Tactics van de Planning en van Workfront als kinderen in de zelfde werkruimtehiërarchie hebben.
  * Als er al een verbinding bestaat tussen de geselecteerde recordtypen, gebruikt het systeem de bestaande verbinding opnieuw.
* Als er geen verbinding bestaat, maakt Workfront er een als onderdeel van de hiërarchische instelling.
* **creeer corresponderend gebied op verbonden verslagtype** het plaatsen moet voor het verbonden gebied voor verslagen en objecten types worden aangezet die u in een hiërarchie wilt omvatten.
* Hieronder vindt u regels voor hiërarchische instellingen:
   * Een recordtype kan slechts één bovenliggend recordtype in een bepaalde werkruimte hebben.

     Een Tactisch recordtype kan bijvoorbeeld niet zowel een campagne- als een Goal-recordtype hebben als een bovenliggend item in dezelfde werkruimte.
   * Een recordtype kan het bovenliggende element in meerdere hiërarchieën zijn.

     U kunt bijvoorbeeld drie verschillende hiërarchieën in één werkruimte hebben en elk van deze hiërarchieën kan Campagnes hebben als het bovenliggende recordtype.
   * Een record kan worden verbonden met meerdere bovenliggende records van hetzelfde type, wanneer u een record verbindt met vele of vele records.

     Tactic A kan bijvoorbeeld tot zowel Campagne X als Campagne Y behoren.
   * Een recordtype kan slechts verbinding maken met één onderliggend recordtype tegelijk. Een onderliggend recordtype kan ook een bovenliggend item voor een ander recordtype zijn.

     Bijvoorbeeld, kan een het verslagtype van de Campagne de ouder aan slechts één ander verslagtype in de zelfde hiërarchie (Tactica) zijn, en de Tactica kunnen de ouder van Programma&#39;s zijn die een ouder aan Projecten kunnen zijn.
   * Een recordtype kan niet het bovenliggende element in een hiërarchie zijn en het onderliggende element in een andere hiërarchie in dezelfde werkruimte.
   * Algemene recordtypen kunnen in meerdere werkruimten binnen meerdere hiërarchieën worden weergegeven nadat ze aan die werkruimten zijn toegevoegd.

     Als een campagne bijvoorbeeld een algemeen recordtype is en deel uitmaakt van een hiërarchie in Workspace 1, kan deze worden toegevoegd als een bestaand recordtype aan Workspace 2 en kan deze daar deel uitmaken van een hiërarchie. Maar het kan geen deel uitmaken van een hiërarchie in Workspace 2 alleen wanneer het wordt aangewezen als een algemeen recordtype in Workspace 1, maar niet worden toegevoegd aan Workspace 2.

## Overwegingen bij het weergeven van broodkruimels

<!-- this might be incomplete, because I have no UI for this yet-->

Wanneer u hiërarchieën tussen recordtypes creeert, produceren zij broodkruimels voor verslagen die tot die verslagtypes behoren.

Bijvoorbeeld, als u een hiërarchie creeert en Campagnes met Tactics, dan met Activiteiten, en dan met Projecten verbindt, wanneer u aan een verslag van om het even welke die types navigeert in de hiërarchie worden verbonden, kunt u bekijken waar in de hiërarchie het verslag wordt geplaatst.

Overweeg het volgende:

* Als een recordtype deel van veelvoudige hiërarchieën uitmaakt, kunt u tussen hiërarchieën van de broodkruimel van het verslag op de pagina van het verslag schakelen.
* Broodkruimels werken in Workfront en Planning.

  Wanneer u bijvoorbeeld een project bekijkt dat is verbonden met planningscampagnes en tactieken, maar ook met Workfront-portfolio&#39;s en -programma&#39;s, kunt u schakelen tussen de objecttypen Planning en Workfront vanuit de breadcrumb.

  Voor meer informatie, zie [ de hiërarchieën van de werkruimte ](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) creëren.
* Wanneer u een record bewerkt, zijn de wijzigingen zichtbaar vanuit alle werkruimten en alle hiërarchieën waarin de record deel uitmaakt.


