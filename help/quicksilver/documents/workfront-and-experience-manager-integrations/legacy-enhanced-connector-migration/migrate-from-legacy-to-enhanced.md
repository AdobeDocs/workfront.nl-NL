---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migreren van de verouderde aansluiting naar de verbeterde aansluiting
description: In het volgende proces worden de beste praktijken beschreven voor het verplaatsen van de bestaande Adobe Experience Manager-connector naar de verbeterde connector voor de integratie van Adobe Workfront met AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Migreren van de verouderde aansluiting naar de verbeterde aansluiting

In het volgende proces worden de beste praktijken beschreven voor het verplaatsen van de bestaande Adobe Experience Manager-connector naar de verbeterde connector voor de integratie van Adobe Workfront met AEM Assets.

>[!IMPORTANT]
>
>Deze documentatie is alleen van toepassing op klanten die Adobe Experience Manager Assets On-Premise- of Managed Services-omgevingen gebruiken.


Voor klanten met Adobe Experience Manager Assets as a Cloud Service zal het migratiepad van de verouderde connector naar de nieuwe native integratie binnen Workfront zijn. Voor meer informatie over dit migratieproces raadpleegt u [Migreren van de verouderde of verbeterde aansluiting naar Workfront voor Adobe Experience Manager as a Cloud Service-integratie](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementeer de verbeterde aansluiting

>[!IMPORTANT]
>
>Een verklaarde partner of de Raadplegende Diensten van de Adobe worden vereist voor implementatie van de verbeterde schakelaar.
>
> Voor partners die op de verbeterde schakelaar willen verklaren gelieve het volgende artikel te herzien: [Workfront for Experience Manager Enhanced connector Expert-reeks](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Om de verbeterde schakelaar uit te voeren, zie [Workfront for Experience Manager Enhanced-connector configureren](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Bestaande elementen verplaatsen

Nadat u de omgeving hebt geconfigureerd, kunt u bestaande gekoppelde elementen en mappen naar Adobe Experience Manager verplaatsen. Dit is een optionele stap, maar zorgt ervoor dat eerder gekoppelde mappen en middelen via de verouderde connector toegankelijk blijven als de verouderde connector wordt verwijderd.

Ga voor meer informatie over het verplaatsen van uw elementen naar [Gekoppelde mappen en documenten migreren](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valideer alle gevallen van kritisch gebruik die zijn bedoeld om te worden gebruikt

Het is belangrijk om alle kritieke gebruiksgevallen te bevestigen die bedoeld zijn om door de verbeterde schakelaar te worden gebruikt alvorens de erfenisschakelaar te verwijderen.

## De oudere aansluiting verwijderen

Ten slotte moet u de oudere connector verwijderen. De oudere connector is niet bedoeld om parallel met de verbeterde connector te worden uitgevoerd.

Als u de installatie wilt verwijderen, raadpleegt u [De Workfront verwijderen met de verouderde Adobe Experience Manager-aansluiting](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
