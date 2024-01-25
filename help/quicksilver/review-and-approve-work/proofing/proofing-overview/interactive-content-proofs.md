---
product-area: documents
navigation-topic: proofing-overview
title: Overzicht van proefdrukken van interactieve inhoud
description: Interactieve inhoud biedt verschillende methoden om gebruikers te engageren. De agentschappen kunnen het succes van hun campagnes meten gebruikend analyses die van reacties op deze inhoud worden verzameld.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Overzicht van proefdrukken van interactieve inhoud

<!-- Audited: 01/2024 -->

Interactieve inhoud biedt verschillende methoden om gebruikers te engageren. De agentschappen kunnen het succes van hun campagnes meten gebruikend analyses die van reacties op deze inhoud worden verzameld.

Voorbeelden van interactieve inhoud zijn:

* Websites
* Ingesloten of streaming video&#39;s
* Interactieve banners
* HTML5-animaties
* Microsites
* Interactieve e-mails

## Proefdrukken maken voor interactieve inhoud

U kunt op een van de volgende manieren een proefdruk maken voor interactieve inhoud:

* Maak een proefdruk van een ZIP-bestand dat de interactieve inhoud bevat.

  Adobe Workfront pakt de inhoud uit van het ZIP-bestand en slaat deze op een Workfront-server op. Omdat de inhoud op deze manier wordt opgeslagen, kunt u erop vertrouwen dat de inhoud tijdens de volledige proefdrukrevisiecyclus hetzelfde blijft.

* Geef de URL voor de inhoud op.

  Dit is de eenvoudigste manier om een proefdruk van interactieve inhoud te maken. Dit is ook de enige manier waarop u uw inhoud interactief kunt bekijken, aangezien gebruikers de inhoud op internet ervaren.

  Op deze manier wordt de inhoud opgeslagen en gehost op een externe server die niet bekend is bij Workfront.

  We raden deze methode aan voor grote websites, omdat het moeilijk is om alle bestanden te verzamelen waaruit een grote website bestaat. Omdat de inhoud van het bewijs extern wordt opgeslagen, kan Workfront het echter niet beschermen tegen wijzigingen die zijn aangebracht door de ontwikkelaars die eraan werken, zodat u er mogelijk niet op kunt vertrouwen dat de inhoud tijdens de hele proefdrukbeoordelingscyclus hetzelfde blijft.

## Informatie over het voorbereiden van interactieve inhoud in een ZIP-bestand voor proefdrukken

Wanneer u interactieve inhoud in een ZIP-bestand bundelt voor proefdrukken, moet u ervoor zorgen dat deze de volgende specificaties bevat:

* Alle elementen, zoals CSS, JavaScript, video&#39;s, geluiden en afbeeldingen, moeten in het bundelbestand worden opgenomen.
* Interactieve inhoud moet het hoofdbestand bevatten (index.html, index.htm). Als dit bestand niet op de hoofdlocatie is geplaatst, zoekt het gereedschap automatisch naar de map om deze te zoeken. Het hoofdbestand hoeft geen naam index te krijgen.html/index.htm, maar er kan slechts één .html/.htm-bestand op de hoofdlocatie worden geplaatst.
* Het bestand moet minstens één webpagina met statische bestanden bevatten.
* De maximale bundelgrootte is 500 MB.
* In het geval van ZIP-bestanden die in iOS zijn gemaakt, identificeert het programma automatisch de map waarin de inhoud zich bevindt.
* Interactieve projecten worden alleen ondersteund als zip-archieven. Standaard ZIP-bestanden worden niet verzonden.
* De website moet beveiligd zijn (HTTPS).

  Dit is niet verplicht wanneer u de Desktop Proofing Viewer gebruikt.

  Zie voor meer informatie [De Desktop Proofing Viewer begrijpen](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* De website moet in een iframe kunnen worden weergegeven.

  Dit is niet verplicht wanneer u de Desktop Proofing Viewer gebruikt.

  Zie voor meer informatie [De Desktop Proofing Viewer begrijpen](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Een interactieve proefdruk maken

Nadat u het ZIP-bundelbestand hebt voorbereid, maakt u een interactieve proefdruk.

Zie voor meer informatie [Een proef maken voor interactieve inhoud in een ZIP-bestand](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Of raadpleeg de sectie als u Workfront Proof gebruikt [Een proefdruk maken voor interactieve inhoud](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) in het artikel [Proefdrukken genereren in Workfront-proefdrukken](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Informatie over het controleren van interactieve proefdrukken

We raden u aan de zelfstandige Desktop Proofing Viewer te gebruiken als de standaardviewer voor interactieve proefdrukken. Als het beleid van uw organisatie het gebruik van de Desktop Proofing Viewer-app echter niet toestaat, kan uw Workfront-beheerder uw systeem zo configureren dat u de interactieve inhoud die in een ZIP-archiefbestand is gebundeld, kunt bekijken in de webtestviewer. Voor vergelijkende informatie over de Desktop Proofing Viewer en de Web Proofing Viewer raadpleegt u [Verschillen tussen de webtestviewer en het overzicht van de Desktop Proofing Viewer](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
