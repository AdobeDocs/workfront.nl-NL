---
title: Verbeteringen voor eerste kwartaal 2024-integratie
description: Verbeteringen voor eerste kwartaal 2024-integratie
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Verbeteringen voor eerste kwartaal 2024-integratie

Op deze pagina worden alle integratieverbeteringen beschreven die zijn aangebracht met de release Eerste kwartaal 2024 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving met de release Eerste kwartaal 2024.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Eerste Kwartaal 2024 versiecyclus, zie [&#x200B; Eerste Kwartaal 2024 releaseoverzicht &#x200B;](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Metagegevens toewijzen in Experience Manager Assets Essentials gebruikt nu `xcm:keywords` in plaats van `dc:subject`

We hebben de Experience Manager Assets Essentials-integratie bijgewerkt en aangepast aan de ervaring die is opgedaan met de as a Cloud Service integratie van Experience Manager Assets. Wanneer u nu meerdere tekstvelden met één regel aan één veld in Experience Manager Assets toewijst, gebruiken beide services het veld `xcm:keywords` .

Eerder werden deze velden toegewezen aan het veld `dc:subject` in Experience Manager Assets Essentials. De as a Cloud Service Experience Manager Assets-functionaliteit blijft ongewijzigd.

Alle Experience Manager Assets Essentials-metagegevens die momenteel zijn toegewezen aan `dc:subject` moeten opnieuw worden toegewezen aan `xcm:keywords` .

Voor informatie bij het in kaart brengen van meta-gegevens aan de Hoofdzaak van Experience Manager Assets, zie [&#x200B; AEM Sleutelwoord &#x200B;](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Typeahead-velden zijn nu beschikbaar in Adobe Experience Manager-integratie

Om het gemakkelijker te maken om gebieden tussen Workfront en Adobe Experience Manager te verbinden, hebben wij steun voor typeahead gebieden in de meta-gegevensafbeelding toegevoegd. Nu kunt u typeahead-velden toewijzen aan corresponderende velden in Adobe Experience Manager.

Als een gebruiker een andere waarde voor een veld in Workfront selecteert, wordt deze wijziging direct doorgevoerd in Adobe Experience Manager. Als een optie voor de veldwaarde wordt gewijzigd (bijvoorbeeld een team dat de naam wijzigt in een nieuwe naam), wordt deze wijziging ook doorgevoerd in Adobe Experience Manager.

Voor informatie en instructies op meta-gegevensafbeelding in de integratie van Adobe Experience Manager, zie [&#x200B; de meta-gegevens van de Opstelling &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Elementen automatisch publiceren in Adobe Experience Manager

We hebben nog een workflow toegevoegd aan de Adobe Experience Manager-integratie. Nu kunt u instellen dat uw elementen automatisch worden gepubliceerd wanneer ze naar Adobe Experience Manager worden verzonden. De integratie kan worden geconfigureerd om te publiceren naar de Adobe Experience Manager-publicatieservice of naar een Adobe Experience Manager-portaalsite.

De automatische Publish-workflow kan worden ingeschakeld en geconfigureerd in de Adobe Experience Manager-integratie. Wanneer toegelaten, kan het werkschema op het projectmalplaatje of projectniveau worden uitgegeven.

Voor meer informatie, zie [&#x200B; het Publiceren activa &#x200B;](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [&#x200B; werkschema&#39;s van het Gebruik in de integratie van Experience Manager Assets &#x200B;](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
