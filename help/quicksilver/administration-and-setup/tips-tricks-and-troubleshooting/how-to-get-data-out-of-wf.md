---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Historische gegevens exporteren uit Adobe Workfront: Pros en Cons'
description: In dit artikel worden de voor- en nadelen beschreven van vier opties die u kunt gebruiken om historische gegevens uit Workfront te exporteren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Historische gegevens exporteren uit [!DNL Adobe Workfront]: Pros en cons

<!-- Audited: 5/2025 -->

In dit artikel worden de voor- en nadelen beschreven van vier opties die u kunt gebruiken om historische gegevens uit Adobe Workfront te exporteren.

## Gebruik één van onze partners

[!DNL AtAppStore] ([&#x200B; www.atappstore.com &#x200B;](https://www.atappstore.com)) heeft een makkelijk te gebruiken app (hun [&#x200B; Opname van Workfront &#x200B;](https://store.atappstore.com/product/workfront-snapshot/) oplossing) die u toestaat om uw gegevens zelf te downloaden. Een facultatieve kijker (hun [&#x200B; oplossing van de Kijker van de Momentopname van Workfront &#x200B;](https://store.atappstore.com/product/workfront-snapshot-viewer/)) staat u toe om uw gegevens offline gemakkelijk te bekijken.

* **Pros:** Al uw kern [!DNL Workfront] voorwerpen worden uitgevoerd, met inbegrip van de douanegebieden en de nota&#39;s, en opgeslagen in een gemakkelijk toegankelijk [!DNL MS Access] gegevensbestand. De interface van de Viewer is gebruiksvriendelijk en leesbaar. Het uitpakken van Documenten is ook afzonderlijk beschikbaar als een service, waarbij de uitvoer is ingedeeld in een logische mapstructuur die is toegewezen aan elk document en de voorgaande versies.

* **Kons:** er is een technische beperking van 2 GB van gegevens, maar AtAppStore staat u toe om slechts te kopen wat u nodig hebt.

* **Kosten:** voor meer informatie, ga [&#x200B; https://store.atappstore.com/product/workfront-snapshot/ &#x200B;](https://store.atappstore.com/product/workfront-snapshot/).

## Vraag een [!DNL Postgres] gegevensdumpbestand aan van ons databaseteam

U moet een verzoek indienen bij ons Customer Support-team, dat vervolgens een aanvraag zal indienen bij ons databaseteam om een databasedumpdump-bestand (.dmp [!DNL Postgres] -bestand) met uw gegevens te exporteren. Een extra verzoek zal naar ons team NOC gaan om al uw opgeslagen documenten terug te winnen.

* **Pros**: U krijgt uw volledige gegevenslading, met inbegrip van douanegebieden, evenals documenten die in het systeem worden opgeslagen.

* **Kons**: Er is geen manier om dit dossier te lezen tenzij u het aan een [!DNL Postgres] gegevensbestand uploadt en de verhoudingen tussen de lijsten herstelt. De documenten worden opgeslagen op een afzonderlijke dossierserver en moeten afzonderlijk worden gehaald gebruikend een afzonderlijk proces door het team NOC. Hierbij, is er geen organisatie aan de documenten, en zij worden allen van verwijzingen voorzien door hun GUID.

* **Kosten**: Er zijn kosten verbonden aan deze download afhankelijk van hoe lang het het team neemt om het dossier tot stand te brengen. Raadpleeg uw AE/CAE voor meer informatie of om dit proces op gang te brengen.

## Exporteren via [!UICONTROL Kick-Starts]

Of u nu externe consultinguren hebt of niet, u kunt een van onze consultants gebruiken om uw gegevens te exporteren in de vorm van rapporten of [!UICONTROL kick-starts] , of u kunt deze rapporten zelf uitvoeren:

* **Pros**: De rapporten zijn gemakkelijk te lezen en kunnen in een verscheidenheid van toepassingen worden ingevoerd. Ze kunnen worden aangepast en gegroepeerd en bekeken.

* **Kons**: De documenten zullen afzonderlijk moeten worden gedownload.

* **Kosten**: Het is vrij als u de rapporten kunt in werking stellen zelf (allen u een login van systeemadmin) nodig hebt, of als u resterende verre raadplegende uren kunt gebruiken. Neem contact op met uw AE/CAE als u hiervoor advies op afstand wilt aanschaffen.

  Voor meer informatie over het gebruiken van Kick-Begint om gegevens uit te voeren, zie [&#x200B; Gegevens van de Uitvoer van  [!DNL Adobe Workfront]  via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Onze open API gebruiken

Als u beschikt over de juiste bronnen in uw organisatie, kunt u een aangepaste API maken om al uw gegevens op te halen uit Workfront:

* **Pros**: U hebt controle over wat de uitvoer van het systeem.

* **Kons**: De tijd wordt besteed aan uw kant, en u zult middelen moeten vinden om API te coderen en de uitvoer uit te voeren.

* **Kosten**: Het is intern aan uw organisatie.
