---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Overzicht van berekende gegevensexpressies
description: U kunt gegevensexpressies gebruiken om berekende aangepaste gegevensvelden in Adobe Workfront te definiëren. Berekende expressies verbinden bestaande Workfront-velden met instructies die een nieuw veld genereren.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '2166'
ht-degree: 0%

---

# Overzicht van berekende gegevensexpressies

<!--Audited: 12/2023-->

U kunt gegevensexpressies gebruiken om berekende aangepaste velden in Adobe Workfront te definiëren. Berekende expressies verbinden bestaande Workfront-velden met instructies die een nieuw veld genereren.

U kunt berekende gegevensexpressies gebruiken in:

* Een berekend aangepast veld op een aangepast formulier

  Ga voor meer informatie over het maken van berekende aangepaste velden op aangepaste formulieren in Workfront naar [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Een berekende aangepaste kolom in een rapport of lijst wanneer u de tekstmodus gebruikt

  Ga voor meer informatie over het gebruik van de tekstmodus in rapporten en weergaven naar [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntaxis van berekende aangepaste velden versus berekende aangepaste kolommen

Hoewel de functies die u gebruikt hetzelfde zijn, kan de syntaxis voor het bouwen van een expressie in een berekend aangepast veld afwijken van de syntaxis voor het bouwen van een berekende aangepaste kolom.

De verschillen tussen de twee syntaxis zijn als volgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berekend aangepast veld</strong></td> 
   <td><strong>Berekend aangepast rapporteringselement</strong></td> 
  </tr> 
   <td>Veldnamen tussen accolades plaatsen</td> 
   <td>Veldnamen tussen haakjes of haakjes plaatsen wanneer u ze in een <p><code>valuefield </code></p>lijn. <p>Veldnamen tussen accolades plaatsen wanneer ze worden gebruikt in een <p><code>valueexpression</code></p> lijn.</p> </td> 
  </tr> 
  <tr> 
   <td>De velden scheiden met punten</td> 
   <td> <p>De velden scheiden met dubbele punten wanneer u ze in een <p><code>valuefield </code></p>line</p> <p>De velden van elkaar scheiden op punten wanneer u ze in een <p><code>valueexpression </code></p>lijn. </p> </td> 
  </tr> 
 </tbody> 
</table>

Bijvoorbeeld:

* In een aangepast veld gebruikt u op een aangepast formulier voor taken de volgende opties om de naam te genereren van het bovenliggende project van de taak waaraan het aangepaste formulier is gekoppeld:


  ` {project}.{name}`


* In een douanekolom in een rapport, zou u het volgende gebruiken om een de douanekolom van de Naam van het Project op een taakrapport toe te voegen:


  `valuefield=project:name`


  of

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >Dezelfde syntaxis is van toepassing op alle rapportelementen in de tekstmodus waarvoor berekende expressies worden gebruikt: weergaven, filters, groepen en aanwijzingen.

Voor meer informatie over de syntaxis moet u in een berekende douanekolom gebruiken, zie [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Gegevensexpressies die u kunt gebruiken

In de onderstaande lijsten worden de beschikbare expressies gedefinieerd die u kunt gebruiken wanneer u een van de drie verschillende typen berekende aangepaste velden maakt in Workfront:

* [Berekende datum en tijd, aangepaste velden](#date-time-calculated-custom-fields)
* [Wiskundige berekende aangepaste velden](#mathematical-calculated-custom-fields)
* [Berekende tekst, aangepaste velden](#text-calculated-custom-fields)

U kunt de hieronder vermelde uitdrukkingen gebruiken om berekende douanekolommen te bouwen. U moet echter de juiste syntaxis gebruiken voor een berekende aangepaste kolom, zoals beschreven in de sectie  [Syntaxis van berekende aangepaste velden versus berekende aangepaste kolommen](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in dit artikel.

### Berekende datum en tijd, aangepaste velden {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Als u een datum- en tijdberekening maakt die geen tijdgedeelte bevat of die de jokertekens $$TODAY of $$NOW gebruikt, gebruikt het systeem de datum volgens de UTC-zone (Coordinated Universal Time), niet volgens uw lokale tijdzone. Dit kan tot een onverwacht datumresultaat leiden.

U kunt een datum- of tijdberekend aangepast veld maken met de volgende expressies:

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
   <td> <p>Hiermee voegt u het aantal dagen toe aan de datum. De getalwaarde kan gedeeltelijke dagen omvatten. 1,5 voegt bijvoorbeeld anderhalve dag toe aan de datum.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Hiermee voegt u het aantal weekdagen toe aan de datum. Met deze expressie worden alleen gehele gehele getallen aan de datum toegevoegd, naar beneden afgerond. </p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Hiermee voegt u het aantal maanden toe aan de datum. De notatie is als volgt:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Hiermee voegt u het aantal jaren toe aan de datum. De notatie is als volgt:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Wist het tijdgedeelte van een datum en is als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Converteert een tekenreeks naar een datum en is als volgt opgemaakt:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Geeft als resultaat het aantal dagen tussen de twee datums, rekening houdend met de begin- en einddagen van de geselecteerde periode en de tijdstempels op die dagen. Als de begintijd van de begindatum bijvoorbeeld 3 PM is, wordt de begindag niet geteld als een volledige dag.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Retourneert de dag van de maand voor de datum als een getal tussen 1 en 31.</p> <p>De expressie wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Retourneert de dag van de week voor de datum als een getal tussen 1 (zondag) en 7 (zaterdag).</p> <p>De expressie wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Retourneert het totaal aantal dagen in de maand van de datum als een getal en wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Geeft als resultaat het totale aantal weekdagen tussen de datum en het einde van de week of, indien dit eerder is, het einde van de maand. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Retourneert het totaal aantal dagen in het jaar van de datum als een getal en wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Retourneert de laatste datum in de lijst en is als volgt opgemaakt:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Retourneert de vroegste datum in de lijst en is als volgt opgemaakt:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UUR</strong> </td> 
   <td> <p>Retourneert het uur van de datum als een getal tussen 0 en 23.</p> <p>De expressie wordt als volgt opgemaakt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUUT</strong> </td> 
   <td> <p>Retourneert de minuut van de datum als een getal tussen 0 en 60, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MAAND</strong> </td> 
   <td> <p>Retourneert de maand van de datum als een getal tussen 1 en 12, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>TWEEDE</strong> </td> 
   <td> <p>Retourneert de tweede van de datum als een getal tussen 0 en 60, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Geeft als resultaat het aantal weekdagen tussen twee datums, rekening houdend met de begin- en einddagen van de geselecteerde periode en de tijdstempels op die dagen. Als de begintijd van de begindatum bijvoorbeeld 3 PM is, wordt de begindag niet als een volledige dag geteld.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Retourneert het aantal geplande minuten tussen de datums volgens het standaardschema.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>JAAR</strong> </td> 
   <td> <p>Retourneert het jaar van de datum als een getal van 4 cijfers, opgemaakt als volgt. In dit voorbeeld is de datum de ingangsdatum voor een werkobject.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Wiskundige berekende aangepaste velden {#mathematical-calculated-custom-fields}

U kunt een berekend aangepast veld maken dat een aantal van de volgende wiskundige expressies gebruikt:

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
   <td>Retourneert de absolute waarde van het getal en is als volgt opgemaakt. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>GEMIDDELD</strong> </td> 
   <td>Retourneert het gemiddelde van getallen en is als volgt opgemaakt:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Rondt een getal af tot op het dichtstbijzijnde gehele getal en wordt als volgt opgemaakt. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Verdeelt alle getallen in de opgegeven volgorde en is als volgt opgemaakt:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Rondt een getal af naar het dichtstbijzijnde gehele getal en wordt als volgt opgemaakt. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Retourneert de natuurlijke logaritmewaarde van het getal en wordt als volgt opgemaakt:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Retourneert de logaritmewaarde van number2 naar het basissenummer1 en is als volgt opgemaakt:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Retourneert het grootste item in de lijst en is als volgt opgemaakt:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Retourneert het kleinste item in de lijst en is als volgt opgemaakt:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMMER</strong> </td> 
   <td>Zet een tekenreeks om in een getal en is als volgt opgemaakt:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Retourneert een getal dat tot een macht is verheven en dat als volgt is opgemaakt:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Vermenigvuldigt alle getallen en is als volgt opgemaakt:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>OPMERKING</b></p>

<p>Wanneer u velden met uren vermenigvuldigt, dient u te weten of de database de uren in geselecteerde velden in minuten, uren of seconden opslaat. Als de uren in notulen of seconden maar vertoning in uren in de interface van Workfront worden bewaard, zou u voor de omzetting van notulen of seconden aan uren kunnen rekenschap moeten geven wanneer het schrijven van een uitdrukking gebruikend deze berekening. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROND</strong> </td> 
   <td>Rondt het getal af tot de opgegeven decimalen met de nauwkeurigheid en wordt als volgt opgemaakt:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> De getallen worden in oplopende volgorde gesorteerd en worden als volgt opgemaakt:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>De getallen worden in aflopende volgorde gesorteerd en worden als volgt opgemaakt:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Retourneert een vierkantswortel van een getal en is als volgt opgemaakt. In dit voorbeeld wordt het aantal objecten gebruikt onder het object waaraan het aangepaste formulier is gekoppeld.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Trekt alle aantallen in de verstrekte orde af en is geformatteerd als volgt:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Voegt alle getallen toe en wordt als volgt opgemaakt:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Berekende tekst, aangepaste velden {#text-calculated-custom-fields}

U kunt een berekend aangepast veld maken waarin een waarde met tekstopmaak wordt weergegeven met de volgende expressies:

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
   <td> <p>Wordt gebruikt met andere expressies om een waarde in een lijst te kiezen op basis van een indexnummer. </p>
   <p>Een indexnummer is een veld of functie die een numerieke waarde retourneert (gewoonlijk in een bekend bereik).</p> 
   <p>De expressie wordt als volgt opgemaakt:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>De volgende expressie retourneert bijvoorbeeld de naam van de dag van de week, waarbij 1=zondag, 2=maandag enzovoort, in een berekende kolom:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Werkt het best met andere expressies die een getal retourneren, zoals DAYOFWEEK, DAYOFMONTH en MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCREET</strong> </td> 
   <td> <p>Voegt de tekenreeks samen en is als volgt opgemaakt:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Hieronder volgen voorbeelden van scheidingstekens die u kunt opnemen:</p> 
    <ul> 
     <li>een spatie: " "</li> 
     <li>een streepje: "-"</li> 
     <li>een slash: "/"</li> 
     <li>een komma: ","</li> 
     <li>een woord: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>BEVATTEN</strong> </td> 
   <td>Retourneert true als de findText-tekenreeks is gevonden binnen de withinText-tekenreeks en als volgt is opgemaakt:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Hiermee worden alle speciale tekens in de tekenreeks verwijderd, zodat deze in een URL-argument kunnen worden opgenomen.<p>De expressie wordt als volgt opgemaakt:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Evalueert een voorwaarde die u specificeert en de waarde van trueExpression terugkeert als het waar is, of de waarde van falseExpression als het vals is.</p>

<p>De expressie wordt als volgt opgemaakt:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>U kunt bijvoorbeeld twee verschillende datumvelden vergelijken, gevolgd door een Waar/Onwaar-resultaat als een gegevenstekenreeks:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>In de dagelijkse toespraak betekent deze verklaring: "ALS de Geprojecteerde Voltooiingsdatum van mijn voorwerp "Groter dan"de Geplande VoltooiingsDatum van mijn zelfde voorwerp is, dan tonen de woorden "Van Spoor"op dit gebied; anders, tonen de woorden "Op Spoor".</p>

<p>Als u geen label wilt toewijzen aan de expressie true of false, moet u een leeg label in de instructie invoegen, zoals:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>of</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Voor meer informatie over het samenstellen van "IF"verklaringen, zie <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Overzicht van "IF"-instructies</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Hiermee kunt u zoeken naar een specifieke waarde in een reeks mogelijke waarden. Als de waarde u zoekt één van de verstrekte waarden evenaart, dan keert de uitdrukking trueExpression terug; anders, keert het falseExpression terug.</p> 
   <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Bijvoorbeeld, kunt u een specifieke Eigenaar van het Project vinden en die projecten met een gespecificeerde markering in een projectweergave merken: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> In de dagelijkse toespraak betekent deze verklaring: "Als de projecteigenaar Jennifer Campbell of Rick Kuvec is, merk dit project met "Marketing Team"; anders, merk het met "Andere Teams"."</p> 
    <p> Als u geen label wilt toewijzen aan de expressie true of false, moet u een leeg label in de instructie invoegen, zoals: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>of </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Retourneert true als de waarde gelijk is aan een van de opgegeven waarden; anders retourneert de expressie false.</p> <p>De expressie wordt als volgt opgemaakt:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Retourneert true als de waarde null of leeg is; anders retourneert de expressie false.</p> <p>De expressie wordt als volgt opgemaakt:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LINKS</strong> </td> 
   <td> <p>Retourneert een opgegeven aantal tekens vanaf de linkerzijde van een tekenreeks en wordt als volgt opgemaakt:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Retourneert de lengte van een tekenreeks en is als volgt opgemaakt:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LAGER</strong> </td> 
   <td>Retourneert de tekenreeks in kleine letters en is als volgt opgemaakt:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>VERVANGEN</strong> </td> 
   <td> <p>Vervangt alle instanties van string2 door string3 in string1.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RECHTS</strong> </td> 
   <td> <p>Retourneert een opgegeven aantal tekens vanaf de rechterzijde van een tekenreeks en wordt als volgt opgemaakt:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ZOEKEN</strong> </td> 
   <td> <p>Retourneert de index van de eerste instantie van findText in de tekenreeks binnenText, te beginnen bij de opgegeven startpositie, of -1 als de tekst niet wordt gevonden.</p> <p>De expressie wordt als volgt opgemaakt:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>TEKENREEKS</strong> </td> 
   <td> <p>Zet een getal om in een tekenreeks en is als volgt opgemaakt:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Hiermee wordt een lijst met tekenreeksen oplopend gesorteerd. De lijst is als volgt opgemaakt:</p>

<p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Sorteert een lijst van koorden in dalende orde en is geformatteerd als volgt:</p>

<p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Retourneert tekens van een tekenreeks op basis van de opgegeven begin- en eindindex en is als volgt opgemaakt:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Verwijdert witruimte aan het begin en einde van een tekenreeks en wordt als volgt opgemaakt:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>BOVEN</strong> </td> 
   <td> <p>Retourneert een tekenreeks in hoofdletters en is als volgt opgemaakt:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
