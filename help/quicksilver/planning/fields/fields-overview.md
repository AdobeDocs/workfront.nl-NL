---
title: Overzicht van velden
description: U kunt nieuwe gebieden in de Planning van Adobe Workfront toevoegen die op de levenscyclus van uw organisatie wijzen. Velden zijn kenmerken van recordtypen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 3667359ba2c6ea0aab3ce6845f1a537183f304ec
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---


# Overzicht van veld

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

U kunt nieuwe gebieden in de Planning van Adobe Workfront toevoegen die op de levenscyclus van uw organisatie wijzen. Velden zijn kenmerken van recordtypen.


## Overwegingen over de gebieden van de Planning van Adobe Workfront

* U kunt alleen velden maken vanuit de tabelweergave van een recordtypepagina. Velden worden als kolommen weergegeven in de tabelweergave. Alle velden die aan een recordtype zijn gekoppeld, worden ook op de recordpagina weergegeven.

  Voor informatie over het beheren van lijstkolommen (of verslaggebieden), zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

  Zie ook de volgende artikelen voor informatie over het beheren van velden:

   * [Veldinstellingen bewerken](/help/quicksilver/planning/fields/edit-fields.md)
   * [Velden verwijderen](/help/quicksilver/planning/fields/delete-fields.md)

* De velden die aan een recordtype zijn gekoppeld, zijn beschikbaar om te worden gekoppeld aan alle records van dat type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Aan een recordtype gekoppelde velden kunnen niet worden toegevoegd aan een ander recordtype. <!-- this will change when they open the Field library tab when creating a field-->

* U kunt velden handmatig of automatisch maken op de volgende manieren:

   * Handmatig:

      * Wanneer u kolommen toevoegt in de tabelweergave van een recordtypepagina. De kolommen van de lijst zijn de gebieden verbonden aan het verslagtype. Het zijn dezelfde velden die op de pagina van een record worden weergegeven.

        U kunt geen velden maken van de recordpagina.

      * Wanneer u recordtypen verbindt. U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee recordtypen of een recordtype en een objecttype vanuit andere toepassingen.

        Voor meer informatie over het verbinden van verslagtypes, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Wanneer u bestaande velden uit Workfront importeert.

        Voor informatie, zie [&#x200B; de gebieden van de Invoer van Adobe Workfront &#x200B;](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automatisch:

      * Wanneer u een recordtype maakt:

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

      * Wanneer u een werkruimte maakt op basis van een sjabloon.

        Voor informatie, zie [&#x200B; werkruimten &#x200B;](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

      * Wanneer u recordtypen importeert met een Excel- of CSV-bestand.

        Voor meer informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

* De gebieden van de Planning van Workfront zijn niet toegankelijk van Workfront.

* Workfront-velden zijn alleen toegankelijk vanuit Workfront Planning wanneer u recordtypen verbindt met Workfront-objecttypen en gekoppelde of opzoekvelden toevoegt uit Workfront-objecten. Voor informatie, zie [&#x200B; verbind verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).

* U kunt de instellingen weergeven en bijwerken voor de velden die u of een andere gebruiker heeft gemaakt, als u beheermachtigingen hebt voor de werkruimte en het recordtype waartoe het veld behoort.

* U kunt maximaal 500 velden hebben voor één recordtype.

* Veldnamen kunnen maximaal 250 tekens bevatten.

* Wanneer u een recordtype of werkruimte verwijdert, worden ook alle bijbehorende velden en de waarden van de velden verwijderd en kunnen deze niet worden hersteld. <!-- this might change with a possible recycle bin solution?!-->
* Wanneer u velden verwijdert die deel uitmaken van een formule-expressie, verandert het veld van de formule.
* Wanneer u een formule-expressie wijzigt en er in andere formulevelden naar wordt verwezen, heeft dit ook invloed op de aanvullende formules.
