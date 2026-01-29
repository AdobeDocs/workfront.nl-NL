---
title: Overzicht van verbonden records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden. In dit artikel worden overwegingen beschreven waarmee u rekening moet houden wanneer u records verbindt in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Overzicht van verbonden records

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

U kunt Adobe Workfront-planningsrecords met elkaar of met objecten van andere toepassingen verbinden.

In dit artikel worden overwegingen beschreven waarmee u rekening moet houden wanneer u records verbindt in Workfront Planning.

Voor informatie over hoe u verslagen met elkaar of met een ander voorwerp kunt verbinden, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

## Vereisten

U moet verbinding maken met het volgende voordat u verbinding kunt maken met records in Workfront Planning:

* Twee recordtypen
* Een recordtype met een object uit een andere toepassing

Voor meer informatie, zie [ Verbonden overzicht van recordtypes ](/help/quicksilver/planning/architecture/connect-record-types-overview.md).


## Overwegingen bij het verbinden van records

* Nadat u recordtypes verbindt, tonen de verbonden verslagtypes als verbindingsgebieden in de lijst van de verslagtypes zij van en op de verslagpagina&#39;s verbonden zijn.
* U kunt records en objecten van de gekoppelde record- en objecttypen bladeren en deze toevoegen vanuit de gekoppelde recordvelden.
* U kunt velden (opzoekvelden) van de gekoppelde recordtypen toevoegen aan de tabel van het recordtype waarvan u een koppeling maakt.

  U kunt ook velden (opzoekvelden) toevoegen van de recordtypen die u koppelt in de tabel van het recordtype waarnaar u een koppeling maakt.

  Als u bijvoorbeeld het recordtype product van het recordtype Campagne koppelt, kunt u zowel productvelden voor campagnes als campagnevelden voor producten weergeven.
* U kunt de waarden van opzoekvelden in de records waarvan u een koppeling maakt, niet handmatig bijwerken.

  De waarden van de opzoekvelden vullen de Workfront-planningsrecord die u koppelt automatisch nadat deze zijn bijgewerkt in de oorspronkelijke record of het oorspronkelijke object.

* Iedereen met toegang tot de Planning en de Mening van Workfront of hogere toestemmingen aan de werkruimte en een verslagtype kan de verbindingen zien die u tussen verslagen of tussen verslagen en andere voorwerpen van toepassingen maakt. Ze kunnen verbonden records en objecten bekijken, ongeacht hun machtigingen in de toepassingen waarmee u verbinding maakt.
* U kunt de verbindingen van iedereen anders weergeven en bewerken als u beheerdersmachtigingen hebt voor de werkruimte en het recordtype waarin de verbonden records zich bevinden.
* U kunt één record verbinden met een of meerdere objecten vanuit een andere toepassing. Dit is afhankelijk van het type verbinding dat u hebt geselecteerd bij het verbinden van de recordtypen. Voor meer informatie, zie de &quot;types van Verbindingen&quot;sectie in het artikel [ Verbonden overzicht van recordtypes ](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* Wanneer verbonden recordtypen deel uitmaken van hiërarchieën, kunt u tot om het even welk objecten type binnen de hiërarchie van de verslagpagina&#39;s toegang hebben. Voor informatie, zie [ Hiërarchie en breadcrumb overzicht ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
* Wanneer verbonden recordtypen deel uitmaken van hiërarchieën, kunt u één record van een onderliggend recordtype verbinden met maximaal 10 records van een bovenliggend recordtype. Voor informatie, zie [ Hiërarchie en breadcrumb overzicht ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Gebieden waar u records kunt verbinden

U kunt records handmatig of automatisch verbinden in Workfront.

### Records handmatig verbinden

U kunt records in de volgende gebieden handmatig verbinden met andere records of met objecten vanuit een andere toepassing:

* U kunt records van Workfront Planning verbinden met Workfront-objecten, Experience Manager Assets-objecten of GenStudio Brands in de volgende gebieden van een Planningsrecord:

   * De verbonden verslaggebieden in de lijstmening van een verslagtype in Planning.
   * De verbonden recordvelden in de voorvertoning of detailpagina van een record.
   * De voorvertoning of detailpagina van de record op de pagina Verbonden records van een record.

* U kunt Workfront-objecten verbinden met Workfront Planning-records in de volgende gebieden van Workfront:

   * Het gedeelte Planning van een Workfront-object.
   * Een veld voor een planningsverbinding in het aangepaste formulier van een Workfront-object.

  Voor informatie, zie [ recordverbindingen van de voorwerpen van Workfront beheren ](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

### Records automatisch verbinden

Nadat u recordtypen met elkaar hebt verbonden of een recordtype met een objecttype vanuit een andere toepassing, kunt u automatisch records en objecten op de volgende manieren verbinden:

* Automatisering gebruiken

  U kunt verslagen of de voorwerpen van Workfront van een verslag van de Planning tot stand brengen waar u automatiseringen vormt.

  Wanneer aan een door u gedefinieerde voorwaarde wordt voldaan, wordt een record of een object gemaakt en wordt deze automatisch verbonden met de record waaruit u de automatisering activeert.

  Voor informatie, zie [ de automatisering van de Planning van Adobe Workfront ](/help/quicksilver/planning/records/configure-automations-to-create-records.md) vormen.

* aanvraagformulieren gebruiken om records te maken

  U kunt verslagen tot stand brengen wanneer u een verzoek van de Planning indient. De aanvraag en de record worden automatisch verbonden.

  >[!NOTE]
  >
  >U kunt een record niet loskoppelen van de oorspronkelijke aanvraag.

  Voor informatie, zie [ de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.
