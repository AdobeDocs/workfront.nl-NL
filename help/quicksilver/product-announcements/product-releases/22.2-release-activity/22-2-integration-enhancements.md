---
title: 22.2 Verbeterde integratie
description: 22.2 Verbeterde integratie
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2 Verbeterde integratie

Op deze pagina worden alle verbeteringen beschreven die zijn aangebracht in de versie 22.2 voor integratie in de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

4 april 2022.

Voor een lijst van alle veranderingen beschikbaar met de versie 22.2, zie [ 22.2 Overzicht van de Versie ](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront met Anaplan-integratie is nu beschikbaar

Om u meer flexibiliteit en insight te geven in de financiële aspecten van uw Workfront-projecten, kan Workfront nu integreren met uw Anaplan-account. Door Workfront-objecten aan Anaplan-objecten te koppelen, kunt u automatisch informatie tussen de twee accounts bijwerken, zodat de informatie in beide accounts up-to-date en identiek is. U kunt geautomatiseerde processen in Anaplan ook activeren op basis van acties in Workfront (of vice versa).

U kunt bijvoorbeeld een campagne maken in Anaplan en vervolgens een Workfront-project of -programma maken dat is gekoppeld aan de campagne. Eventuele kosten die in Workfront worden bijgehouden, kunnen vervolgens naar Anaplan worden geüpload om de prestaties van de campagne te beoordelen.

Andere workflows die u kunt overwegen om de integratie van Workfront naar Anaplan te gebruiken voor zijn:

* Aanvragen voor Anaplan-begrotingsmiddelen voor nieuwe Workfront-projecten maken
* Workfront-projecten maken van nieuwe Anaplan-lijstonderdelen
* Aanvang van verzoeken van Anaplan-leveranciers uit Workfront-projecten

Voor meer informatie, zie [ Adobe Workfront met Anaplan ](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront for Experience Manager verbeterde connectorupdates

Workfront for Experience Manager Enhanced Connector bevat nu de volgende updates:

* U kunt nu gekoppelde mappen maken tussen Adobe Workfront en Adobe Experience Manager Assets as a Cloud Service, zelfs als er meerdere aan een project gekoppelde mapconfiguraties zijn.
* Extra ondersteuning voor paginering van abonnementen voor gebeurtenissen
* Extra ondersteuning voor AEM 6.4.x
* Extra ondersteuning voor proxyomgevingen
* Verscheidene insectenmoeilijke situaties die op partner en klant worden gebaseerd terugkoppelen

Voor meer informatie, zie [ Workfront voor Experience Manager verbeterd schakelaaroverzicht ](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Voor de implementatie en configuratie van deze connector is een gecertificeerde partner vereist. Zie [ installeer Workfront voor Experience Manager verbeterde schakelaar ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install) voor meer informatie.

## Adobe Creative Cloud-integratie gebruikt nu OAuth2

Voor grotere veiligheid, en om een consistentere ervaring over integratie te maken, hebben wij de integratie van Adobe Creative Cloud bijgewerkt om authentificatie te gebruiken OAuth2, een industrie-standaardmanier om gebruikers voor authentiek te verklaren. Wanneer uw gebruikers zich nu aanmelden, kunnen ze de specifieke acties en gebieden zien waartoe de integratie toegang heeft en toegang verlenen. Hierna hoeven ze zich niet zo vaak aan te melden.

Voor meer informatie, zie [ de Uitbreiding van Workfront voor Illustrator en InDesign ](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md) gebruiken.

## Zie details van het Geheim van de Cliënt voor douaneOAuth2 of integratie JWT

Om transparantie in het gebruik van uw douaneOAuth2 en integratie te verstrekken JWT, hebben wij het voor u mogelijk gemaakt om details van de Ontwerpen van de Cliënt te zien uw integratiegebruik. Nu, kunt u de data zien dat het Geheime Geheime van de Cliënt werd gecreeerd en het laatst gebruikt. U kunt ook uw eigen notities over het clientgeheim toevoegen en weergeven.

Eerder waren deze gegevens niet beschikbaar.

Voor meer informatie over de Secreten van de Cliënt in OAuth2 of JWT douaneintegratie, zie [ tot toepassingen OAuth2 voor de integratie van Workfront ](../../../administration-and-setup/configure-integrations/create-oauth-application.md) leiden.

## Zie type authentificatie in lijst van douaneOAuth2 toepassingen

Nu, wanneer u de lijst van douaneOAuth2 toepassingen in uw organisatie bekijkt, kunt u zien of elke toepassing gebruikersauthentificatie of de authentificatie van de Server gebruikt.

Eerder kon u deze informatie alleen zien door in de bewerkingsopties voor elke toepassing te gaan.

Voor meer informatie, zie [ toepassingen OAuth2 voor de integratie van Workfront ](../../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

## Vervaldatum instellen voor vernieuwingstokens in uw aangepaste OAuth2-integratie

Om toegang en veiligheid voor uw douaneOAuth2 integratie beter te controleren, kunt u de levensduur van verfrist tokens nu aanpassen. Nadat het vernieuwingstoken van een gebruiker verloopt, zullen zij aan login aan de integratie opnieuw moeten.

Voor meer informatie, zie [ toepassingen OAuth2 voor de integratie van Workfront ](../../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

## De openbare en privé sleutels van het gebruik in uw douaneOAuth2 integratie voor server-aan-server apps

U kunt server-aan-server OAuth2 toepassingen nu in uw douaneservers plaatsen. Door openbare en persoonlijke sleutels in te stellen, kunt u Workfront toestaan te communiceren met een andere toepassing zonder aanmeldingsgegevens te gebruiken.

Eerder, gebruikte alle authentificatie in uw douane OAuth2 toepassingen de login van de gebruiker geloofsbrieven.

Voor meer informatie, zie [ toepassingen OAuth2 voor de integratie van Workfront ](../../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

## Google Google Workspace-integratie gebruikt nu OAuth2

Voor meer veiligheid, en om een consistentere ervaring over integratie te maken, hebben wij de integratie van Google Google Workspace bijgewerkt om authentificatie te gebruiken OAuth2, een industrie-standaardmanier om gebruikers voor authentiek te verklaren. Wanneer uw gebruikers zich nu aanmelden, kunnen ze de specifieke acties en gebieden zien waartoe de integratie toegang heeft en toegang verlenen. Hierna hoeven ze zich niet zo vaak aan te melden.

Voor meer informatie, zie [ Login en uit Adobe Workfront voor Google Workspace ](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
