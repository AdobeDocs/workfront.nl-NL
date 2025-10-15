---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operatoren voor voorwaarde in berekende aangepaste expressies
description: U kunt voorwaarde-operatoren of wijzigingstoetsen gebruiken bij het samenstellen van berekende aangepaste gegevens in Adobe Workfront wanneer u de tekstmodus gebruikt.
author: Jenny
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# Operatoren voor voorwaarde in berekende aangepaste velden

<!-- Audited: 2/2024 -->

U kunt voorwaarde-operatoren of wijzigingstoetsen gebruiken bij het samenstellen van berekende aangepaste gegevens in Adobe Workfront wanneer u de tekstmodus gebruikt. Voor informatie over het gebruiken van tekstwijze in Workfront, zie [&#x200B; Overzicht van de Wijze van de Tekst &#x200B;](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Met Condition-operatoren of modifiers kunt u een voorwaardeninstructie maken door bestaande Workfront-velden in instructies te verbinden en een nieuw veld te genereren. Voorwaarde-operatoren worden vooral gebruikt om de voorwaarde van een &quot;IF&quot;-instructie op te bouwen.

U kunt &quot;IF&quot;verklaringen in Workfront gebruiken om, gebieden van gegevens voor zowel het melden als douanegegevensdoeleinden te vergelijken, te formatteren en te koord samen te brengen.

U kunt &quot;IF&quot;-instructies maken voor de volgende Workfront-elementen:

* Weergaven
* Groepen
* Berekende aangepaste velden
* Bedrijfsvoorschriften

Voor meer informatie over de bouw van &quot;IF&quot;verklaringen, zie [&#x200B; &quot;IF&quot;verklaringen overzicht &#x200B;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

De voorbeelden in deze handleiding illustreren het gebruik van voorwaardelijke operatoren in berekende aangepaste velden. U kunt ze ook gebruiken in berekende aangepaste kolommen of groepen wanneer u de juiste syntaxis volgt voor berekende aangepaste velden in rapporten.

Voor informatie over het verschil in syntaxis tussen de berekende douanegebieden en berekende douanegegevens in rapporten, zie [&#x200B; Berekende douanegebieden vs. berekende kolommen &#x200B;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Voor informatie over bedrijfsregels, zie [&#x200B; bedrijfsregels &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md) creëren en uitgeven.

Raadpleeg de API Explorer om de velden te zoeken waarnaar u wilt verwijzen in de berekende aangepaste expressies. Voor informatie over de API Ontdekkingsreiziger, zie [&#x200B; API Ontdekkingsreiziger &#x200B;](../../../wf-api/general/api-explorer.md).

In Workfront kunt u de volgende voorwaardelijke modifiers gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Condition, operator</th> 
   <th>Syntaxis van Condition-operator</th> 
   <th>Definitie van Condition-operator</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Gelijk</td> 
   <td>= </td> 
   <td> <p>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer het eerste veld van uw instructie gelijk is aan het tweede veld.</p> <p>Gebruik bijvoorbeeld de volgende instructie in een berekend aangepast veld om een instructie "IF" te maken die de geplande Voltooiingsdatum vergelijkt met de geplande Voltooiingsdatum van een taak: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Groter dan </td> 
   <td>&gt; </td> 
   <td>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer het eerste veld van uw instructie groter is dan het tweede veld. <p>Gebruik bijvoorbeeld de volgende instructie in een berekend aangepast veld om een instructie "IF" te maken die de geplande Voltooiingsdatum vergelijkt met de geplande Voltooiingsdatum van een taak: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Groter dan of gelijk aan </td> 
   <td>&gt;= </td> 
   <td>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer het eerste veld van uw instructie groter dan of gelijk is aan het tweede veld. <p>Gebruik bijvoorbeeld de volgende instructie in een berekend aangepast veld om een instructie "IF" te maken die de geplande Voltooiingsdatum vergelijkt met de geplande Voltooiingsdatum van een taak: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner dan </td> 
   <td>&lt; </td> 
   <td>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer  het eerste veld van de instructie is kleiner dan het tweede veld. <p>Gebruik bijvoorbeeld de volgende instructie in een berekend aangepast veld om een instructie "IF" te maken die de geplande Voltooiingsdatum vergelijkt met de geplande Voltooiingsdatum van een taak: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner dan of gelijk aan </td> 
   <td>&lt;= </td> 
   <td>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer  het eerste veld van de instructie is kleiner dan of gelijk aan het tweede veld. <p>Gebruik bijvoorbeeld de volgende instructie in een berekend aangepast veld om een instructie "IF" te maken die de geplande Voltooiingsdatum vergelijkt met de geplande Voltooiingsdatum van een taak: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Is niet </td> 
   <td>! </td> 
   <td> <p>Voeg deze operator toe vóór een van de bovenstaande operatoren om de operator te negeren. </p> <p>Bijvoorbeeld: </p> 
    <ul> 
     <li>Gelijk aan: = </li> 
     <li>Is niet gelijk aan: != </li> 
    </ul> <p>Wanneer u deze operator toevoegt vóór de volgende gegevensexpressies, wordt een negatieve instructie toegevoegd aan expressies: </p> 
    <ul> 
     <li>BEVATTEN </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Voor informatie over deze gegevensuitdrukkingen en voor een volledige lijst, zie <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref"> Overzicht van berekende gegevensuitdrukkingen </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>of </td> 
   <td>|| </td> 
   <td> <p>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer de expressie  vindt of de eerste of tweede waarde van uw verklaring. </p> <p>Bijvoorbeeld, gebruik de volgende verklaring op een berekend douanegebied om een "IF"verklaring te bouwen die projecten in of de Huidige of Planning status als "Actief"merkt: </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> en </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Gebruik deze operator om aan te geven dat aan de voorwaarde is voldaan wanneer de expressie  zoekt een item dat tegelijkertijd aan twee voorwaarden voldoet. </p> <p>Bijvoorbeeld, gebruik de volgende verklaring op een berekend douanegebied om een "IF"verklaring te bouwen die projecten vindt die in Huidige status zijn en een Voorwaarde van bij Risico hebben en hen als "Bemiddeling nodig"merken. </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
