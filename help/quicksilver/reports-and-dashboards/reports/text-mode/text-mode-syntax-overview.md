---
product-area: reporting
navigation-topic: text-mode-reporting
title: Overzicht van syntaxis in tekstmodus
description: U kunt de interface van de tekstwijze gebruiken om complexere meningen, filters, groeperingen, en aangepaste herinneringen in lijsten en rapporten tot stand te brengen. Met de tekstmodus hebt u toegang tot velden en de bijbehorende kenmerken die niet beschikbaar zijn in de standaardmodus.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 6279106f56fa0d128e0dd03cd13b63a71d4c2952
workflow-type: tm+mt
source-wordcount: '1865'
ht-degree: 0%

---

# Overzicht van syntaxis in tekstmodus

U kunt de interface van de tekstwijze gebruiken om complexere meningen, filters, groeperingen, en aangepaste herinneringen in lijsten en rapporten tot stand te brengen. Met de tekstmodus hebt u toegang tot velden en de bijbehorende kenmerken die niet beschikbaar zijn in de standaardmodus.

Voor informatie en overwegingen over tekstwijze alvorens u begint, zie [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Voor een volledige lijst van al onze te rapporteren gebieden en hun attributen, zie [API Explorer](../../../wf-api/general/api-explorer.md).

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

  **Voorbeeld:** U kunt de naam of GUID van de Eigenaar van het Portfolio in een taakmening tonen:


  `valuefield=project:portfolio:ownerID`

  U kunt niet groeperen, filteren of vragen voor de Eigenaar van het Portfolio in een taakmening:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  In deze voorbeelden bevindt de Portfolio-eigenaar-id zich op drie objecten afstand van het object in de lijst.

  Zie voor meer informatie over de hiërarchie van objecten in Workfront:

   * [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
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

**Voorbeeld:** Als u wilt verwijzen naar de datum van daadwerkelijke voltooiing van een project, is de naam van het veld dat u zou gebruiken bij het samenstellen van de tekstmodus die elementen rapporteert,

`actualCompletionDate`

## Syntaxis van de tekstmodus voor verschillende rapportelementen

De volgende overeenkomsten bestaan tussen de syntaxis van de hieronder vermelde sets met rapporteringselementen wanneer u deze maakt met de tekstmodus:

* De regels code en syntaxis zijn vergelijkbaar voor weergaven en groepen.

  Voor informatie over de belangrijkste lijnen van codes voor meningen en groeperingen wanneer het bouwen van hen op tekstwijze, zie:

   * [Een weergave bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Tekstmodus in een groep bewerken](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* De regels van code en syntaxis zijn gelijkaardig voor filters en douaneherinneringen.

  Zie voor meer informatie:

   * [Een filter bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntaxis voor weergaven en groepen

De coderegels bij het samenstellen van weergaven en groepen zijn vergelijkbaar.

Raadpleeg de volgende artikelen voor informatie over het maken van weergaven en groepen:

* [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

De belangrijkste coderegel voor een weergave of groep is de regel die het object aangeeft waarnaar wordt verwezen in de kolom van de weergave of in de groep. Deze coderegel kan beginnen met `valuefield` of `valueexpression` op basis van of dit veld een directe verwijzing naar een Workfront-databaseveld of een berekening tussen verschillende velden is.

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
>  Zie voor informatie over het delen van kolommen [Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` syntaxisoverzicht voor weergaven en groepen

`Valuefield=` is een belangrijke coderegel in weergaven en groepen die het object aangeeft waarnaar u rechtstreeks verwijst.

De syntaxis voor velden die rechtstreeks naar velden verwijzen, is identiek voor groepen en weergaven.

De volgende regels zijn van toepassing wanneer wordt verwezen naar Workfront-objecten die een `valuefield` regel:

* Gebruik kameel-hoofdlettergebruik om rechtstreeks naar velden te verwijzen.

  **Voorbeeld:** Als u in een taakweergave wilt verwijzen naar de datum van feitelijke voltooiing van de taak, gebruikt u de volgende regel:

  `valuefield=actualCompletionDate`

* Gebruik kameelhoofdletters en dubbele punten om aan elkaar verwante velden voor hetzelfde object te scheiden.

  **Voorbeeld:** Als u in een taakweergave wilt verwijzen naar de geplande projectuitvoeringsdatum, gebruikt u de volgende regel:

  `valuefield=project:plannedCompletionDate`

  Voor informatie over hoe objecten naar elkaar verwijzen in de Workfront-database raadpleegt u de [API Explorer](../../../wf-api/general/api-explorer.md).

* Wanneer u naar een aangepast veld verwijst, gebruikt u de naam van het veld exact zoals deze in de interface wordt weergegeven.

  **Voorbeeld:** Om een gebied van de projectdouane van verwijzingen te voorzien geëtiketteerd Extra Details in een taakmening, gebruik de volgende lijn:

  `valuefield=project:Additional Details`

#### `Valueexpression` syntaxisoverzicht voor weergaven en groepen

U kunt de opdracht `valuefield=` regel met code `valueexpression=` wanneer u weergaven en groepen maakt in de tekstmodus wanneer u wilt verwijzen naar een berekening tussen twee of meer velden.

>[!TIP]
>
>Hoewel u berekende velden kunt maken die u in rapporten kunt weergeven, zijn berekende weergaven en groeperingen dynamischer. De berekende meningen en de groeperingen verfrissen zich met nieuwe informatie telkens als u het rapport in werking stelt of een lijst toont.
>
>Zie voor informatie over het maken van berekende kolommen in een weergave [Berekende aangepaste velden versus berekende kolommen](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Het bouwen van een berekende groepering is gelijkaardig aan het bouwen van een berekende kolom in een mening.

De volgende regels zijn van toepassing wanneer wordt verwezen naar Workfront-objecten die een `valueexpression` regel:

* Gebruik kameel-hoofdlettergebruik om rechtstreeks naar velden te verwijzen en sluit elk veld tussen accolades.

  **Voorbeeld:** Om het gebied van de Naam van de Taak in een taakkolom te tonen die `valueexpression`gebruikt u de volgende regel:

  `valueexpression={name}`


* Gebruik kameelhoofdletters en -punten om velden die aan elkaar zijn gerelateerd, van elkaar te scheiden.

  **Voorbeeld:** Om de naam van een project te tonen dat met de naam van de taak in een taakrapport wordt aaneengeschakeld, gebruik de volgende lijnen:

   * In een weergave:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * In een groep:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Voor informatie over hoe objecten naar elkaar verwijzen in de Workfront-database raadpleegt u de [API Explorer](../../../wf-api/general/api-explorer.md).

* Gebruik de volgende regels wanneer u naar een aangepast veld verwijst:

   * Gebruik de naam van het veld exact zoals deze wordt weergegeven in de interface.
   * Plaats voor de naam van het veld de tekst &quot;DE:&quot;.
   * Plaats het veld tussen accolades.
   * Scheid de velden die betrekking hebben op het object met punten.

  **Voorbeeld:** Om het Extra het projectdouaneveld van Details in een taakmening in een lijn van de waardeuitdrukking te tonen, gebruik de volgende lijn:

  `valueexpression={project}.{DE:Additional Details}`

* U kunt jokertekens gebruiken in een `valueexpression` maar niet in een `valuefield` lijn.

  Voor informatie over vervangingen, zie [Overzicht van jokertekenfiltervariabelen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` overzicht voor weergaven en groepen

De tweede belangrijkste coderegel in een weergave of groep is de `valueformat=` lijn. Dit vertelt Workfront in welke notatie de waarde die u opgeeft in het dialoogvenster `valuefield` of `valueexpression` lijnen. Hoewel u verschillende indelingen kunt gebruiken voor de `valueformat` lijnen, adviseren wij altijd de volgende waarde te gebruiken wanneer het gebruiken `valueexpression`:

`valueformat=HTML`

Voor extra `valueformat` waarden, zie ook de volgende artikelen:

* [Datums opmaken in tekstmodusrapporten](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` overzicht voor weergaven

`width=` Dit is de coderegel waarin u de breedte van elke kolom in pixels kunt opgeven. Workfront biedt een aanbevolen breedte voor elk veld, maar afhankelijk van het type veld en de indeling kunt u de breedte aanpassen.

U moet de extra `usewidths=true` coderegel om de voor de kolom opgegeven breedte af te dwingen.

**Voorbeeld:** Gebruik de volgende regels om een kolom met een breedte van 80 pixels weer te geven:

`width=80`

`usewidths=true`

#### `stretch` overzicht voor weergaven

De `stretch` wordt gebruikt om aan te geven welke kolommen extra ruimte innemen die niet nodig is voor de weergave. De breedte van de gebruikersinterface van de werkruimte voor een standaardgebruiker is ongeveer 850 pixels. Dit betekent dat als u een weergave hebt met vier kolommen (elk 150 pixels), uw weergave 600 van 850 pixels in beslag neemt. Er zijn 250 extra pixel in UI die aan de kolommen zullen worden toegevoegd die een rekbaarheidspercentage hebben verstrekt.

Het uitrekken van een kolom wordt afgedwongen wanneer u de extra coderegel gebruikt: `usewidths=true` voor ten minste een van de kolommen in de weergave.

**Voorbeeld:** Als u wilt aangeven dat een kolom 70% van de lege ruimte in een weergave kan gebruiken, gebruikt u de volgende regels:

`stretch=70`

`usewidths=true`

### Syntaxis voor filters en aangepaste aanwijzingen

De syntaxis voor het maken van filters lijkt op die voor het maken van aangepaste aanwijzingen.

>[!TIP]
>
>U kunt een douaneherinnering tot stand brengen door een filter voor de verklaring eerst te bouwen u in de herinnering wilt omvatten. Sluit alle coderegels in een filter aan op &quot;&amp;&quot; zonder spaties tussen de regels en dat wordt de aangepaste aanwijzing.

Voor informatie over het bouwen van filters en douaneherinneringen, zie:

* [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Zie voor informatie over het maken van filters in de tekstmodus [Een filter bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

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

* Jokertekens om filters dynamischer te maken en ze aan te passen voor de huidige tijd of de gebruiker die is aangemeld. Voor informatie over vervangingen, zie [Overzicht van jokertekenfiltervariabelen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
