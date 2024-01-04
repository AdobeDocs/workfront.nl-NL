---
product-area: reporting
navigation-topic: text-mode-reporting
title: Complexe tekstmodusfilters maken met EXISTS-instructies
description: Complexe tekstmodusfilters maken met EXISTS-instructies
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2766'
ht-degree: 0%

---

# Complexe tekstmodusfilters maken met EXISTS-instructies

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Dit artikel vereist een grondig inzicht in de Adobe Workfront API en de rapportinterface voor de tekstmodus. Zie voor informatie over de Workfront API [Basisbeginselen van API](../../../wf-api/general/api-basics.md).\
>Zie voor informatie over het gebruik van de tekstmodus [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Overzicht van objectrelaties in Workfront

Alle objecten zijn gekoppeld aan andere objecten in de Workfront-database.

Als u de hiërarchie en de onderlinge afhankelijkheid van objecten begrijpt, kunt u beter achterhalen naar welke objecten in rapporten kan worden verwezen.

Zie voor informatie over welke objecten zich in Workfront bevinden en over hun hiërarchie en onderlinge afhankelijkheid [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Wanneer u filters maakt, kunt u naar andere objecten verwijzen die met het object van het filter zijn verbonden binnen maximaal twee relatieniveaus met behulp van de standaardrapportinterface.

U kunt bijvoorbeeld naar de Portfolio-id in een emissiefilter verwijzen om alleen problemen weer te geven voor projecten die zijn gekoppeld aan een bepaald portfolio met behulp van de standaardinterface. In dit geval is de portfolio 2 niveaus verwijderd van emissies.

U kunt echter niet verwijzen naar de eigenaar van het Portfolio in een emissiefilter met de standaardinterface om alleen problemen weer te geven van projecten die zijn gekoppeld aan portfolio&#39;s waarbij de eigenaar een specifieke gebruiker is. U moet de tekstmodus gebruiken om toegang te krijgen tot het veld Naam eigenaar Portfolio, dat drie niveaus verwijderd is van problemen.

![issue_to_portfolio_owner_sraight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Voor een volledige lijst met objecten in Workfront raadpleegt u de [API Explorer](../../../wf-api/general/api-explorer.md).

Voor informatie over hoe u door de API Explorer kunt navigeren en objecten kunt zoeken, raadpleegt u [De API Explorer gebruiken](../../../wf-api/general/using-api-explorer.md).

Wanneer u filters maakt, moet u complexe instructies maken in de interface voor tekstmodus om naar deze typen objecten te verwijzen.

Voor informatie over het bouwen van complexe filters, zie [Overzicht van complexe tekstmodusfilters die bestaande instructies gebruiken](#overview-of-complex-text-mode-filters-that-use-exists-statements) sectie.

## Overzicht van complexe tekstmodusfilters die EXISTS-instructies gebruiken {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Houd rekening met het volgende wanneer u filters maakt die meerdere niveaus in de objecthiërarchie of het filter beslaan voor ontbrekende objecten:

* U moet complexe filters maken wanneer u wilt verwijzen naar objecten die niet rechtstreeks met het filterobject zijn verbonden.
* U moet een EXISTS verklaring gebruiken om het volgende te doen:

   * Maak filters die meerdere niveaus omspannen.
   * Maak filters die zoeken naar objecten die ontbreken.\
     Bijvoorbeeld, wanneer het bouwen van een gebruikersrapport, kunt u voor gebruikers filtreren die geen tijd voor een bepaalde periode hebben geregistreerd.

Houd rekening met de volgende regels wanneer u EXISTS-instructies in een filter gebruikt:

* Er zijn drie objecten waarnaar u in een EXISTS-filter kunt verwijzen:

   * Het object van het filter (Origineel object).
   * Het object waarnaar u wilt verwijzen (doelobject).
   * Het object dat het origineel en de doelobjecten met elkaar verbindt, voor het geval ze niet rechtstreeks met elkaar zijn verbonden (Object koppelen).

* Filters die gebruikmaken van EXISTS bevatten twee afzonderlijke instructies die zijn gekoppeld met een isgelijkteken:

   * De instructie vóór het gelijkteken verwijst naar het object waarnaar u verwijst (de koppeling of het doelobject).
   * De instructie na het gelijkteken verwijst naar het object waarvan u verwijst (het oorspronkelijke object).

* U moet de objectcode van het object Koppelen gebruiken om uw instructies te verbinden.\
  U kunt de objectcode van alle objecten vinden in de API Explorer.\
  Voor informatie over de API Explorer raadpleegt u de [API Explorer](../../../wf-api/general/api-explorer.md).

* Wanneer een object Koppelen ontbreekt omdat het origineel en de doelobjecten rechtstreeks met elkaar zijn verbonden, kunt u de objectcode van het doelobject gebruiken in plaats van het object Koppelen.
* U kunt naar meerdere velden (doelvelden) op hetzelfde object (doelobject) verwijzen. In dat geval moet u de regels verbinden die naar de velden verwijzen door AND.\
  Voor een voorbeeld van het filtreren voor meer dan één gebied dat tot het Voorwerp van het Doel behoort, zie [Voorbeeld 4: Filteren op meerdere velden: taken op basis van de naam van de eigenaar van het Portfolio en de ID van het scorebord voor uitlijning van het Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) in dit artikel.

* De enige bepaling die voor een EXISTS verklaring wordt gesteund is NOTEXISTS.

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
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om filters in een rapport te bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om filters in een rapport te bewerken</p> <p>Machtigingen voor een filter beheren om het te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Filters voor complexe tekstmodus maken die meerdere niveaus in de objecthiërarchie beslaan

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

U kunt een filter maken dat naar objecten verwijst op meerdere niveaus van de objecthiërarchie waarin het filterobject bestaat. U kunt bijvoorbeeld een filter voor uitgaven maken voor problemen die zich voordoen in projecten die niet aan een bepaalde eigenaar van het Portfolio zijn gekoppeld.

U moet altijd een EXISTS verklaring en de interface van de tekstwijze gebruiken om dit filter te bouwen.

Zie voor voorbeelden van filters de [Voorbeeld 1: Filter voor uitgaven op naam van eigenaar Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) in dit artikel.

Een filter maken dat zich uitstrekt over meerdere niveaus in de objecthiërarchie:

1. Identificeer het voorwerp van uw filter. Dit object wordt het oorspronkelijke object genoemd.\
   Bijvoorbeeld Issue.
1. Identificeer het veld waarop u wilt filteren. Wij verwijzen naar dit voorwerp als het Gebied van het Doel dat tot een Voorwerp van het Doel behoort.\
   Bijvoorbeeld het veld ownerID (Doelveld) dat tot een Portfolio behoort (doelobject).
1. (Voorwaardelijk) als het Oorspronkelijke Voorwerp (Uitgave) en het Gebied van het Doel (ownerID) niet direct met elkaar worden verbonden, moet u een derde voorwerp vinden, een Verbonden Voorwerp (Project) dat hen verbindt. Het object Koppelen moet ten minste één veld hebben waarnaar wordt verwezen op de tabbladen Velden of Verwijzingen van het oorspronkelijke object (het veld Koppelen dat wordt weergegeven op het oorspronkelijke object) en het moet ook een koppelingsveld hebben met het doelobject dat wordt weergegeven op de tabbladen Velden of Verwijzingen van het object Koppelen. Het koppelingsveld naar het doelobject dat wordt weergegeven op het koppelingsobject (of het koppelingsveld dat wordt weergegeven op het koppelingsobject) moet overeenkomen met het doelveld.\
   Bijvoorbeeld, (Project) identiteitskaart (het Gebied van de Verbinding die op het Oorspronkelijke Voorwerp wordt getoond) van Kwesties (Origineel Voorwerp) van verwijzingen wordt voorzien. (Portfolio) ownerID (het Gebied van de Verbinding met het Voorwerp van het Doel) wordt getoond op het lusje van Gebieden van het Project (het Verbonden Voorwerp). Portfolio ownerID is ook een veld op het doelobject (Portfolio). Het koppelingsveld op het koppelingsobject komt overeen met het doelveld.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Gebruik de API Explorer om de **Objectcode** van het object Koppelen (project).\
   De Objectcode voor Project is bijvoorbeeld PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Maak een filter voor het oorspronkelijke object.\
   Maak bijvoorbeeld een filter Uitgave.\
   Zie voor informatie over het maken van filters [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Overschakelen naar tekstmodus**.
1. Plak het volgende voorbeeld van de formule in de tekstmodus-interface van het nieuwe filter en vervang de voorgestelde tekst door de juiste objecten en velden:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Zie voor een voorbeeld met de velden die we hierboven hebben aangegeven de [Voorbeeld 1: Filter voor uitgaven op naam van eigenaar Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) in dit artikel.

1. Klikken **Filter opslaan**.

## Filters voor complexe tekstmodus maken voor ontbrekende objecten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

U kunt een filter maken dat verwijst naar objecten die ontbreken. U kunt bijvoorbeeld een gebruikersfilter maken waarin wordt aangegeven welke gebruikers zich niet hebben aangemeld bij Workfront.

U moet altijd een *BESTAAT* en de interface van de tekstwijze om dit filter te bouwen.

Zie de volgende secties in dit artikel voor voorbeelden van filters voor ontbrekende objecten:

* [Voorbeeld 2: Filter voor ontbrekende objecten: aangepaste velden die niet in aangepaste formulieren voorkomen](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Voorbeeld 3: Filter voor ontbrekende objecten: gebruikers die de tijd gedurende een bepaalde periode niet hebben geregistreerd](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Een filter maken dat naar ontbrekende objecten verwijst:

1. Identificeer het voorwerp van uw filter. Dit object wordt het oorspronkelijke object genoemd.\
   Bijvoorbeeld Parameter of Aangepast veld.
1. Identificeer het veld waarop u wilt filteren. Wij verwijzen naar dit voorwerp als het Gebied van het Doel dat tot een Voorwerp van het Doel behoort.\
   Het veld categoryID (doelveld) dat tot categorie (doelobject) behoort.
1. Omdat het Originele Voorwerp (Parameter) en het Gebied van het Doel (categoryID) niet direct met elkaar worden verbonden, moet u een derde voorwerp vinden, een Verbonden Voorwerp (een Parameter van de Categorie) die hen verbindt. Het object Koppelen moet ten minste één veld hebben waarnaar wordt verwezen op de tabbladen Velden of Verwijzingen van het oorspronkelijke object (het veld Koppelen dat wordt weergegeven op het oorspronkelijke object) en het moet ook een koppelingsveld hebben met het doelobject dat wordt weergegeven op de tabbladen Velden of Verwijzingen van het object Koppelen. Het koppelingsveld naar het doelobject dat wordt weergegeven op het koppelingsobject (of het koppelingsveld dat wordt weergegeven op het koppelingsobject) moet overeenkomen met het doelveld.\
   Bijvoorbeeld, wordt identiteitskaart van de Parameter van de Categorie (het Verbonden Gebied dat op het Oorspronkelijke Voorwerp wordt getoond) van Parameter (Origineel Voorwerp) van verwijzingen voorzien. parameterID (Link Field to the Target Object) wordt weergegeven op het tabblad Velden van de Categorieparameter (Linking Object). Het veld Koppelen aan het doelobject dat op het object Koppelen wordt weergegeven, komt overeen met het doelveld.
1. Gebruik de API Explorer om de **Objectcode** van het gekoppelde object (categorieparameter).\
   Bijvoorbeeld, is de Code van Objecten voor de Parameter van de Categorie CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Maak een filter voor het oorspronkelijke object.\
   Maak bijvoorbeeld een parameterfilter.\
   Zie voor informatie over het maken van filters [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Overschakelen naar tekstmodus**.
1. (Voorwaardelijk) Als u filtert voor objecten die ontbreken, plakt u het volgende voorbeeld van de formule in de tekstmodusinterface van het nieuwe filter en vervangt u de voorgestelde tekst door de juiste objecten en velden:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Zie voor een voorbeeld van rapportage over aangepaste velden die niet zijn gekoppeld aan Aangepaste Forms de [Voorbeeld 2: Filter voor ontbrekende objecten: aangepaste velden die niet in aangepaste formulieren voorkomen](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) in dit artikel.

1. Klikken **Filter opslaan**.

## Voorbeelden van tekstmodusfilters die meerdere niveaus in de objecthiërarchie beslaan

* [Voorbeeld 1: Filter voor uitgaven op naam van eigenaar Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Voorbeeld 2: Filter voor ontbrekende objecten: aangepaste velden die niet in aangepaste formulieren voorkomen](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Voorbeeld 3: Filter voor ontbrekende objecten: gebruikers die de tijd gedurende een bepaalde periode niet hebben geregistreerd](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Voorbeeld 4: Filteren op meerdere velden: taken op basis van de naam van de eigenaar van het Portfolio en de ID van het scorebord voor uitlijning van het Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Voorbeeld 1: Filter voor uitgaven op naam van eigenaar Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

Met de interface van de tekstmodus kunt u een filter maken voor een lijst met uitgaven om alleen problemen weer te geven die zich voordoen in projecten die zijn gekoppeld aan een portfolio waarvan de eigenaar een specifieke gebruiker is.

Om kwesties door de Naam van de Eigenaar van het Portfolio te filtreren:

1. Maak een filter Uitgave.\
   Zie voor informatie over het maken van filters [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Overschakelen naar tekstmodus**.
1. Raadpleeg de volgende algemene code:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Plak de volgende code in de **Filterregels instellen voor uw rapport** gebied ter vervanging van de bovenstaande algemene code:
   <pre>BESTAAT:A:$$OBJCODE=PROJ<br>BESTAAT:A:ID=FIELD:projectID<br>BESTAAT:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* Het oorspronkelijke object is het object van het rapport: Issue
   >* Het doelobject is Portfolio.
   >* Het object Linking is Project.
   >* Het doelveld en het koppelingsveld naar het doelobject waarnaar vanuit het koppelingsobject wordt verwezen, zijn ownerID.
   >* De objectcode van het object Koppelen hier is PROJ.
   >* Het verbindingsgebied dat op het Originele Voorwerp wordt getoond is projectID en het Verbindende Gebied is identiteitskaart

1. Vervang de waarde van het Gebied van het Doel (ownerID) in de laatste verklaring met een Gebruiker - identiteitskaart van uw milieu.
1. Klikken **Filter opslaan**.

### Voorbeeld 2: Filter voor ontbrekende objecten: aangepaste velden die niet in aangepaste formulieren voorkomen {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Met behulp van de interface van de tekstmodus kunt u een filter maken om aangepaste velden (parameters) weer te geven die niet zijn gekoppeld aan Aangepaste Forms (categorieën). Dit filter koppelt Parameters aan Categorieën, die door een ander voorwerp, de Parameter van de Categorie worden verbonden. Omdat de twee gebieden niet direct met elkaar worden verbonden en omdat u voor ontbrekende informatie filtreert moet u een EXISTS verklaring gebruiken.

>[!IMPORTANT]
>
>Een parameter is een veld dat bestaat in de veldbibliotheek waarnaar wordt verwezen in een aangepast formulier. Een categorieparameter is de versie van een veld dat op een specifiek formulier wordt weergegeven. Als hetzelfde veld bijvoorbeeld wordt weergegeven op 5 formulieren, zijn er 1 parameter- en 5 categorieparameters in de Workfront-database.

Filteren voor aangepaste velden die niet zijn gekoppeld aan een aangepast formulier:

1. Maak een parameter of een filter Aangepast veld.\
   Zie voor informatie over het maken van filters [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Overschakelen naar tekstmodus**.
1. Raadpleeg de volgende algemene code:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Plak de volgende code in de **Filterregels instellen voor uw rapport** gebied ter vervanging van de bovenstaande algemene code:
   <pre>BESTAAT:A:$$OBJCODE=CTGYPA<br>BESTAAT:A:parameterID=FIELD:ID<br>BESTAAT:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* Het oorspronkelijke object is het object van het rapport: Parameter.
   >* Het doelobject is categorie.
   >* Het object Linking is een categorieparameter.
   >* De objectcode van het object Koppelen is CTGYPA.
   >* Het koppelingsveld naar het doelobject is parameterID omdat parameterID bestaat in zowel de tabel met gekoppelde objecten als de tabel met doelobjecten.
   >* Het koppelingsveld dat op het oorspronkelijke object wordt weergegeven, is een id (van de categorieparameter).

1. Klikken **Filter opslaan**.

### Voorbeeld 3: Filter voor ontbrekende objecten: gebruikers die de tijd gedurende een bepaalde periode niet hebben geregistreerd {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Gebruikend de interface van de tekstwijze, kunt u een filter aan meningsGebruikers bouwen die niet tijd voor een bepaalde tijdspanne registreerden. Dit filter koppelt Gebruikers aan Uren, die direct met elkaar worden verbonden. Nochtans, moet u een EXISTS verklaring en de interface van de tekstwijze gebruiken om voor ontbrekende information.information te kunnen filtreren.

Hiermee filtert u voor gebruikers die zich vorige week niet hebben aangemeld:

1. Maak een gebruikersfilter.\
   Zie voor informatie over het maken van filters [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Overschakelen naar tekstmodus**.
1. Raadpleeg de volgende algemene code:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Plak de volgende code in de **Filterregels instellen voor uw rapport** gebied ter vervanging van de bovenstaande algemene code:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* Het originele voorwerp is het voorwerp van het rapport: Gebruiker.
   >* Het doelobject is Uur.
   >* In dit voorbeeld hebt u geen koppelingsobject nodig omdat Gebruikers en uren rechtstreeks zijn verbonden in de Workfront-database.
   >* Omdat er geen Verbonden Voorwerp is, moet u de Code van Objecten van het Voorwerp van het Doel gebruiken: UUR.
   >* Het koppelingsveld naar het doelobject is ownerID (die wordt weergegeven op het oorspronkelijke object; het koppelingsobject ontbreekt).
   >* Het koppelingsveld dat op het oorspronkelijke object wordt weergegeven, is een id (van het uur) (die wordt weergegeven op het doelobject; het koppelingsobject ontbreekt.)
   >* DE BESTAANDE:A:entryDate-instructie verwijst naar velden die het doelobject (Uur) definiëren en dezelfde syntaxis gebruiken als in een gewone filterinstructie. Dit zorgt ervoor dat u slechts die gebruikers toont die geen tijd voor een specifieke periode, in dit geval, de vorige week registreerden.
   >* De bepaling NOTEXISTS wijst erop dat wij punten (Uren) zoeken die niet voor het voorwerp van het rapport (Gebruikers) bestaan.

1. Klikken **Filter opslaan**.

### Voorbeeld 4: Filteren op meerdere velden: taken op basis van de naam van de eigenaar van het Portfolio en de ID van het scorebord voor uitlijning van het Portfolio {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Met de interface van de tekstmodus kunt u een filter maken dat naar meer dan één veld in het doelobject verwijst. In dit geval moeten de filterinstructies die verwijzen naar de doelvelden, via AND worden verbonden.

U kunt bijvoorbeeld een takenlijst filteren om alleen taken weer te geven die aan de volgende criteria voldoen:

* Ze bevinden zich op een project dat is gekoppeld aan een portfolio waarvan de eigenaar een specifieke gebruiker is.
* Zij zijn op een project verbonden aan een portefeuille de waarvan projecten niet met een specifieke groeperingsscorecard worden geassocieerd.

Om taken door de Naam van de Eigenaar van het Portfolio en identiteitskaart van het Scorecard van de Uitlijning van het Portfolio te filtreren:

1. Maak een taakfilter.\
   Zie voor informatie over het maken van filters [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Overschakelen naar tekstmodus**.
1. Plak de volgende code in de **Filterregels instellen voor uw rapport** gebied:
   <pre>BESTAAT:A:$$OBJCODE=PROJ<br>BESTAAT:A:ID=FIELD:projectID<br>BESTAAT:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f<br>EN:A:BESTAAT:A:$$EXISTSMOD=NOTEXISTS<br>EN:A:BESTAAT:A:$$OBJCODE=PROJ<br>EN:A:BESTAAT:A:ID=FIELD:projectID<br>EN:A:BESTAAT:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* Het oorspronkelijke object is het object van het filter Taak.
   >* Het doelobject is Portfolio.
   >* Het eerste doelveld is ownerID.
   >* Het tweede doelveld is de ID van het uitlijningsscorebord.
   >* Het object Linking is Project.
   >* De objectcode van het object Koppelen is PROJ.
   >* Het veld Koppelen aan het doelobject is de id (van het Portfolio).
   >* Het verbindingsgebied dat op het Originele Voorwerp wordt getoond is projectID.
   >* Vervang de ownerID door een gebruikersnaam uit uw omgeving.

1. Klikken **Filter opslaan**.
