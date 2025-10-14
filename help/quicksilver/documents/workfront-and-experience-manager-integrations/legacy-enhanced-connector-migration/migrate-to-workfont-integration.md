---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie
description: In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud verbeterde of verouderde connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service met elkaar verbindt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie

In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud verbeterde of verouderde connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service met elkaar verbindt.

>[!IMPORTANT]
>
>Deze informatie is niet van toepassing op klanten die Adobe Experience Manager Assets On-Premise- of Managed Services-omgevingen gebruiken.

## Workfront-instantie naar Admin Console verplaatsen

Klanten die van plan zijn om de nieuwe native integratie tussen Workfront en Adobe Experience Manager Assets as a Cloud Service te gebruiken, moeten ervoor zorgen dat hun Workfront-omgeving aan een Adobe Admin Console is gekoppeld. Voor bestaande Workfront-omgevingen is hiervoor waarschijnlijk een migratie van de omgeving naar een aangesloten Adobe Admin Console vereist. Voor meer details betreffende deze migratie en bijbehorende controlelijst, zie [&#x200B; voorbereidingen treffen aan aan boord van uw organisatie aan Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe moet helpen deze migratie uit te voeren. Voer een van de volgende handelingen uit om hulp aan te vragen:

* Als u de toegang van de Hub van Workfront hebt, leg uw verzoek aan de [&#x200B; Migratie van Workfront aan Adobe Admin Console &#x200B;](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=) voor.
* Als u geen toegang van de Hub van Workfront hebt, kunt u uw verzoek aan [&#x200B; Workfront voorleggen aan de Vroege Rij van het Verzoek van de Migratie van Adobe Admin Console &#x200B;](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## De nieuwe Workfront voor Adobe Experience Manager-middelen configureren - integratie met as a Cloud Service

Nadat uw Workfront-omgeving is gemigreerd naar een Adobe Admin Console, kunnen Workfront-beheerders de nieuwe native integratie configureren. Voor configuratiehulp, zie [&#x200B; de integratie van Experience Manager Assets as a Cloud Service &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen.

## Bestaande middelen verplaatsen naar uw Workfront for Adobe Experience Manager Assets as a Cloud Service-integratie

Nadat u de omgeving hebt geconfigureerd, kunt u bestaande gekoppelde elementen en mappen naar Adobe Experience Manager verplaatsen. Dit is een optionele stap, maar zorgt ervoor dat eerder gekoppelde mappen en middelen via de verouderde of verbeterde connector toegankelijk blijven als deze connectors worden verwijderd.

Voor meer informatie bij het bewegen van uw activa, zie [&#x200B; Gekoppelde omslagen en documenten migreren &#x200B;](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valideer alle gevallen van kritisch gebruik die zijn bedoeld om te worden gebruikt

Het zal belangrijk zijn om alle kritieke gebruiksgevallen te bevestigen die bedoeld zijn om door de inheemse integratie te worden gebruikt alvorens de erfenis of de verbeterde schakelaar te verwijderen.

## De oudere of verbeterde aansluiting verwijderen

Ten slotte moet u de oudere of verbeterde aansluiting verwijderen. De native integratie is niet bedoeld om parallel met een van beide connectors te worden uitgevoerd.

Als u de installatie wilt verwijderen, raadpleegt u

* De verouderde schakelaar desinstalleert instructies: [&#x200B; desinstalleert de Workfront met de verouderde schakelaar van Adobe Experience Manager &#x200B;](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Verbeterde schakelaar desinstalleert instructies: [&#x200B; desinstalleert de Workfront met Adobe Experience Manager verbeterde schakelaar &#x200B;](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
