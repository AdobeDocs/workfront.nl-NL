---
title: Overzicht van veld
description: U kunt nieuwe velden in Adobe Maestro toevoegen die de levenscyclus van uw organisatie weerspiegelen. Velden zijn kenmerken van recordtypen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Overzicht van veld

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

U kunt nieuwe velden in Adobe Maestro toevoegen die de levenscyclus van uw organisatie weerspiegelen. Velden zijn kenmerken van recordtypen.


## Overwegingen over Maestro-velden

* U kunt alleen velden maken vanuit de tabelweergave van een recordtypepagina. Velden worden als kolommen weergegeven in de tabelweergave. Alle velden die aan een recordtype zijn gekoppeld, worden ook weergegeven op de pagina Details van elke record van dat type.

  Voor informatie over het beheren van lijstkolommen (of verslaggebieden), zie [De tabelweergave beheren](../views/manage-the-table-view.md).

  Zie ook de volgende artikelen voor informatie over het beheren van velden:

   * [Velden bewerken](../fields/edit-fields.md)
   * [Velden verwijderen](../fields/delete-fields.md)

* De velden die aan een recordtype zijn gekoppeld, zijn beschikbaar om te worden gekoppeld aan alle records van dat type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Aan een recordtype gekoppelde velden kunnen niet worden toegevoegd aan een ander recordtype. <!-- this will change when they open the Field library tab when creating a field-->

* U kunt velden handmatig of automatisch maken op de volgende manieren:

   * Handmatig:

      * Door kolommen toe te voegen in de tabelweergave van een pagina met recordtypen. De kolommen van de lijst zijn de gebieden verbonden aan het verslagtype. Dit zijn dezelfde velden die worden weergegeven op de pagina Details van een record.

        U kunt geen velden maken op de pagina Details van een record.

        In dit artikel wordt beschreven hoe u handmatig velden kunt maken.

      * Door recordtypen aan te sluiten. U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee recordtypen van Maestro, of een recordtype en een objecttype vanuit andere toepassingen.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Zie voor meer informatie over het verbinden van Maestro-recordtypen [Verbind recordtypen](../architecture/connect-record-types.md).

      * Door recordtypen te importeren met een Excel- of CSV-bestand. Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

   * Automatisch:

      * Standaard elke keer dat u een recordtype maakt.

        Hieronder vindt u standaardvelden die standaard worden gemaakt voor elk nieuw type operationeel record:

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

        Hier volgen de standaardvelden die standaard worden gemaakt voor elk nieuw type taxonomy-record:

         * Naam <!--will more be added? If not, consider rephrasing this bullet-->

      * Wanneer u een werkruimte maakt op basis van een sjabloon. Maestro creeert gebieden voor operationele verslagtypes en taxonomieën wanneer u een werkruimte van een malplaatje creeert. Zie voor meer informatie [Werkruimten maken](../architecture/create-workspaces.md).

* Maestro-velden zijn niet toegankelijk vanuit Workfront.

* Workfront-velden zijn alleen toegankelijk vanuit Maestro wanneer u Maestro-recordtypen verbindt met Workfront-objecttypen en gekoppelde of opzoekvelden toevoegt vanuit Workfront-objecten. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).

* U kunt de instellingen weergeven en bijwerken voor de velden die u of een andere gebruiker heeft gemaakt, als u beheerdersmachtigingen hebt voor de werkruimte waartoe het veld behoort.

* U kunt maximaal 500 velden hebben voor één recordtype.

* Veldnamen kunnen maximaal 250 tekens bevatten.

* Wanneer u een operationeel recordtype, taxonomie of werkruimte verwijdert, worden alle bijbehorende velden en de waarden van de velden ook verwijderd en kunnen deze niet worden hersteld. <!-- this might change with a possible recycle bin solution?!-->
