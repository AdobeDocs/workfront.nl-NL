---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Objecten begrijpen in [!DNL Adobe Workfront]
description: Objecten begrijpen in [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1946'
ht-degree: 0%

---

# Objecten begrijpen in [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

De informatie die u in [!DNL Adobe Workfront] wordt voorgesteld door voorwerpen die in [!DNL Workfront] database. De objecten zijn de drijvende kracht achter de informatie in [!DNL Workfront].

Begrijpen hoe de objecten worden gedefinieerd in [!DNL Workfront] is belangrijk, zodat u het juiste object kunt gebruiken voor de behoeften die nodig zijn in uw organisatie.

Als u bijvoorbeeld een grote hoeveelheid werk wilt uitvoeren, moet u de opdracht [!UICONTROL Project] -object om dat werk te definiëren. Als u dit werk in kleinere geplande stappen wilt verdelen, kunt u de opdracht [!UICONTROL Task] object. Voor een kleinere hoeveelheid werk die niet gepland is en onverwacht kan voorkomen, kunt u het voorwerp van de Uitgave gebruiken. Als u de voortgang en de naleving van de begroting en het tijdschema van een groep projecten wilt bijhouden, kunt u deze ordenen in [!UICONTROL Portfolios] en [!UICONTROL Programs]. Als u andere elementen wilt definiëren die u helpen uw werk op te lossen, wilt u andere objecten gebruiken die onder [!UICONTROL Projects], [!UICONTROL Tasks], [!UICONTROL Issues], of [!UICONTROL Portfolios], zoals [!UICONTROL Documents], [!UICONTROL Updates], [!UICONTROL Hours], [!UICONTROL Users], of [!UICONTROL Job Roles].

[!UICONTROL Reports] en [!UICONTROL Dashboards] Dit is een ander voorbeeld van objecten waarmee u de hoeveelheid gegevens in [!DNL Workfront] visueel, om het voor alle gebruikers gemakkelijk toegankelijk te maken.

Voor een volledige lijst met objecten in [!DNL Workfront], zie de [API Explorer](../../../wf-api/general/api-explorer.md).

## Interdependentie en hiërarchie van objecten

Objecten zijn in [!UICONTROL Workfront]. Een taak of een probleem kan bijvoorbeeld nooit zelfstandig buiten een project bestaan. [!UICONTROL Tasks] en [!UICONTROL issues] zijn voorbeelden van objecten die zijn opgeslagen in het dialoogvenster [!UICONTROL project] object. [!UICONTROL Tasks] en [!UICONTROL issues] worden beschouwd als onderliggende objecten bij projecten.

Hier volgen enkele voorbeelden van de meest gebruikte objecten in [!DNL Workfront] en de bijbehorende bovenliggende en onderliggende objecten:

| **Object** | **Bovenliggende objecten** | **Onderliggende objecten** |
|---|---|---|
| [!UICONTROL Portfolios] |  | [!UICONTROL Programs], [!UICONTROL Projects], [!UICONTROL Documents], [!DNL Notes], [!UICONTROL Users] |
| [!UICONTROL Programs] | [!UICONTROL Portfolios] | [!UICONTROL Projects], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Users] |
| [!UICONTROL Projects] | [!UICONTROL Portfolios], [!UICONTROL Programs] | [!UICONTROL Tasks], [!UICONTROL Issues], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Tasks] | [!UICONTROL Projects] | [!UICONTROL Issues], [!UICONTROL Children Tasks], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Issues] | [!UICONTROL Tasks], [!UICONTROL Projects] | [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Dashboards] |  | [!UICONTROL Reports], Externe pagina&#39;s |
| [!UICONTROL Reports] | [!UICONTROL Dashboards] |  |
| [!UICONTROL Groups] |  | [!UICONTROL Users] |
| [!UICONTROL Teams] |  | [!UICONTROL Users] |
| [!UICONTROL Users] | [!UICONTROL Groups], [!UICONTROL Teams], [!UICONTROL Companies] | [!UICONTROL Job Roles] |
| [!UICONTROL Companies] |  | [!UICONTROL Users] |
| [!UICONTROL Documents] | [!UICONTROL Tasks], [!UICONTROL Issues], [!UICONTROL Projects], [!UICONTROL Portfolios], [!UICONTROL Programs], [!UICONTROL Users] |  |
| [!UICONTROL Plans]* |  | [!UICONTROL Initiatives] |
| [!DNL Goals]* |  | [!UICONTROL Results], [!UICONTROL Activities] |

