---
product-area: documents
navigation-topic: approvals
title: Objectmachtigingen en overzicht van het toegangsniveau voor het Adobe-bedrijfsopslagmodel
description: Adobe Enterprise Storage-machtigingen en toegangsoverzicht
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
source-git-commit: 522175549d1a2b19c9e6a47a7e4b0d63ac08e3a3
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---

# Objectmachtigingen en overzicht van het toegangsniveau voor het Adobe-bedrijfsopslagmodel

<!--linked in UI -->

Adobe Enterprise Storage is een op cloud gebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe. Workfront-omgevingen die gebruikmaken van Adobe Enterprise Storage hebben iets andere objectmachtigingen en ander gedrag op toegangsniveau dan de omgevingen die gebruikmaken van verouderde Workfront-documentopslag.

## Toegangsniveaus

Workfront-toegangsniveaus zijn alleen van toepassing in Workfront. Project- en documentbeperkingen in Workfront zijn niet altijd van toepassing op andere Adobe-toepassingen.

### Omgevingen die zowel gebruikmaken van Adobe Enterprise Storage als van oudere Workfront-opslag

De toegang tot documenten gedraagt zich verschillend afhankelijk van of het project op de ondernemingsopslag van Adobe of erfenisWorkfront opslag is:

* **de opslag van Workfront van de Verouderde**: De projecten, de programma&#39;s, de portefeuilles, en de malplaatjes die de opslag van erfenisWorkfront gebruiken volgen de standaardlogica van het de toegangsniveau van Workfront voor documenttoegang. Wanneer een toegangsniveau **geen toegang** voor documenten heeft geselecteerd, kunnen zij documenten in Workfront of andere producten van Adobe zoals Frame.io of Creative Cloud zien.
* **de ondernemingsopslag van Adobe**: De projecten, de programma&#39;s, de portefeuilles, en de malplaatjes die de ondernemingsopslag van Adobe gebruiken volgen de logica van het de toegangsniveau van de ondernemingsopslag van Adobe voor andere producten van Adobe.


   * **Projecten, programma&#39;s, portefeuilles, en malplaatjeobjecten toestemmingen**: Wanneer een toegangsniveau **geen toegang** voor projecten, programma&#39;s, portefeuilles, en malplaatjes heeft geselecteerd maar het voorwerp met hen wordt gedeeld, kunnen de gebruikers het voorwerp in Workfront zien, maar zij kunnen de objecten naam en om het even welke bijbehorende documenten in andere hulpmiddelen van Adobe, zoals Frame.io en Adobe Creative Cloud nog bekijken.
   * **de toestemmingen van Documenten**: Wanneer een toegangsniveau **geen toegang** voor documenten heeft geselecteerd, kunnen de gebruikers documenten op projecten in Workfront zien, maar zij kunnen documenten voor projecten nog bekijken en beheren die met hen in andere hulpmiddelen van Adobe, zoals Frame.io en Adobe Creative Cloud worden gedeeld. Dit komt omdat de documenttoegang door project-vlakke toestemmingen in de ondernemingsopslag van Adobe, eerder dan de toegangsniveaus van Workfront alleen wordt bepaald.

Als u Adobe Enterprise Storage hebt ingeschakeld in uw Workfront-omgeving, kunt u zowel Adobe Enterprise Storage-projecten als oudere Workfront-opslagprojecten maken. Bij verouderde Workfront-opslagprojecten wordt een pictogram weergegeven naast de projectnaam, waar deze ook wordt weergegeven in Workfront. Adobe Enterprise Storage-projecten geven geen pictogram weer.

![ pictogram van de erfeniswerkfront opslag naast projectnaam ](assets/legacy-project-icon.png)


### Omgevingen die alleen gebruikmaken van Adobe Enterprise Storage

U kunt documenttoestemmingen op het toegangsniveau niet wijzigen voor projecten, programma&#39;s, en portefeuilles die de ondernemingsopslag van Adobe gebruiken.

