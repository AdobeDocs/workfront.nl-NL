---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Berekende gegevensexpressies
description: U kunt gegevensexpressies gebruiken om berekende aangepaste gegevensvelden in Adobe Workfront te definiëren. Ze verbinden bestaande Workfront-velden met instructies die een nieuw veld genereren.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 1e91514f86a307ffa71cde650b35a2e3b8f0fa88
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Berekende gegevensexpressies

U kunt gegevensexpressies gebruiken om berekende aangepaste gegevensvelden in Adobe Workfront te definiëren. Ze verbinden bestaande Workfront-velden met instructies die een nieuw veld genereren.

U kunt berekende gegevensexpressies gebruiken in:

* Een aangepast formulier

   Ga voor meer informatie over het maken van berekende aangepaste gegevensvelden op aangepaste formulieren in Workfront naar [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Een berekende aangepaste kolom in een rapport of lijst wanneer u de tekstmodus gebruikt

   Ga voor meer informatie over het gebruik van de tekstmodus in rapporten en weergaven naar [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntaxis van berekende aangepaste velden versus berekende aangepaste kolommen

Hoewel de functies die u gebruikt hetzelfde zijn, kan de syntaxis voor het bouwen van een expressie in een berekend aangepast veld anders zijn dan voor het bouwen van een berekende aangepaste kolom.

Bijvoorbeeld:

* In een aangepast veld gebruikt u op een aangepast formulier voor taken de volgende opties om de naam te genereren van het bovenliggende project van de taak waaraan het aangepaste formulier is gekoppeld:

   ```
   {project}.{name}
   ```

* In een douanekolom in een rapport, zou u het volgende gebruiken om een de douanekolom van de Naam van het Project op een taakrapport toe te voegen:

   ```
   valuefield=project:name
   ```

   of

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >Dezelfde syntaxis is van toepassing op alle rapportelementen in de tekstmodus waar berekende expressies worden gebruikt: weergaven, filters, groepen, aanwijzingen.

De verschillen tussen de twee syntaxis zijn als volgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berekend aangepast veld</strong></td> 
   <td><strong>Berekend aangepast rapporteringselement</strong></td> 
  </tr> 
   <td>Vul veldnamen in accolades in.</td> 
   <td>Veldnamen tussen haakjes of haakjes plaatsen wanneer u ze in een <code>valuefield </code>lijn. <p>Veldnamen tussen accolades plaatsen wanneer ze worden gebruikt in een <code>valueexpression</code> lijn.</p> </td> 
  </tr> 
  <tr> 
   <td>Scheid de velden door punten.</td> 
   <td> <p>De velden scheiden met dubbele punten wanneer u ze in een <code>valuefield </code>line</p> <p>De velden van elkaar scheiden op punten wanneer u ze in een <code>valueexpression </code>lijn. </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over de syntaxis moet u in een berekende douanekolom gebruiken, zie [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Gegevensexpressies die u kunt gebruiken

In de onderstaande lijsten worden de beschikbare expressies gedefinieerd die u kunt gebruiken wanneer u een van de drie verschillende typen berekende aangepaste velden maakt in Workfront:

* [Berekende datum en tijd, aangepaste velden](#date-time-calculated-custom-fields)
* [Wiskundige berekende aangepaste velden](#mathematical-calculated-custom-fields)
* [Berekende tekst, aangepaste velden](#text-calculated-custom-fields)

### Berekende datum en tijd, aangepaste velden {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Als u een datum- en tijdberekening maakt die geen tijdgedeelte bevat of die de jokertekens $$TODAY of $$NOW gebruikt, gebruikt het systeem de datum volgens de UTC-zone (Coordinated Universal Time), niet volgens uw lokale tijdzone. Dit kan tot een onverwacht datumresultaat leiden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uitdrukking</th> 
   <th>Uitleg en voorbeeld</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Met deze expressie wordt het aantal dagen aan de datum toegevoegd. De getalwaarde kan gedeeltelijke dagen omvatten (1,5 voegt bijvoorbeeld anderhalve dag toe aan de datum).</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>ADDDAYS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Met deze expressie wordt het aantal weekdagen aan de datum toegevoegd. Met deze expressie worden alleen gehele gehele getallen aan de datum toegevoegd, naar beneden afgerond. </p> <p>De expressie wordt als volgt opgemaakt:</p><pre>ADDWEEKDAYS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Met deze expressie wordt het aantal maanden toegevoegd aan de datum. De notatie is als volgt:</p><pre>ADDMONTHS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Met deze expressie wordt het aantal jaren toegevoegd aan de datum en wordt de notatie als volgt weergegeven:</p><pre>ADDYEARS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Deze expressie wist het tijdgedeelte van een datum en is als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATUM</strong> </td> 
   <td> <p>Deze expressie converteert een tekenreeks naar een datum en is als volgt opgemaakt:</p><pre>DATE(tekenreeks)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Deze expressie retourneert het aantal dagen tussen de twee datums, rekening houdend met de begin- en einddagen van de geselecteerde periode en de tijdstempels op die dagen. Als de begintijd van de begindatum bijvoorbeeld 3 PM is, wordt de begindag niet als een volledige dag geteld.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Deze expressie geeft de dag van de maand voor de datum als een getal tussen 1 en 31.</p> <p>De expressie wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Deze expressie retourneert de dag van de week voor de datum als een getal, tussen 1 (zondag) en 7 (zaterdag).</p> <p>De expressie wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Deze expressie geeft het totaal aantal dagen in de maand van de datum als een getal en heeft de volgende notatie. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Deze expressie retourneert het totale aantal weekdagen tussen de datum en het einde van de week, of het einde van de maand, afhankelijk van welke het eerst komt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Deze expressie geeft het totaal aantal dagen in het jaar van de datum als een getal en heeft de volgende notatie. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Deze expressie retourneert de laatste datum in de lijst en heeft de volgende notatie:</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Deze expressie retourneert de vroegste datum in de lijst en heeft de volgende notatie:</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UUR</strong> </td> 
   <td> <p>Deze expressie geeft het uur van de datum als een getal tussen 0 en 23.</p> <p>De expressie wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUUT</strong> </td> 
   <td> <p>Deze expressie retourneert de minuut van de datum als een getal tussen 0 en 60, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MAAND</strong> </td> 
   <td> <p>Deze expressie retourneert de maand van de datum als een getal tussen 1 en 12, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TWEEDE</strong> </td> 
   <td> <p>Deze expressie retourneert de tweede van de datum als een getal tussen 0 en 60, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Deze expressie retourneert het aantal weekdagen tussen twee datums, rekening houdend met de begin- en einddagen van de geselecteerde periode en de tijdstempels op die dagen. Als de begintijd van de begindatum bijvoorbeeld 3 PM is, wordt de begindag niet als een volledige dag geteld.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>WEEKDAYDIFF(datum2, datum1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Deze expressie retourneert het aantal geplande minuten tussen de datums volgens het standaardschema.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>JAAR</strong> </td> 
   <td> <p>Deze expressie geeft het jaar van de datum als een getal van 4 cijfers weer, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p><pre>JAAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Wiskundige berekende aangepaste velden {#mathematical-calculated-custom-fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uitdrukking</th> 
   <th>Toelichting</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Deze expressie retourneert de absolute waarde van het getal en is als volgt opgemaakt. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>GEMIDDELD</strong> </td> 
   <td>Deze expressie retourneert het gemiddelde van getallen en is als volgt opgemaakt:<pre>AVERAGE(nummer1, nummer2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Met deze expressie wordt een getal afgerond tot op het dichtstbijzijnde gehele getal en wordt de notatie als volgt weergegeven. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Deze expressie deelt alle getallen in de opgegeven volgorde en is als volgt opgemaakt:<pre>DIV(nummer1, nummer2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Met deze expressie wordt een getal omlaag afgerond naar het dichtstbijzijnde gehele getal en wordt de notatie als volgt weergegeven. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Deze expressie retourneert de natuurlijke logaritmewaarde van het getal en is als volgt opgemaakt:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Deze uitdrukking keert de logaritmewaarde van number2 aan base number1 terug en is geformatteerd als volgt:<pre>LOG(nummer1, nummer2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Deze expressie retourneert het grootste item in de lijst en is als volgt opgemaakt:<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Deze expressie retourneert het kleinste item in de lijst en is als volgt opgemaakt:<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMMER</strong> </td> 
   <td>Deze expressie converteert een tekenreeks naar een getal en heeft de volgende notatie:<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Deze uitdrukking keert een aantal terug dat aan een macht wordt opgeheven en als volgt geformatteerd:<pre>POWER(nummer, vermogen)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Deze expressie vermenigvuldigt alle getallen en is als volgt opgemaakt:<pre>PROD(nummer1, nummer2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ROND</strong> </td> 
   <td>Met deze expressie wordt het getal afgerond tot het opgegeven aantal decimalen met de precisie en wordt het als volgt opgemaakt:<p>ROUND(getal, precisie)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Deze expressie geeft de getallen in oplopende volgorde weer en heeft de volgende notatie:</p><pre>SORTASCNUM(nummer1,nummer2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Deze expressie geeft de getallen in aflopende volgorde weer en heeft de volgende notatie:<pre>SORTDESCNUM(nummer1, nummer2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Deze expressie retourneert een vierkantswortel van een getal en is als volgt opgemaakt. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Deze expressie trekt alle getallen af in de opgegeven volgorde en is als volgt opgemaakt:<pre>SUB(nummer1, nummer2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Deze expressie voegt alle getallen toe en heeft de volgende notatie:<pre>SUM(nummer1, nummer2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Berekende tekst, aangepaste velden {#text-calculated-custom-fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uitdrukking</th> 
   <th>Toelichting</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>CASE</strong> </td> 
   <td> <p>Deze expressie wordt samen met andere expressies gebruikt om een waarde in een lijst te kiezen op basis van een indexnummer. Een indexnummer is een veld of functie die een numerieke waarde retourneert (gewoonlijk in een bekend bereik).</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>De volgende expressie retourneert bijvoorbeeld de naam van de dag van de week, waarbij 1=zondag, 2=maandag enzovoort, in een berekende kolom:</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Maandag","Dinsdag","Woensdag","Donderdag","Vrijdag","Zaterdag")</pre> <p>Deze expressie werkt het best met andere expressies die een getal retourneren, zoals DAYOFWEEK, DAYOFMONTH en MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCREET</strong> </td> 
   <td> <p>Deze expressie voegt de tekenreeks samen en wordt als volgt opgemaakt:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>Hieronder volgen voorbeelden van scheidingstekens die u kunt opnemen:</p> 
    <ul> 
     <li>een spatie: "</li> 
     <li>een streepje: "-"</li> 
     <li>een schuine streep: "/"</li> 
     <li>een komma: ","</li> 
     <li>een woord: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>BEVATTEN</strong> </td> 
   <td>Deze expressie retourneert true als de string findText is gevonden binnen de withinText-tekenreeks en als volgt is opgemaakt:<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Deze expressie verwijdert speciale tekens uit de tekenreeks, zodat deze kunnen worden opgenomen in een URL-argument.<p>De expressie wordt als volgt opgemaakt:</p><pre>ENCODEURL(tekenreeks)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Deze expressie evalueert een voorwaarde die u opgeeft en retourneert de waarde van de expressie true als deze waar is, of de waarde van de expressie false als deze onwaar is.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>IF (voorwaarde, trueExpression, falseExpression)</pre> <p>U kunt bijvoorbeeld twee verschillende datumvelden vergelijken, gevolgd door een Waar/Onwaar-resultaat als een gegevenstekenreeks:</p><pre>IF({projectedCompletionDate}&gt;{scheduledCompletionDate},"Off Track","On Track")</pre> <p>In de dagelijkse toespraak betekent deze verklaring: "IF the Projected Completion Date of my object is "Groter dan" the Planned Completion Date of my same object, then display the words 'Off Track' in this field; anders geeft u de woorden 'Op track' weer.</p> <p>Als u geen label wilt toewijzen aan de expressie true of false, moet u een leeg label in de instructie invoegen, zoals:</p><pre>IF({projectedCompletionDate}&gt;{scheduledCompletionDate},"","On Track")</pre> <p>of</p><pre>IF({projectedCompletionDate}&gt;{scheduledCompletionDate},"Off Track",")</pre> <p>Voor meer informatie over het samenstellen van "IF"verklaringen, zie <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Overzicht van "IF"-instructies</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Met deze expressie kunt u zoeken naar een specifieke waarde in een reeks mogelijke waarden. Als de waarde u zoekt één van de verstrekte waarden evenaart, dan keert de uitdrukking trueExpression terug; anders, keert het falseExpression terug.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>Bijvoorbeeld, kunt u een specifieke Eigenaar van het Project vinden en die projecten met een gespecificeerde markering in een projectweergave merken: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> In de dagelijkse toespraak betekent deze verklaring: "Als de eigenaar van het project Jennifer Campbell of Rick Kuvec is, markeert u dit project met 'Marketing Team'; anders markeert u het met 'Other Teams'."</p> <p> Als u geen label wilt toewijzen aan de expressie true of false, moet u een leeg label in de instructie invoegen, zoals: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>of </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Deze expressie retourneert true als de waarde gelijk is aan een van de opgegeven waarden. anders retourneert de expressie false.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>IN(waarde, waarde1[, waarde2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Deze expressie retourneert true als de waarde null of leeg is. anders retourneert de expressie false.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>ISBLANK(waarde)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LINKS</strong> </td> 
   <td> <p>Deze expressie retourneert een opgegeven aantal tekens vanaf de linkerzijde van een tekenreeks en is als volgt opgemaakt:</p><pre>LEFT(tekenreeks, lengte)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Deze expressie retourneert de lengte van een tekenreeks en is als volgt opgemaakt:</p><pre>LEN (tekenreeks)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LAGER</strong> </td> 
   <td>Deze expressie retourneert de tekenreeks in kleine letters en is als volgt opgemaakt:<pre>LOWER(tekenreeks)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>VERVANGEN</strong> </td> 
   <td> <p>Deze expressie vervangt alle instanties van string2 door string3 in string1.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RECHTS</strong> </td> 
   <td> <p>Deze expressie retourneert een opgegeven aantal tekens vanaf de rechterzijde van een tekenreeks en is als volgt opgemaakt:</p><pre>RIGHT (tekenreeks, lengte)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ZOEKEN</strong> </td> 
   <td> <p>Deze expressie retourneert de index van de eerste instantie van findText in de tekenreeks withinText, te beginnen bij de opgegeven startpositie, of -1 als de tekst niet wordt gevonden.</p> <p>De expressie wordt als volgt opgemaakt:</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TEKENREEKS</strong> </td> 
   <td> <p>Deze expressie converteert een getal naar een tekenreeks en heeft de volgende notatie:</p><pre>STRING(nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Met deze expressie wordt een lijst met tekenreeksen oplopend gesorteerd. De opmaak is als volgt:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Met deze expressie wordt een lijst met tekenreeksen in aflopende volgorde gesorteerd. De opmaak is als volgt:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Deze expressie retourneert tekens van een tekenreeks op basis van de opgegeven begin- en eindindex en is als volgt opgemaakt:</p><pre>SUBSTR({string}, aantal startpositie, aantal eindpositie)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Deze expressie verwijdert witruimte van het begin en einde van een tekenreeks en is als volgt opgemaakt:</p><pre>TRIM(tekenreeks)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>BOVEN</strong> </td> 
   <td> <p>Deze expressie retourneert een tekenreeks in hoofdletters en is als volgt opgemaakt:</p><pre>UPPER(tekenreeks)</pre> </td> 
  </tr> 
 </tbody> 
</table>
