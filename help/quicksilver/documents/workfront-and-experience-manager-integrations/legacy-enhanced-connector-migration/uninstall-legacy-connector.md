---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: De oudere aansluiting verwijderen
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 1%

---

# De Workfront verwijderen met de verouderde Adobe Experience Manager-aansluiting

U moet de Workfront met de verouderde Adobe Experience Manager-aansluiting verwijderen voor de meest recente native integratie die Workfront en Adobe Experience Manager Assets as a Cloud Service verbindt.

## Abonnement op Workfront opzeggen

1. Open Adobe Experience Manager.
1. Ga in de Experience Manager naar **Gereedschappen** > **Cloud Services** > **Workfront Integration Configuration**.
1. Selecteer uw configuratie (globaal-werkfront door gebrek), en klik **Eigenschappen**.
   ![abonnement opzeggen van werkfront](assets/unsubscribe-from-workfront.png)
1. Documentsynchronisatie, Opmerking en Metagegevenssynchronisatie uitschakelen. De label moet dag uitgeschakeld zijn.
Hiermee worden de abonnementen in Workfront verwijderd en kan de gebruiker een nieuw abonnement maken met dezelfde URL als die is gedefinieerd in Day CQ Link Externalzer.

## Workfront Integration Configuration verwijderen

Na het verwijderen van het abonnement is het nu veilig om de Configuratie van de Integratie van Workfront te schrappen.

1. Open de configuratie en selecteer **Verwijderen**.
   ![configuratie verwijderen](assets/delete-wf-configuration.png)

## Koppeling verwijderen

Vervolgens moet u Workfront-eigenschappentoewijzing verwijderen.

1. Ga in de Experience Manager naar **Gereedschappen** > **Activa** > **Workfront-eigenschappentoewijzing**.

1. Selecteer alle toewijzingen en klik op **Verwijderen**.

## Gebruikersmachtigingen

Alle gebruikers die AEM Dam van Workfront toegang hebben, kregen leestemmingen aan `/content/dam`. Als een gebruiker dat niet meer nodig heeft, kunt u de toestemmingen verwijderen die aan genoemde gebruikers worden gegeven.

De connector werkt met behulp van de workfront-service van de systeemgebruiker. Dit wordt verwijderd wanneer u de aansluiting verwijdert.

>[!NOTE]
>
>Als u connecter versie 2.0.3 gebruikt en de groep hebt toegevoegd `workfront-aem-connector-group`, moet ook worden verwijderd door **Gereedschappen** > **Beveiliging** > **Groepen**.

## Day CQ Link ExternalAlizer

Als u niet de Verbinding Externalzer van de Vraag van de Dag CQ nodig hebt, kunt u dit terug naar `localhost:4502` door naar `/system/console/configMgr` en op zoek naar &#39;Day CQ Link Externalzer&#39;.

>[!NOTE]
>
>Als u Adobe Experience Manager as a Cloud Service gebruikt, kunt u dit wijzigen door uw project te bekijken en het bestand te zoeken _com.day.cq.commons.impl.ExternalImpl.xml_ binnenkant _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ Link ExternalAlizer](assets/Day-CQ-Link-Externalizer.png)

## Connector-pakket verwijderen

De stappen die nodig zijn om het schakelaarpakket te verwijderen, verschillen afhankelijk van welke versie van Adobe Experience Manager u hebt.

### Adobe Experience Manager op locatie

Als je Adobe Experience Manager op locatie gebruikt, ga je naar _crx/packmgr/index.jsp_ en zoekt naar de `workfront-aem-connector.all-<version>.zip`, klikt u op **Meer** en vervolgens **Verwijderen**.

Gelieve onder te checken `/conf` om ervoor te zorgen dat alle door Workfront gemaakte bestanden zijn verwijderd.

###  voor Adobe Experience Manager as a Cloud Service

Voor Adobe Experience Manager as a Cloud Service, kunt u de gebiedsdelen voor de schakelaar uit pom.files van het project verwijderen.

## Firewall en Dispatcher

Vergeet niet je gewitste Workfront-URL&#39;s te verwijderen als communicatie niet meer nodig is. Bovendien gebruikt de connector de headers apiKey en de gebruikersnaam die op de dispatcher zijn ingesteld. Deze kunnen ook worden verwijderd.
