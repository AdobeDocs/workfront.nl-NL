---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Overzicht van groepen in Adobe Workfront
description: U kunt groepen toevoegen om de indeling van de gegevens in uw rapporten en lijsten te beheren.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Overzicht van groepen in Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

U kunt groepen toevoegen om de indeling van de gegevens in uw rapporten en lijsten te beheren.

U kunt op de volgende manieren groepen aan rapporten toevoegen:

* U kunt groepen maken door bestaande groepen te bewerken.

  Voor informatie over het aanpassen van een bestaande Groepering, zie [ bestaande groeperingen ](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md) uitgeven.

* U kunt geheel nieuwe groepen maken.

  Voor informatie over het creëren van een groepering van kras, zie [ groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md) creëren.

Standaard worden groepen weergegeven in een grijze markering in uw rapport of lijst. De resultaten van het rapport of de lijst worden vermeld onder hun individuele groepering, zonder nadruk.

![ het voorbeeld van Groepen ](assets/grouping-example-blue.png)

U kunt maximaal drie groepen aan een rapport toevoegen. U kunt uw informatie met maximaal vier groepen organiseren door een matrixrapport te maken. Voor meer informatie over matrixrapporten, zie [ een matrixrapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md) creëren.

Het getal tussen haakjes achter de naam van de groep geeft het aantal resultaten onder die groep aan. Als uw rapport veelvoudige pagina&#39;s overspant, zorg ervoor dat u *allen* de resultaten in het rapport of de lijst toont om een nauwkeurige telling voor uw resultaten onder elke groepering te krijgen.

Houd rekening met het volgende wanneer u werkt met groepen:

* U kunt de gegevens in bestaande groepen aanpassen. Alle gebruikers die de groepen kunnen bekijken, kunnen uw veranderingen ook zien.
* Uw Workfront-beheerder moet u toegang geven tot Filters, Weergaven en Groepen bewerken om groepen te maken.

  Voor informatie over het verlenen van toegang tot Filters, Meningen, en Groepen, zie [ toegang van de Verlening tot filters, meningen, en groeperingen ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Uw niveau van toestemmingen aan een groepering dicteert hoe een groepering wordt bewaard. Als u de groep oorspronkelijk hebt gemaakt, kunt u de wijzigingen opslaan. Als u dit niet doet, wordt u gevraagd een versie van de groep op te slaan. Als u wijzigingen aanbrengt in een groep die u met anderen hebt gedeeld, heeft dit ook invloed op deze groepen.
* U kunt een groepering aanpassen die met u werd gedeeld slechts als de gebruiker die het deelde u toegang leidde verleende. Voor informatie over het delen van een groepering, zie [ een filter, mening, of groepering ](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md) delen.
* U kunt een groepering niet inline bewerken.
* U kunt niet groeperen op meerdere geselecteerde aangepaste velden (bijvoorbeeld selectievakjes) of op velden die meerdere waarden kunnen hebben (bijvoorbeeld Resource Manager).

## Aanvullende informatie over groepen

U kunt rapportinformatie verder beheren wanneer het gebruiken van Groepen door de waarden in elke kolom op de rij van de Groepering samen te voegen, evenals uw informatie te sorteren door het gebied van uw Groepering. U kunt een groepering ook verwijderen wanneer deze niet meer nodig is.

* [ samengevoegde waarden in groeperingen ](#aggregate-values-in-groupings)
* [ Soort door een groepering ](#sort-by-a-grouping)
* [Een groep verwijderen](#remove-a-grouping)

### Samengevoegde waarden in groepen {#aggregate-values-in-groupings}

U kunt de gegevens samenvoegen die in uw rapport in uw groeperingslijn worden getoond door de waarden in elke kolom van het rapport samen te vatten. Voor meer informatie over het samenvatten van kolomgegevens in een groepering, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>De volgende uitzonderingen zijn van toepassing op bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvoegt voor de volgende velden in groepen:
>
>* Alle getallen en valutavelden behalve Werkelijke uren (bijvoorbeeld Geplande/Werkelijke loonkosten, Geplande/Werkelijke kosten, Geplande/Werkelijke kosten, Geplande/Geplande uren) tellen alleen de waarden voor de kindertaken en standalone taken samen. De waarden voor de bovenliggende taken of ouders van ouders worden niet samengevoegd.
>* Werkelijke uren tellen de waarden voor de hoofdbovenliggende en zelfstandige taken samen; ze tellen de getallen voor de bovenliggende taken of de onderliggende taken niet samen.
>* Aangepaste gegevensvelden voor getal- en valutawaarden bevatten alle taken: ouders, kinderen, ouders van ouders en zelfstandige taken.

### Sorteren op een groep {#sort-by-a-grouping}

Groepen kunnen niet worden gesorteerd. U kunt weergaven sorteren. Als u een lijst wilt sorteren op de waarde die in de groep is vastgelegd, moet u dezelfde waarde in een van de kolommen van de weergave opnemen en de sortering in de weergave toepassen. Op deze manier wordt in de lijst gesorteerd op de waarde in de groep (er wordt gesorteerd op de waarde in de weergave die ook in de groep wordt vastgelegd). Voor meer informatie over het creëren van meningen en het sorteren door waarden binnen de meningen, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Een groep verwijderen {#remove-a-grouping}

Hoe u een groep verwijdert, hangt af van het feit of u de groepering hebt gemaakt of dat de groepering met u is gedeeld. U kunt een standaardgroep niet verwijderen.

* **als u het groeperen creeerde en u het** verwijdert, wordt het groeperen verwijderd uit het systeem van Workfront. De groepering is niet meer beschikbaar voor gebruikers met wie u deze eerder hebt gedeeld.
* **als het groeperen met u werd gedeeld en u het** verwijdert, wordt het groeperen verwijderd slechts voor u. De gebruiker die het oorspronkelijk creeerde en om het even welke andere gebruikers het met is gedeeld hebben nog toegang tot de groepering.

Voor informatie over het verwijderen van een groepering, zie het artikel [ filters, meningen, en groeperingen ](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md) verwijderen.
