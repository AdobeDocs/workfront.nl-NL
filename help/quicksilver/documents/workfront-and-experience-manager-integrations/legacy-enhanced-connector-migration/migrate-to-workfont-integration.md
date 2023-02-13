---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie
description: In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud enhanced of legacy connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service verbindt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie

In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud enhanced of legacy connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service verbindt.

>[!IMPORTANT]
>
>Deze informatie is niet van toepassing op klanten die Adobe Experience Manager Assets On-Premise- of Managed Services-omgevingen gebruiken.

## Workfront-instantie naar de Admin Console verplaatsen

Klanten die van plan zijn de nieuwe geïntegreerde technologie tussen Workfront en Adobe Experience Manager Assets as a Cloud Service te gebruiken, moeten ervoor zorgen dat hun Workfront-omgeving aan een Adobe Admin Console is gekoppeld. Voor bestaande Workfront-omgevingen is hiervoor waarschijnlijk een migratie van de omgeving naar een aangesloten Adobe Admin Console vereist. Voor meer informatie over deze migratie en de bijbehorende checklist raadpleegt u [Voorbereiden om aan boord van uw organisatie te gaan naar de Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe moet helpen deze migratie uit te voeren. Voer een van de volgende handelingen uit om hulp aan te vragen:

* Als u de toegang van de Hub van Workfront hebt, leg uw verzoek aan voor [Workfront-migratie naar Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Als u geen toegang van de Hub van Workfront hebt, kunt u uw verzoek aan voorleggen [Workfront naar Adobe Admin Console Early Migration Request-wachtrij](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Uw nieuwe Workfront voor Adobe Experience Manager-middelen as a Cloud Service integratie configureren

Nadat uw Workfront-omgeving is gemigreerd naar een Adobe Admin Console, kunnen Workfront-beheerders de nieuwe native integratie configureren. Voor configuratiehulp, zie [De as a Cloud Service integratie met Experience Manager Assets configureren](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Bestaande middelen verplaatsen naar uw Workfront for Adobe Experience Manager-middelen as a Cloud Service integratie

Nadat u de omgeving hebt geconfigureerd, kunt u bestaande gekoppelde elementen en mappen naar Adobe Experience Manager verplaatsen. Dit is een optionele stap, maar zorgt ervoor dat eerder gekoppelde mappen en middelen via de verouderde of verbeterde connector toegankelijk blijven als deze connectors worden verwijderd.

Ga voor meer informatie over het verplaatsen van uw elementen naar [Gekoppelde mappen en documenten migreren](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valideer alle gevallen van kritisch gebruik die zijn bedoeld om te worden gebruikt

Het zal belangrijk zijn om alle kritieke gebruiksgevallen te bevestigen die bedoeld zijn om door de inheemse integratie te worden gebruikt alvorens de erfenis of de verbeterde schakelaar te verwijderen.

## De oudere of verbeterde aansluiting verwijderen

Ten slotte moet u de oudere of verbeterde aansluiting verwijderen. De native integratie is niet bedoeld om parallel met een van beide connectors te worden uitgevoerd.

Als u de installatie wilt verwijderen, raadpleegt u

* Instructies voor verwijdering van verouderde connector: [De Workfront verwijderen met de verouderde Adobe Experience Manager-aansluiting](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Uitgebreide instructies voor het verwijderen van de aansluiting: [De Workfront verwijderen met de Adobe Experience Manager Enhanced-aansluiting](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
