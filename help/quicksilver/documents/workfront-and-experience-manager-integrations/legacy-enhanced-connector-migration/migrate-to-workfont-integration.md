---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie
description: In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud verbeterde of verouderde connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service met elkaar verbindt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie

In de informatie op deze pagina vindt u een uitleg van de aanbevolen procedures voor het overstappen van de Workfront for Experience Cloud verbeterde of verouderde connectors naar de nieuwste native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service met elkaar verbindt.

>[!IMPORTANT]
>
>Deze informatie is niet van toepassing op klanten die Adobe Experience Manager Assets On-Premise- of Managed Services-omgevingen gebruiken.

## Workfront-instantie naar Admin Console verplaatsen

>[!IMPORTANT]
>
>Omdat alle Workfront-organisaties naar de Adobe Admin Console zijn gemigreerd, wordt deze sectie in de nabije toekomst verwijderd.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## De nieuwe Workfront voor Adobe Experience Manager-middelen configureren - integratie met as a Cloud Service

Nadat uw Workfront-omgeving is gemigreerd naar een Adobe Admin Console, kunnen Workfront-beheerders de nieuwe native integratie configureren. Voor configuratiehulp, zie [ de integratie van Experience Manager Assets as a Cloud Service ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen.

## Bestaande middelen verplaatsen naar uw Workfront for Adobe Experience Manager Assets as a Cloud Service-integratie

Nadat u de omgeving hebt geconfigureerd, kunt u bestaande gekoppelde elementen en mappen naar Adobe Experience Manager verplaatsen. Dit is een optionele stap, maar zorgt ervoor dat eerder gekoppelde mappen en middelen via de verouderde of verbeterde connector toegankelijk blijven als deze connectors worden verwijderd.

Voor meer informatie bij het bewegen van uw activa, zie [ Gekoppelde omslagen en documenten migreren ](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valideer alle gevallen van kritisch gebruik die zijn bedoeld om te worden gebruikt

Het zal belangrijk zijn om alle kritieke gebruiksgevallen te bevestigen die bedoeld zijn om door de inheemse integratie te worden gebruikt alvorens de erfenis of de verbeterde schakelaar te verwijderen.

## De oudere of verbeterde aansluiting verwijderen

Ten slotte moet u de oudere of verbeterde aansluiting verwijderen. De native integratie is niet bedoeld om parallel met een van beide connectors te worden uitgevoerd.

Als u de installatie wilt verwijderen, raadpleegt u

* De verouderde schakelaar desinstalleert instructies: [ desinstalleert de Workfront met de verouderde schakelaar van Adobe Experience Manager ](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Verbeterde schakelaar desinstalleert instructies: [ desinstalleert de Workfront met Adobe Experience Manager verbeterde schakelaar ](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
