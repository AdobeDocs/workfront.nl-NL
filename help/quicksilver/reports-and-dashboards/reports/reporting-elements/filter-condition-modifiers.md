---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- en voorwaardenmodificatoren
description: Met de filter- en voorwaardemodities kunt u filters maken en voorwaarden instellen voor het opmaken van de rapportresultaten.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 0%

---

# Filter- en voorwaardenmodificatoren

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Met de filter- en voorwaardemodities kunt u filters maken en voorwaarden instellen voor het opmaken van de rapportresultaten.

Voor meer informatie over de bouw van filters, zie het overzicht van artikel [ Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Voor meer informatie over het gebruiken van voorwaardelijke het formatteren in Meningen, zie het artikel [ Voorwaardelijke het formatteren van het Gebruik in meningen ](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- en voorwaardenmodificatoren

Sommige bepalingen zijn ingebouwd en u kunt hen van een drop-down menu binnen uw filter of voorwaardelijke het formatteren verklaring kiezen. Andere wijzigingstoetsen kunnen alleen worden gebruikt in tekstmodusfilters.

Voor meer informatie over het begrip van tekstwijze, zie [ Overzicht van de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Voor een lijst van ingebouwde tijdkaderbepalingen, zie de artikel [ rapporten van de Filter door tijdkaders ](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

U kunt de volgende voorwaardelijke wijzigingstoetsen in filters en voorwaardelijke het formatteren verklaringen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> ingebouwde Modifier </strong> </p> </th> 
   <th> <p><strong> Bepaling van de Wijze van de Tekst </strong> </p> </th> 
   <th> <p><strong> Beschrijving </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong> is leeg </strong> </p> </td> 
   <td> <p><strong> leeg </strong> </p> </td> 
   <td> <p>Het veld bestaat voor het object, maar het veld heeft momenteel geen waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> is niet leeg </strong> </p> </td> 
   <td> <p><strong> niet leeg </strong> </p> </td> 
   <td> <p>Het veld waarop u filtert, bestaat en heeft een waarde gekregen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> ongeldig </strong> </p> </td> 
   <td> <p>Het veld is leeg of bestaat niet. U wilt bijvoorbeeld zoeken naar items zonder bovenliggende taak-id. Dit betekent dat u alleen zelfstandige taken wilt zien. Het bepalende element voor "identiteitskaart van de oudertaak"zou <strong> ongeldig </strong> zijn, aangezien een taak zonder identiteitskaart (in dit geval de ouder) niet bestaat. </p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> ongeldig </strong> </p> </td> 
   <td> <p>Het veld waarop u filtert, bestaat en bevat een andere waarde dan null.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> bevat </strong> </p> </td> 
   <td> <p><strong> Bevat </strong> </p> </td> 
   <td> <p>Dit is het <i> geval ongevoelige </i> versie van <strong> bevat </strong>. <code>cicontains inf</code> legt bijvoorbeeld een waarde vast die <code>Inf</code> of <code>inf</code> bevat.</p> <p> <p>Opmerking: Adobe Workfront zoekt naar het exacte woord of de exacte woordgroep die u opgeeft voor elke filterinstructie. Als u bijvoorbeeld zoekt naar een project dat de uitdrukking <code>new project</code> in de naam bevat, geeft Workfront geen projecten weer die alleen <code>new</code> of alleen <code>project</code> of <code>new main project</code> in de naam hebben. Met dit filter zoekt u alleen projecten met de exacte woordgroep <code>new project</code> in de naam.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> bevat niet </strong> </p> </td> 
   <td> <p><strong> cinotcontains </strong> </p> </td> 
   <td> <p>Dit is het <i> geval ongevoelige </i> versie van <strong> bevat </strong> niet.</p><p>Deze wijzigingfilters voor items waarvoor de opgegeven waarde ontbreekt.</p> <p><code>does not contain inf</code> legt bijvoorbeeld iets vast zonder <code>Inf</code> of <code>inf</code> in de naam.</p> <p>Nota: <span> als het gebied u voor filtert veelvoudige opties heeft, filter dit de resultaten uit die zowel de keus bevatten u specificeert, evenals de keus u specificeert en om het even welke extra keuzen.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong> bevat </strong> </p> </td> 
   <td> <p> Zoekt naar de gespecificeerde <i> geval gevoelige </i> tekst door een volledig tekstkoord.</p> <p>Als u bijvoorbeeld <code>contains Inf</code> gebruikt, wordt er alles met <code>Inf</code> vastgelegd, zoals het woord <code>Infinity.</code></p> <p>Deze bepaling kan slechts op de filters van de tekstwijze worden gebruikt.Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> bevat niet </strong> </p> </td> 
   <td> <p>Het filters voor punten die de <i> gespecificeerde gevoelig geval </i> waarde missen.</p> <p><code>notcontains inf</code> legt bijvoorbeeld alles vast zonder <code>inf</code> , maar geeft waarden weer die <code>Inf</code> bevatten.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> cieq </strong> </p> </td> 
   <td> <p>Dit is de <i> ongevoelige geval </i> optie van <strong> eq </strong>. Het geeft alleen een exacte overeenkomst met de gezochte waarde.</p> <p>Wanneer u bijvoorbeeld zoekt naar een taak met een specifieke naam, zoekt <code>task name cieq test</code> naar taken met de naam <code>Test</code> , <code>TEST</code> of <code>Test</code> , maar wordt er geen taak met de naam gevonden <code>test 123.</code></p> <p>Wanneer het zoeken naar een status, wordt de <strong> cieq </strong> bepaling niet gesteund. U zou de case sensitive bepaling, <strong> eq </strong> moeten gebruiken, om naar een status te zoeken.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong> cine </strong> </td> 
   <td> <p>Dit is het <i> geval ongevoelige </i> optie van <strong> ne </strong>, en het is het tegenovergestelde van de <b> cieq </b> bepaling. Het geeft alleen resultaten die niet exact overeenkomen met de gezochte waarde, zonder rekening te houden met het geval van de waarde.</p> <p>Bijvoorbeeld, <b> </b> keert om het even welke waarden terug die of "huidig"of "huidig"niet gelijk zijn. </p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong> eq </strong> </p> </td> 
   <td> <p>Deze bepaling keert slechts een nauwkeurige, <i> gevoelig geval </i> gelijke van de gezochte waarde terug.</p> <p>Wanneer u bijvoorbeeld naar volledige projecten zoekt, retourneert <code>eq CPL</code> alle projecten in de status Voltooid. <code>eq CPL, CUR</code> retourneert geen resultaat omdat een project niet gelijktijdig kan worden voltooid en actief is.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong> ne </strong> </td> 
   <td> <p>Dit is het <i> gevoelige geval </i> tegengesteld van <strong> eq </strong>. Het retourneert alleen resultaten die niet exact overeenkomen met de gezochte waarde en het komt ook overeen met het hoofdlettergebruik van de waarde.</p> <p>Bijvoorbeeld, <b> ne </b> keert om het even welke waarden terug die "Huidig"niet gelijk zijn, maar het keert geen waarden terug die "huidig"niet evenaren. </p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> ciin </strong> </p> </td> 
   <td> <p> Dit is het <i> geval ongevoelige </i> versie van <strong> in </strong>.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> cinotin </strong> </p> </td> 
   <td> <p>Dit is het <i> geval ongevoelige </i> versie van <strong> niets </strong>.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong> Gelijk </strong> </p> </td> 
   <td> <p><strong> in </strong> </p> </td> 
   <td> <p>Deze bepaling staat u toe om een komma-gescheiden lijst van <i> geval gevoelige </i> variabelen tot stand te brengen om met één enkel die attribuut te vergelijken in een filter wordt geëvalueerd. De volledige lijst wordt behandeld als OF verklaring en keert om het even welke resultaten terug die aan de criteria van één of meerdere variabelen voldoen.</p> <p>Bijvoorbeeld, wanneer het zoeken naar projecten, het gebruiken van <code>in CUR, PLN, CPL</code> keert alle projecten terug die in de Huidige, OF Planning, OF Volledige status zijn.</p> <p>De ingebouwde bepaling <strong> Gelijk </strong> beantwoordt aan de bepaling van de tekstwijze van <strong> in </strong>. Dit betekent dat u Gelijk kunt kiezen met meerdere waarden voor het veld.</p> <p>Bijvoorbeeld, kunt u een "Status evenaart Huidige, Planning, Dode"in een projectrapport kiezen en u kunt projecten in om het even welk van deze statussen bekijken.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> niet Gelijk </strong> </p> </td> 
   <td> <p><strong> niets </strong> </p> </td> 
   <td> <p>Dit is het <i> gevoelige geval </i> tegenover <strong> binnen </strong>. Het retourneert alleen resultaten die niet in de opgegeven lijst voorkomen.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> <p>Nota: <span> als het gebied u voor filtert veelvoudige opties heeft, filter dit de resultaten uit die zowel de keus bevatten u specificeert, evenals de keus u specificeert en om het even welke extra keuzen.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> als </strong> </p> </td> 
   <td> <p>Deze bepaling zoekt naar gedeelten van a <i> gevoelig geval </i> tekstkoord op gelijkaardige wijze aan <strong> bevat </strong>. Nochtans, <strong> als </strong> verstrekt de capaciteit om wilde kaartkarakters op te nemen om de tekst te breken.</p> <p>Als u bijvoorbeeld zoekt naar notities, wordt met <code>like %Current% %Dead%</code> een willekeurige notitie geretourneerd die de uitdrukking "Huidig naar dood" bevat. Notities met de tekst "Dead to Current" worden hier niet in opgenomen. Elke waarde wordt doorzocht in de volgorde waarin deze wordt vermeld. Het percentage vertegenwoordigt een jokerteken waarmee tekens of tekstsegmenten worden vervangen. Een onderstrepingsteken kan ook voor één enkel vervangingskarakter, zoals in <code>like Project_</code> worden gebruikt dat zowel "Project"als "Projecten"terugkeert. Als u van plan bent om a <strong> als </strong> of <strong> te gebruiken als </strong> bepaling in uw het filtreren, adviseren wij vermijdend % of _ karakters in de namen van het douanegegevensgebied, parameteropties, of andere objecten namen.</p><p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> cilike </strong> </p> </td> 
   <td> <p>Dit is het <i> geval ongevoelige </i> versie van <strong> als </strong>. <code>cilike %Current% %Dead%</code> retourneert bijvoorbeeld alle notities die <code>Current to Dead</code> of <code>current to dead</code> bevatten.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong> bestaat niet </strong> </td> 
   <td><strong> NOTEXISTS </strong> </td> 
   <td> <p>Deze bepaling wordt gebruikt slechts met complexe filters in een EXISTS verklaring. Deze filters verwijzen alleen naar de volgende objecten: </p> 
    <ul> 
     <li>Objecten die meerdere niveaus in de objecthiërarchie beslaan </li> 
     <li>Ontbrekende objecten </li> 
    </ul> <p>Voor informatie over het creëren van complexe filters die instructies gebruiken ziet het artikel <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md"> Complexe tekst-Wijze Filters creëren die EXISTS Verklaringen </a> gebruiken. Dit is de enige bepaling die in EXISTS verklaringen wordt gebruikt.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> groter dan </strong> </p> </td> 
   <td> <p><strong> gt </strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die groter is dan de ingevoerde waarde, exclusief de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> minder dan </strong> </p> </td> 
   <td> <p><strong> lt </strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die lager is dan de ingevoerde waarde, exclusief de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> groter dan Gelijk </strong> </p> </td> 
   <td> <p><strong> gte </strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met waarden die groter zijn dan of gelijk zijn aan de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> minder dan Gelijk </strong> </p> </td> 
   <td> <p><strong> lte </strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die kleiner is dan of gelijk is aan de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong> tussen </strong> </p> </td> 
   <td> <p><strong> tussen </strong> </p> </td> 
   <td> <p>Verstrekt twee vereiste gebiedswaarden en onderzoeken naar alle resultaten binnen waaier van beide gebieden, met inbegrip van de ingegaan waarden.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong> niet tussen </strong> </p> </td> 
   <td> <p>Dit is het omgekeerde van <strong> tussen </strong>. Er worden twee vereiste waardevelden weergegeven en er wordt gezocht naar alle resultaten buiten het bereik van beide velden, inclusief de ingevoerde waarden.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Voor meer informatie over tekstwijze in filters, zie <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref"> een filter uitgeven gebruikend tekstwijze </a>.</p> </td> 
  </tr>

</tbody> 
</table>
