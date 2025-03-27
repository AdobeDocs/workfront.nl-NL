---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect-gegevenswoordenboek
description: Deze pagina bevat informatie over de structuur en inhoud van de gegevens in Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: eccc878f4b6fdeeffbcd5635b80ac3e26f7fb8c6
workflow-type: tm+mt
source-wordcount: '4719'
ht-degree: 0%

---

# Workfront Data Connect-gegevenswoordenboek

Deze pagina bevat informatie over de structuur en inhoud van de gegevens in Workfront Data Connect.

>[!NOTE]
>
>De gegevens in Data Connect worden elke vier uur vernieuwd, zodat recente wijzigingen mogelijk niet direct worden doorgevoerd.

## Tabeltypen

Er zijn een aantal tabeltypen die u in Data Connect kunt gebruiken om uw Workfront-gegevens op een manier te bekijken die het meest inzicht biedt.

* **Huidige lijst**

  De tabel Huidig bevat gegevens die ongeveer overeenkomen met de status in Workfront, elk object en de huidige status. U kunt er echter veel minder latentie aan toevoegen dan in Workfront.

* **lijst van de Gebeurtenis**

  De gebeurtenissentabel houdt elke veranderingsverslag in Workfront bij: namelijk telkens als een voorwerp staat verandert, wordt een verslag gecreeerd dat toont wanneer de verandering gebeurde, die de verandering aanbracht, en wat werd veranderd. Daarom is deze lijst nuttig voor punt-in-tijd vergelijkingen. Deze tabel bevat alleen gegevens van de afgelopen drie jaar.

* **Dagelijkse lijst van de Geschiedenis**

  De tabel Dagelijkse historie bevat een verkorte versie van de tabel Gebeurtenis, in die zin dat de status van elk object dagelijks wordt weergegeven in plaats van wanneer elke afzonderlijke gebeurtenis zich heeft voorgedaan. Daarom is deze tabel nuttig voor trendanalyse.

<!-- Custom table -->

## Relatiediagram voor entiteit

Objecten in Workfront (en dus ook in het Data Connect Data Lake) worden niet alleen gedefinieerd door hun individuele waarden, maar ook door hun relaties met andere objecten. In het onderstaande diagram voor de entiteitsrelatie wordt een overzicht op hoog niveau gegeven van objectrelaties in Data Connect. Het diagram kan worden bekeken en gedownload gebruikend de volgende verbinding:

