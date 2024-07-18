---
title: Overzicht van veld
description: U kunt nieuwe gebieden in de Planning van Adobe Workfront toevoegen die op de levenscyclus van uw organisatie wijzen. Velden zijn kenmerken van recordtypen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Overzicht van veld

<!--
title: Field overview
description: You can add new fields in Adobe Workfront Planning that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

U kunt nieuwe gebieden in de Planning van Adobe Workfront toevoegen die op de levenscyclus van uw organisatie wijzen. Velden zijn kenmerken van recordtypen.


## Overwegingen over de gebieden van de Planning van Adobe Workfront

* U kunt alleen velden maken vanuit de tabelweergave van een recordtypepagina. Velden worden als kolommen weergegeven in de tabelweergave. Alle velden die aan een recordtype zijn gekoppeld, worden ook op de recordpagina weergegeven.

  Voor informatie over het beheren van lijstkolommen (of verslaggebieden), zie [ de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

  Zie ook de volgende artikelen voor informatie over het beheren van velden:

   * [Veldinstellingen bewerken](/help/quicksilver/planning/fields/edit-fields.md)
   * [Velden verwijderen](/help/quicksilver/planning/fields/delete-fields.md)

* De velden die aan een recordtype zijn gekoppeld, zijn beschikbaar om te worden gekoppeld aan alle records van dat type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Aan een recordtype gekoppelde velden kunnen niet worden toegevoegd aan een ander recordtype. <!-- this will change when they open the Field library tab when creating a field-->

* U kunt velden handmatig of automatisch maken op de volgende manieren:

   * Handmatig:

      * Door kolommen toe te voegen in de tabelweergave van een pagina met recordtypen. De kolommen van de lijst zijn de gebieden verbonden aan het verslagtype. Het zijn dezelfde velden die op de pagina van een record worden weergegeven.

        U kunt geen velden maken van de recordpagina.

      * Door recordtypen aan te sluiten. U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee recordtypen of een recordtype en een objecttype vanuit andere toepassingen.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Voor meer informatie over het verbinden van verslagtypes, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Door recordtypen te importeren met een Excel- of CSV-bestand. Voor meer informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   * Automatisch:

     Hieronder vindt u standaardvelden die standaard worden gemaakt voor elk nieuw recordtype:

      * Naam
      * Beschrijving
      * Begindatum
      * Einddatum
      * Status. De standaardwaarden voor recordstatussen zijn:
         * Ontwikkeling
         * Geplant
         * Actief
         * Voltooid
         * In de wachtstand

        U kunt meer waarden toevoegen of de naam van de bestaande waarden wijzigen.

     Workfront Planning maakt velden voor recordtypen wanneer u een werkruimte maakt op basis van een sjabloon. Voor informatie, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

* De gebieden van de Planning van Workfront zijn niet toegankelijk van Workfront.

* Workfront-velden zijn alleen toegankelijk vanuit Workfront Planning wanneer u recordtypen verbindt met Workfront-objecttypen en gekoppelde of opzoekvelden toevoegt uit Workfront-objecten. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

* U kunt de instellingen weergeven en bijwerken voor de velden die u of een andere gebruiker heeft gemaakt, als u beheerdersmachtigingen hebt voor de werkruimte waartoe het veld behoort.

* U kunt maximaal 500 velden hebben voor één recordtype.

* Veldnamen kunnen maximaal 250 tekens bevatten.

* Wanneer u een recordtype of werkruimte verwijdert, worden ook alle bijbehorende velden en de waarden van de velden verwijderd en kunnen deze niet worden hersteld. <!-- this might change with a possible recycle bin solution?!-->
