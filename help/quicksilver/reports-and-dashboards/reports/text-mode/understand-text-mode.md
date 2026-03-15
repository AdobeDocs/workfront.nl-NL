---
product-area: reporting
navigation-topic: text-mode-reporting
title: Overzicht van de tekstmodus
description: You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list.
author: Courtney
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Overzicht van de tekstmodus

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list.

The standard interface allows you to reference fields and their attributes that are readily available in the Workfront interface.

In de tekstmodus kunt u verwijzen naar velden en kenmerken die mogelijk niet beschikbaar zijn in de standaardmodus, maar wel in de Workfront-database.

Zie de sectie Leren op de website van de Adobe Experience League voor meer informatie over het maken van rapporten met gebruik van de tekstmodus, waaronder klassen, video&#39;s en zelfstudies.

## Overwegingen voordat de tekstmodus wordt gebruikt

>[!TIP]
>
>U kunt ook de mogelijkheden van berekende aangepaste velden uitbreiden met een versie van de tekstmodus voor aangepaste velden. De syntaxis en regels voor het maken van een berekend aangepast veld verschillen van de syntaxis en regels die u gebruikt in rapporten en lijsten. Voor informatie over het toevoegen van een berekend douanegebied, zie [&#x200B; berekende gebieden aan een vorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

* Voordat u de tekstmodus in uw rapporten gaat gebruiken, raden we u ten zeerste aan onze klassen voor geavanceerde rapportage te gebruiken om meer inzicht te krijgen in de taal van de tekstmodus.
* We recommend that you use standard mode to ensure the reports you create remain intact when the Workfront software is updated. In de tekstmodus kunt u complexere weergaven, filters en groepen maken, maar het is ook moeilijker om deze te onderhouden en het is niet gegarandeerd wanneer de Workfront-software wordt bijgewerkt.
* We recommend that you always try to build all reporting elements in the standard interface and switch to the text mode builder only for few adjustments.

  >[!TIP]
  >
  >Using the standard builder gives you important building blocks and patterns of code that you can then use when modifying the code in text mode.

* There are a set of rules and a unique syntax that you must use in order to successfully build reports and lists in text mode. Make sure you are familiar with the Workfront syntax for text mode before you begin.

  Voor informatie over de syntaxis en de regels voor het gebruiken van tekstwijze, zie [&#x200B; overzicht van de de wijzesyntaxis van de Tekst &#x200B;](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* Nadat u een rapporteringselement op tekstwijze aanpast, zou u of niet op standaardwijze (in een mening) kunnen kunnen kunnen terugschakelen of de code voor het element zou kunnen worden geschrapt u creeerde (in filters en groepen.) Niet alle velden die in de tekstmodus worden ondersteund, worden in de standaardmodus ondersteund.

## Standaardmodusinterface

De Standaardinterface van de Wijze toont gebieden om de toepassingselementen in kaart te brengen die u in een rapport of een lijst wilt tonen. De standaardmodusinterface is een set vervolgkeuzemenu&#39;s waarmee u de velden kunt selecteren die u in uw rapporten of lijsten wilt weergeven.

Voor meer informatie over de standaardwijzeinterface en leren hoe te om een rapport of een lijst tot stand te brengen, zie:

* [&#x200B; creeer een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Elementen rapporteren: filters, weergaven en groepen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Text Mode interface

Text mode enables you to create more complex views, filters, groupings, and prompts by allowing you to use fields that are not available in the standard mode interface. In Workfront text mode is a collection of coded statements that indicate what objects you want to display in a report or a list.

For a complete list of all our reportable fields, see the [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Niet alle velden die beschikbaar zijn via de API, zijn beschikbaar via de tekstmodusinterface. Als u het juiste veld in de code van de tekstmodus gebruikt en u niet de verwachte resultaten weergeeft, is het mogelijk dat het veld alleen via de API moet worden gemeld.

## Rapportelementen openen en tekstmodus bewerken {#access-reporting-elements-and-edit-text-mode}

Toegang tot de interface van de tekstmodus is vergelijkbaar voor weergaven, groepen en filters wanneer u deze benadert vanuit een rapport of lijst.

Zie voor meer informatie over het gebruik van de tekstmodus in weergaven, filters en groepen:

* [&#x200B; geef een mening uit gebruikend tekstwijze &#x200B;](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [&#x200B; geef een filter uit gebruikend tekstwijze &#x200B;](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Een groep bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Custom prompts can only be edited in text mode. You can access prompts only from a report.

For information about accessing the text mode interface for custom prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Common reasons to use Text Mode {#common-reasons-to-use-text-mode}

Buiten het creëren van douaneherinneringen die slechts gebruikend tekstwijze kunnen worden gevormd, adviseren wij dat u de rapportbouwer gebruikt om uw meningen, filters en groeperingen te bouwen. In sommige gevallen kunt u echter de tekstmodus gebruiken om uw rapporten en lijsten te verbeteren.

Voor meer informatie over gemeenschappelijk gebruik voor tekstwijze, zie [&#x200B; Overzicht van gemeenschappelijk gebruik voor de Wijze van de Tekst &#x200B;](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
