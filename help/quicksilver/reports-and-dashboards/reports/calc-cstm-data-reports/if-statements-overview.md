---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Overzicht van IF-instructies
description: U kunt "IF"verklaringen in algemene programmeertalen gebruiken. In Adobe Workfront kunt u met 'IF'-instructies gegevensvelden vergelijken, opmaken en ordenen voor zowel rapportage- als aangepaste gegevensdoeleinden. Bovendien leidt het wiskundig denken over 'IF'-instructies tot een beter conceptueel begrip, aangezien variabelen voor expressies veel worden gebruikt.
author: Courtney
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Overzicht van &quot;IF&quot;-instructies

<!-- Audited: 1/2024 -->

U kunt &quot;IF&quot;verklaringen in algemene programmeertalen gebruiken. In Adobe Workfront kunt u met &#39;IF&#39;-instructies gegevensvelden vergelijken, opmaken en ordenen voor zowel rapportage- als aangepaste gegevensdoeleinden. Bovendien leidt het wiskundig denken over &#39;IF&#39;-instructies tot een beter conceptueel begrip, aangezien variabelen voor expressies veel worden gebruikt.

## Aanbevelingen voor &quot;IF&quot;-instructies

Overweeg het volgende voordat u een &quot;IF&quot;-instructie maakt:

* Wij bevelen een basisbegrip van om het even welke algemene programmeertaal aan, maar wij vereisen het niet, voor deze gids.
* We hebben een geavanceerd inzicht nodig in de syntaxis van de Workfront-tekstmodus. Dit helpt u bij het begrijpen van de terminologie van de Workfront API en bij het begrijpen van de syntaxis van aangepaste gegevens in deze specifieke indelingen.

  Voor informatie over Workfront API, zie [ API basiscs ](../../../wf-api/general/api-basics.md).

  Voor informatie over het gebruiken van tekstwijze, zie [ Overzicht van de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* U kunt &quot;IF&quot;-instructies maken voor de volgende Workfront-elementen:

   * Weergaven
   * Groepen
   * Calculated custom fields

* You cannot build &quot;IF&quot; statements for filters. This results in a &quot;Whoops&quot; error in Workfront.
* The Support Team does not help with building custom data. U kunt het Team van de Steun contacteren nadat u de douanegebieden of de kolommen bouwt en u ziet niet de gewenste resultaten. Neem voor hulp bij het samenstellen van een expressie contact op met uw accountmanager voor informatie over onze adviesopties.
* Wij adviseren het schrijven van deze uitdrukkingen in een tekstredacteur eerst, zoals Sublime of de Code van Visual Studio, omdat dit u helpt gegevens duidelijker zien dan in Workfront zou verschijnen.

## Componenten van een &quot;IF&quot;-instructie

U kunt &#39;IF&#39;-instructies in Workfront maken met de volgende indeling:
<pre>IF (Voorwaarde,Ware uitdrukking,Onjuiste uitdrukking)</pre>The components of an "IF" statement are:

* **IF** = This is the Workfront calculated data expression for &quot;function.&quot; Similar to the SUM and PROD expressions, this first tells the system to understand the function as an &quot;IF&quot; statement. Always use capital letters for &quot;IF&quot; in this statement.\
  Voor een lijst van alle berekende gegevensuitdrukkingen, zie [ Overzicht van berekende gegevensuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Voorwaarde** = dit is de voorwaarde dat de variabele van Workfront moet ontmoeten en het is de stichting voor deze vergelijking. Alles wat later in de vergelijking kan worden gespecificeerd hangt van de voorwaarde af. U kunt een aantal verwijzingen, vergelijkingen of wiskundige expressies gebruiken om een vergelijking te starten. Voorbeelden van voorwaarden zijn:

   * Een datum is groter dan een andere datum op een opgegeven object.
   * Een status is gelijk aan een van de beschikbare statussen voor een opgegeven object.
   * Percentage voltooide taken is kleiner dan of groter dan een bepaald percentage.

* **de Exploitant van de Voorwaarde** = dit is de exploitant die u helpt de voorwaarde van uw &quot;IF&quot;verklaring bouwen. &#39;is gelijk aan&#39; of &#39;is groter dan&#39; zijn bijvoorbeeld voorwaarde-operatoren. Voor een lijst van voorwaardenexploitanten die u in verklaringen kunt gebruiken, zie [ de exploitanten van de Voorwaarde in berekende douaneuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **Waar***Uitdrukking** = dit is de &quot;Waar&quot;variabele, die de vergelijking vertelt die indicator om te tonen zodra de criteria van de voorwaarde worden voldaan aan (ware indicatoren).

* **Vals Uitdrukking** = dit is de &quot;Vals&quot;variabele, die de vergelijking vertelt welke indicator om te tonen wanneer de criteria van de voorwaarde niet worden voldaan aan (valse indicatoren).

In the following example, the original statement format is used to write a simple data expression for an &quot;IF&quot; statement. The expression compares two different date fields in Workfront followed by a True/False result as a data string:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

In alledaagse toespraken zou deze verklaring betekenen: Als de Geprojecteerde VoltooiingsDatum van mijn voorwerp &quot;Groter dan&quot;de Geplande VoltooiingsDatum van mijn zelfde voorwerp is, dan toon de woorden &quot;van Spoor&quot;op dit gebied. Als dat niet het geval is, geeft u de woorden &quot;Op track&quot; weer.

## Berekende velden samenstellen in aangepaste formulieren of aangepaste kolommen met de instructies &#39;IF&#39;

U kunt &#39;IF&#39;-instructies in een berekend veld opbouwen in een aangepast formulier of in een aangepaste kolom.

Er is een verschil in de syntaxis u in een berekend douaneformulier tegenover een berekende douanekolom gebruikt. Raadpleeg de volgende voorbeelden:

* [Single &quot;IF&quot; statements](#single-if-statements)
* [Multiple &quot;IF&quot; statements](#multiple-if-statements)

### Single &quot;IF&quot; statements {#single-if-statements}

The following are examples of a calculated custom field and its corresponding column using an &quot;IF&quot; statement:

* Calculated custom field:

Wanneer u een aangepast veld maakt, gebruikt u de volgende syntaxis voor de instructie &quot;IF&quot;:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Berekende aangepaste kolom:

Wanneer u een aangepaste kolom maakt, moet u de volgende syntaxis gebruiken voor de instructie &quot;IF&quot; in de regel met de expressie value:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Meerdere &quot;IF&quot;-instructies {#multiple-if-statements}

U kunt meerdere &quot;IF&quot;-instructies samenvoegen met de volgende instructie om een complexere en dynamische expressie te maken:

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>Notice, there is now no false statement for the first "IF". Instead, we replaced it with the start of a second "IF".

The following are examples of a calculated custom field and its corresponding custom column using multiple &quot;IF&quot; statements:

* Calculated custom field:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Berekende aangepaste kolom:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

In dit voorbeeld is hetzelfde bereikt door twee verschillende criteria te combineren.\
U kunt deze opties verder verkennen door deze voorbeelden opnieuw samen te stellen in uw eigen omgeving.

De beste manier om dit te leren is door met diverse gebieden en scenario&#39;s te experimenteren. U moet ook vertrouwd raken met de API Explorer, die de veldnamen onthult die kunnen worden gebruikt. For information on the API Explorer, see [API Explorer](../../../wf-api/general/api-explorer.md).

For more information about Workfront syntax of calculated data expressions, see [Overview of calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
