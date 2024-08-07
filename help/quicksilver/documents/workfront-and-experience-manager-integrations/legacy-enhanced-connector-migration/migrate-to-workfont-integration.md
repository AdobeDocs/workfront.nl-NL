---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie
description: In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud Enhanced of legacy connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service met elkaar verbindt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie

In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud Enhanced of legacy connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service met elkaar verbindt.

>[!IMPORTANT]
>
>Deze informatie is niet van toepassing op klanten die Adobe Experience Manager Assets On-Premise- of Managed Services-omgevingen gebruiken.

## Workfront-instantie naar de Admin Console verplaatsen

Klanten die van plan zijn de nieuwe geïntegreerde native integratie tussen Workfront en Adobe Experience Manager Assets as a Cloud Service te gebruiken, moeten ervoor zorgen dat hun Workfront-omgeving aan een Adobe Admin Console is gekoppeld. Voor bestaande Workfront-omgevingen is hiervoor waarschijnlijk een migratie van de omgeving naar een aangesloten Adobe Admin Console vereist. Voor meer details betreffende deze migratie en bijbehorende controlelijst, zie [ voorbereidingen treffen aan aan boord van uw organisatie aan Adobe Admin Console ](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe moet helpen bij het uitvoeren van deze migratie. Voer een van de volgende handelingen uit om hulp aan te vragen:

* Als u de toegang van de Hub van Workfront hebt, leg uw verzoek aan de [ Migratie van Workfront aan Adobe Admin Console ](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=) voor.
* Als u geen toegang van de Hub van Workfront hebt, kunt u uw verzoek aan [ Workfront voorleggen aan de Vroege Rij van het Verzoek van de Migratie van Adobe Admin Console ](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Uw nieuwe Workfront voor Adobe Experience Manager-middelen as a Cloud Service integreren

Nadat uw Workfront-omgeving is gemigreerd naar een Adobe Admin Console, kunnen Workfront-beheerders de nieuwe native integratie configureren. Voor configuratiehulp, zie [ de as a Cloud Service integratie van Experience Manager Assets ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen.

## Bestaande middelen verplaatsen naar uw Workfront for Adobe Experience Manager Assets as a Cloud Service integratie

Nadat u de omgeving hebt geconfigureerd, kunt u bestaande gekoppelde elementen en mappen naar Adobe Experience Manager verplaatsen. Dit is een optionele stap, maar zorgt ervoor dat eerder gekoppelde mappen en middelen via de verouderde of verbeterde connector toegankelijk blijven als deze connectors worden verwijderd.

Voor meer informatie bij het bewegen van uw activa, zie [ Gekoppelde omslagen en documenten migreren ](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valideer alle gevallen van kritisch gebruik die zijn bedoeld om te worden gebruikt

Het zal belangrijk zijn om alle kritieke gebruiksgevallen te bevestigen die bedoeld zijn om door de inheemse integratie te worden gebruikt alvorens de erfenis of de verbeterde schakelaar te verwijderen.

## De oudere of verbeterde aansluiting verwijderen

Ten slotte moet u de oudere of verbeterde aansluiting verwijderen. De native integratie is niet bedoeld om parallel met een van beide connectors te worden uitgevoerd.

Als u de installatie wilt verwijderen, raadpleegt u

* De verouderde schakelaar desinstalleert instructies: [ desinstalleert de Workfront met de verouderde schakelaar van Adobe Experience Manager ](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Verbeterde schakelaar desinstalleert instructies: [ desinstalleert de Workfront met Adobe Experience Manager verbeterde schakelaar ](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
