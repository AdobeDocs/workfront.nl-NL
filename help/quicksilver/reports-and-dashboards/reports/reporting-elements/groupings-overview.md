---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Overzicht van groepen in Adobe Workfront
description: U kunt groepen toevoegen om de indeling van de gegevens in uw rapporten en lijsten te beheren.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Overzicht van groepen in Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

U kunt groepen toevoegen om de indeling van de gegevens in uw rapporten en lijsten te beheren.

U kunt op de volgende manieren groepen aan rapporten toevoegen:

* U kunt groepen maken door bestaande groepen te bewerken.

   Voor informatie over het aanpassen van een bestaande Groepering, zie [Bestaande groepen bewerken](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* U kunt geheel nieuwe groepen maken.

   Voor informatie over het maken van een geheel nieuwe groep raadpleegt u [Groepen maken in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Standaard worden groepen in een grijze of blauwe markering in uw rapport of lijst weergegeven. De resultaten van het rapport of de lijst worden vermeld onder hun individuele groepering, zonder nadruk.

U kunt maximaal drie groepen aan een rapport toevoegen. U kunt uw informatie met maximaal vier groepen organiseren door een matrixrapport te maken. Voor meer informatie over matrixrapporten raadpleegt u [Een matrixrapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

In een standaardgroeperingsrapport is de eerste groepering een donkerdere kleur, de tweede en derde groep zijn lichter. U kunt de kleur van de markering voor de groepering of het lettertype van de groepsnaam niet aanpassen. Het getal tussen haakjes achter de naam van de groep geeft het aantal resultaten onder die groep aan. Als uw rapport meerdere pagina&#39;s beslaat, controleert u of u de pagina weergeeft *Alles* de resultaten in het rapport of de lijst om een nauwkeurige telling voor uw resultaten onder elke groepering te krijgen.

![Monstergroepering](assets/grouping-example-blue.png)

Houd rekening met het volgende wanneer u werkt met groepen:

* U kunt de gegevens in bestaande groepen aanpassen. Alle gebruikers die de groepen kunnen bekijken, kunnen uw veranderingen ook zien.
* Uw Workfront-beheerder moet u toegang geven tot Filters, Weergaven en Groepen bewerken om groepen te maken.

   Voor informatie over het verlenen van toegang tot Filters, Mening, en Groepen, zie [Toegang verlenen tot filters, weergaven en groepen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Uw niveau van toestemmingen aan een groepering dicteert hoe een groepering wordt bewaard. Als u de groep oorspronkelijk hebt gemaakt, kunt u de wijzigingen opslaan. Als u dit niet doet, wordt u gevraagd een versie van de groep op te slaan. Als u wijzigingen aanbrengt in een groep die u met anderen hebt gedeeld, heeft dit ook invloed op deze groepen.
* U kunt een groepering aanpassen die met u werd gedeeld slechts als de gebruiker die het deelde u toegang leidde verleende. Voor informatie over het delen van een groep raadpleegt u [Een filter, weergave of groep delen](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* U kunt een groepering niet inline bewerken.
* U kunt niet groeperen op meerdere geselecteerde aangepaste velden (bijvoorbeeld selectievakjes) of op velden die meerdere waarden kunnen hebben (bijvoorbeeld Resource Manager).

## Aanvullende informatie over groepen

U kunt rapportinformatie verder beheren wanneer het gebruiken van Groepen door de waarden in elke kolom op de rij van de Groepering samen te voegen, evenals uw informatie te sorteren door het gebied van uw Groepering. U kunt een groepering ook verwijderen wanneer deze niet meer nodig is.

* [Samengevoegde waarden in groepen](#aggregate-values-in-groupings)
* [Sorteren op een groep](#sort-by-a-grouping)
* [Een groep verwijderen](#remove-a-grouping)

### Samengevoegde waarden in groepen {#aggregate-values-in-groupings}

U kunt de gegevens samenvoegen die in uw rapport in uw groeperingslijn worden getoond door de waarden in elke kolom van het rapport samen te vatten. Voor meer informatie over het samenvatten van kolomgegevens in een groepering, zie [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>De volgende uitzonderingen gelden voor bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvoegt voor de volgende velden in groepen:
>
>* Alle getallen en valutavelden behalve Werkelijke uren (bijvoorbeeld Geplande/Werkelijke loonkosten, Geplande/Werkelijke kosten, Geplande/Werkelijke kosten, Geplande/Geplande uren) tellen alleen de waarden voor de kindertaken en standalone taken samen. De waarden voor de bovenliggende taken of ouders van ouders worden niet samengevoegd.
>* Werkelijke uren tellen de waarden voor de hoofdouder en de standalone taken samen; zij tellen niet de aantallen voor de ouders van oudertaken of de kindtaken samen.
>* Aangepaste gegevensvelden voor getal- en valutawaarden voegen alle taken samen: ouders, kinderen, ouders van ouders en zelfstandige taken.


### Sorteren op een groep {#sort-by-a-grouping}

Groepen kunnen niet worden gesorteerd. Weergaven kunnen worden gesorteerd. Als u een lijst wilt sorteren op de waarde die in de groep is vastgelegd, moet u dezelfde waarde in een van de kolommen van de weergave opnemen en de sortering in de weergave toepassen. Op deze manier wordt in de lijst gesorteerd op de waarde in de groep (er wordt gesorteerd op de waarde in de weergave die ook in de groep wordt vastgelegd). Ga voor meer informatie over het maken van weergaven en het sorteren op waarden in de weergaven naar [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Een groep verwijderen {#remove-a-grouping}

Hoe u een groep verwijdert, hangt af van het feit of u de groepering hebt gemaakt of dat de groepering met u is gedeeld. U kunt een standaardgroep niet verwijderen.

* **Als u de groep hebt gemaakt en u deze verwijdert**, wordt de groepering verwijderd uit het Workfront-systeem. De groepering is niet meer beschikbaar voor gebruikers met wie u deze eerder hebt gedeeld.
* **Als de groep met u is gedeeld en u deze verwijdert**, wordt de groepering alleen voor u verwijderd. De gebruiker die het oorspronkelijk creeerde en om het even welke andere gebruikers het met is gedeeld hebben nog toegang tot de groepering.

Zie het artikel voor informatie over het verwijderen van een groep [Filters, weergaven en groepen verwijderen](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
