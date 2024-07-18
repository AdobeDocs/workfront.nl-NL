---
product-area: reporting
navigation-topic: text-mode-reporting
title: Overzicht van syntaxis in tekstmodus
description: U kunt de interface van de tekstwijze gebruiken om complexere meningen, filters, groeperingen, en aangepaste herinneringen in lijsten en rapporten tot stand te brengen. Met de tekstmodus hebt u toegang tot velden en de bijbehorende kenmerken die niet beschikbaar zijn in de standaardmodus.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# Overzicht van syntaxis in tekstmodus

<!--Audited: 12/2023-->

U kunt de interface van de tekstwijze gebruiken om complexere meningen, filters, groeperingen, en aangepaste herinneringen in lijsten en rapporten tot stand te brengen. Met de tekstmodus hebt u toegang tot velden en de bijbehorende kenmerken die niet beschikbaar zijn in de standaardmodus.

Voor informatie en overwegingen over tekstwijze alvorens u begint, zie [ Overzicht van de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Voor een volledige lijst van al onze te melden gebieden en hun attributen, zie de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md).

Ga naar de sectie Leren op de Adobe Experience League-site voor meer informatie over het maken van rapporten in de tekstmodus, waaronder klassen, video&#39;s en zelfstudies.

## Overwegingen bij de syntaxis van de tekstmodus

* U moet de syntaxis van Adobe Workfront begrijpen voordat u rapportelementen kunt gaan maken in de tekstmodus. De Workfront-syntaxis voor de tekstmodus is uniek voor deze toepassing en heeft unieke kenmerken waarmee u vertrouwd moet zijn.
* Voordat u de tekstmodus in uw rapporten gaat gebruiken, raden we u ten zeerste aan onze klassen voor geavanceerde rapportage te gebruiken om meer inzicht te krijgen in de taal van de tekstmodus. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* U kunt weergaven, filters en groepen aanpassen met de standaardmodusinterface. U kunt echter alleen aangepaste vragen maken met behulp van de tekstmodus.

## Gemeenschappelijke richtsnoeren voor het samenstellen van rapporteringselementen in tekstmodus

De volgende richtlijnen gelden voor het samenstellen van rapporten of lijstelementen in de tekstmodus:

* Gebruik altijd kameel-hoofdlettergebruik wanneer u verwijst naar objecten of kenmerken in de Workfront-database.
* Houd rekening met de objecthiërarchie in Workfront. De volgende verschillen bestaan tussen weergaven, filters en groepen:

   * U kunt een object weergeven dat zich drie objecten buiten het rapport- of lijstobject in een weergave bevindt.
   * U kunt niet verwijzen naar objecten die zich meer dan twee objecten buiten het hoofdobject bevinden in een groep, filter of aangepaste vraag.

  **Voorbeeld:** u kunt de naam of GUID van de Eigenaar van het Portfolio in een taakmening tonen:


  `valuefield=project:portfolio:ownerID`

  U kunt niet groeperen, filteren of vragen voor de Eigenaar van het Portfolio in een taakmening:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  In deze voorbeelden bevindt de Portfolio-eigenaar-id zich op drie objecten afstand van het object in de lijst.

  Zie voor meer informatie over de hiërarchie van objecten in Workfront:

   * [ Begrijp voorwerpen in Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)

* Gebruik zoveel mogelijk jokertekens om uw rapporten en lijsten dynamischer te maken en om te voorkomen dat deze voor verschillende gebruikers en vergelijkbare tijdlijnen worden gedupliceerd.

## Camel case-overzicht

Als u in de tekstmodus naar Workfront-velden of de bijbehorende kenmerken verwijst, moet u in Workfront de namen van die velden invoeren in camelgevallen. In dit geval worden de velden met één naam in kleine letters gespeld. Samengestelde velden worden gespeld volgens het volgende patroon:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Alle rapportelementen volgen dit casingpatroon.