Voor een volledige lijst met objecten in [!DNL Workfront], zie de [API Explorer](../../../wf-api/general/api-explorer.md).

*Plannen zijn de objecten van het [!DNL Adobe Workfront Scenario Planner]. Voor informatie over de [!DNL Scenario Planner], zie [De [!UICONTROL Scenario Planner] overzicht](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Goals] zijn de objecten van [!DNL Adobe Workfront Goals]. Voor informatie over [!DNL Workfront Goals], zie [[!DNL Adobe Workfront Goals] overzicht](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Objectnamen aanpassen

Als [!DNL Workfront] beheerder, kunt u objectnamen aanpassen in [!DNL Workfront] door een  [!UICONTROL Layout Template].

Voor meer informatie over het aanpassen van objectnamen met een  [!UICONTROL Layout Template], zie [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Nadat u een lay-outmalplaatje aanpast en u het aan gebruikers toewijst, zien die gebruikers de aangepaste namen voor de voorwerpen. De gebruikers die aan het lay-outmalplaatje zijn toegewezen zien niet meer de standaardnamen voor de voorwerpen overal in de Webtoepassing.

>[!NOTE]
>
>Als u wilt dat de nieuwe namen van de objecten zichtbaar zijn voor de gebruikers, moet u zich afmelden en zich weer aanmelden bij [!DNL Workfront] nadat u het  [!UICONTROL Layout Template].

>[!IMPORTANT]
>
>De [!DNL Workfront] documentatie verwijst altijd naar de standaardnamen van de objecten. Als [!DNL Workfront] beheerder, zorg ervoor dat u gebruikers op de hoogte brengt van de wijzigingen in objectnamen, zodat zij kunnen begrijpen hoe de [!DNL Workfront] documentatie, alsmede de gebieden van de toepassingen die niet de veranderingen in de namen van de voorwerpen weerspiegelen.

* [Objectnamen die kunnen worden aangepast met een  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template)
* [Gebieden van [!DNL Workfront] die de aangepaste objectnamen weerspiegelen](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Gebieden van [!DNL Workfront] die de aangepaste objectnamen niet weerspiegelen](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Objectnamen die kunnen worden aangepast met een [!UICONTROL Layout Template]

Als [!DNL Workfront] beheerder, kunt u de namen van de volgende voorwerpen aanpassen om de terminologie in uw organisatie aan te passen:

* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Issue]
* [!UICONTROL Goal]*
* [!UICONTROL Result]*
* [!UICONTROL Activity]*

  *[!UICONTROL Goals], [!UICONTROL results], en [!UICONTROL activities] alleen beschikbaar zijn als uw bedrijf is aangeschaft [!DNL Workfront Goals]. Voor informatie over [!DNL Workfront Goals], zie [[!DNL Adobe Workfront Goals] overzicht](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Scenario]**
* [!UICONTROL Plan]**

  **[!UICONTROL Initiatives], [!UICONTROL scenarios], en [!UICONTROL plans] zijn alleen beschikbaar als uw bedrijf [!DNL Workfront Scenario Planner]. Voor informatie over de [!DNL Scenario Planner], zie [Aan de slag met de [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


Als bijvoorbeeld het grotere werk in uw organisatie bekend staat als een &#39;Betrokkenheid&#39;, kunt u de naam &#39;[!UICONTROL Project]&quot; met &quot;Betrokkenheid&quot;. Uw [!DNL Workfront] interface toont &#39;Betrokkenheid&#39; in plaats van &#39;[!UICONTROL Project]&#39; overal waar de naam &#39;[!UICONTROL Project]&#39; weergegeven.

Voor meer informatie over hoe u objectnamen kunt aanpassen met  [!UICONTROL Layout Templates], zie [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

U kunt de namen van andere objecten in Workfront niet aanpassen. Voor een volledige lijst met objecten in [!DNL Workfront], zie de [API Explorer](../../../wf-api/general/api-explorer.md).

Wanneer u de naam van een object aanpast, wordt de nieuwe naam voor dat object in de meeste gebieden van het dialoogvenster [!DNL Workfront] toepassing waarin de naam van dat object wordt weergegeven.

### Gebieden van [!DNL Workfront] die de aangepaste objectnamen weerspiegelen

In de volgende gebieden wordt de bijgewerkte naam van de objecten weergegeven:

* Bovenste navigatie
* Alle secties in de navigatie van het linkerpaneel
* Alle menu&#39;s
* Meldingen in apps
* De bouwer van het rapport en rapporteringselementen (meningen, filters, en groeperingen)
* [!UICONTROL Save] knoppen
* Geëxporteerde bestanden
* E-mails
* Mobiele apps

### Gebieden van [!DNL Workfront] die de aangepaste objectnamen niet weerspiegelen

In de volgende gebieden wordt de bijgewerkte naam van de objecten niet weergegeven:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Add-in

### Implicaties van het aanpassen van objectnamen

Houd rekening met het volgende wanneer u objectnamen aanpast in [!DNL Workfront]:

* Er kunnen fouten optreden in het weergeven van systemen met een stilistische of grammaticale werking. Als u bijvoorbeeld de naam &#39;[!UICONTROL Issue]&#39; aan &quot;Verzoek&quot;en u ziet overal in het systeem de uitdrukking &quot;Een verzoek&quot;, dit functioneert zoals bedoeld en zou niet als insect moeten worden beschouwd.
* Uw aangepaste namen voor de objecten kunnen niet worden vertaald. Alleen de [!DNL Workfront] de standaardnamen kunnen in de gesteunde talen worden vertaald. Voor meer informatie over talen die worden ondersteund in [!DNL Workfront], zie [Ondersteunde talen in [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). De naamvelden van aangepaste objecten ondersteunen vreemde tekens, zodat u in elke taal terminologie kunt invoeren.
* Wanneer u objectnamen aanpast met een  [!UICONTROL Layout Template], adviseren wij u uw  [!UICONTROL Layout Templates] rond uw bedrijfseenheden (teams of groepen).\
   Wij adviseren dat u namen gebruikt die duidelijk door de gebruikers van deze bedrijfseenheden worden begrepen, om verwarring te vermijden.
* E-mailmeldingen en geleverde rapporten bevatten altijd objectnamen zoals gedefinieerd door  [!UICONTROL Layout Template] van de gebruiker die de e-mail genereert. Uw gebruikers moeten voorbereid zijn om objectnamen in hun e-mailberichten te zien die niet gerelateerd zijn aan hun groep of team, als ze e-mailmeldingen ontvangen van gebruikers in andere teams en groepen.\
   Als [!DNL Workfront] beheerder, raadt gebruikers aan de pictogrammen die aan elk object zijn gekoppeld, op te geven. De pictogrammen blijven consistent tussen verschillende objectnamen en zijn consistent met het standaardobject, zoals dat in de database wordt weergegeven. Voor een lijst van allen [!DNL Workfront] pictogrammen die aan objecten zijn gekoppeld, zie [Objectpictogrammen](#object-icons).

  >[!TIP]
  >
  >Voor gemeenschappelijke taken in uw organisatie, denk na creërend douanedocumentatie om uw terminologie te weerspiegelen.

## Objectpictogrammen

De [!DNL Workfront] documentatie verwijst altijd naar de standaardnamen van objecten. Als de namen van de objecten zijn aangepast, kunt u ervan uitgaan dat het pictogram aan de objecten is gekoppeld om te begrijpen welk aangepast object overeenkomt met welk [!DNL Workfront] standaardobject.

Voor meer informatie over welke objecten aangepaste namen kunnen hebben in [!DNL Workfront], zie [Objectnamen die kunnen worden aangepast met een  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).

Hieronder volgt een lijst met objecten en de bijbehorende pictogrammen in Workfront.

| **Object** | **Pictogram** | **Aanpasbare objectnaam** |
|---|---|---|
| [!UICONTROL Company] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Goal] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Group] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Issue] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Job Role] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Program] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Project] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Report] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Task] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Template] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Referentienummers van objecten