Alle toegangsniveaus hebben toegang tot documenten uitgeven. Rechten op projectniveau bepalen de toegang tot documenten in andere Adobe-gereedschappen.

U kunt de toegang tot overerving van documenten niet beperken.


### Omgevingen die alleen gebruikmaken van verouderde Workfront-opslag

Geen wijzigingen in de toegangsniveaus of het gedrag van het document.

## Objectmachtigingen

Objectmachtigingen bepalen wat u kunt zien en doen met projecten, taken, problemen en documenten in Workfront. Machtigingen worden toegewezen wanneer iemand een object met u deelt.

>[!IMPORTANT]
>
>In Adobe Enterprise Storage werken documentmachtigingen anders dan in oudere Workfront-opslagsystemen. De documenten erven toestemmingen van het project, de taak, of uitgeven zij met verbonden zijn.


### Documentmachtigingen werken

Documentmachtigingen worden aangestuurd door het object waaraan het document is gekoppeld. U kunt geen machtigingen instellen voor afzonderlijke documenten.

Wanneer u een document uploadt naar een taak of uitgave, wordt een door het systeem gegenereerde map gemaakt met de taak- of uitgavenaam. Deze map is gekoppeld aan de taak of uitgave en neemt de machtigingen ervan over.

U kunt submappen maken in de door het systeem gegenereerde map om documenten verder te ordenen. Alle submappen overerven machtigingen van de bovenliggende map. Op projectniveau, kunt u documenten buiten een omslag uploaden, maar slechts kunnen de gebruikers met project-vlakke toegang hen zien.

Op projectniveau, tonen de systeem-geproduceerde omslagen een verbonden voorwerp. Dit is meestal de taak- of uitgavennaam en het systeem weet welke taak of uitgave de map moet worden weergegeven.

### Projectmachtigingen

Wanneer u toestemmingen op projectniveau hebt, kunt u documenten voor dat project in Workfront en andere producten van Adobe zoals Frame.io en Adobe Creative Cloud bekijken en beheren. De projectnaam is ook zichtbaar in die hulpmiddelen. Andere projectgegevens zijn niet zichtbaar buiten Workfront.

### Machtigingen voor taken en afgifte

Taken en uitgaven nemen toestemmingen van het project over. Als u machtigingen voor taken of niveaus hebt, kunt u documenten die aan die taak of uitgave zijn gekoppeld, weergeven en beheren in Workfront en andere Adobe-producten, zoals Frame.io en Adobe Creative Cloud.

**Systeem-geproduceerde omslagen**

* Als u gebruikers uit een taak of uitgave verwijdert, wordt hun maptoegang niet automatisch verwijderd. Zij kunnen toegang door project-vlakke toestemmingen nog hebben.
* Subtaken nemen door het systeem gegenereerde mapmachtigingen niet over van bovenliggende taken. U moet rechtstreeks aan een subtaak worden toegevoegd om tot zijn systeem-geproduceerde omslag toegang te hebben.
* Wanneer u gebruikers aan een taak toevoegt of uitgeeft, wordt de door het systeem gegenereerde map met die taak gedeeld.

**het bewegen en het anders noemen van systeem-geproduceerde omslagen:**

* Door het systeem gegenereerde mappen kunnen worden hernoemd en verplaatst.
* Als een door het systeem gegenereerde map naar een andere locatie wordt verplaatst, wordt het gekoppelde object bijgewerkt naar het nieuwe object. Rechten worden vervolgens overgenomen van het nieuwe bovenliggende object.

Verzoeken volgen hetzelfde gedrag als taken en problemen.

### Goedkeuringen

Wanneer u aan een werkschema van de documentgoedkeuring wordt toegevoegd, kunt u het volgende zien ongeacht projecttoestemmingen:

* Projectnaam
* Documentnaam
* Documentminiatuur










