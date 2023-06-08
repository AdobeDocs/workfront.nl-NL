---
product-area: reporting
navigation-topic: text-mode-reporting
title: Voorwaardelijke opmaak gebruiken in tekstmodus
description: Voorwaardelijke opmaak gebruiken in tekstmodus
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 0%

---

# Voorwaardelijke opmaak gebruiken in tekstmodus

<!--
(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))
-->

De standaardinterfacebouwer verstrekt een grote waaier van flexibiliteit wanneer het creëren van rapporteringselementen om aan de behoeften in uw organisatie te voldoen.

U kunt voorwaardelijke opmaak toepassen in een weergave met behulp van de standaardinterface.\
Zie voor meer informatie over het toepassen van voorwaardelijke opmaak op een weergave [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om weergaven in een rapport te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om weergaven in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Voorwaardelijke opmaak in tekstmodus

In de tekstmodus kunt u complexere weergaven, filters, groepen en aanwijzingen maken door u toe te staan velden te gebruiken die niet beschikbaar zijn in de standaardinterface.

Voor een volledige lijst van al onze te melden gebieden, zie  [API Explorer](../../../wf-api/general/api-explorer.md).

Zie voor meer informatie over het gebruik van syntaxis in de tekstmodus [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

U kunt de tekstmodus ook gebruiken om weergaven in rapporten en lijsten op te maken. Met voorwaardelijke opmaak kunt u de weergaven van uw rapporten wijzigen door het lettertype en de achtergrond van de resultaten in het rapport te wijzigen, maar ook door pictogrammen en markeringen. Wij adviseren dat u altijd uw meningen gebruikend de standaardinterface eerst bouwt en op de interface van de tekstwijze slechts wanneer absoluut noodzakelijk schakelt.

>[!NOTE]
>
> Het gebruik van CSS-stijlen voor het aanpassen van voorwaardelijke opmaak wordt niet ondersteund. In plaats daarvan moet u de vooraf ontworpen opmaakopties gebruiken die beschikbaar zijn in Adobe Workfront.

## Voorwaardelijke opmaak toevoegen aan weergaven

Zie voor meer informatie over het toepassen van voorwaardelijke opmaak op een weergave in de standaardbuilderinterface [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

Voorwaardelijke opmaak toevoegen aan een weergave in de interface van de tekstmodus:

1. Ga naar een lijst met objecten.
1. Vouw het vervolgkeuzemenu uit van een weergave waaraan u voorwaardelijke opmaak wilt toevoegen.
1. Klikken **Weergave aanpassen**.
1. Klik op de kolom in de weergave waarop u voorwaardelijke opmaak wilt toepassen.
1. Klikken **Overschakelen naar tekstmodus**.
1. In de **Tonen in deze kolom:** gebied, klikken **Klik om tekst te bewerken**.
1. Voeg de codesteekproeven toe die in worden verstrekt [Weergaven opmaken met de tekstmodus](#format-views-using-text-mode) onder aan de tekst in de kolom die u hebt geselecteerd.
1. Klikken **Opslaan** en klik vervolgens op **Weergave opslaan**.

## Weergaven opmaken met de tekstmodus {#format-views-using-text-mode}

U kunt de volgende componenten aan een kolom in een mening toevoegen om het voorwaardelijk op tekstwijze te formatteren:

* [Kolominstellingen](#column-settings)
* [Kolomregels](#column-rules)
* [Voorwaardelijk een waarde-expressie opmaken](#conditionally-format-a-valueexpression)

### Kolominstellingen {#column-settings}

Voordat u voorwaardelijke opmaak kunt toevoegen aan uw weergaven, moet u bekend zijn met de interface van de tekstmodus.

U kunt de volgende elementen van een kolom aanpassen wanneer u voorwaardelijke opmaak gebruikt in een weergave:

* [Kolomkoppen](#column-headers)
* [Datums opmaken](#format-dates)
* [Getallen opmaken](#format-numbers)

#### Kolomkoppen {#column-headers}

Als u de weergegeven kolomkop wilt wijzigen, voegt u de volgende code toe aan uw kolom: `displayname= [Name of column]`. Als u bijvoorbeeld een kolomeigenaar een naam wilt geven, ziet de tekstcode er als volgt uit:

```
displayname=Project Owner
```

#### Datums opmaken {#format-dates}

Datums kunnen worden geconfigureerd voor weergave in verschillende indelingen.

Zie voor meer informatie [Datums opmaken in tekstmodusrapporten](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat= [new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate </pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code> text mode values:</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example </th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Getallen opmaken {#format-numbers}

U kunt numerieke waarden opmaken om informatie weer te geven die het beste aansluit bij uw rapportagebehoeften.

Zie voor meer informatie [Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the <strong>valueformat</strong> line of your column.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers using the following values for the <code>valueformat</code> line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### Kolomregels {#column-rules}

Met kolomregels kunt u afbeeldingen, kleur, opmaak en tekstoverschrijvingen in een weergave toevoegen. Kolomregels kunnen onafhankelijk worden opgesteld of kunnen meerdere voorwaarden voor een kolom bevatten.

* [Voorwaardelijke opmaak](#conditional-formatting)
* [Meerdere voorwaardelijke indelingen](#multiple-conditional-formats)
* [Tekst toepassen](#apply-text)
* [Rijindelingen toepassen](#apply-row-formats)
* [Afbeeldingen toepassen](#apply-images)

#### Voorwaardelijke opmaak {#conditional-formatting}

Er moet een specifieke instructie voor de tekstmodus worden toegepast bij het opnemen van kleur- of opmaaktekst.

>[!NOTE]
>
>Voorwaardelijke opmaak wordt mogelijk niet ondersteund in samengevoegde kolommen.\
>Voor meer informatie over het samenvoegen van kolommen met de Wijze van de Tekst, zie [Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

Voeg de volgende code in een kolom in waaraan u voorwaardelijke opmaak wilt toevoegen:

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>De *styledef.case.0.compare.icon* regel is altijd false, tenzij u met pictogrammen werkt.
>
>De *styledef.case.0.compare.truetext* regel wordt altijd leeg gelaten totdat u werkt met overschrijven van tekst.
>
>De *styledef.case.0.compare.righttext* regel is leeg wanneer de kwalificatie niet leeg is.

Bijvoorbeeld, als wij de Naam van het Bedrijf in groene tekst op een projectrapport wilden tonen, kunt u de volgende code gebruiken:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* Terwijl deze verklaring op een kolom van de Naam van het Bedrijf kon worden toegepast, kon het ook op een andere kolom op het rapport worden toegepast. De groene tekst zou slechts worden getoond als het project een Bedrijf verbonden aan het had. Onthoud de `[field name]`, `[value]`, en `[qualifier]` rijden, ongeacht of de conditionering uiteindelijk op de kolom wordt weergegeven.
>* Als u werkt met kwalificatietekens, raden we u aan `cicontains` eerder dan `equal`. Standaard, `equal` zoekt naar id-nummers. Met de `cicontains` kwalificatie, kunt u tot punten door hun naam toegang hebben.

![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

Of Tekstkleur, Uitlijning, Lettertypestijl of Achtergrondkleur nu worden toegepast op een tekstmodus, dezelfde instructie (hierboven weergegeven) wordt gebruikt.

De volgende regels moeten worden aangepast aan de overeenkomstige opmaak die nodig is voor de kolom:

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

Gebruik de volgende tabellen om te bepalen welke regels moeten worden gewijzigd en welke waarden u moet opgeven om de opmaakstijl van de kolom te definiëren:

| **Tekstkleur** | **Regel: textcolor=** |
|---|---|
| Zwart | `000000` |
| Donkerblauw | `0c6aca` |
| Groenblauw | `1b878c` |
| Groen | `03a219` |
| Paars | `6408c4` |
| Grijs | `767676` |
| Rood | `d30519` |
| Geel | `e19503` |

{style="table-layout:auto"}

| **Uitlijning** | **Regel: align=** |
|---|---|
| Links uitlijnen | `left` |
| Rechts uitlijnen | `right` |
| Centreren | `center` |

{style="table-layout:auto"}

| Lettertype | Regel: ***fontstyle=*** |
|---|---|
| Vet | `bold` |
| Cursief | `italic` |

{style="table-layout:auto"}

| **Achtergrondkleur** | **Regel: bgcolor=** |
|---|---|
| Groenblauw | `dcf6f7` |
| Groen | `def6e2` |
| Grijs | `e8e8e8` |
| Blauw | `e8f1ff` |
| Paars | `e9def4` |
| Rood | `eac6c9` |
| Geel | `feecc8` |
| Wit | `ffffff` |

{style="table-layout:auto"}

#### Meerdere voorwaardelijke indelingen {#multiple-conditional-formats}

U kunt meerdere opmaakstijlen toepassen op een instructie. De kerninstructie blijft ongewijzigd en eventuele extra opmaakexpressies worden toegevoegd aan de instructie.

Bijvoorbeeld, gebruikend de vroegere verklaring om de Naam van het Bedrijf in groene boldtekst te omvatten. De instructie wordt geschreven met de volgende code:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>Wanneer u meerdere voorwaardelijke opmaakexpressies toevoegt, moet u elke expressie numeriek identificeren in de instructie. expression 0 en expression 1 zijn geïdentificeerd.

#### Tekst toepassen {#apply-text}

Als u de standaardwaarden wilt vervangen die in een kolom met een door u gekozen waarde bevolken, is het mogelijk om tekst op de kolom toe te passen.

Voor een projectrapport stelt u bijvoorbeeld de kolomwaarde Geplande begindatum in om de geplande begindatum voor het project niet weer te geven, maar de tekst &#39;Niet vandaag&#39;. Gebruik de volgende code voor de Geplande kolom van de Datum van het Begin:

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>De regels waarmee wordt begonnen `case.0.` gebruik vergelijkingen tussen hoofdletters en kleine letters om het gebruik van tekst te identificeren. De regels waarmee wordt begonnen **styledef.case.0.** zijn vroege voorwaardelijke het formatteren verklaringen waar wij het gebruik van tekst door `truetext` expressie. Zorg ervoor dat deze is ingesteld `truetext` naar een waarde, in plaats van deze leeg te laten.

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### Rijindelingen toepassen {#apply-row-formats}

Als u een voorwaarde op de volledige rij wilt toepassen, gebruik de volgende code met uw kolomcode:

```
styledef.case.0.comparison.icon=false
```

```
styledef.case.0.comparison.isrowcase=true
```

```
styledef.case.0.comparison.leftmethod= [field name]
```

```
styledef.case.0.comparison.lefttext= [field name]
```

```
styledef.case.0.comparison.operator= [qualifier]
```

```
styledef.case.0.comparison.operatortype= [data type]
```

```
styledef.case.0.comparison.righttext= [field value]
```

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
styledef.case.0.comparison.truetext=
```

```
row.0.styledef.applyallcases=true
```

```
row.0.styledef.case.0.comparison.icon=false
```

```
row.0.styledef.case.0.comparison.isrowcase=true
```

```
row.0.styledef.case.0.comparison.leftmethod= [field name]
```

```
row.0.styledef.case.0.comparison.lefttext= [field name]
```

```
row.0.styledef.case.0.comparison.operator= [qualifier]
```

```
row.0.styledef.case.0.comparison.operatortype= [data type]
```

```
row.0.styledef.case.0.comparison.righttext= [field value]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
row.0.styledef.case.0.comparison.truetext=
```


#### Afbeeldingen toepassen {#apply-images}

Net als bij het opmaken met tekst, kunnen afbeeldingen worden gebruikt om informatie in rapporten weer te geven. Workfront heeft een aantal ingebouwde beelden om visuele informatie in een rapport het plaatsen te brengen. Als u afbeeldingen wilt gebruiken in de instelling voor voorwaardelijke opmaak, is de volgende instructie nodig:

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

Bijvoorbeeld, op een projectrapport, wilt u een kolom bouwen waar u een voorproefgezicht voor elke Geplande Datum van de Voltooiing zou tonen die niet aan de datum van vandaag gelijk is. Gebruik de volgende code van de tekstwijze om het pictogram aan uw kolom toe te voegen:

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>De instructie gebruikt de instructie `icon=true` expressie. Deze instructie verschilt ook van andere instructies voor voorwaardelijke opmaak, omdat deze geen gebruik maakt van de instructie `style.def` , maar een unieke afbeeldingsindeling.

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

Als u de beschikbare afbeeldingen wilt gebruiken, past u de volgende code en waarden toe:

| **Pictogram** | **Regel: image.case.0.compare.truetext=** |
|---|---|
| Kikkervlak ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Happy Face ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| Blauwe vlag  ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| Groene vlag  ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| Rode vlag  ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| Gele vlag  ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| Zwarte cirkel  ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| Blauwe cirkel ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| Grijze cirkel ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| Groene cirkel ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| Oranje cirkel ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| Roze cirkel ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| Paarse cirkel ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| Rode cirkel ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| Witte cirkel ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| Gele cirkel ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style="table-layout:auto"}

### Maak een `valueexpression` {#conditionally-format-a-valueexpression}

Als u een berekende waarde in een kolom wilt weergeven, kunt u de optie `valuefield` coderegel in de kolom met een `valueexpression`. Met een berekende waarde kunt u een nieuwe waarde voor een object weergeven op basis van de berekening tussen twee bestaande velden op hetzelfde object.

Voor meer informatie over het opmaken van de `valueexpression line`, zie [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

U kunt een kolom die een `valueexpression` coderegel. In plaats daarvan kunt u een berekend aangepast veld toevoegen aan een aangepast formulier en dit koppelen aan de objecten die u in het rapport weergeeft. Vervolgens kunt u de kolommen waarin dit veld wordt weergegeven voorwaardelijk opmaken.

Voor meer informatie over Berekende Gebieden van de Douane, zie [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Een aggregatorwaarde toevoegen aan een tekstmoduskolom

Wij adviseren dat u de kolom in de bouwerinterface eerst bouwt, daar de aggregatorwaarde toevoegt, en dan de kolom in de Wijze van de Tekst uitgeeft.

Houd rekening met het volgende wanneer u aggregators toevoegt aan een kolom in de Tekstmodus:

* De waarden in de kolom moeten een indeling hebben die kan worden samengevat. Ze moeten bijvoorbeeld een van de volgende indelingen hebben:

   * Getal
   * Datum
   * Valuta

* U kunt een aggregator aan een kolom toevoegen die een berekening toont. De samengevoegde waarde wordt weergegeven in de groep van de weergave of het rapport. Zie voor meer informatie [Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* De coderegels voor de definitie van de kolom moeten identiek zijn aan de coderegels die de aggregator introduceren en worden voorafgegaan door &quot;aggregator&quot;. Als u bijvoorbeeld een kolom hebt waarin u de geplande uren voor een project weergeeft, is de tekstmodus van de hoofdlijnen van de kolom:

  ```
  valuefield=workRequired
  valueformat=compound
  ```

  Wanneer u de waarde van alle regels in de groepering van de mening wilt samenvoegen, kunnen wij de volgende code toevoegen om de aggregatorwaarden toe te voegen: `aggregator.valuefield=workRequired` (de `aggregator.valuefield` regel moet gelijk zijn aan `valuefield` die de kolom beschrijft) `aggregator.valueformat=compound` (de `aggregator.valueformat` regel moet dezelfde waarde hebben als de regel `valueformat` die de kolom beschrijft) `aggregator.function=SUM` (Dit is een verplichte regel die aangeeft hoe u de kolom wilt samenvoegen. In dit geval wilt u alle individuele geplande uren toevoegen aan één getal in de groeperingsregel.) `aggregator.displayformat=minutesAsHoursString` (omdat de uren in Workfront in minuten worden opgeslagen, willen wij wijzen op `displayformat` voor uren dat ze in minuten worden opgeslagen)
