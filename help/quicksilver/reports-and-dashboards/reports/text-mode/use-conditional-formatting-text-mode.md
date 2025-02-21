---
product-area: reporting
navigation-topic: text-mode-reporting
title: Voorwaardelijke opmaak gebruiken in tekstmodus
description: Voorwaardelijke opmaak gebruiken in tekstmodus
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 0%

---

# Voorwaardelijke opmaak gebruiken in tekstmodus

<!--Audited: 01/2025-->

De standaardinterfacebouwer verstrekt een grote waaier van flexibiliteit wanneer het creëren van rapporteringselementen om aan de behoeften in uw organisatie te voldoen.

U kunt voorwaardelijke opmaak toepassen in een weergave met behulp van de standaardinterface.\
Voor meer informatie over het toepassen van voorwaardelijke het formatteren op een mening, zie [ Voorwaardelijk het gebruiken formatterend in meningen ](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om weergaven in een rapport te bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om weergaven in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voorwaardelijke opmaak in tekstmodus

In de tekstmodus kunt u complexere weergaven, filters, groepen en aanwijzingen maken door u toe te staan velden te gebruiken die niet beschikbaar zijn in de standaardinterface.

Voor een volledige lijst van al onze te melden gebieden, zie [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md).

Voor meer informatie over het gebruiken van de syntaxis van de tekstwijze, zie [ overzicht van de wijzesyntaxis van de Tekst ](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

U kunt de tekstmodus ook gebruiken om weergaven in rapporten en lijsten op te maken. Met voorwaardelijke opmaak kunt u de weergaven van uw rapporten wijzigen door het lettertype en de achtergrond van de resultaten in het rapport te wijzigen, maar ook door pictogrammen en vlaggen. Wij adviseren dat u altijd uw meningen gebruikend de standaardinterface eerst bouwt en op de interface van de tekstwijze slechts wanneer absoluut noodzakelijk schakelt.

>[!NOTE]
>
> Het gebruik van CSS-stijlen voor het aanpassen van voorwaardelijke opmaak wordt niet ondersteund. In plaats daarvan moet u de vooraf ontworpen opmaakopties gebruiken die beschikbaar zijn in Adobe Workfront.

## Voorwaardelijke opmaak toevoegen aan weergaven

Voor meer informatie over het toepassen van voorwaardelijke het formatteren op een mening in de standaard bouwerinterface, zie [ Voorwaardelijk het Gebruik formatteren in meningen ](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

Voorwaardelijke opmaak toevoegen aan een weergave in de interface van de tekstmodus:

1. Ga naar een lijst met objecten.
1. Vouw het vervolgkeuzemenu uit van een weergave waaraan u voorwaardelijke opmaak wilt toevoegen.
1. Klik **aanpassen Mening**.
1. Klik op de kolom in de weergave waarop u voorwaardelijke opmaak wilt toepassen.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. In **toon in deze kolom:** gebied, klik **om tekst** uit te geven.
1. Voeg de codesteekproeven toe die in [ de Mening van het Formaat worden verstrekt gebruikend de Wijze van de Tekst ](#format-views-using-text-mode) bij de bodem van de tekst in de kolom u selecteerde.
1. Klik **sparen**, dan klik **sparen Mening**.

## Weergaven opmaken met de tekstmodus {#format-views-using-text-mode}

U kunt de volgende componenten aan een kolom in een mening toevoegen om het voorwaardelijk op tekstwijze te formatteren:

* [ montages van de Kolom ](#column-settings)
* [ de regels van de Kolom ](#column-rules)
* [Voorwaardelijk een waarde-expressie opmaken](#conditionally-format-a-valueexpression)

### Kolominstellingen {#column-settings}

Voordat u voorwaardelijke opmaak kunt toevoegen aan uw weergaven, moet u bekend zijn met de interface van de tekstmodus.

U kunt de volgende elementen van een kolom aanpassen wanneer u voorwaardelijke opmaak gebruikt in een weergave:

* [ Kopballen van de Kolom ](#column-headers)
* [ data van het Formaat ](#format-dates)
* [Getallen opmaken](#format-numbers)

#### Kolomkoppen {#column-headers}

Als u de weergegeven kolomkop wilt wijzigen, voegt u de volgende code toe aan de kolom: `displayname= [Name of column]` . Als u bijvoorbeeld een kolomeigenaar een naam wilt geven, ziet de tekstcode er als volgt uit:

`displayname=Project Owner`

#### Datums opmaken {#format-dates}

Datums kunnen worden geconfigureerd voor weergave in verschillende indelingen.

Voor meer informatie, zie [ data van het Formaat op de rapporten van de tekstwijze ](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

#### Getallen opmaken {#format-numbers}

U kunt numerieke waarden opmaken om informatie weer te geven die het beste aansluit bij uw rapportagebehoeften.

Voor meer informatie, zie {de aantallen van 0} Formaat, munt en percentagewaarden op de rapporten van de tekstwijze ](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).[

### Kolomregels {#column-rules}

Met kolomregels kunt u afbeeldingen, kleur, opmaak en tekstoverschrijvingen in een weergave toevoegen. Kolomregels kunnen onafhankelijk worden opgesteld of kunnen meerdere voorwaarden voor een kolom bevatten.

* [ Voorwaardelijke het formatteren ](#conditional-formatting)
* [ Veelvoudige voorwaardelijke formaten ](#multiple-conditional-formats)
* [ pas tekst ](#apply-text) toe
* [ pas rijformaten ](#apply-row-formats) toe
* [Afbeeldingen toepassen](#apply-images)

#### Voorwaardelijke opmaak {#conditional-formatting}

Er moet een specifieke instructie voor de tekstmodus worden toegepast bij het opnemen van kleur- of opmaaktekst.

>[!NOTE]
>
>Voorwaardelijke opmaak wordt mogelijk niet ondersteund in samengevoegde kolommen.\
>Voor meer informatie bij het samenvoegen van kolommen met de Wijze van de Tekst, zie [ Mening: fusie informatie van veelvoudige kolommen in één gedeelde kolom ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

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
>De regel `styledef.case.0.comparison.icon` is altijd false, tenzij u met pictogrammen werkt.
>
>De regel `styledef.case.0.comparison.truetext` wordt altijd leeg gelaten totdat u werkt met het overschrijven van tekst.
>
>De regel `styledef.case.0.comparison.righttext` is leeg wanneer de kwalificatie niet leeg is.

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
>* Terwijl deze verklaring op een kolom van de Naam van het Bedrijf kon worden toegepast, kon het ook op een andere kolom op het rapport worden toegepast. De groene tekst zou slechts worden getoond als het project een Bedrijf verbonden aan het had. Onthoud het station `[field name]` , `[value]` en `[qualifier]` , ongeacht of de conditionering uiteindelijk op de kolom wordt weergegeven.
>* Als u met kwalificatietoetsen werkt, raden we u aan `cicontains` te gebruiken in plaats van `equal` . Standaard zoekt `equal` naar id-nummers. Met de kwalificatie `cicontains` hebt u toegang tot items op basis van hun naam.

![ de wijzevoorbeeld van de Tekst ](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png){width="500"}


![ resultaten van het de wijzevoorbeeld van de Tekst ](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png){width="400"}

Of Tekstkleur, Uitlijning, Lettertypestijl of Achtergrondkleur nu worden toegepast op een tekstmodus, dezelfde instructie (hierboven weergegeven) wordt gebruikt.

De volgende regels moeten worden aangepast aan de overeenkomstige opmaak die nodig is voor de kolom:

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

Gebruik de volgende tabellen om te bepalen welke regels moeten worden gewijzigd en welke waarden u moet opgeven om de opmaakstijl van de kolom te definiëren:

| **Kleur van de Tekst** | **Lijn: textcolor=** |
|---|---|
| Zwart | `000000` |
| Donkerblauw | `0c6aca` |
| Groen | `1b878c` |
| Groen | `03a219` |
| Paars | `6408c4` |
| Grijs | `767676` |
| Rood | `d30519` |
| Geel | `e19503` |

{style="table-layout:auto"}

| **Uitlijning** | **Lijn: align=** |
|---|---|
| Links uitlijnen | `left` |
| Rechts uitlijnen | `right` |
| Centreren | `center` |

{style="table-layout:auto"}

| Lettertype | Lijn: ***fontstyle=*** |
|---|---|
| Vet | `bold` |
| Cursief | `italic` |

{style="table-layout:auto"}

| **Achtergrondkleur** | **Lijn: bgcolor=** |
|---|---|
| Groen | `dcf6f7` |
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
>De regels die beginnen met `case.0.` gebruiken hoofdlettervergelijkingen met het identificeren van het gebruik van tekst. De regels die beginnen met `styledef.case.0.` zijn vroege voorwaardelijke opmaakinstructies waarin we het gebruik van tekst identificeren via de `truetext` -expressie. Stel `truetext` in op een waarde in plaats van deze leeg te laten.

![ pas tekstvoorbeeld ](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png){width="500"} toe

![ pas tekstresultaten ](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png){width="400"} toe

#### Rijindelingen toepassen {#apply-row-formats}

Als u een voorwaarde op de volledige rij wilt toepassen, gebruik de volgende code met uw kolomcode:

```
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.isrowcase=true
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
styledef.case.0.comparison.truetext=
row.0.styledef.applyallcases=true
row.0.styledef.case.0.comparison.icon=false
row.0.styledef.case.0.comparison.isrowcase=true
row.0.styledef.case.0.comparison.leftmethod= [field name]
row.0.styledef.case.0.comparison.lefttext= [field name]
row.0.styledef.case.0.comparison.operator= [qualifier]
row.0.styledef.case.0.comparison.operatortype= [data type]
row.0.styledef.case.0.comparison.righttext= [field value]
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
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
>De instructie gebruikt de expressie `icon=true` . Deze instructie verschilt ook van andere instructies voor voorwaardelijke opmaak, omdat deze niet de `style.def` -indeling gebruikt, maar een unieke afbeeldingsindeling.

![ de tekstwijze van het Pictogram ](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png){width="500"}

![ de resultaten van de de tekstwijze van het Pictogram ](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png){width="400"}

Als u de beschikbare afbeeldingen wilt gebruiken, past u de volgende code en waarden toe:

| **Pictogram** | **Lijn: image.case.0.compare.truetext=** |
|---|---|
| Van het Gezicht van de voorzijde ![ Voorzijde ](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Fijne Gezicht ![ Fijne gezicht ](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| Blauwe vlag ![ Blauwe vlag ](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| Groene Vlag ![ Groene vlag ](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| De rode vlag van de Vlag ![ Rode vlag ](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| De gele vlag van de Vlag ![ Gele vlag ](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| De zwarte cirkel ![ Zwarte cirkel ](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| Blauwe cirkel ![ Blauwe cirkel ](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| Grijze cirkel ![ Grijze cirkel ](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| Groene Cirkel ![ Groene cirkel ](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| Oranje cirkel ![ Oranje cirkel ](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| Roze Cirkel ![ Roze cirkel ](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| Paarse Cirkel ![ Paarse cirkel ](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| Rode cirkel ![ Rode cirkel ](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| Witte cirkel ![ Witte cirkel ](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| Gele Cirkel ![ Gele cirkel ](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style="table-layout:auto"}

### Een `valueexpression` voorwaardelijk opmaken {#conditionally-format-a-valueexpression}

Als u een berekende waarde in een kolom wilt weergeven, kunt u de coderegel `valuefield` in de kolom vervangen door een `valueexpression` . Met een berekende waarde kunt u een nieuwe waarde voor een object weergeven op basis van de berekening tussen twee bestaande velden op hetzelfde object.

Voor meer informatie over hoe te om `valueexpression line` te formatteren, zie [ overzicht van de de wijzesyntaxis van de Tekst ](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

U kunt een kolom met een coderegel `valueexpression` niet voorwaardelijk opmaken. In plaats daarvan kunt u een berekend aangepast veld toevoegen aan een aangepast formulier en dit koppelen aan de objecten die u in het rapport weergeeft. Vervolgens kunt u de kolommen met dit veld voorwaardelijk opmaken.

Voor meer informatie over Berekende Gebieden van de Douane, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

## Een aggregatorwaarde toevoegen in een tekstmoduskolom

Wij adviseren dat u de kolom in de bouwerinterface eerst bouwt, daar de aggregatorwaarde toevoegt, en dan de kolom in de Wijze van de Tekst uitgeeft.

Houd rekening met het volgende wanneer u aggregators toevoegt aan een kolom in de Tekstmodus:

* De waarden in de kolom moeten een indeling hebben die kan worden samengevat. Ze moeten bijvoorbeeld een van de volgende indelingen hebben:

   * Getal
   * Datum
   * Valuta

* U kunt een aggregator aan een kolom toevoegen die een berekening toont. De samengevoegde waarde wordt weergegeven in de groep van de weergave of het rapport. Voor meer informatie, zie [ Groepering: toon het resultaat van het samenvoegen van veelvoudige berekende waarden in een groepering ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* De coderegels voor de definitie van de kolom moeten identiek zijn aan de coderegels die de aggregator introduceren en worden voorafgegaan door &quot;aggregator&quot;. Als u bijvoorbeeld een kolom hebt waarin u de geplande uren voor een project weergeeft, is de tekstmodus van de hoofdlijnen van de kolom:

```
  valuefield=workRequired
  valueformat=compound
```

Als u de waarden van alle regels in de groepering van de weergave wilt samenvoegen, kunt u de volgende code toevoegen om de aggregatorwaarden toe te voegen:

`aggregator.valuefield=workRequired` (de `aggregator.valuefield` lijn moet het zelfde zijn als `valuefield` die de kolom beschrijft)

`aggregator.valueformat=compound` (de `aggregator.valueformat` -regel moet dezelfde waarde hebben als de `valueformat` die de kolom beschrijft)

`aggregator.function=SUM` (dit is een verplichte regel die aangeeft hoe u de kolom wilt samenvoegen. In dit geval wilt u alle individuele geplande uren in één getal op de groeperingsregel plaatsen)

`aggregator.displayformat=minutesAsHoursString` (omdat uren in Workfront in minuten worden opgeslagen, willen we de `displayformat` aangeven voor uren dat ze in minuten worden opgeslagen)
