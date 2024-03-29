---
title: 23.3 Verbeterde integratie
description: 23.3 Verbeterde integratie
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# 23.3 Verbeterde integratie

Op deze pagina worden alle integratieverbeteringen beschreven die zijn aangebracht met de release 23.3. Deze verbeteringen zijn beschikbaar gesteld in de productieomgeving met de release 23.3 op 20 en 21 juli 2023.

Voor een lijst van alle veranderingen beschikbaar op dit punt in de 23.3 versiecyclus, zie [23.3 Overzicht van de release](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Nieuwe G Suite-integratie nu beschikbaar

Er is nu een nieuwe G Suite-integratie beschikbaar in de Google Marketplace. De nieuwe integratie verifieert gebruikend OAuth2, en vervangt de vorige integratie.

De vorige G Suite-integratie is nu afgekeurd en wordt automatisch verwijderd.

Voor instructies over het installeren van de nieuwe integratie raadpleegt u [Installeren [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Zie voor meer informatie over Workfront for G Suite [Workfront for G Suite](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## De integratie van Adobe Creative Cloud steunt nu veelvoudige toegewezen gebruikers

De Adobe Creative Cloud-integratie ondersteunt nu de mogelijkheid te kiezen tussen &quot;Gereed met mijn onderdeel&quot; en &quot;Voltooid&quot; (of &quot;Opgelost&quot;) wanneer een taak of uitgave meerdere toegewezen gebruikers heeft.

Eerder, stond de integratie gebruikers toe om een taak te merken zoals gedaan, zonder &quot;Gedaan met mijn deel&quot;te specificeren of &quot;Volledig&quot;/&quot;Opgelost.&quot;

Download en installeer de nieuwste Workfront for Creative Cloud-plug-ins om deze functionaliteit te benutten.

Zie voor meer informatie over de functionaliteit [Werkitems markeren die zijn voltooid met de Adobe Workfront-insteekmodule](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Voor informatie over het installeren van de Workfront for Creative Cloud plug-ins raadpleegt u [De Adobe Workfront-insteekmodule voor Creative Cloud-toepassingen installeren](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Workfront-meldingen van de Workfront for Creative Cloud-plug-ins weergeven en beheren

Om het voor u gemakkelijker te maken om de berichten te ontvangen u wenst, hebben wij het mogelijk gemaakt om Workfront berichten te bekijken en te beheren zonder de Adobe Creative Cloud te verlaten. U kunt nu meldingen en de bijbehorende werkitems en opmerkingen rechtstreeks bekijken in het Workfront-insteekvenster van de toepassing Creative Cloud.

Eerder waren meldingen alleen beschikbaar in Workfront en via e-mail.

Download en installeer de nieuwste Workfront for Creative Cloud-plug-ins om deze functionaliteit te benutten.

Zie voor meer informatie [Weergeven en beheren [!DNL Adobe Workfront] kennisgevingen van Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Voor informatie over het installeren van de Workfront for Creative Cloud plug-ins raadpleegt u [De Adobe Workfront-insteekmodule voor Creative Cloud-toepassingen installeren](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Automatisch gekoppelde mappen naar Adobe Experience Manager Assets maken wanneer u een project maakt

Met de nieuwe workflow voor het maken van een gekoppelde map voor de Adobe Experience Manager-integratie kunt u de integratie configureren met een pad naar een Adobe Experience Manager Assets-map. Wanneer de integratie aan een projectmalplaatje wordt toegevoegd, zullen om het even welke projecten die van het malplaatje worden gecreeerd automatisch tot een verbonden subfolder in Experience Manager Assets in de gespecificeerde omslag leiden.

Eerder moest de gebruiker actie ondernemen bij het maken van gekoppelde mappen.

Deze functionaliteit is alleen beschikbaar bij Adobe Experience Manager as a Cloud Service-integratie in Workfront. Dit is niet beschikbaar in de verbeterde Adobe Experience Manager-connector.

Zie voor meer informatie [Workflows gebruiken in de Experience Manager Assets-integratie](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Workfront-veldwaarden toewijzen aan labels in Experience Manager Assets

Nu kunt u elementen categoriseren en snel zoeken op basis van gegevens van Workfront. U kunt deze gegevens toewijzen als onderdeel van de configuratie van metagegevens in de Workfront for Experience Manager Assets-integratie.

Eerder was het niet mogelijk om Workfront-gegevens toe te wijzen aan Experience Manager Assets-tags.

Voor meer informatie over deze functionaliteit in as a Cloud Service Experience Manager Assets raadpleegt u [Vorm [!UICONTROL Experience Manager Assets as a Cloud Service] integratie](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Zie voor meer informatie over deze functionaliteit in Experience Manager Assets Essentials [De integratie met Experience Manager Assets Essentials configureren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Workfront-velden toewijzen aan aangepaste Experience Manager Assets-metagegevensvelden

Met de geïntegreerde native modus kunt u nu zowel native als ingebouwde Workfront-velden toewijzen aan aangepaste metagegevensschemavelden in Experience Manager Assets as a Cloud Service.

Voor meer informatie over deze functionaliteit in as a Cloud Service Experience Manager Assets raadpleegt u [Vorm [!UICONTROL Experience Manager Assets as a Cloud Service] integratie](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Zie voor meer informatie over deze functionaliteit in Experience Manager Assets Essentials [De integratie met Experience Manager Assets Essentials configureren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Instellingen voor automatische proefdrukwerkstromen aanpassen met Adobe Workfront for Creative Cloud

U kunt de bestaande sjablooninstellingen voor geautomatiseerde workflows nu rechtstreeks in het Creative Cloud aanpassen. Nadat u een bestaande automatische werkstroomsjabloon hebt gekozen, kunt u:

* Frames uitschakelen
* Extra ontvangers toevoegen
* Proefdrukrollen wijzigen
* De deadline aanpassen
* E-mailmeldingen bijwerken
* En meer!

Zie voor meer informatie [Documenten en proefdrukken uploaden met de [!DNL Adobe Workfront] insteekmodule voor [!DNL Creative Cloud] Toepassingen](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Deze verbeteringen zijn beschikbaar voor de volgende Creative Cloud-apps:

* Photoshop
* XD
* InDesign
* Illustrator
