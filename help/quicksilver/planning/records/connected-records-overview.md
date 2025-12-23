---
title: Overzicht van verbonden records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden. In dit artikel worden overwegingen beschreven waarmee u rekening moet houden wanneer u records verbindt in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Overzicht van verbonden records

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken.</span>

{{planning-important-intro}}

U kunt Adobe Workfront-planningsrecords met elkaar of met objecten van andere toepassingen verbinden.

In dit artikel worden overwegingen beschreven waarmee u rekening moet houden wanneer u records verbindt in Adobe Workfront Planning.

Voor informatie over hoe u verslagen met elkaar of met een ander voorwerp kunt verbinden, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).


## Overwegingen bij het verbinden van records

* Nadat u recordtypen hebt verbonden, worden de verbonden recordtypen weergegeven als gekoppelde recordvelden in de tabel met de recordtypen waarvan ze zijn gekoppeld en op de recordpagina&#39;s.
* U kunt records en objecten van de gekoppelde record- en objecttypen bladeren en deze toevoegen vanuit de gekoppelde recordvelden.
* U kunt velden (opzoekvelden) van de gekoppelde recordtypen toevoegen aan de tabel van het recordtype waarvan u een koppeling maakt.

  U kunt ook velden (opzoekvelden) toevoegen van de recordtypen die u koppelt in de tabel van het recordtype waarnaar u een koppeling maakt.

  Als u bijvoorbeeld het recordtype product van het recordtype Campagne koppelt, kunt u zowel productvelden voor campagnes als campagnevelden voor producten weergeven.
* U kunt de waarden van opzoekvelden in de records waarvan u een koppeling maakt, niet handmatig bijwerken.

  De waarden van de opzoekvelden vullen de Workfront-planningsrecord die u koppelt automatisch nadat deze zijn bijgewerkt in de oorspronkelijke record of het oorspronkelijke object.

* Iedereen met toegang tot de Planning en de Mening van Workfront of hogere toestemmingen aan de werkruimte en een verslagtype kan de verbindingen zien die u tussen verslagen of tussen verslagen en andere voorwerpen van toepassingen maakt. Ze kunnen verbonden records en objecten bekijken, ongeacht hun machtigingen in de toepassingen waarmee u verbinding maakt.
* U kunt de verbindingen van iedereen anders weergeven en bewerken als u beheerdersmachtigingen hebt voor de werkruimte en het recordtype waarin de verbonden records zich bevinden.
* U kunt één record verbinden met een of meerdere objecten vanuit een andere toepassing. Dit is afhankelijk van het type verbinding dat u hebt geselecteerd bij het verbinden van de recordtypen. Voor meer informatie, zie de &quot;types van Verbindingen&quot;sectie in het artikel [&#x200B; Verbonden overzicht van recordtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* <span class="preview"> als de verbonden recordtypes deel van hiërarchieën uitmaken, kunt u tot om het even welk objecten type binnen de hiërarchie van de verslagen&#39; pagina&#39;s toegang hebben. Voor informatie, zie [&#x200B; Hiërarchie en breadcrumb overzicht &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). </span>
* <span class="preview">* Wanneer verbonden recordtypen deel uitmaken van hiërarchieën, kunt u één record van een onderliggend recordtype verbinden met maximaal 10 records van een bovenliggend recordtype. Voor informatie, zie [&#x200B; Hiërarchie en breadcrumb overzicht &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). </span>

## Gebieden waar u records kunt verbinden

U kunt records in de volgende gebieden verbinden met andere records of met objecten vanuit een andere toepassing:

* U kunt records van Workfront Planning verbinden met Workfront-objecten, Experience Manager Assets-objecten of GenStudio Brands in de volgende gebieden van een Planningsrecord:

   * De verbonden verslaggebieden in de lijstmening van een verslagtype in Planning.
   * De voorvertoning of detailpagina van de record in de verbonden recordvelden op het tabblad Details.
   * De voorvertoning of detailpagina van de record op het tabblad Verbindingen.
   * De pagina van het verslag in een Verbonden verslagenpagina tabel van een verbonden verslag.

* U kunt Workfront-objecten verbinden met Workfront Planning-records in de volgende gebieden van Workfront:

   * Het gedeelte Planning van een Workfront-object.
   * Een veld voor een planningsverbinding in het aangepaste formulier van een Workfront-object.

  Voor informatie, zie [&#x200B; recordverbindingen van de voorwerpen van Workfront beheren &#x200B;](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
