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
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
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

![&#x200B; pictogram van de erfeniswerkfront opslag naast projectnaam &#x200B;](assets/legacy-project-icon.png)


### Omgevingen die alleen gebruikmaken van Adobe Enterprise Storage

U kunt documenttoestemmingen op het toegangsniveau niet wijzigen voor projecten, programma&#39;s, en portefeuilles die de ondernemingsopslag van Adobe gebruiken.

Alle toegangsniveaus hebben toegang tot documenten uitgeven. Rechten op projectniveau bepalen de toegang tot documenten in andere Adobe-gereedschappen.

U kunt de toegang tot overerving van documenten niet beperken.


### Omgevingen die alleen gebruikmaken van verouderde Workfront-opslag

Geen wijzigingen in de toegangsniveaus of het gedrag van het document.


## Projecten

De gebruikers met project-vlakke toestemmingen kunnen documenten voor projecten in andere producten van Adobe zoals Frame.io en Adobe Creative Cloud bekijken en beheren.

Projectnamen zijn ook zichtbaar buiten Workfront voor ESM-projecten.

Financiële gegevens zijn buiten Workfront voor ESM-projecten niet zichtbaar.

## Taken en problemen

Documenten worden opgeslagen op projectniveau, maar kunnen zo nodig worden gedeeld met afzonderlijke taken en problemen. Gebruikers met taak- en uitgavetoegang nemen automatisch documenttoegang over van het project. U kunt hun toegangsniveau niet wijzigen. Ze hebben toegang of geen toegang beheerd.