---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migreren van de verouderde aansluiting naar de verbeterde aansluiting
description: In het volgende proces worden de beste praktijken beschreven voor het verplaatsen van de bestaande Adobe Experience Manager-connector naar de verbeterde connector voor de integratie van Adobe Workfront met AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Migreren van de verouderde aansluiting naar de verbeterde aansluiting

In het volgende proces worden de beste praktijken beschreven voor het verplaatsen van de bestaande Adobe Experience Manager-connector naar de verbeterde connector voor de integratie van Adobe Workfront met AEM Assets.

>[!IMPORTANT]
>
>Deze documentatie is alleen van toepassing op klanten die Adobe Experience Manager Assets On-Premise- of Managed Services-omgevingen gebruiken.


Voor klanten op Adobe Experience Manager Assets as a Cloud Service zal het migratiepad van de verouderde connector naar de nieuwe native integratie binnen Workfront zijn. Meer over dit migratieproces leren, zie [&#x200B; van de erfenis of verbeterde schakelaar aan Workfront voor de integratie van Adobe Experience Manager as a Cloud Service &#x200B;](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md) migreren.

## Implementeer de verbeterde aansluiting

>[!IMPORTANT]
>
>Een verklaarde partner of de Diensten van Adobe Consulting worden vereist voor implementatie van de verbeterde schakelaar.
>
> Voor partners die op de verbeterde schakelaar willen verklaren gelieve het volgende artikel te herzien: [&#x200B; Workfront voor Experience Manager verbeterde schakelaarDeskundige Reeks &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

Om de verbeterde schakelaar uit te voeren, zie [&#x200B; Workfront voor Experience Manager verbeterde schakelaar &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure) vormen.


## Bestaande elementen verplaatsen

Nadat u de omgeving hebt geconfigureerd, kunt u bestaande gekoppelde elementen en mappen naar Adobe Experience Manager verplaatsen. Dit is een optionele stap, maar zorgt ervoor dat eerder gekoppelde mappen en middelen via de verouderde connector toegankelijk blijven als de verouderde connector wordt verwijderd.

Voor meer informatie bij het bewegen van uw activa, zie [&#x200B; Gekoppelde omslagen en documenten migreren &#x200B;](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valideer alle gevallen van kritisch gebruik die zijn bedoeld om te worden gebruikt

Het is belangrijk om alle kritieke gebruiksgevallen te bevestigen die bedoeld zijn om door de verbeterde schakelaar te worden gebruikt alvorens de erfenisschakelaar te verwijderen.

## De oudere aansluiting verwijderen

Ten slotte moet u de oudere connector verwijderen. De oudere connector is niet bedoeld om parallel met de verbeterde connector te worden uitgevoerd.

Om te desinstalleren, zie [&#x200B; de Workfront met de erfenisschakelaar van Adobe Experience Manager &#x200B;](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md) desinstalleren.
