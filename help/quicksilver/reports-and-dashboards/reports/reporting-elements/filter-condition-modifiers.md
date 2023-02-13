---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- en voorwaardenmodificatoren
description: Met de filter- en voorwaardemodities kunt u filters maken en voorwaarden instellen voor het opmaken van de rapportresultaten.
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 0%

---

# Filter- en voorwaardenmodificatoren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Met de filter- en voorwaardemodities kunt u filters maken en voorwaarden instellen voor het opmaken van de rapportresultaten.

Raadpleeg het artikel voor meer informatie over het maken van filters. [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Raadpleeg het artikel voor meer informatie over het gebruik van voorwaardelijke opmaak in Weergaven [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- en voorwaardenmodificatoren

Raadpleeg het artikel voor een lijst met ingebouwde tijdframewijzigingstoetsen [Rapporten filteren op tijdframes](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Sommige bepalingen zijn ingebouwd en u kunt hen van een drop-down menu binnen uw filter of voorwaardelijke het formatteren verklaring kiezen. Andere wijzigingstoetsen kunnen alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over het begrijpen van de tekstmodus [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

U kunt de volgende voorwaardelijke wijzigingstoetsen in filters en voorwaardelijke het formatteren verklaringen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ingebouwde modifier</strong> </p> </th> 
   <th> <p><strong>Tekstmodus wijzigen</strong> </p> </th> 
   <th> <p><strong>Beschrijving</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Is leeg</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>Het veld bestaat voor het object, maar aan het veld is nog geen waarde toegewezen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Is niet leeg</strong> </p> </td> 
   <td> <p><strong>niet leeg</strong> </p> </td> 
   <td> <p>Het veld waarop u filtert, bestaat en heeft een waarde gekregen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Het veld is leeg of bestaat niet. U wilt bijvoorbeeld zoeken naar items zonder bovenliggende taak-id. Dit betekent dat u alleen zelfstandige taken wilt zien. De kwalificatie voor de "bovenliggende taak-id" zou <strong>null</strong>, omdat een taak zonder id (in dit geval het bovenliggende element) niet bestaat. </p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Het veld waarop u filtert, bestaat en bevat een andere waarde dan null.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Bevat</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>(Niet-hoofdlettergevoelig) Dit is de niet-hoofdlettergevoelige versie van <strong>contains</strong>. Bijvoorbeeld: Met "cicontains inf" wordt elke waarde vastgelegd die "Inf" of "inf" bevat.</p> <p> <p>Opmerking: Adobe Workfront zoekt naar het exacte woord of de exacte woordgroep die u opgeeft voor elke filterinstructie. Als u bijvoorbeeld zoekt naar een project dat de uitdrukking "nieuw project" in de naam bevat, geeft Workfront geen projecten weer die alleen "nieuw" of alleen "project" of "nieuw hoofdproject" in de naam hebben. Het filter vindt slechts projecten met de nauwkeurige uitdrukking "nieuw project"in de naam.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(Niet-hoofdlettergevoelig) Dit is de niet-hoofdlettergevoelige optie van <strong>eq</strong>. Er wordt alleen een exacte overeenkomst met de gezochte waarde geretourneerd.</p> <p>Wanneer u bijvoorbeeld zoekt naar een taak met een specifieke naam, zoekt "task name cieq test" naar taken met de naam "Test", "TEST" of "Test", maar wordt geen taak met de naam "test 123" gevonden.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciïne</strong> </p> </td> 
   <td> <p>(Niet-hoofdlettergevoelig) Dit is de niet-hoofdlettergevoelige versie van <strong>in</strong>.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>knap</strong> </p> </td> 
   <td> <p>Dit is de niet-vertrouwelijke versie van <strong>leuk</strong>. Bijvoorbeeld: "cilike %Current% %Dead%" retourneert alle notities met "Current to Dead" of "current to dood".</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>(Niet-hoofdlettergevoelig) Dit is de niet-hoofdlettergevoelige versie van <strong>niets</strong>.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over het maken van filters met gebruik van de tekstmodus <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contains</strong> </p> </td> 
   <td> <p>(Hoofdlettergevoelig) Hiermee wordt gezocht naar de opgegeven tekst in een hele tekstreeks.</p> <p>Als u bijvoorbeeld "contains Inf" gebruikt, wordt alles met "Inf" vastgelegd, zoals het woord "Infinity".</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters.Zie voor meer informatie over tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Bevat niet</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>(Niet-hoofdlettergevoelig) Het filtert voor items waarvoor de opgegeven waarde ontbreekt.</p> <p>Met 'bevat geen inf' wordt bijvoorbeeld iets vastgelegd zonder 'Inf' of 'inf' in de naam.</p> <p>Opmerking: <span>Als het veld waarvoor u filtert meerdere opties heeft, worden hiermee de resultaten uitgefilterd die zowel de door u opgegeven keuze bevatten als de door u opgegeven keuze en eventuele extra opties.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Bestaat niet</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Deze bepaling wordt gebruikt slechts met complexe filters in een EXISTS verklaring. Deze filters verwijzen alleen naar de volgende objecten: </p> 
    <ul> 
     <li>Objecten die meerdere niveaus in de objecthiërarchie beslaan </li> 
     <li>Ontbrekende objecten </li> 
    </ul> <p>Zie het artikel voor informatie over het maken van complexe filters met gebruik van EXISTS-instructies <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Complexe tekstmodusfilters maken met bestaande instructies</a>. Dit is de enige bepaling die in EXISTS verklaringen wordt gebruikt.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Gelijk</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>(Hoofdlettergevoelig) Met deze optie kunt u een lijst met door komma's gescheiden variabelen maken die u wilt vergelijken met één kenmerk dat in een filter wordt geëvalueerd. De volledige lijst wordt behandeld als OF verklaring en keert om het even welke resultaten terug die aan de criteria van één of meerdere variabelen voldoen.</p> <p>Bijvoorbeeld, wanneer het zoeken naar projecten, die "in CUR, PLN, CPL"gebruiken keert alle projecten terug die in de Huidige, OF Planning, OF de Volledige status zijn.</p> <p>De ingebouwde optie <strong>Gelijk</strong> komt overeen met de tekstmoduswijziging van <strong>in</strong>. Dit betekent dat u Gelijk kunt kiezen met meerdere waarden voor het veld.</p> <p>Bijvoorbeeld, kunt u een "Status evenaart Huidige, Planning, Dode"in een projectrapport kiezen en u kunt projecten in om het even welk van deze statussen bekijken.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(Hoofdlettergevoelig) Hiermee wordt alleen een exacte overeenkomst met de gezochte waarde geretourneerd.</p> <p>Bijvoorbeeld, wanneer het zoeken naar volledige projecten, "eq CPL"keert alle projecten in de volledige status terug. "eq CPL, CUR"keert geen resultaat terug omdat een project niet volledig en actueel kan zijn tezelfdertijd.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over het gebruik van de tekstmodus om filters te maken <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Groter dan</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die groter is dan de ingevoerde waarde, exclusief de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>leuk</strong> </p> </td> 
   <td> <p>(Hoofdlettergevoelig) Hiermee zoekt u op vergelijkbare wijze naar delen van een tekstreeks <strong>contains</strong>. Maar <strong>leuk</strong> hiermee kunt u jokertekens invoegen om de tekst te verbreken.</p> <p>Als u bijvoorbeeld zoekt naar notities en "bijvoorbeeld %Current% %Dead%" gebruikt, wordt een notitie geretourneerd met de zin "Current to Dead" (Huidig om te worden vervangen). Notities met de tekst "Dead to Current" worden hier niet in opgenomen. Elke waarde wordt doorzocht in de volgorde waarin deze wordt vermeld. Het percentage vertegenwoordigt een jokerteken ter vervanging van tekens of tekstsegmenten.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Minder dan</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die lager is dan de ingevoerde waarde, exclusief de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Groter dan gelijk</strong> </p> </td> 
   <td> <p><strong>gist</strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met waarden die groter zijn dan of gelijk zijn aan de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Minder dan gelijk</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die kleiner is dan of gelijk is aan de ingevoerde waarde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Tussen</strong> </p> </td> 
   <td> <p><strong>Tussen</strong> </p> </td> 
   <td> <p>Verstrekt twee vereiste gebiedswaarden en onderzoeken naar alle resultaten binnen waaier van beide gebieden met inbegrip van de ingegaan waarden.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>(Hoofdlettergevoelig) Het filter filtert voor items waarvoor de opgegeven waarde ontbreekt.</p> <p>Met 'notcontains inf' wordt bijvoorbeeld alles vastgelegd zonder 'inf', maar worden waarden weergegeven die 'Inf' bevatten.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nobetween</strong> </p> </td> 
   <td> <p>Dit is het omgekeerde van <strong>Tussen</strong>. Er worden twee vereiste waardevelden weergegeven en er wordt gezocht naar alle resultaten buiten het bereik van beide velden, inclusief de ingevoerde waarden.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Niet gelijk</strong> </p> </td> 
   <td> <p><strong>niets</strong> </p> </td> 
   <td> <p>(Hoofdlettergevoelig) Dit is het tegenovergestelde van <strong>in</strong>. Het retourneert alleen resultaten die niet in de opgegeven lijst voorkomen.</p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> <p>Opmerking: <span>Als het veld waarvoor u filtert meerdere opties heeft, worden hiermee de resultaten uitgefilterd die zowel de door u opgegeven keuze bevatten als de door u opgegeven keuze en eventuele extra opties.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(Hoofdlettergevoelig) Dit is het tegenovergestelde van <strong>eq</strong>. Het retourneert alleen resultaten die niet exact overeenkomen met de gezochte waarde en het komt ook overeen met het hoofdlettergebruik van de waarde.</p> <p>Bijvoorbeeld: <b>ne</b> Geeft alle waarden die niet gelijk zijn aan "Current", maar retourneert geen waarden die niet gelijk zijn aan "current". </p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>varkens</strong> </td> 
   <td> <p>(Niet-hoofdlettergevoelig) Dit is de niet-hoofdlettergevoelige optie van <strong>ne</strong> en het is het tegenovergestelde van <b>cieq</b> modifier. Het geeft alleen resultaten die niet exact overeenkomen met de gezochte waarde, zonder rekening te houden met het geval van de waarde.</p> <p>Bijvoorbeeld: <b>varkens</b> geeft waarden weer die niet gelijk zijn aan "current" of "Current". </p> <p>Deze optie kan alleen worden gebruikt in tekstmodusfilters. Zie voor meer informatie over de tekstmodus in filters <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Een filter bewerken in de tekstmodus</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