Elk object gemaakt in [!DNL Workfront] wordt een uniek referentienummer toegewezen. Referentienummers zijn handig voor het maken van onderscheid tussen twee overigens vergelijkbare objecten (zoals taken met dezelfde naam). U kunt naar objecten zoeken met hun referentienummers en u kunt referentienummers opnemen in rapporten.

Ga voor informatie over het zoeken naar objecten op referentienummer naar [Het referentienummer van objecten gebruiken](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Objectspecifieke zoekopdrachten

U kunt zoeken in alle objecten waarin u kunt zoeken [!DNL Workfront]of u kunt een specifiek object selecteren waarnaar u wilt zoeken in uw standaard en geavanceerde zoekopdrachten.

Niet alle objecten kunnen worden doorzocht in [!DNL Workfront]. U kunt standaard- en geavanceerde zoekopdrachten uitvoeren naar de volgende objecten in [!DNL Workfront]:

| **Object** | **Standaardzoekopdracht** | **Geavanceerd zoeken** |
|---|---|---|
| [!UICONTROL Projects] | ✓ | ✓ |
| [!UICONTROL Tasks] | ✓ | ✓ |
| [!UICONTROL Issues] | ✓ | ✓ |
| [!UICONTROL Reports] | ✓ | ✓ |
| [!UICONTROL Users] | ✓ | ✓ |
| [!UICONTROL Templates] | ✓ | ✓ |
| [!UICONTROL Documents] | ✓ | ✓ |
| [!UICONTROL Portfolios] | ✓ | ✓ |
| [!UICONTROL Programs] | ✓ | ✓ |
| [!UICONTROL Dashboards] | ✓ | ✓ |
| [!UICONTROL Companies] | ✓ | ✓ |
| [!UICONTROL Notes] (of [!UICONTROL Updates]) | ✓ |  |

Voor meer informatie over het uitvoeren van standaard en geavanceerde zoekopdrachten in [!DNL Workfront], zie [Zoeken [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Objecten rapporteren

Kennis van de hiërarchie en de onderlinge afhankelijkheid van objecten is uiterst belangrijk voordat u rapporten gaat samenstellen in [!DNL Workfront]. Rapporten zijn objectspecifiek. U moet het correcte voorwerp voor uw rapport selecteren alvorens u de gegevens kunt tonen die u wilt.

Afhankelijk van welk voorwerp u voor uw rapport selecteerde, kunt u tot slechts die voorwerpen toegang hebben die direct met het voorwerp van het rapport verbonden zijn.

>[!IMPORTANT]
>
>U kunt alleen het object rapporteren dat u selecteert en de bovenliggende objecten in hetzelfde rapport. U kunt geen informatie over de kindvoorwerpen in een ouderobjecten rapport hebben. Bijvoorbeeld, kunt u projectinformatie in een taakrapport tonen, maar niet taakinformatie in een projectrapport.

U kunt alle objecten in de database rapporteren met de geopende API. Voor een volledige lijst van alle voorwerpen in het gegevensbestand, zie [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Als u de namen van uw voorwerpen gebruikend een lay-outmalplaatje hebt aangepast, zijn de namen voor het voorwerp in de rapportbouwer ook aangepast. Zorg ervoor u weet welke voorwerpen zijn aangepast en zoek de aangepaste naam in de rapportbouwer. Voor meer informatie over welke objecten aangepaste namen kunnen hebben in [!DNL Workfront], zie *[Objectnamen die kunnen worden aangepast met een  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).*
>Als u de tekstmodus in uw rapporten gebruikt, zijn de namen van de objecten in tekstmodusexpressies de standaardnamen in [!DNL Workfront]en niet de aangepaste objectnamen. Voor meer informatie over het gebruiken van tekstwijze in rapporten, zie [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Ga voor meer informatie over het samenstellen van een rapport naar [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Zie voor meer informatie over onze API [API Explorer](../../../wf-api/general/api-explorer.md).

U kunt op de volgende voorwerpen rapporteren wanneer het gebruiken van de rapportbouwer in [!DNL Workfront] webtoepassing:

* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Hour]
* [!UICONTROL Issue]
* [!UICONTROL User]
* [!UICONTROL Access] Niveau
* [!UICONTROL Approval]
* [!UICONTROL Approval Process]
* [!UICONTROL Assignment]
<!--this is no longer available: * [!UICONTROL Backlog Work Item]\
   Displays tasks or issues on the agile backlog. For more information about the agile backlog, see [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).-->

* [!UICONTROL Baseline]
* [!UICONTROL Baseline Task]
* [!UICONTROL Billing Record]
* [!UICONTROL Budgeted Hour]

  Dit is het [!UICONTROL Budgeted Hours], zoals deze in de oudere, verouderde hulpmiddelen voor middelenbeheer worden weergegeven.

  The &quot;Bud. Uren&quot; in het veld [!UICONTROL Budgeted Hour] het rapport verwijst naar de uren die in de begroting zijn opgenomen voor functies in het [!UICONTROL Resource Planner]. Zie voor meer informatie [Begrijpen [!UICONTROL Budgeted Labor Cost] en [!UICONTROL Budgeted Hours] voor projecten](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Calendar Event]
* [!UICONTROL Company]
* [!UICONTROL Custom Form]
* [!UICONTROL Dashboard]
* [!UICONTROL Document]
* [!UICONTROL Document Approval]
* [!UICONTROL Document Version]\
   U kunt informatie weergeven over de versie van het document, het document waaraan de versie is gekoppeld, wie de versie heeft gemaakt en de gebruiker die de proefdruk heeft gemaakt op de documentversie, als deze bestaat (Maker van proef).
* [!UICONTROL Email Template]
* [!UICONTROL Expense]
* [!UICONTROL Expense Type]
* [!UICONTROL External Page]
* [!UICONTROL Favorite]
* [!UICONTROL Filter]
* [!UICONTROL Goal]

  U kunt een rapport voor strategische doelstellingen bouwen of u kunt op doel betrekking hebbende informatie in een projectrapport tonen wanneer de projecten met doelstellingen als doelactiviteiten worden geassocieerd. U kunt strategische doelen maken en alleen projecten verbinden als uw organisatie een [!DNL Workfront Goals] licentie. Voor informatie over [!DNL Workfront Goals], zie [[!DNL Workfront Goals] overzicht](../../../workfront-goals/goal-management/wf-goals-overview.md). Voor informatie over het verbinden van projecten met strategische doelstellingen, zie [Projecten toevoegen aan doelen in Adobe Workfront-doelen](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

  >[!TIP]
  >
  >U kunt niet over projectdoelstellingen rapporteren die met een [!UICONTROL Business Case]. Voor informatie over projectdoelstellingen versus strategische doelstellingen, zie [Verklarende woordenlijst [!DNL Adobe Workfront] terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Group]
* [!UICONTROL Grouping]
* [!UICONTROL Hour Type]
* [!UICONTROL Initiative]

  U kunt alleen een rapport maken voor initiatieven die de onderliggende objecten van een plan zijn als uw bedrijf een [!DNL Workfront Scenario Planner] licentie. Zie voor informatie over initiatieven [Overzicht van initiatieven in het [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).


* Rol initiatieftaak

  U kunt een rapport voor de baanrollen verbonden aan de initiatieven in een plan slechts bouwen als uw bedrijf een [!DNL Workfront Scenario Planner] licentie. Voor informatie over het creëren van initiatieven en het associëren van hen met baanrollen, zie [Initiatieven maken en bewerken in het dialoogvenster [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL Iteration]
* [!UICONTROL Job Role]
* [!UICONTROL Journal Entry]

  U kunt de bijgehouden systeemupdates rapporteren in het dialoogvenster [!UICONTROL Updates] gebied met objecten zoals taken, projecten, problemen, enz. Zie voor meer informatie [Verslag over de [!UICONTROL Updates] gebied](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Layout Template]
* [!UICONTROL Milestone]
* [!UICONTROL Milestone Path]
* [!UICONTROL Note] of [!UICONTROL Updates]

  >[!NOTE]
  >
  >U kunt opmerkingen rapporteren die door individuele gebruikers zijn toegevoegd.

* [!UICONTROL Parameter] (of [!UICONTROL Custom Field])
* [!UICONTROL Parameter Group] (of [!UICONTROL Section Break])
  <!--this is no longer in the UI: * [!UICONTROL Portal Profile] (this displays information that has been deprecated)-->
* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project] ([!UICONTROL Financial Data])

  >[!NOTE]
  >
  >Financiële informatie wordt ingevuld in [!UICONTROL Project] ([!UICONTROL Financial Data]) alleen worden gerapporteerd wanneer de gegevens die ermee verband houden jonger zijn dan 5 jaar. Als bijvoorbeeld in januari 2015 een functie werd toegewezen aan een taak en vandaag september 2021, dan is een financieel dossier zoals de [!UICONTROL Allocation Date] voor de rol job niet wordt gevuld in het dialoogvenster [!UICONTROL Project (Financial Data)] verslag.

* [!UICONTROL Proof Approval]\
   Hiermee kunt u verschillende informatie over de goedkeuring van het bewijs bekijken, zoals: het bewijs dat ter goedkeuring is ingediend, informatie over de [!UICONTROL Approver], informatie over de aanvrager (als de aanvrager een vergunning heeft [!DNL Workfront] gebruiker), versiegegevens, de proefdruk-id en de aanmaakdatum van de proefdruk.\
   [!UICONTROL Proof Approval] rapporten bevatten alleen proefdrukken die beschikbaar zijn op de gebieden Mijn werk van gebruikers waar nog geen beslissingen zijn genomen.\
   Goedkeuringen van proefdrukken worden toegewezen in [!DNL Workfront] zoals beschreven [Gebruikers aan een proefdruk toevoegen](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Een proefdruk delen binnen [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Queue]
* [!UICONTROL Queue Topic]
* [!UICONTROL Rate] (hiermee wordt de taakrol weergegeven [!UICONTROL Billing Rate] informatie)
* [!UICONTROL Reminder Notification]
* [!UICONTROL Report]
* [!UICONTROL Resource Pool]
* [!UICONTROL Risk]
* [!UICONTROL Risk Type]
* [!UICONTROL Schedule]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Template]
* [!UICONTROL Template Task]
* [!UICONTROL Time Off]

  U kunt melding maken van de time-out van een gebruiker, zoals deze door de gebruiker in het profiel wordt aangegeven.

* [!UICONTROL Timesheet]
* [!UICONTROL Timesheet Profile]
* [!UICONTROL Topic Group]
* [!UICONTROL User Approval]
* [!UICONTROL User Delegation]

  U kunt rapporteren over gebruikers die zijn gedelegeerd om taken en problemen van anderen uit te voeren terwijl ze buiten het kantoor zijn. Dit rapport toont de gebruiker die uit het bureau evenals de gebruiker is die hun taken vervult terwijl zij uit zijn.
* [!UICONTROL Users Decisions]
* [!UICONTROL View]
* [!UICONTROL Work Item] (dit levert een rapport op voor taken en kwesties)