[Relatiediagram van gegevensConnect-entiteit](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Het diagram van de entiteitverhouding is een werk lopend-als dusdanig, is het slechts voor verwijzingsdoeleinden en is onderhevig aan verandering.

## Datumtypen

Er zijn een aantal datumobjecten die informatie bevatten over wanneer specifieke gebeurtenissen plaatsvinden.

* `DL_LOAD_TIMESTAMP`: Deze datum wordt gebruikt voor interne referentie en geeft aan wanneer de gegevens zijn geladen in de tabel Huidige, Gebeurtenis of Dagelijkse historie. Deze datum mag niet worden gebruikt voor gegevensanalyse en zal worden verwijderd tijdens de bètafase van het Workfront data Lake.
* `CALENDAR_DATE`: Deze datum is alleen aanwezig in de tabel Dagelijkse historie. In deze tabel wordt een record weergegeven van hoe de gegevens er uitzien bij 11:59 UTC voor elke datum die is opgegeven in `CALENDAR_DATE` .
* `BEGIN_EFFECTIVE_TIMESTAMP`: Deze datum is aanwezig in zowel de lijsten van de Geschiedenis van de Gebeurtenis als van de Dagelijkse Geschiedenis, en verslagen precies wanneer een verslag __ veranderde de waarde het in de huidige rij heeft.
* `END_EFFECTIVE_TIMESTAMP`: Deze datum is aanwezig in zowel de lijsten van de Geschiedenis van de Gebeurtenis als van de Dagelijkse Geschiedenis, en verslagen precies wanneer een verslag _van_ de waarde in de huidige rij in een waarde in een verschillende rij veranderde. Als u ruimte wilt maken tussen query&#39;s op `BEGIN_EFFECTIVE_TIMESTAMP` en `END_EFFECTIVE_TIMESTAMP` , is deze waarde nooit null, zelfs als er geen nieuwe waarde is. Als een record nog geldig is (de waarde is dus niet gewijzigd), heeft `END_EFFECTIVE_TIMESTAMP` de waarde 2300-01-01.

## Terminologie tabel

De volgende tabel correleert objectnamen in Workfront (en hun namen in de interface en API) met hun equivalente namen in Data Connect.

<table>
  <thead>
    <tr>
        <th>Naam Workfront-entiteit</th>
        <th>Interfaceverwijzingen</th>
        <th>API-naslag | Label</th>
        <th>Gegevens Meer tabellen</th>
        <th>Relatiegebied</th>
        <th>Relatietabel en veld</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Toegangsniveau</td>
        <td>Toegangsniveau</td>
        <td>ACSLVL | Toegangsniveau</td>
        <td>ACCESSLEVELS_CURRENT <br> ACCESSLEVELS_DAILY_HISTORY <br> ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (zelf) <br> APPGLOBALID <br> LASTUPDATEDBYID <br> LEGACYACCESSLEVELID <br> OBJID <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USER_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> identiteitskaart van het voorwerp dat in het gebied OBJCODE <br> wordt geïdentificeerd geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Toegangsregel</td>
        <td>Delen</td>
        <td>ACSRUL | Delen</td>
        <td>ACCESSRULES_CURRENT <br> ACCESSRULES_DAILY_HISTORY <br> ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br> ACCESSRULEID (zelf) <br> ANCESTORID <br> LASTUPDATEDBYID <br> SECURITYOBJID <br> SYSID</td>
        <td>Identiteitskaart van het voorwerp dat in ACCESSOROBJCODE gebied <br> wordt geïdentificeerd Zelf <br> identiteitskaart van het voorwerp dat in het gebied ANCESTOROBJCODE <br> wordt geïdentificeerd USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat in het gebied SECURITYOBJCODE <br> wordt geïdentificeerd geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Goedkeuringspad</td>
        <td>Goedkeuringspad</td>
        <td>ARVPTH | Goedkeuring</td>
        <td>GOEDKEURVALPATHS_CURRENT <br> GOEDKEURVALPATHS_DAILY_HISTORY <br> ERKVALPATHS_EVENT</td>
        <td>GOEDGEKEURDE (zelf) <br> GOEDKEURINGVALPROCESSID <br> ENTEREDBYID <br> GLOBALPATHID <br> LASTUPDATEDBYID <br> SYSID</td>
        <td>Zelf <br> GOEDKEURINGSPROCESSES_CURRENT | ERKVALPROCESSID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Goedkeuringsproces</td>
        <td>Goedkeuringsproces</td>
        <td>ARVPRC | Goedkeuringsproces</td>
        <td>GOEDKEURINGSPROCESSES_CURRENT <br> GOEDKEURINGPROCESSES_DAILY_HISTORY <br> GOEDKEURINGPROCESSES_EVENT</td>
        <td>GOEDKEURINGSPROCESSID (zelf) <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> SYSID</td>
        <td>Zelf <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Goedkeuringsstap</td>
        <td>Goedkeuringsstap</td>
        <td>ARVSTP | Goedkeuringsfase</td>
        <td>GOEDVALSTEPS_CURRENT <br> GOEDKEURINGSSTPS_DAILY_HISTORY <br> GOEDKEURINGSSTEPS_EVENT</td>
        <td>GOEDGEKEURDE <br> GOEDGEKEURDE GOEDGEKEURDE (zelf) <br> SYSID</td>
        <td>METHOVALPATHS_CURRENT | GOEDGEKEURDE <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>Status fiatteur</td>
        <td>ARVSTS | ApproverStatus</td>
        <td>GOEDVERSTATUSES_CURRENT <br> GOEDVERSTATUSES_DAILY_HISTORY <br> GOEDVERSTATUSES_EVENT</td>
        <td>GOEDGEKEURDE (zelf) <br> GOEDKEURDE 1} GOEDKEURDE GOEDKEURING <br> GOEDKEURDE <br> DELEGATEUSERID <br> LASTUPDATEDBYID <br> OPTASKID <br> OVERRIDDENUSERID <br> PROJECTID <br> STEPAPPROVERID <br> SYSID <br> SKID <br> WILDCARDUSERID<br></td>
        <td>Zelf <br> identiteitskaart van het voorwerp dat op het gebied <br> wordt geïdentificeerd GOEDKEURING_CURRENT | GOEDGEKEURDE <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> OPTASKS_CURRENT | OPTASKID <br> USERS_CURRENT | USERID <br> PROJECTS_CURRENT | PROJECTID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Toewijzing</td>
        <td>Toewijzing</td>
        <td>ASSGN | Toewijzing</td>
        <td>ASSIGNMENTS_CURRENT <br> ASSIGNMENTS_DAILY_HISTORY <br> ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID <br> ASSIGNEDTOID <br> ASSIGNMENTID (zelf) <br> CATEGORYID <br> CLASSIFIERID <br> OPTASKID <br> PRIVATERATECARDID <br> PROJECTID <br> ROLEID <br> TIJDELIJKE TAAKID <br></td>
        <td>USER_CURRENT | USERID <br> USER_CURRENT | USERID <br> Zelf <br> CATEGORIEËN_CURRENT | CATEGORYID <br> Lijst van de Classificator momenteel niet gesteund <br> OPTASK_CURRENT | OPTASKID <br> RATECARD_CURRENT | RATECARDID <br> PROJECT_CURRENT | PROJECTID <br> ROLE_CURRENT | ROLEID <br> TASK_CURRENT | TASKID <br> TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Wachtend op goedkeuring</td>
        <td>Wachtend op goedkeuring</td>
        <td>AWAPVL | Wachtend op goedkeuring</td>
        <td>AWAITINGGOEDVALS_CURRENT <br> AWAITINGGOEDVALS_DAILY_HISTORY <br> AWAITINGGOEDVALS_EVENT</td>
        <td>ACCESSREQUESTID <br> GOEDKEURDE <br> GOEDGEKEURDE <br> AWAITING GOEDKEURDE (zelf) <br> DOCUMENTID <br> DOCUMENTVERSIONID <br> OPTASKID <br> PROJECTID <br> ROLEID <br> SUBMITTEDBYID <br> SYSID <br> TASKID {11 <br> TIMESHEETID <br> GEBRUIKERSNAAM VAN HET TEAMID<br></td>
        <td>De lijst van het Verzoek van de toegang die momenteel niet wordt gesteund <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> Zelf <br> DOCUMENTS_CURRENT | DOCUMENTID <br> DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID <br> OPTASKS_CURRENT | OPTASKID <br> PROJECTS_CURRENT | PROJECTID <br> ROLES_CURRENT | ROLEID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID <br> TEAMS_CURRENT | TEAMID <br> TIMESHEETS_CURRENT | TIMESHEETID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Basislijn</td>
        <td>Basislijn</td>
        <td>BLIN | Basislijn</td>
        <td>BASELINES_CURRENT <br> BASELINES_DAILY_HISTORY <br> BASELINES_EVENT</td>
        <td>BASELINEID (zelf) <br> EXCHANGERATEID <br> PROJECTID <br> SYSID</td>
        <td>Zelf <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Basislijntaak</td>
        <td>Basislijntaak</td>
        <td>BSTSK | Basislijntaak</td>
        <td>BASELINETASKS_CURRENT <br> BASELINETASKS_DAILY_HISTORY <br> BASELINETASKS_EVENT</td>
        <td>BASELINEID <br> BASELINETASKID (zelf) <br> EXCHANGERATEID <br> PROJECTID <br> SYSID <br> TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID <br> ZELFDE <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Factureringsgraad</td>
        <td>Snelheid of Override Rate</td>
        <td>TARIEF | Factureringsgraad</td>
        <td>RATES_CURRENT <br> RATES_DAILY_HISTORY <br> RATES_EVENT</td>
        <td>ASSIGNMENTID <br> CLASSIFIERID <br> EXCHANGERATEID <br> NLBRCATEGORYID <br> NONLABORRESOURCEID <br> OBJID <br> PROJECTID <br> RATECARDID <br> RATEID (zelf) <br> ROLEID <br> SOURCERATECARDID <br> SYSID <br> TEMPLATEID <br> GEBRUIKERSNAAM</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br> lijst van het Klassificator die momenteel niet <br> EXCHANGERATES_CURRENT wordt gesteund | EXCHANGERATEID <br> niet-Arbeidslijst van het Middel momenteel niet gesteund <br> NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> wordt geïdentificeerd PROJECTS_CURRENT | PROJECTID <br> RATECARD_CURRENT | RATECARDID <br> Zelf <br> ROLES_CURRENT | ROLEID <br> RATECARD_CURRENT | RATECARDID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEMPLATES_CURRNT | TEMPLATEID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Factureringsrecord</td>
        <td>Factureringsrecord</td>
        <td>BILL | Factureringsrecord</td>
        <td>BILLINGRECORDS_CURRENT <br> BILLINGRECORDS_DAILY_HISTORY <br> BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (zelf) <br> CATEGORYID <br> EXCHANGERATEID <br> INVOICEID <br> LASTUPDATEDBYID <br> PROJECTID <br> SYSID</td>
        <td>Zelf <br> CATEGORIEËN_CURRENT | CATEGORYID <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> Factuurentabel wordt momenteel niet ondersteund <br> USERS_CURRENT | USERID <br> PROJECTS_CURRENT | PROJECTIEF   <br> Geen relatie; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Boking</td>
        <td>Boking</td>
        <td>BOOKN | Boking</td>
        <td>BOOKINGS_CURRENT <br> BOOKINGS_EVENT<br></td>
        <td>BOOKINGID (zelf) <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> NLBRCATEGORYID <br> NONLABORRESOURCEID <br> OBJID <br> PROJECTID <br> SYSID <br> TASKID <br> TEMPLATEID <br> TEMPLATETASKID <br> TOTASKID POBJID</td>
        <td>Zelf <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> niet-arbeidsLijst van het Middel momenteel niet gesteund <br> NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID <br> identiteitskaart van het voorwerp dat op het gebied OBJOBJCODE <br> wordt geïdentificeerd PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID <br> TEMPLATES_CURRENT | TEMPLATEID <br> TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> identiteitskaart van het voorwerp dat in het TOPOBJCODE- gebied wordt geïdentificeerd</td>
    </tr>
    <tr>
        <td>Bedrijfsprofiel</td>
        <td>Bedrijfsprofiel</td>
        <td>BSNPRF | BusinessProfile</td>
        <td>BUSINESSPROFILE_CURRENT <br> BUSINESSPROFILE_DAILY_HISTORY <br> BUSINESSPROFILE_EVENT</td>
        <td>ACCESSLEVELID <br> BUSINESSPROFILEID (zelf) <br> ENTEREDBYID <br> GROUPID <br> LASTUPDATEDBYID <br> SYSID</td>
        <td>ACCESSLEVELS_CURRENT | ACCESSLEVELID <br> ZELFDE <br> USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Zakelijke regel</td>
        <td>Zakelijke regel</td>
        <td>BSNRUL | Zakelijke regel</td>
        <td>BUSINESSRULE_CURRENT <br> BUSINESSRULE_DAILY_HISTORY <br> BUSINESSRULE_EVENT</td>
        <td>BUSINESSRULEID (zelf) <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> SYSID</td>
        <td>Zelf <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Categorie</td>
        <td>Aangepast formulier</td>
        <td>CTGIE | Categorie</td>
        <td>CATEGORIEËN_CURRENT <br> CATEGORIEËN_DAILY_HISTORY <br> CATEGORIEËN_EVENT</td>
        <td>CATEGORYID (zelf) <br> ENTEREDBYID <br> GROUPID <br> LASTUPDATEDBYID <br> SYSID</td>
        <td>Zelf <br> USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID <br> USERS_CURRENT | USERID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Categorieparameter</td>
        <td>Aangepaste formuliervelden</td>
        <td>CTGYPA | Categorieparameter</td>
        <td>CATEGORIESPARAMETERS_CURRENT <br> CATEGORIESPARAMETERS_DAILY_HISTORY <br> CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (zelf) <br> CATEGORYID <br> PARAMETERGROUPID <br> PARAMETERID <br> SYSID</td>
        <td>Zelf <br> CATEGORIEËN_CURRENT | CATEGORYID <br> Lijst van de Groep van de Parameter niet momenteel <br> PARAMETERS_CURRENT | PARAMETERS    <br> Geen relatie; wordt gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Klassificator</td>
        <td>Locatie</td>
        <td>CLSF | Locatie</td>
        <td>CLASSIFIER_CURRENT <br> CLASSIFIER_DAILY_HISTORY <br> CLASSIFIER_EVENT</td>
        <td>CLASSIFIERID (zelf) <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> PARENTID <br> SYSID</td>
        <td>Zelf <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> CLASSIFIER_CURRENT | CLASSIFIERID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Bedrijf</td>
        <td>Bedrijf</td>
        <td>CMPY | Bedrijf</td>
        <td>COMPANIES_CURRENT <br> COMPANIES_DAILY_HISTORY <br> COMPANIES_EVENT</td>
        <td>CATEGORYID <br> COMPANYID (zelf) <br> ENTEREDBYID <br> GROUPID <br> LASTUPDATEDBYID <br> PRIVATERATECARDID <br> SYSID</td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORYID <br> Zelf <br> USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID <br> USERS_CURRENT | USERID <br> RATECARD_CURRENT | RATECARDID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Aangepast kwartaal</td>
        <td>Aangepast kwartaal</td>
        <td>CSTQRT | Aangepast kwartaal</td>
        <td>CUSTOMQUARTERS_CURRENT <br> CUSTOMQUARTERS_DAILY_HISTORY <br> CUSTOMQUARTERS_EVENT</td>
        <td>AANGEPAST (zelf) <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Voorwaarde, Prioriteit, Prioriteit, Status</td>
        <td>CSTEM | Aangepaste Enum</td>
        <td>CUSTOMENUMS_CURRENT <br> CUSTOMENUMS_DAILY_HISTORY <br> CUSTOMENUMS_EVENT <br>* Het type van verslag wordt geïdentificeerd door het bezit ` enumClass `. Het volgende is de verwachte types:<br> CONDITION_OPTASK <br> CONDITION_TASK <br> PRIORITY_OPTASK <br> PRIORITY_PROJ <br> PRIORITY_TASK <br> SEVERITY_OPTASK <br> STATUS_OPTASK <br> STATUS_PROJ <br> STATUS_TASK SK<br></td>
        <td>ENTEREDBYID <br> GROUPID</td>
        <td>USER_CURRENT | USERID <br> GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Document</td>
        <td>Document</td>
        <td>DOCU | Document</td>
        <td>DOCUMENTS_CURRENT <br> DOCUMENTS_DAILY_HISTORY <br> DOCUMENTS_EVENT <br> DOCUMENTS_CUSTOM_VALUE_CURRENT <br> DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY <br> DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID <br> CONTROKEDOUTBYID <br> DOCUMENTID <br> DOCUMENTREQUESTID <br> EXCHANGERATEID <br> ITERATIONID <br> LASTNOTEID <br> LASTUPDATEDBYID <br> NOTEID <br> OBJID <br> OPTASKID <br> OWNERID ID <br> PORTFOLIOID <br> PROGRAMID <br> PROJECTID <br> RELEASEVERSIONID <br> TASKID <br> TEMPLATEID <br> TEMPLATETASKID <br> TOPOBJID <br> USERID</td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORIE <br> USER_CURRENT | GEBRUIKERID <br> ZELFDE <br> Lijst van het Verzoek van het Document niet momenteel <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> ITERATIONS_CURRENT | ITERATIONID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> NOTE_CURRENT | NOTEID <br> Variabele afhankelijk van de waarde DOCOBJCODE <br> OPTASK_CURRENT | OPTASKID <br> USER_CURRENT | USERID <br> PORTFOLIO_CURRENT | PORTFOLIOID <br> PROGRAM_CURRENT | PROGRAMID <br> PROJECT_CURRENT | De lijst van de Versie van de PROJECTIDE <br> Versie van de PROJECTIE niet momenteel <br> TASK_CURRENT | TASKID <br> TEMPLATES_CURRENT | TEMPLATEID <br> TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> Variabele afhankelijk van TOPOBJCODE waarde <br> USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Documentgoedkeuring</td>
        <td>Documentgoedkeuring</td>
        <td>DOCAPL | Documentgoedkeuring</td>
        <td>DOCAPPROVALS_CURRENT <br> DOCAPPROVALS_DAILY_HISTORY <br> DOCAPPROVALS_EVENT</td>
        <td>GOEDGEKEURDE <br> DOCAPPROVALID (zelf) <br> DOCUMENTID <br> NOTEID <br> VERZOEK <br> SYSID</td>
        <td>USERS_CURRENT | USERID <br> ZELFDE <br> DOCUMENTS_CURRENT | DOCUMENTID <br> NOTES_CURRENT | NOTEID <br> USERS_CURRENT | USERID <br> Geen relatie; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Documentmap</td>
        <td>Documentmap</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT <br> DOCFOLDERS_DAILY_HISTORY <br> DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (zelf) <br> ENTEREDBYID <br> ISSUEID <br> ITERATIONID    <br> LINKEDFOLDERID <br> PARENTID <br> PORTFOLIOID <br> PROGRAMID    <br> PROJECTID <br> SYSID <br> TASKID     <br> TEMPLATEID <br> TEMPLATETASKID <br> GEBRUIKERSNAAM</td>
        <td>Zelf <br> USERS_CURRENT | USERID <br> OPTASKS_CURRENT | OPTASKID <br> ITERATIONS_CURRENT | ITERATIONID <br> LINKEDFOLDERS_CURRENT | LINKEDFOLDERID <br> DOCFOLDERS_CURRENT | DOCFOLDERID <br> PORTFOLIO_CURRENT | PORTFOLIOID <br> PROGRAM_CURRENT | PROGRAMMA    <br> PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID     <br> TEMPLATES_CURRENT | TEMPLATEID <br> TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentProviderMetadata</td>
        <td>Document biedt metagegevens</td>
        <td>DOCMET | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT <br> DOCPROVIDERMETA_DAILY_HISTORY <br> DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID (zelf) <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Documentprovider</td>
        <td>DOCPRO | Documentprovider</td>
        <td>DOCPROVIDERS_CURRENT <br> DOCPROVIDERS_DAILY_HISTORY <br> DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID <br> DOCPROVIDERID (zelf) <br> OWNERID    <br> SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID <br> ZELF<br> USERS_CURRENT | USERID    <br> Geen relatie; wordt gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Configuratie van documentprovider</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT <br> DOCPROVIDERCONFIG_DAILY_HISTORY <br> DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID (zelf) <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Documentversie</td>
        <td>DOCV | Documentversie</td>
        <td>DOCUMENTVERSIONS_CURRENT <br> DOCUMENTVERSIONS_DAILY_HISTORY <br> DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTPROVIDERID <br> DOCUMENTVERSIONID <br> ENTEREDBYID <br> EXTERNALSTORAGEID <br> PROOFGOEDVALSTATUSID <br> PROOFEDBYUSERID <br> PROOFOWNERID <br> PROOFOWNERID <br> PROOFSTAGEID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID <br> DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID <br> ZELF<br> USER_CURRENT | USERID <br> Externe identiteitskaart <br> lijst van de Status van de Goedkeuring van het Bewijs niet momenteel gesteund <br> USER_CURRENT | USERID <br> lijst van het Bewijs momenteel niet gesteund <br> USER_CURRENT | De lijst van het Stadium van het Bewijs van USERID <br> wordt momenteel niet gesteund</td>
    </tr>
    <tr>
        <td>Wisselkoers</td>
        <td>Wisselkoers</td>
        <td>EXRATEN | Wisselkoers</td>
        <td>EXCHANGERATES_CURRENT <br> EXCHANGERATES_DAILY_HISTORY <br> EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID (zelf) <br> PROJECTID <br> SYSID <br> TEMPLATEID  </td>
        <td>Zelf <br> PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Kosten</td>
        <td>Kosten</td>
        <td>EXPNS | Kosten</td>
        <td>EXPENSES_CURRENT <br> EXPENSES_DAILY_HISTORY <br> EXPENSES_EVENT</td>
        <td>BILLINGRECORDID <br> CATEGORYID <br> ENTEREDBYID <br> EXCHANGERATEID <br> UITGAANDE (zelf) <br> UITGAANDE <br> LASTUPDATEDBYID <br> OBJID <br> PROJECTID <br> SYSID <br> TASKID <br> TEMPLATEID <br> TEMPLATETASKID <br> TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> USERS_CURRENT | USERID <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> Zelf <br> EXPENSETYPES_CURRENT | EXPENSETYPEID <br> USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> wordt geïdentificeerd PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID <br> TEMPLATES_CURRENT | TEMPLATEID <br> TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> identiteitskaart van het voorwerp dat in het TOPOBJCODE- gebied wordt geïdentificeerd</td>
    </tr>
    <tr>
        <td>Type uitgave</td>
        <td>Type uitgave</td>
        <td>EXPTYP | Type uitgave</td>
        <td>EXPENSETYPES_CURRENT <br> EXPENSETYPES_DAILY_HISTORY <br> EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID <br> UITGAVEN (zelf) <br> OBJID <br> SYSID  </td>
        <td>Geen verband; gebruikt voor interne toepassingsdoeleinden <br> Zelf <br> identiteitskaart van het voorwerp dat in het gebied OBJCODE <br> wordt geïdentificeerd geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Groep</td>
        <td>Groep</td>
        <td>GROEP | Groep</td>
        <td>GROUPS_CURRENT <br> GROUPS_DAILY_HISTORY <br> GROUPS_EVENT</td>
        <td>BUSINESSLEADERID <br> CATEGORYID <br> ENTEREDBYID <br> GROUPID <br> LAYOUTTEMPLATEID <br> PARENTID <br> ROOTID <br> UITEMPLATEID</td>
        <td>USER_CURRENT | USERID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> USER_CURRENT | USERID <br> Zelf <br> lijst van het Malplaatje van de Lay-out zal niet <br> GROUP_CURRENT worden gesteund | GROUPID <br> GROUP_CURRENT | GROUPID <br> UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Uur</td>
        <td>Uur</td>
        <td>UUR | Uur</td>
        <td>HOURS_CURRENT <br> HOURS_DAILY_HISTORY <br> HOURS_EVENT</td>
        <td>GOEDGEKEURDE <br> CATEGORYID 1} BILLINGRECORDID <br> CLASSIFIERID <br> DUPID <br> EXCHANGERATEID <br> EXTERNALTIMESHEETID <br> HOURTYPEID <br> LASTUPDATEDBYID <br> OPTASKID <br> <br> PROJECTID <br> PROJECTOVERHEADID <br> ROLEID <br> TASKID <br> TIMESHEETID<br><br></td>
        <td>USER_CURRENT | USERID <br> BILLINGRECORDS_CURRENT | BILLINGRECORDID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> Lijst van de Classificator die momenteel niet wordt gesteund <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> geen relatie van Workfront; gebruikt voor integratie aan externe systemen <br> Zelf <br> HOURTYPE_CURRENT | HOURTYPEID <br> USER_CURRENT | USERID <br> OPTASK_CURRENT | OPTASKID <br> USER_CURRENT | USERID <br> PROJECT_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> ROLE_CURRENT | ROLEID <br> TASK_CURRENT | TASKID <br> TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Uurtype</td>
        <td>Uurtype</td>
        <td>HOURT | Uurtype</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID <br> HOURTYPEID <br> OBJID</td>
        <td>Niet een verband; gebruikt voor interne toepassingsdoeleinden <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Iteratie</td>
        <td>Iteratie</td>
        <td>ITRN | Iteratie</td>
        <td>ITERATIONS_CURRENT <br> ITERATIONS_DAILY_HISTORY <br> ITERATIONS_EVENT</td>
        <td>CATEGORYID <br> ENTEREDBYID <br> ITERATIONID (zelf) <br> LASTUPDATEDBYID <br> OWNERID <br> SYSID <br> TEAMID</td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORIE <br> USERS_CURRENT | USERID <br> ZELFDE <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Dagboekinvoer</td>
        <td>Dagboekinvoer</td>
        <td>JRNLE | Dagboekinvoer</td>
        <td>JOURNALENTRIES_CURRENT <br> JOURNALENTRIES_DAILY_HISTORY <br> JOURNALENTRIES_EVENT</td>
        <td>GOEDKEURING <br> AUDITRECORDID <br> BASELINEID <br> BILLINGRECORDID <br> COMPANYID <br> DOCUMENTID <br> DOCUMENTSHAREID <br> EDITEDBYID <br> UITGAANDE <br> HOURID 10} INITIATIVEID 1} JOURNALENTRIEID (zelf) <br> OBJID <br> OPTASKID <br> PORTFOLIOID <br> PROGRAMID <br> PROJECTID <br> SUBOBJID <br> SUBSCRIBEID <br> SYSID <br> TASKID <br> TEMPEG LATEID <br> TIMESHEETID <br> TOPOBJID <br> GEBRUIKERSNAAM<br><br><br></td>
        <td>RESVERSTATUSES_CURRENT | GOEDKEURINGSSTATUSID <br> ASSIGNMENTS_CURRENT | ASSIGNMENTID <br> de verslaglijst van de Controle niet momenteel <br> BASELINES_CURRENT | BASELINEID <br> BILLINGRECORDS_CURRENT | BILLINGRECORDID <br> COMPANIES_CURRENT | COMPANYID <br> DOCUMENTS_CURRENT | DOCUMENTID <br> de lijst van het Aandeel van het Document niet momenteel <br> USERS_CURRENT | USERID <br> EXPENSES_CURRENT | EXPENSEID <br> HOURS_CURRENT | HOURID <br> lijst van het Initiatief niet momenteel <br> Zelf <br> wordt gesteund identiteitskaart van het voorwerp dat in het gebied OBJCODE <br> wordt geïdentificeerd OPTASKS_CURRENT | OPTASKID <br> PORTFOLIO_CURRENT | PORTFOLIOID <br> PROGRAM_CURRENT | PROGRAMID <br> PROJECTS_CURRENT | PROJECTID <br> identiteitskaart van het voorwerp dat in het gebied SUBOBJCODE <br> wordt geïdentificeerd onderschrijf lijst momenteel niet <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID <br> TEMPLATES_CURRENT | TEMPLATEID <br> TIMESHEETS_CURRENT | TIMESHEETID <br> identiteitskaart van het voorwerp dat op het TOPOBJCODE- gebied <br> wordt geïdentificeerd USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT <br> LINKEDFOLDERS_DAILY_HISTORY <br> LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID <br> EXTERNALSTORAGEID <br> FOLDERID <br> LINKEDBYID <br> LINKEDFOLDERID (zelf) <br> SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID <br> Externe identiteitskaart <br> DOCFOLDERS_CURRENT | DOCFOLDERID <br> USERS_CURRENT | USERID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Mijlsteen</td>
        <td>Mijlsteen</td>
        <td>MILE | Mijlsteen</td>
        <td>MILESTONES_CURRENT <br> MILESTONES_DAILY_HISTORY <br> MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID <br> MILESTONEID <br> MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID <br> ZELFDE <br> MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilestonePath</td>
        <td>Mijlpad</td>
        <td>MPATH | Mijlpad</td>
        <td>MILESTONEPATHS_CURRENT <br> MILESTONEPATHS_DAILY_HISTORY <br> MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID <br> LASTUPDATEDBYID <br> MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID <br> USER_CURRENT | USERID <br> Zelf</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>Bron voor niet-arbeid</td>
        <td>NLBR | Bron voor niet-arbeid</td>
        <td>NONLABORRESOURCES_CURRENT <br> NONLABORRESOURCES_DAILY_HISTORY <br> NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID <br> NONLABORRESOURCEID (zelf) <br> ENTEREDBYID <br> HOMEGROUPID <br> LASTUPDATEDBYID <br> NONLABORRESOURCECATEGORYID <br> SYSID  </td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORYID <br> Zelf <br> USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID <br> USERS_CURRENT | USERID <br> niet-arbeidsLijst van het Middel momenteel niet gesteund <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Niet-arbeidsuitrustingscategorie</td>
        <td>Niet-arbeidsuitrustingscategorie</td>
        <td>NLBRCY | Broncategorie voor niet-arbeid</td>
        <td>NLBRCATEGORIES_CURRENT <br> NLBRCATEGORIES_DAILY_HISTORY <br> NLBRCATEGORIES_EVENT</td>
        <td>CATEGORYID <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> NLBRCATEGORYID (zelf) <br> PRIVATERATECARDID <br> SCHEDULEID <br> SYSID</td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORIE <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> Zelf <br> RATECARD_CURRENT | RATECARDID <br> USERS_CURRENT | USERID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Onwerkdag</td>
        <td>Uitzondering schema</td>
        <td>NONWKD | Onwerkdag</td>
        <td>NONWORKDAYS_CURRENT <br> NONWORKDAYS_DAILY_HISTORY <br> NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (zelf) <br> OBJID <br> SCHEDULEID <br> SYSID <br> GEBRUIKERSNAAM  </td>
        <td>Zelf <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> wordt geïdentificeerd SCHEDULES_CURRENT | SCHEDULEID <br> Geen relatie; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Opmerking</td>
        <td>Opmerking</td>
        <td>OPMERKING | Opmerking</td>
        <td>NOTES_CURRENT <br> NOTES_DAILY_HISTORY <br> NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID <br> ATTACHOBJID <br> ATTACHOPTASKID <br> ATTACHWORKID <br> ATTACHWORKUSERID <br> AUDITRECORDID <br> COMPANYID <br> DOCUMENTID <br> EXTERNALSERVICEID <br> ITERATIONID <br> NOTEID <br> OBJID <br> OPTASKID <br> OWNERID <br> PARENTENDORSEMENTID <br> PARENTJOURNALENTRYID <br> PARENTNOTEID <br> PORTFOLIOID <br> PROGRAMID VAN HET PROJECT <br> PROJECTID <br> PROOFID <br> RICHTEXTNOTEID <br> TASKID <br> TEMPLATEID <br> TEMPLATETASKID <br> THREADID <br> TIMESHEETID <br> TOPOBJID <br> GEBRUIKERSNAAM<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID <br> Variabele afhankelijk van ATTACHOBJCODE <br> OPTASK_CURRENT | OPTASKID <br> WORKITEMS_CURRENT <br> USER_CURRENT | USERID <br> Lijst van het Verslag van de Controle niet momenteel <br> COMPANIES_CURRENT wordt gesteund | COMPANYID <br> DOCUMENT_CURRENT | DOCUMENTID <br> niet een verhouding van Workfront; gebruikt voor integratie aan externe systemen <br> ITERATIONS_CURRENT | ITERATIONID <br> Zelf <br> Variabel afhankelijk van NOTEOBJCODE <br> OPTASK_CURRENT | OPTASKID <br> USER_CURRENT | USERID <br> de geen lijst van de Bevestiging momenteel <br> JOURNALENTRIES_CURRENT wordt gesteund | JOURNALENTRYID <br> NOTE_CURRENT | NOTEID <br> PORTFOLIO_CURRENT | PORTFOLIOID <br> PROGRAM_CURRENT | PROGRAMID <br> PROJECT_CURRENT | PROJECTID <br> lijst van de Actie van het Bewijs momenteel niet gesteund <br> lijst van het Bewijs momenteel niet <br> RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID <br> TASK_CURRENT | TASKID <br> TEMPLATES_CURRENT | TEMPLATEID <br> TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> NOTE_CURRENT | NOTEID <br> TIMESHEET_CURRENT | TIMESHEETID <br> Variabele afhankelijk van TOPOBJCODE <br> USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Objectintegratie</td>
        <td>Objectintegratie</td>
        <td>OBJINT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT <br> OBJECTINTEGRATION_DAILY_HISTORY <br> OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID <br> OBJECTINTEGRATIONID   (zelf) <br> OBJID <br> SYSID  </td>
        <td>Identiteitskaart van het voorwerp dat in het gebied LINKEDOBJECTCODE <br> wordt geïdentificeerd Zelf <br> identiteitskaart van het voorwerp dat in het gebied OBJCODE <br> wordt geïdentificeerd geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Objectcategorie</td>
        <td>Objectcategorieën</td>
        <td>OBJCAT | Objectcategorie</td>
        <td>OBJECTSCATEGORIES_CURRENT <br> OBJECTSCATEGORIES_DAILY_HISTORY <br> OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID <br> OBJECTSCATEGORYID (zelf) <br> OBJID <br> SYSID  </td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORYID <br> Zelf <br> identiteitskaart van het voorwerp dat in het gebied OBJCODE <br> wordt geïdentificeerd geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Uitgave, verzoek</td>
        <td>OPTASK | Probleem</td>
        <td>OPTASKS_CURRENT <br> OPTASKS_DAILY_HISTORY <br> OPTASKS_EVENT <br> OPTASKS_CUSTOM_VALUE_CURRENT <br> OPTASKS_CUSTOM_VALUE_DAILY_HISTORY <br> OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>DE GOEDKEURING <br> TOEGEWEZENDE <br> CATEGORYID <br> CURRENTAPPROVALSTEPID <br> ENTEREDBYID <br> EXCHANGERATEID <br> ITERATIONID <br> KANBANBOARDID <br> LASTCONDITIONNOTEID <br> LASTNOTEID <br> LASTUPDATEDBATE} YID <br> OPTASKID <br> OWNERID <br> PROJECTID <br> QUEUEDEFID <br> QUEUETOPICID <br> RESOLVEOPTASKID <br> RESOLVEPROJECTID <br> RESOLVETASKID <br> RESOLVINGOBJID 19} ROLEID <br> SOURCEOBJID <br> SOURCETASKID <br> SUBMITTEDBYID <br> TEAMID<br></td>
        <td>METHODES_CURRENT | GOEDKEURINGSPESSID <br> USER_CURRENT | USERID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> GOEDKEURINGSSTEPS_CURRENT | GOEDGEKEURDE <br> USER_CURRENT | USERID <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> ITERATIONS_CURRENT | ITERATIONID <br> de lijst van de Raad Kanban die momenteel niet <br> NOTE_CURRENT wordt gesteund | NOTEID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> Zelf <br> USER_CURRENT | USERID <br> PROJECT_CURRENT | PROJECTID <br> lijst van de Definitie van de Rij die momenteel niet <br> Lijst van het Onderwerp van de Rij wordt gesteund momenteel niet <br> OPTASK_CURRENT | OPTASKID <br> PROJECT_CURRENT | PROJECTID <br> TASK_CURRENT | TASKID <br> Variabele afhankelijk van RESOLVINGOBJCODE <br> ROLE_CURRENT | ROLEID <br> Variabele afhankelijk van SOURCEOBJCODE <br> TASK_CURRENT | TASKID <br> USER_CURRENT | USERID <br> TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Parameter</td>
        <td>Aangepast veld</td>
        <td>PARAM | Parameter</td>
        <td>PARAMETERS_CURRENT <br> PARAMETERS_DAILY_HISTORY <br> PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID <br> PARAMETERFILTERID <br> PARAMETERID (zelf) <br> SYSID  </td>
        <td>USERS_CURRENT | De lijst van de Filter van de Gebruiker <br> Parameter die momenteel niet <br> Zelf <br> wordt gesteund geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Parameteroptie</td>
        <td>Parameteroptie</td>
        <td>POPT | Parameteroptie</td>
        <td>PARAMETEROPTIONS_CURRENT <br> PARAMETEROPTIONS_DAILY_HISTORY <br> PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID <br> PARAMETEROPTIONID (zelf) <br> SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Poortsectie</td>
        <td>Rapport</td>
        <td>PTLSEC | Rapport</td>
        <td>PORTALSECTIONS_CURRENT <br> PORTALSECTIONS_DAILY_HISTORY <br> PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID <br> ENTEREDBYID <br> FILTERID <br> GROUPBYID <br> LASTUPDATEDBYID <br> LASTVIEWEDBYID <br> OBJID <br> PORTALSECTIONID (zelf) <br> VOORKEUREN <br> PUBLIEKUNASUSERID <br> REPORTFOLDERID {1 RUNASUSERID <br> SCHEDULEDREPORTID <br> SYSID <br> VIEWID<br></td>
        <td>Geen relatie; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> UIFILTERS_CURRENT | FILTERID <br> UIGROUPBYS_CURRENT | GROUPBYID <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat op het gebied OBJOBJCODE <br> wordt geïdentificeerd Zelf <br> PREFERENCES_CURRENT | VOORKEUR <br> USERS_CURRENT | USERID <br> REPORTFOLDERS_CURRENT | REPORTFOLDERID <br> USERS_CURRENT | USERID <br> Geplande Lijst van het Rapport momenteel niet gesteund <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Portal, tabblad</td>
        <td>Dashboard</td>
        <td>PTLTAB | Dashboard</td>
        <td>PORTALTABS_CURRENT <br> PORTALTABS_DAILY_HISTORY <br> PORTALTABS_EVENT</td>
        <td>DOCID <br> LASTUPDATEDBYID <br> PORTALPROFILEID <br> PORTALTABID (zelf) <br> SYSID <br> GEBRUIKERS</td>
        <td>Geen relatie; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | DE GEBRUIKERSNAAM <br> Poortlijst van het Profiel zal niet <br> Zelf <br> worden gesteund geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Sectie tabblad Portal</td>
        <td>Sectie dashboard</td>
        <td>PRTBSC | Sectie tabblad Portal</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT <br> PORTALTABSPORTALSECTIONS_DAILY_HISTORY <br> PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID <br> EXTERNALSECTIONID <br> INTERNALSECTIONID <br> PORTALSECTIONOBJID <br> PORTALTABID <br> PORTALTABSECTIONID (zelf) <br> SYSID</td>
        <td>De sectie van het Portaal van de kalender die momenteel niet wordt gesteund <br> Externe Sectielijst niet momenteel <br> PORTALSECTIONS_CURRENT | PORTALSECTIONID <br> identiteitskaart van het voorwerp dat in het PORTALSECTIONOBJCODE- gebied <br> wordt geïdentificeerd PORTALTABS_CURRENT | PORTALTABID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Laatste lezers rapporteren</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT <br> REPORTLASTVIEWERS_DAILY_HISTORY <br> REPORTLASTVIEWERS_EVENT</td>
        <td>RAPPORTID <br> REPORTLASTVIEWERID (zelf) <br> SYSID <br> VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br> REPORTLASTVIEWERID (zelf) <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>POORT | Portfolio</td>
        <td>PORTFOLIOS_CURRENT <br> PORTFOLIOS_DAILY_HISTORY <br> PORTFOLIOS_EVENT <br> PORTFOLIOS_CUSTOM_VALUE_CURRENT <br> PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY <br> PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID <br> CATEGORYID <br> ENTEREDBYID <br> GROUPID <br> LASTUPDATEDBYID <br> EIWNERID <br> PORTFOLIOID</td>
        <td>De lijst van het scorebord die momenteel niet <br> CATEGORIEËN_CURRENT wordt gesteund | CATEGORYID <br> USER_CURRENT | USERID <br> GROUP_CURRENT | GROUPID <br> USER_CURRENT | USERID <br> USER_CURRENT | USERID <br> Zelf</td>
    </tr>
    <tr>
        <td>Voorkeur</td>
        <td>Weergeven, Filteren, Groeperen, Rapportdefinitie</td>
        <td>PROSET | Voorkeur</td>
        <td>PREFERENCES_CURRENT <br> PREFERENCES_DAILY_HISTORY <br> PREFERENCES_EVENT</td>
        <td>APPGLOBALID <br> VOORKEUR (zelf) <br> SYSID  </td>
        <td>Niet een verband; gebruikt voor interne toepassingsdoeleinden <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Programma</td>
        <td>Programma</td>
        <td>PRGM | Programma</td>
        <td>PROGRAMS_CURRENT <br> PROGRAMMS_DAILY_HISTORY <br> PROGRAMS_EVENT <br> PROGRAMS_CUSTOM_VALUE_CURRENT <br> PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY <br> PROGRAMMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID <br> ENTEREDBYID <br> GROUPID <br> LASTUPDATEDBYID <br> OWNERID <br> PORTFOLIOID <br> PROGRAMID</td>
        <td>CATEGORIEËN_HUIDIGE | CATEGORIE <br> USER_CURRENT | USERID <br> GROUP_CURRENT | GROUPID <br> USER_CURRENT | USERID <br> USER_CURRENT | USERID <br> PORTFOLIO_CURRENT | PORTFOLIOID <br> Zelf</td>
    </tr>
    <tr>
        <td>Project</td>
        <td>Project</td>
        <td>PROJ | Project</td>
        <td>PROJECTS_CURRENT <br> PROJECTS_DAILY_HISTORY <br> PROJECTS_EVENT <br> PROJECTS_CUSTOM_VALUE_CURRENT <br> PROJECTS_CUSTOM_VALUE_DAILY_HISTORY <br> PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID <br> ALIGNMENTSCORECARDID <br> GOEDKEURINGPROCESSID <br> ATTACHEDRATECARDID <br> CATEGORYID <br> COMPANYID <br> CONVERTEDOPTASKID <br> CONVERTEDOPTASKORIGINATORID <br> CURRENTAPPROVALSTEPSTPSTPTAPTAPSTPTAPTAPTAPSTPROPROSTPROSTAPSTPROPROPROPROPROPROPROSTRED ID <br> LEVERABLESCORECARDID <br> ENTEREDBYID <br> GROUPID <br> LASTCONDITIONNOTEID <br> LASTNOTEID <br> LASTUPDATEDBYID <br> MILESTONEPATHID <br> OWNERID <br> PACCOUNTID <br> PORTFOLIOID <br> PRIVATERATECARDID <br> PROGRAMID <br> PROJECTID <br> QUEUEDEFID <br> REJECTIONISSUEID <br> RESOURCEPOLID <br> SCHEDULEID <br> SPONSORID <br> SUBMITTEDBYID <br> TEAMID <br> TEMPLATEID</td>
        <td>Geen relatie van Workfront; gebruikt voor integratie aan externe systemen <br> Scorecard lijst momenteel niet gesteund <br> GOEDKEURINGPROCESSES_CURRENT | ERKVALPROCESSID <br> RATECARD_CURRENT | RATECARDID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> COMPANIES_CURRENT | COMPANYID <br> OPTASK_CURRENT | OPTASKID <br> USER_CURRENT | USERID <br> GOEDKEURINGSSTEPS_CURRENT | GOEDGEKEURDE <br> Scorecard- lijst momenteel niet gesteund <br> USER_CURRENT | USERID <br> GROUP_CURRENT | GROUPID <br> NOTE_CURRENT | NOTEID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> MILESTONEPATH_CURRENT | MILESTONEPATHID <br> USER_CURRENT | USERID <br> Pop de lijst van de Rekening momenteel niet gesteund <br> PORTFOLIO_CURRENT | PORTFOLIOID <br> RATECARD_CURRENT | RATECARDID <br> PROGRAM_CURRENT | PROGRAMID <br> Zelf <br> lijst van de Definitie van de Rij die momenteel niet wordt gesteund <br> OPTASK_CURRENT | OPTASKID <br> RESOURCEPOLS_CURRENT | RESOURCEPOLID <br> SCHEDULE_CURRENT | SCHEDULEID <br> USER_CURRENT | USERID <br> USER_CURRENT | USERID <br> TEAM_CURRENT | TEAMID <br> TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Projectteamgebruiker</td>
        <td>Projectteamgebruiker</td>
        <td>PRTU | Projectgebruiker</td>
        <td>PROJECTSUSERS_CURRENT <br> PROJECTSUSERS_DAILY_HISTORY <br> PROJECTSUSERS_EVENT</td>
        <td>PROJECTID <br> PROJECTSUSERID (zelf) <br> SYSID <br> TMPUSERID <br> GEBRUIKERSNAAM</td>
        <td>PROJECTS_CURRENT | PROJECTID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEMPLATES_CURRENT | TEMPLATEID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Gebruikersrol projectteam</td>
        <td>Gebruikersrol projectteam</td>
        <td>PTEAM | ProjectUserRole</td>
        <td>PROJECTSUSERSROLES_CURRENT <br> PROJECTSUSERSROLES_DAILY_HISTORY <br> PROJECTSUSERSROLES_EVENT</td>
        <td>PROJECTID <br> PROJECTSUSERSROLEID (zelf) <br> ROLEID <br> SYSID <br> GEBRUIKERSNAAM</td>
        <td>PROJECTS_CURRENT | PROJECTID <br> Zelf <br> ROLES_CURRENT | ROLEID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Creditcard</td>
        <td>RTCRD |Creditcard</td>
        <td>RATECARD_CURRENT <br> RATECARD_DAILY_HISTORY <br> RATECARD_EVENT</td>
        <td>CATEGORYID <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> RATECARDID (zelf) <br> SECURITYROOTID <br> SOURCEID <br> SYSID</td>
        <td>CATEGORIE <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID    <br> Zelf <br> identiteitskaart van het voorwerp dat op het gebied SECURITYOBJCODE <br> wordt geïdentificeerd identiteitskaart van het voorwerp dat in het gebied SOURCEOBJCODE <br> wordt geïdentificeerd geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Rapportmap</td>
        <td>Rapportmap</td>
        <td>RPTFDR | Rapportmap</td>
        <td>REPORTFOLDERS_CURRENT <br> REPORTFOLDERS_DAILY_HISTORY <br> REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID (zelf) <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Statistisch aantal rapportweergave</td>
        <td>Statistisch aantal rapportweergave</td>
        <td>PLSVST | PortalSectionStatisticInfo</td>
        <td>REPORTVIEWSTATISTICCOUNTS_CURRENT <br> REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY <br> REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        <td>RAPPORTID <br> REPORTVIEWSTATISTICCOUNTID (zelf) <br> SYSID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Te rapporteren begrotingsuren</td>
        <td>Te rapporteren begrotingsuren</td>
        <td>RPBGHR | Budgeted Hour</td>
        <td>REPORTABLEBUDGETEDHOURS_CURRENT <br> REPORTABLEBUDGETEDHOURS_DAILY_HISTORY <br> REPORTABLEBUDGETEDHOURS_EVENT</td>
        <td>PROJECTID <br> REPORTABLEBUDGETEDHOURID (zelf) <br> ROLEID <br> SYSID <br> GEBRUIKERSNAAM</td>
        <td>PROJECTS_CURRENT | PROJECTID <br> Zelf <br> ROLES_CURRENT | ROLEID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Gereserveerde tijd</td>
        <td>(Persoonlijk) Tijd weg</td>
        <td>HERVATTEN | Tijd uit</td>
        <td>RESERVEDTIMES_CURRENT <br> RESERVEDTIMES_DAILY_HISTORY <br> RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID (zelf) <br> SYSID <br> TASKID <br> GEBRUIKERSNAAM</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Resource Manager</td>
        <td>Resource Manager</td>
        <td>RESMGR | Resource Manager</td>
        <td>RESOURCEMANAGERS_CURRENT <br> RESOURCEMANAGERS_DAILY_HISTORY <br> RESOURCEMANAGERS_EVENT</td>
        <td>ID (zelf) <br> PROJECTID <br> RESOURCEMANAGERID <br> SYSID <br> TEMPLATEID</td>
        <td>Zelf <br> PROJECTS_CURRENT | PROJECTID <br> USERS_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Bronpool</td>
        <td>Bronpool</td>
        <td>RSPL | Bronpool</td>
        <td>RSRCPOOLS_CURRENT <br> RSRCPOOLS_DAILY_HISTORY <br> RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID <br> LASTUPDATEDBYID <br> RESOURCEPOLID (zelf) <br> SYSID  </td>
        <td>USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>RTF-notitie</td>
        <td>RTF-notitie</td>
        <td>RHNOTE | RTF-notitie</td>
        <td>RESERVEDTEXTNOTES_CURRENT <br> RESERVEDTEXTNOTES_DAILY_HISTORY <br> RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID (zelf) <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Waarde van RTF-parameter</td>
        <td>Waarde van RTF-parameter</td>
        <td>RCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT <br> RICHTEXTPARAMETERVALUES_DAILY_HISTORY <br> RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID <br> RICHTEXTPARAMETERVALUEID (zelf) <br> SYSID  </td>
        <td>De lijst van de Waarde van Paramter die momenteel niet <br> Zelf <br> wordt gesteund geen verhouding; gebruikt voor interne toepassingsdoeleinden  </td>
    </tr>
    <tr>
        <td>Risico</td>
        <td>Risico</td>
        <td>RISICO | Risico</td>
        <td>RISKS_CURRENT <br> RISKS_DAILY_HISTORY <br> RISKS_EVENT</td>
        <td>ENTEREDBYID <br> EXCHANGERATEID <br> LASTUPDATEDBYID <br> PROJECTID <br> RISKID (zelf) <br> RISKTYPEID <br> SYSID <br> TEMPLATEID</td>
        <td>USERS_CURRENT | USERID <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> USERS_CURRENT | USERID <br> PROJECTS_CURRENT | PROJECTIEF   <br> Zelf <br> RISKTYPES_CURRENT | RISKTYPEID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Type risico</td>
        <td>Type risico</td>
        <td>RSKTYP | Type risico</td>
        <td>RISKTYPES_CURRENT <br> RISKTYPES_DAILY_HISTORY <br> RISKTYPES_EVENT</td>
        <td>RISKTYPEID <br> SYSID</td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Rol</td>
        <td>Functie</td>
        <td>ROL | Functie</td>
        <td>ROLES_CURRENT <br> ROLES_DAILY_HISTORY <br> ROLES_EVENT</td>
        <td>ENTEREDBYID <br> LAYOUTTEMPLATEID <br> PRIVATERATECARDID <br> ROLEID <br> UITEMPLATEID</td>
        <td>USER_CURRENT | DE GEBRUIKERSNAAM <br> lijst van het Malplaatje van de Lay-out zal niet <br> RATECARD_CURRENT worden gesteund | RATECARDID <br> Zelf <br> UITEMPLATES_CURRENT |VERENIGD</td>
    </tr>
    <tr>
        <td>Schema</td>
        <td>Schema</td>
        <td>GEPLAND | Schema</td>
        <td>SCHEDULES_CURRENT <br> SCHEDULES_DAILY_HISTORY <br> SCHEDULES_EVENT</td>
        <td>ENTEREDBYID <br> GROUPID <br> HOMEGROUPID <br> SCHEDULEID</td>
        <td>USER_CURRENT | USERID <br> GROUP_CURRENT | GROUPID <br> GROUP_CURRENT | GROUPID <br> Zelf</td>
    </tr>
    <tr>
        <td>Stap fiatteur</td>
        <td>Stap fiatteur</td>
        <td>SPAPVR | Stage-fiatteur</td>
        <td>STEPAPPROVERS_CURRENT <br> STEPAPPROVERS_DAILY_HISTORY <br> STEPAPPROVERS_EVENT</td>
        <td>GOEDGEKEURDE <br> ROLEID <br> STEPAPPROVERID (zelf) <br> SYSID <br> TEAMID <br> GEBRUIKERSNAAM</td>
        <td>METHOVALSTEPS_CURRENT | GOEDGEKEURDE <br> ROLES_CURRENT | ROLEID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEAMS_CURRENT | TEAMID <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Taak</td>
        <td>Taak</td>
        <td>TAAK | Taak</td>
        <td>TASKS_CURRENT <br> TASKS_DAILY_HISTORY <br> TASKS_EVENT <br> TASKS_CUSTOM_VALUE_CURRENT <br> TASKS_CUSTOM_VALUE_DAILY_HISTORY <br> TASKS_CUSTOM_VALUE_EVENT</td>
        <td>DE GOEDKEURINGPROCESSID <br> BILLINGRECORDID <br> CATEGORYID <br> CONVERTEDOPTASKID <br> CONVERTEDOPTASKORIGINATORID <br> CURRENTAPPROVALSTEPID <br> ENTEREDBYID <br> EXCHANGERATEID <br> GROUPID 9} ITERATIONID <br> KANBANBOARDID <br> LASTCONDITIONNOTEID <br> LASTNOTEID <br> LASTUPDATEDBYID <br> MILESTONEID <br> PARENTID <br> PROJECTID <br> RECURRENCERULEID <br> JECTIONISSUEID <br> RESERVEDTIMEID <br> ROLEID <br> SUBMITTEDBYID <br> TASKID <br> TEAMID <br> TEMPLATETASKID<br><br></td>
        <td>METHODES_CURRENT | GOEDKEURINGSPESSID <br> USER_CURRENT | USERID <br> BILLINGRECORDS_CURRENT | BILLINGRECORDID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> OPTASK_CURRENT | OPTASKID <br> USER_CURRENT | USERID <br> GOEDKEURSTEPS_CURRENT | GOEDGEKEURDE <br> USER_CURRENT | USERID <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> GROUP_CURRENT | GROUPID <br> ITERATIONS_CURRENT | ITERATIONID <br> de lijst van de Raad Kanban die momenteel niet <br> NOTE_CURRENT wordt gesteund | NOTEID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> MILESTONE_CURRENT | MILESTONEID <br> TASK_CURRENT | TASKID <br> PROJECT_CURRENT | PROJECTID <br> lijst van de Regel van de Herhaling niet momenteel <br> OPTASK_CURRENT gesteund | OPTASKID <br> RESERVEDTIMES_CURRENT | RESERVEDTIMEID <br> ROLE_CURRENT | ROLEID <br> USER_CURRENT | USERID <br> Zelf <br> TEAM_CURRENT | TEAMID <br> TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Taakvoorganger</td>
        <td>Voorganger</td>
        <td>PRED | Voorganger</td>
        <td>PREDECESSORS_CURRENT <br> PREDECESSORS_DAILY_HISTORY <br> PREDECESSORS_EVENT</td>
        <td>ID (zelf) <br> PREDECESSORID <br> SUCCESSORID <br> SYSID</td>
        <td>Zelf <br> TASKS_CURRENT | TASKID <br> TASKS_CURRENT | TASKID <br> Geen relatie; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Team</td>
        <td>TEAMOB | Team</td>
        <td>TEAMS_CURRENT <br> TEAMS_DAILY_HISTORY <br> TEAMS_EVENT</td>
        <td>ENTEREDBYID <br> GROUPID <br> LAYOUTTEMPLATEID <br> MYWORKVIEWID <br> OWNERID <br> REQUESTSVIEWID <br> SCHEDULEID <br> TEAMID <br> UITEMPLATEID</td>
        <td>USER_CURRENT | USERID <br> GROUP_CURRENT | De GROUPID <br> lijst van het Malplaatje van de Lay-out zal niet <br> UIVIEWS_CURRENT worden gesteund | UIVIEWID <br> USER_CURRENT | USERID <br> UIVIEWS_CURRENT | UIVIEWID <br> SCHEDULE_CURRENT | SCHEDULEID <br> Zelf <br> UITEMPLATES_CURRENT |VERENIGD</td>
    </tr>
    <tr>
        <td>Teamlid</td>
        <td>Overige teams, teamlid</td>
        <td>TEAMMB | Teamlid</td>
        <td>TEAMMEMBERS_CURRENT <br> TEAMMEMBERS_DAILY_HISTORY <br> TEAMMEMBERS_EVENT</td>
        <td>SYSID <br> TEAMID <br> TEAMMEMBERID (zelf) <br> GEBRUIKERSNAAM</td>
        <td>Geen relatie; gebruikt voor interne toepassingsdoeleinden <br> TEAMS_CURRENT | TEAMID <br> Zelf <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Functie teamlid</td>
        <td>TEAMMR | Functie teamlid</td>
        <td>TEAMMEMBERROLES_CURRENT <br> TEAMMEMBERROLES_EVENT<br></td>
        <td>ROLEID <br> TEAMID <br> TEAMMEMBERROLEID (zelf) <br> GEBRUIKERSNAAM</td>
        <td>ROLES_CURRENT | ROLEID <br> TEAMS_CURRENT | TEAMID <br> Zelf <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Sjabloon</td>
        <td>Sjabloon</td>
        <td>TMPL | Sjabloon</td>
        <td>TEMPLATES_CURRENT <br> TEMPLATES_DAILY_HISTORY <br> TEMPLATES_EVENT</td>
        <td>GOEDKEURSTPROCESSID <br> COMPANYID VAN DE CATEGORIE <br> LEVERABLESCORECARDID <br> ENTEREDBYID <br> GROUPID <br> LASTNOTEID <br> LASTUPDATEDBYID <br> MILESTONEPATHID <br> EIWNERID <br> PRIVATERADCARDID ID <br> PROGRAMID <br> QUEUEDEFID <br> SCHEDULEID <br> SYSID <br> TEAMID <br> TEMPLATEID (zelf)<br></td>
        <td>METHODES_CURRENT | GOEDKEURINGSPROESSID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> COMPANIES_CURRENT | COMPANYID   <br> DELIVERABLESCORECARDID <br> USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID <br> NOTES_CURRENT | NOTEID <br> USERS_CURRENT | USERID <br> MILESTONEPATH_CURRENT | MILESTONEPATHID <br> USERS_CURRENT | USERID <br> RATECARD_CURRENT | RATECARDID <br> PROGRAM_CURRENT | PROGRAMID <br> lijst van de Definitie van de Rij niet momenteel <br> SCHEDULES_CURRENT wordt gesteund | SCHEDULEID <br> Geen relatie; gebruikt voor interne toepassingsdoeleinden <br> TEAMS_CURRENT | TEAMID <br> Zelf</td>
    </tr>
    <tr>
        <td>Sjabloontoewijzing</td>
        <td>Sjabloontoewijzing</td>
        <td>TASSGN | Sjabloontoewijzing</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT <br> TEMPLATEASSIGNMENTS_DAILY_HISTORY <br> TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID <br> CATEGORYID <br> LASTUPDATEDBYID <br> OBJID <br> ROLEID <br> SYSID <br> TEAMTIMELINEABLEID <br> TEAMTIMELINEABLEID <br> TEMPLATEASSIGNMENTID (zelf) <br> TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> wordt geïdentificeerd ROLES_CURRENT | ROLEID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEAMS_CURRENT | TEAMID <br> Eigen lijst van het Team niet die momenteel <br> Zelf <br> TEMPLATETASKS_CURRENT wordt gesteund |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Sjabloontaak</td>
        <td>Sjabloontaak</td>
        <td>TTSK | Sjabloontaak</td>
        <td>TEMPLATETASKS_CURRENT <br> TEMPLATETASKS_DAILY_HISTORY <br> TEMPLATETASKS_EVENT</td>
        <td>GOEDKEURINGSPROCESSID <br> ASSIGNEDTOID <br> CATEGORYID <br> ENTEREDBYID <br> EXCHANGERATEID <br> LASTNOTEID <br> LASTUPDATEDBYID <br> MILESTONEID <br> PARENTID <br> RECURRENCERULEID <br> ROLEID <br> SYSID 1} TEAMID <br> TEAMTIMELINEABLEID <br> TEMPLATEID <br> TEMPLATETASKID (zelf)<br></td>
        <td>METHODES_CURRENT | ERKVALPROCESSID <br> USERS_CURRENT | USERID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> USERS_CURRENT | USERID <br> EXCHANGERATES_CURRENT | EXCHANGERATEID <br> NOTES_CURRENT | NOTEID <br> USERS_CURRENT | USERID <br> MILESTONE_CURRENT | MILESTONEID <br> TEMPLATETASKS_CURRENT |TEMPLATETASKID <br> lijst van de Regel van de Herhaling die momenteel niet <br> ROLES_CURRENT wordt gesteund | ROLEID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TEAMS_CURRENT | TEAMID <br> Tijdlijnbare lijst van het Team niet momenteel gesteund <br> TEMPLATES_CURRENT | TEMPLATEID <br> Zelf</td>
    </tr>
    <tr>
        <td>Sjabloontaakvoorganger</td>
        <td>Sjabloonvoorganger</td>
        <td>TPRED | Voorganger</td>
        <td>TEMPLATEPREDECESSORS_CURRENT <br> TEMPLATEPREDECESSORS_DAILY_HISTORY <br> TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID <br> SUCCESSORID <br> TEMPLATEPREDECESSORID (zelf) <br> SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br> TEMPLATETASKS_CURRENT |TEMPLATETASKID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
       <tr>
        <td>Tijdgefaseerde KPI-valuta (beperkte beschikbaarheid van klanten)</td>
        <td>Tijd-gefaseerde KPI</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMESHEETS_CURRENT <br> TIMESHEETS_DAILY_HISTORY <br> TIMESHEETS_EVENT</td>
        <td>GOEDGEKEURDE <br> LASTUPDATEDBYID <br> TIMESHEETID <br> TIMESHEETPROFILEID <br> GEBRUIKERID<br></td>
        <td>USER_CURRENT | USERID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> ZELFDE <br> TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID <br> USER_CURRENT | USERID</td>
    </tr>
        <tr>
        <td>Tijd-gefaseerde Duur van KPI (beperkte klantenbeschikbaarheid)</td>
        <td>Tijd-gefaseerde KPI</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMEPHASED_DURATION_CURRENT <br> TIMEPHASED_DURATION_DAILY_HISTORY <br> TIMEPHASED_DURATION_EVENT</td>
        <td>ASSIGNMENTID <br> LOCATIONID <br> OPTASKID <br> PORTFOLIOID <br> PROGRAMMA <br> PROJECTID <br> VERWIJZING <br> ROLEID <br> SOURCETASKID <br> TIMEPHASEDDURATIONID (zelf) <br> GEBRUIKERS ID<br><br></td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br> GROUPS_CURRENT | GROUPID <br> CLASSIFIER_CURRENT | CLASSIFIERID <br> OPTASKS_CURRENT | OPTASKID <br> PORTFOLIOS_CURRENT | PORTFOLIOID <br> PROGRAMS_CURRENT | PROGRAMID <br> PROJECTS_CURRENT | PROJECTID <br> identificeert het onderwerp van het KPI- verslag <br> ROLES_CURRENT | ROLEID <br> TASKS_CURRENT | TASKID <br> TASKS_CURRENT | TASKID <br> Zelf <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tijdschema</td>
        <td>Tijdschema</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMEPHASED_CURRENCY_CURRENT <br> TIMEPHASED_CURRENCY_DAILY_HISTORY <br> TIMEPHASED_CURRENCY_EVENT</td>
        <td>ASSIGNMENTID <br> LOCATIONID <br> OPTASKID <br> PORTFOLIOID <br> PROGRAMMA <br> PROJECTID <br> VERWIJZING <br> ROLEID <br> SOURCETASKID <br> TIMEPHASEDCURRENCYID (zelf) <br> USSKID ERID<br><br></td>
        <td>USER_CURRENT | USERID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> ZELFDE <br> TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID <br> USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tijdbladprofiel</td>
        <td>Tijdbladprofiel</td>
        <td>TSPRO | Tijdbladprofiel</td>
        <td>TIMESHEETPROFILES_CURRENT <br> TIMESHEETPROFILES_DAILY_HISTORY <br> TIMESHEETPROFILES_EVENT</td>
        <td>GOEDGEKEURDE <br> ENTEREDBYID <br> GROUPID <br> SYSID <br> TIMESHEETPROFILEID (zelf)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br> GROUPS_CURRENT | GROUPID <br> CLASSIFIER_CURRENT | CLASSIFIERID <br> OPTASKS_CURRENT | OPTASKID <br> PORTFOLIOS_CURRENT | PORTFOLIOID <br> PROGRAMS_CURRENT | PROGRAMID <br> PROJECTS_CURRENT | PROJECTID <br> identificeert het onderwerp van het KPI- verslag <br> ROLES_CURRENT | ROLEID <br> TASKS_CURRENT | TASKID <br> TASKS_CURRENT | TASKID <br> Zelf <br> USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>UI-filter</td>
        <td>Filter</td>
        <td>UIFT | Filter</td>
        <td>UIFILTERS_CURRENT <br> UIFILTERS_DAILY_HISTORY <br> UIFILTERS_EVENT</td>
        <td>APPGLOBALID <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> OBJID <br> VOORKEUR <br> SYSID <br> (zelf)</td>
        <td>Geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> PREFERENCES_CURRENT wordt geïdentificeerd | PREFERENCEID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> Zelf</td>
    </tr>
    <tr>
        <td>UI-groep door</td>
        <td>Groepering</td>
        <td>UIGB | Groepering</td>
        <td>UIGROUPBYS_CURRENT <br> UIGROUPBYS_DAILY_HISTORY <br> UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID <br> GROUPID <br> LASTUPDATEDBYID <br> SYSID <br> UITEMPLATEID (zelf)</td>
        <td>USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID <br> USERS_CURRENT | USERID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> Zelf</td>
    </tr>
    <tr>
        <td>UI-sjabloon</td>
        <td>Lay-outsjabloon</td>
        <td>UITMPL | Lay-outsjabloon</td>
        <td>UITEMPLATES_CURRENT <br> UITEMPLATES_DAILY_HISTORY <br> UITEMPLATES_EVENT</td>
        <td>APPGLOBALID <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> OBJID <br> VOORKEUR <br> SYSID <br> UIGROUPBYID (zelf)</td>
        <td>Geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> PREFERENCES_CURRENT wordt geïdentificeerd | PREFERENCEID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> Zelf</td>
    </tr>
    <tr>
        <td>UI-weergave</td>
        <td>Weergave</td>
        <td>UIVIEW | Weergave</td>
        <td>UIVIEWS_CURRENT <br> UIVIEWS_DAILY_HISTORY <br> UIVIEWS_EVENT</td>
        <td>APPGLOBALID <br> ENTEREDBYID <br> LASTUPDATEDBYID <br> OBJID <br> VOORKEUR <br> SYSID <br> UIVIEWID (zelf)</td>
        <td>Geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> USERS_CURRENT | USERID <br> identiteitskaart van het voorwerp dat op het gebied OBJCODE <br> PREFERENCES_CURRENT wordt geïdentificeerd | PREFERENCEID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> Zelf</td>
    </tr>
    <tr>
        <td>Gebruiker</td>
        <td>Gebruiker</td>
        <td>GEBRUIKER | Gebruiker</td>
        <td>USERS_CURRENT <br> USERS_DAILY_HISTORY <br> USERS_EVENT <br> USERS_CUSTOM_VALUE_CURRENT <br> USERS_CUSTOM_VALUE_DAILY_HISTORY <br> USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID <br> COMPANYID VAN DE CATEGORIE VAN DE CATEGORIE <br> DEFAULTHOURTYPEID <br> EAUTHUSERID <br> ENTEREDBYID <br> HOMEGROUPID <br> HOMETEAMID <br> LASTENTEREDNOTEID <br> LASTUPDATEIT YID <br> LATESTUPDATENOTEID <br> LAYOUTTEMPLATEID <br> MANAGERID <br> PORTALPROFILEID <br> PREFUID <br> PRIVATERATECARDID <br> RESOURCEPOLID <br> ROLEID <br> SCHEDULEID <br> TIMESHEETPROFILEID <br> UITEMPLATEID <br> GEBRUIKERSNAAM <br> UMUSERID<br><br></td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID <br> CATEGORIEËN_CURRENT | CATEGORYID <br> COMPANIES_CURRENT | COMPANYID <br> HOURTYPE_CURRENT | HOURTYPEID <br> USER_CURRENT | USERID <br> niet een verhouding; gebruikt voor interne toepassingsdoeleinden <br> USER_CURRENT | USERID <br> GROUP_CURRENT | GROUPID <br> TEAM_CURRENT | TEAMID <br> NOTE_CURRENT | NOTEID <br> USER_CURRENT | USERID <br> NOTE_CURRENT | NOTEID <br> de lijst van het Malplaatje van de Lay-out zal niet <br> USER_CURRENT worden gesteund | USERID <br> Poortlijst van het Profiel zal niet <br> worden gesteund geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> RATECARD_CURRENT | RATECARDID <br> RESOURCEPOLS_CURRENT | RESOURCEPOLID <br> ROLE_CURRENT | ROLEID <br> SCHEDULE_CURRENT | SCHEDULEID <br> TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID <br> UITEMPLATES_CURRENT |UITEMPLATEID <br> Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden</td>
    </tr>
    <tr>
        <td>Gebruikersdelegatie</td>
        <td>Gebruikersdelegatie</td>
        <td>USRDEL | Gebruikersdelegatie</td>
        <td>USERDELEGATIONS_CURRENT <br> USERDELEGATIONS_DAILY_HISTORY <br> USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID <br> SYSID <br> TOUSERID <br> GEBRUIKERSDELEGATIONID (zelf)</td>
        <td>USERS_CURRENT | USERID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> Zelf</td>
    </tr>
    <tr>
        <td>Gebruikersgroep</td>
        <td>Overige groepen</td>
        <td>USRGPS | Gebruikersgroep</td>
        <td>USERSGROUPS_CURRENT <br> USERSGROUPS_DAILY_HISTORY <br> USERSGROUPS_EVENT</td>
        <td>GROUPID <br> SYSID <br> GEBRUIKERSGROUPID <br> (zelf)</td>
        <td>GROUPS_CURRENT | GROUPID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> Zelf</td>
    </tr>
    <tr>
        <td>Locatie gebruiker</td>
        <td>Locatie gebruiker</td>
        <td>USRLOC | UserLocation</td>
        <td>USERLOCATIONS_CURRENT <br> USERLOCATIONS_DAILY_HISTORY <br> USERLOCATIONS_EVENT</td>
        <td>CLASSIFIERID <br> SYSID <br> GEBRUIKERSNAAM <br> (zelf) GEBRUIKERSONDERZOEK</td>
        <td>CLASSIFIER_CURRENT | CLASSIFIERID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> Zelf</td>
    </tr>
    <tr>
        <td>Gebruikersrol</td>
        <td>Andere rollen</td>
        <td>USRROL | Gebruikersrol</td>
        <td>USERSROLES_CURRENT <br> USERSROLES_DAILY_HISTORY <br> USERSROLES_EVENT</td>
        <td>ROLEID <br> SYSID <br> GEBRUIKER    <br> USERROLESETID <br> USERSROLEID (zelf)</td>
        <td>ROLES_CURRENT | ROLEID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID    <br> USERROLESET_CURRENT | USERROLESETID <br> Zelf</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Gebruikersvoorkeur</td>
        <td>USERPREFVALUES_CURRENT <br> USERPREFVALUES_DAILY_HISTORY <br> USERPREFVALUES_EVENT</td>
        <td>SYSID    <br> GEBRUIKERDE <br> USERPREFVALUEID (zelf)</td>
        <td>Geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID    <br> Zelf</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT <br> USERROLESET_DAILY_HISTORY <br> USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br> SYSID <br> USERID    <br> USERROLESETID (zelf)</td>
        <td>ROLES_CURRENT | ROLEID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID <br> Zelf</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>Gebruikersbeslissingen</td>
        <td>USRDEC | Gebruikersbeslissingen</td>
        <td>USERSDECISION_CURRENT <br> USERSDECISION_DAILY_HISTORY <br> USERSDECISION_EVENT</td>
        <td>USERBESLISIONID (zelf) <br> SYSID <br> GEBRUIKERSNAAM  </td>
        <td>Zelf <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Werkitem</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT <br> WORKITEMS_DAILY_HISTORY <br> WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br> OBJID <br> OPTASKID    <br> PROJECTID <br> SYSID <br> TASKID    <br> USERID <br> WORK-ID (zelf)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br> identiteitskaart van het voorwerp dat op het gebied OBJOBJCODE <br> wordt geïdentificeerd OPTASK_CURRENT | OPTASKID    <br> PROJECTS_CURRENT | PROJECTID <br> geen verhouding; gebruikt voor interne toepassingsdoeleinden <br> TASKS_CURRENT | TASKID    <br> USERS_CURRENT | USERID    <br> Zelf </td>
    </tr>
  </tbody>
</table>