De kenmerken van kamelendoosjes zijn:

* Het eerste woord begint altijd met een kleine letter.
* De volgende woorden beginnen altijd met een hoofdletter.
* Er zijn geen spaties tussen de woorden.

**Voorbeeld:** om de Ware Datum van de Voltooiing van een project van verwijzingen te voorzien, de naam van het gebied dat u zou gebruiken wanneer het bouwen van tekstwijze het melden van elementen is

`actualCompletionDate`

## Syntaxis van de tekstmodus voor verschillende rapportelementen

De volgende overeenkomsten bestaan tussen de syntaxis van de hieronder vermelde sets met rapporteringselementen wanneer u deze maakt met de tekstmodus:

* De regels code en syntaxis zijn vergelijkbaar voor weergaven en groepen.

  Voor informatie over de belangrijkste lijnen van codes voor meningen en groeperingen wanneer het bouwen van hen op tekstwijze, zie:

   * [ geef een mening uit gebruikend tekstwijze ](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Tekstmodus in een groep bewerken](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* De regels van code en syntaxis zijn gelijkaardig voor filters en douaneherinneringen.

  Zie voor meer informatie:

   * [ geef een filter uit gebruikend tekstwijze ](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntaxis voor weergaven en groepen

De coderegels bij het samenstellen van weergaven en groepen zijn vergelijkbaar.

Raadpleeg de volgende artikelen voor informatie over het maken van weergaven en groepen:

* [ Overzicht van meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

De belangrijkste coderegel voor een weergave of groep is de regel die het object aangeeft waarnaar wordt verwezen in de kolom van de weergave of in de groep. Deze coderegel kan beginnen met `valuefield` of `valueexpression` op basis van het feit of dit veld een directe verwijzing naar een Workfront-databaseveld of een berekening tussen verschillende velden is.

De volgende tabel bevat een lijst met de meestvoorkomende regels voor codes in een weergave of groep:

| Codelijn | Beschrijving |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Hiermee wordt het object aangegeven waarnaar wordt verwezen in de kolom van de weergave of de groepering. Dit is een directe verwijzing naar het object waarnaar wordt verwezen. |
| `valueexpression` | Hiermee wordt het object aangegeven waarnaar wordt verwezen in de kolom van de weergave of de groepering. Dit is een berekening tussen verschillende velden. |
| `valueformat` | Identificeert de indeling waarin Workfront de waarde retourneert die is opgegeven in het veld value of value expression regels. |
| `width` | Hiermee wordt de breedte van een kolom in pixels aangegeven. |
| `stretch` | Hiermee wordt aangegeven welke kolommen extra ruimte innemen die niet nodig is voor de weergave. |

>[!TIP]
>
>* Hoewel de coderegels in de onderstaande voorbeelden vergelijkbaar zijn tussen weergaven en groepen, moet u er altijd rekening mee houden dat elke coderegel voor een groepering begint met het groeperingsnummer.
>
>  Om door de Naam van het Project in een projectlijst of een rapport te groeperen, gebruik de volgende lijn voor de eerste rij groeperen:
>
>  `group.0.valuefield=name`
>  
>* Als u meerdere kolommen bewerkt in een weergave in dezelfde kolom (zoals het geval is bij gedeelde kolommen), moet u niet vergeten dat elke coderegel voor elke kolom begint met het kolomnummer.
>
>  Gebruik de volgende indeling om de eerste kolom van een weergave te identificeren:
>
>  `column.0.valuefield=name`
>  
>  Voor informatie over het delen van kolommen, zie [ Mening: voeg informatie van veelvoudige kolommen in één gedeelde kolom ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md) samen.
>

#### `Valuefield` syntaxisoverzicht voor weergaven en groepen

`Valuefield=` is een belangrijke coderegel in weergaven en groepen die het object identificeert waarnaar u rechtstreeks verwijst.

De syntaxis voor velden die rechtstreeks naar velden verwijzen, is identiek voor groepen en weergaven.

De volgende regels zijn van toepassing wanneer wordt verwezen naar Workfront-objecten die een `valuefield` -regel gebruiken:

* Gebruik kameel-hoofdlettergebruik om rechtstreeks naar velden te verwijzen.

  **Voorbeeld:** om de Werkelijke Datum van de Voltooiing van de Taak in een taakmening van verwijzingen te voorzien, gebruik de volgende lijn:

  `valuefield=actualCompletionDate`

* Gebruik kameelhoofdletters en dubbele punten om aan elkaar verwante velden voor hetzelfde object te scheiden.

  **Voorbeeld:** om het Project Geplande Datum van de Voltooiing in een taakmening van verwijzingen te voorzien, gebruik de volgende lijn:

  `valuefield=project:plannedCompletionDate`

  Voor informatie over hoe de voorwerpen naar elkaar in het gegevensbestand van Workfront van verwijzingen voorzien, zie de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md).

* Wanneer u naar een aangepast veld verwijst, gebruikt u de naam van het veld exact zoals deze in de interface wordt weergegeven.

  **Voorbeeld:** om een gebied van de projectdouane van verwijzingen te voorzien geëtiketteerd Extra Details in een taakmening, gebruik de volgende lijn:

  `valuefield=project:Additional Details`

#### `Valueexpression` syntaxisoverzicht voor weergaven en groepen

U kunt de coderegel `valuefield=` vervangen door `valueexpression=` bij het samenstellen van weergaven en groepen in de tekstmodus als u wilt verwijzen naar een berekening tussen twee of meer velden.

>[!TIP]
>
>Hoewel u berekende velden kunt maken die u in rapporten kunt weergeven, zijn berekende weergaven en groeperingen dynamischer. De berekende meningen en de groeperingen verfrissen zich met nieuwe informatie telkens als u het rapport in werking stelt of een lijst toont.
>
>Voor informatie over het creëren van berekende kolommen in een mening, zie [ Berekende douanegebieden vs. berekende kolommen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Het bouwen van een berekende groepering is gelijkaardig aan het bouwen van een berekende kolom in een mening.

De volgende regels zijn van toepassing wanneer wordt verwezen naar Workfront-objecten die een `valueexpression` -regel gebruiken:

* Gebruik kameel-hoofdlettergebruik om rechtstreeks naar velden te verwijzen en sluit elk veld tussen accolades.

  **Voorbeeld:** om het gebied van de Naam van de Taak in een taakkolom te tonen gebruikend `valueexpression`, gebruik de volgende lijn:

  `valueexpression={name}`


* Gebruik kameelhoofdletters en -punten om velden die aan elkaar zijn gerelateerd, van elkaar te scheiden.

  **Voorbeeld:** om de naam van een project te tonen dat met de naam van de taak in een taakrapport wordt samengevoegd, gebruik de volgende lijnen:

   * In een weergave:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * In een groep:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Voor informatie over hoe de voorwerpen naar elkaar in het gegevensbestand van Workfront van verwijzingen voorzien, zie de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md).

* Gebruik de volgende regels wanneer u naar een aangepast veld verwijst:

   * Gebruik de naam van het veld exact zoals deze wordt weergegeven in de interface.
   * Plaats voor de naam van het veld de tekst &quot;DE:&quot;.
   * Plaats het veld tussen accolades.
   * Scheid de velden die betrekking hebben op het object met punten.

  **Voorbeeld:** om het Extra gebied van de het projectdouane van Details in een taakmening in een lijn van de waardeuitdrukking te tonen, gebruik de volgende lijn:

  `valueexpression={project}.{DE:Additional Details}`

* U kunt een jokerteken gebruiken in een `valueexpression` maar niet in een `valuefield` -regel.

  Voor informatie over vervangingen, zie [ overzicht van de de filtervariabelen van de Vervanging ](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` overzicht voor weergaven en groepen

De tweede belangrijkste coderegel in een weergave of groep is de regel `valueformat=` . Dit vertelt Workfront in welke notatie de waarde moet worden geretourneerd die u opgeeft in de `valuefield` - of `valueexpression` -regels. Hoewel u verschillende indelingen kunt gebruiken voor de `valueformat` -regels, raden we u aan altijd de volgende waarde te gebruiken wanneer u `valueexpression` gebruikt:

`valueformat=HTML`

Zie ook de volgende artikelen voor aanvullende `valueformat` -waarden:

* [Datums opmaken in tekstmodusrapporten](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` overzicht voor weergaven

`width=` is de coderegel waarin u de breedte van elke kolom in pixels kunt opgeven. Workfront biedt een aanbevolen breedte voor elk veld, maar afhankelijk van het type veld en de indeling kunt u de breedte aanpassen.

U moet de extra `usewidths=true` coderegel gebruiken om de voor de kolom opgegeven breedte in te stellen.

**Voorbeeld:** om een kolom met een breedte van 80 pixel te tonen, gebruik de volgende lijnen:

`width=80`

`usewidths=true`

#### `stretch` overzicht voor weergaven

`stretch` wordt gebruikt om te identificeren welke kolommen extra ruimte innemen die niet nodig is voor de weergave. De breedte van de gebruikersinterface van de werkruimte voor een standaardgebruiker is ongeveer 850 pixels. Dit betekent dat als u een weergave hebt met vier kolommen (elk 150 pixels), uw weergave 600 van 850 pixels in beslag neemt. Er zijn 250 extra pixel in UI die aan de kolommen zullen worden toegevoegd die een rekbaarheidspercentage hebben verstrekt.

Het uitrekken van een kolom wordt afgedwongen wanneer u de extra coderegel: `usewidths=true` gebruikt voor ten minste een van de kolommen in de weergave.

**Voorbeeld:** om erop te wijzen dat een kolom 70% van de lege ruimte in een mening kon gebruiken, gebruik de volgende lijnen:

`stretch=70`

`usewidths=true`

### Syntaxis voor filters en aangepaste aanwijzingen

De syntaxis voor het maken van filters lijkt op die voor het maken van aangepaste aanwijzingen.

>[!TIP]
>
>U kunt een douaneherinnering tot stand brengen door een filter voor de verklaring eerst te bouwen u in de herinnering wilt omvatten. Sluit alle coderegels in een filter aan op &quot;&amp;&quot; zonder spaties tussen de regels en dat wordt de aangepaste aanwijzing.

Voor informatie over het bouwen van filters en douaneherinneringen, zie:

* [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Voor informatie over het creëren van filters op tekstwijze, zie [ een filter uitgeven gebruikend tekstwijze ](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

U kunt de volgende elementen gebruiken om filters en aangepaste herinneringen op tekstwijze te bouwen:

* Een coderegel die naar het object van de filterinstructie verwijst. Gebruik een kameelhoofdletter voor het filterobject.
* Een coderegel die verwijst naar het filterobject en de modifier voor de waarde van het filterobject. Gebruik kameel-hoofdlettergebruik voor het filterobject op deze regel.

  >[!TIP]
  >
  >Wanneer het van verwijzingen voorzien van waaiers, vereist dit 2 bepalingslijnen.

* Een instructieconnector die meerdere filterinstructies verbindt:

   * EN

     Dit is de standaardaansluiting tussen filterinstructies.

   * OF

     >[!TIP]
     >
     >De schakelaars van de verklaring zijn case sensitive en altijd in hoofdletters. &quot;AND&quot; kan worden weggelaten in de tekstmodus.

* Jokertekens om filters dynamischer te maken en ze aan te passen voor de huidige tijd of de gebruiker die is aangemeld. Voor informatie over vervangingen, zie [ overzicht van de de filtervariabelen van de Vervanging ](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
