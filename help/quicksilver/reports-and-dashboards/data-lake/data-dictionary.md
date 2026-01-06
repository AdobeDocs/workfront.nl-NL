---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect-gegevenswoordenboek
description: Deze pagina bevat informatie over de structuur en inhoud van de gegevens in Workfront Data Connect.
author: Courtney
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: c669086f5954f9e2cf850887f4100e53c0c3e716
workflow-type: tm+mt
source-wordcount: '8904'
ht-degree: 1%

---

# Workfront Data Connect-gegevenswoordenboek

Deze pagina bevat informatie over de structuur en inhoud van de gegevens in Workfront Data Connect.

>[!NOTE]
>
>De gegevens in Data Connect worden elke 4 uur vernieuwd, zodat recente wijzigingen mogelijk niet direct worden doorgevoerd.

## Typen weergeven

In Data Connect kunt u een aantal weergavetypen gebruiken om uw Workfront-gegevens op een manier weer te geven die de meeste insight biedt.

* **Huidige mening**

  In de huidige weergave worden gegevens op vergelijkbare wijze weergegeven als in Workfront, elk object en de huidige status. U kunt er echter veel minder latentie aan toevoegen dan in Workfront.

* **mening van de Gebeurtenis**

  In de weergave Gebeurtenis wordt elke wijzigingsrecord in Workfront bijgehouden. Elke keer dat een object de status wijzigt, wordt een record gemaakt die aangeeft wanneer de wijziging heeft plaatsgevonden, wie de wijziging heeft aangebracht en wat is gewijzigd. Daarom is deze mening nuttig voor punt-in-tijd vergelijkingen. Dit beeld omvat slechts verslagen van de afgelopen drie jaar.

* **Dagelijkse mening van de Geschiedenis**

  De weergave Dagelijkse historie biedt een verkorte versie van de weergave Gebeurtenis, in die zin dat deze de status van elk object dagelijks weergeeft in plaats van wanneer elke afzonderlijke gebeurtenis plaatsvond. Dit standpunt is als zodanig nuttig voor trendanalyse.

<!-- Custom view -->

## Relatiediagrammen van entiteiten

Objecten in Workfront (en dus ook in het Data Connect Data Lake) worden niet alleen gedefinieerd door hun individuele waarden, maar ook door hun relaties met andere objecten.

De onderstaande ERD&#39;s (eenheidrelaties) bieden een overzicht op hoog niveau van de objectrelaties in Data Connect voor Workfront-kernobjecten.

>[!IMPORTANT]
>
>De diagrammen worden gecentreerd rond afzonderlijke objecten en vertegenwoordigen geen volledig entiteitrelatiediagram voor de volledige Workfront-toepassing. <br>
>Deze diagrammen zijn bedoeld om voorbeelden te geven van hoe de relaties kunnen worden gebruikt om gegevens aan aangrenzende objecten te koppelen.

### Voorbeeld van entiteitrelatiediagrammen

+++ Uitbreiden om de voorbeelddiagrammen weer te geven

>[!TIP]
>
>Om een diagram in meer detail te bekijken, klik op het beeld met de rechtermuisknop aan en selecteer **Open beeld in nieuw lusje**.


### Toewijzingen

![ het diagram van de entiteitverhouding van Taken entiteit ](assets/Assignment-centered-ERD.png)


### Documenten en documentgoedkeuringen

![ Documenten en document goedkeurings entiteitrelatiediagram ](assets/Document-and-Document-Approvals-centered-ERD.png)

### Uren en timesheets

![ Uren en Timesheets entiteitrelatiediagram ](assets/Hours-and-Timesheet-centered-ERD.png)


### Problemen

![ de entiteitrelatiediagram van Kwesties ](assets/Issue-centered-ERD.png)

### Projecten

![ de entiteitrelatiediagram van Projecten ](assets/Project-centered-ERD.png)


### Taken

![ het diagram van de entiteitverhouding van Taken ](assets/Task-centered-ERD.png)


### Gebruikers

![ het diagram van de entiteitverhouding van Gebruikers ](assets/User-centered-ERD.png)

+++

## Datumtypen

Er zijn een aantal datumobjecten die informatie bevatten over wanneer specifieke gebeurtenissen plaatsvinden.

* `DL_LOAD_TIMESTAMP`: Deze datum wordt bijgewerkt nadat de gegevens zijn vernieuwd en bevat de tijdstempel van het begin van de vernieuwingstaak die de laatste versie van een record heeft geleverd.
* `CALENDAR_DATE`: Deze datum is alleen aanwezig in de weergave Dagelijkse historie. In de weergave Dagelijkse historie wordt een record weergegeven van hoe de gegevens eruit zien bij 11 :59 UTC voor elke datum die is opgegeven in `CALENDAR_DATE` .
* `BEGIN_EFFECTIVE_TIMESTAMP`: Deze datum is aanwezig in zowel de weergave Gebeurtenis als Dagelijkse historie en staat voor de tijd dat een record de huidige waarde in de toepassing wordt.
* `END_EFFECTIVE_TIMESTAMP`: Deze datum is aanwezig in zowel de meningen van de Gebeurtenis als van de Dagelijkse Geschiedenis, en verslagen precies wanneer een verslag _van_ de waarde in de huidige rij in een waarde in een verschillende rij veranderde. Als u ruimte wilt maken tussen query&#39;s op `BEGIN_EFFECTIVE_TIMESTAMP` en `END_EFFECTIVE_TIMESTAMP` , is deze waarde nooit null, zelfs als er geen nieuwe waarde is. Als een record nog geldig is (de waarde is dus niet gewijzigd), heeft `END_EFFECTIVE_TIMESTAMP` de waarde 2300-01-01.

## Terminologie tabel

De volgende tabel correleert objectnamen in Workfront (en hun namen in de interface en API) met hun equivalente namen in Data Connect en bevat referentievelden voor elk object naar andere Workfront-objecten.

>[!NOTE]
>
>Nieuwe velden kunnen zonder voorafgaande kennisgeving aan de objectweergaven worden toegevoegd ter ondersteuning van de veranderende gegevensbehoeften van de Workfront-toepassing. Wij waarschuwen tegen het gebruiken van &quot;UITGEZOCHTE&quot;vragen waar de stroomafwaartse gegevensontvanger niet bereid is om extra kolommen te behandelen aangezien zij worden toegevoegd.<br>
>Als het anders noemen of het verwijderen van een kolom wordt vereist, zullen wij vooraf bericht van deze veranderingen verstrekken.

### Toegangsniveau

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Toegangsniveau</td>
            <td>Toegangsniveau</td>
            <td>ACSLVL</td>
            <td>Toegangsniveau</td>
            <td>ACCESSLEVELS_CURRENT <br> ACCESSLEVELS_DAILY_HISTORY <br> ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LEGACYACCESSLEVELID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Toegangsregel

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Toegangsregel</td>
            <td>Delen</td>
            <td>ACSRUL</td>
            <td>Delen</td>
            <td>ACCESSRULES_CURRENT <br> ACCESSRULES_DAILY_HISTORY <br> ACCESSRULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSORID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op ACCESSOROBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld ACCESSOROBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>ACCESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>Variabele, gebaseerd op ANCESTOROBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld ANCESTOROBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op SECURITYOBJCODE</td>
             <td>De primaire sleutel/id van het object dat wordt geïdentificeerd in het veld SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Goedkeuringspad

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Goedkeuringspad</td>
            <td>Goedkeuringspad</td>
            <td>ARVPTH</td>
            <td>Goedkeuring</td>
            <td>GOEDKEURVALPATHS_CURRENT <br> GOEDKEURVALPATHS_DAILY_HISTORY <br> ERKVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDGEKEURD</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>FK</td>
             <td>METHODES_CURRENT</td>
             <td>GOEDVALPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Goedkeuringsproces

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Goedkeuringsproces</td>
            <td>Goedkeuringsproces</td>
            <td>ARVPRC</td>
            <td>Goedkeuringsproces</td>
            <td>GOEDKEURINGSPROCESSES_CURRENT <br> GOEDKEURINGPROCESSES_DAILY_HISTORY <br> GOEDKEURINGPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Goedkeuringsstap

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Goedkeuringsstap</td>
            <td>Goedkeuringsstap</td>
            <td>ARVSTP</td>
            <td>Goedkeuringsfase</td>
            <td>GOEDVALSTEPS_CURRENT <br> GOEDKEURINGSSTPS_DAILY_HISTORY <br> GOEDKEURINGSSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDGEKEURD</td>
             <td>FK</td>
             <td>METHOVALPATHS_CURRENT</td>
             <td>GOEDGEKEURD</td>
        </tr>
        <tr>
             <td>GOEDGEKEURDE</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Status fiatteur

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Status fiatteur</td>
            <td>Status fiatteur</td>
            <td>ARVSTS</td>
            <td>ApproverStatus</td>
            <td>GOEDVERSTATUSES_CURRENT <br> GOEDVERSTATUSES_DAILY_HISTORY <br> GOEDVERSTATUSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDKEURINGSTATUSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CIVABLEOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op GOEDKEURINGSBAREOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld GOEDKEURINGSBLEOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>GOEDGEKEURDE</td>
             <td>FK</td>
             <td>METHOVALSTEPS_CURRENT</td>
             <td>GOEDGEKEURDE</td>
        </tr>
        <tr>
             <td>GOEDKEURINGSBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSYSYSYID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>WILDCARDUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Toewijzing

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Toewijzing</td>
            <td>Toewijzing</td>
            <td>ASSGN</td>
            <td>Toewijzing</td>
            <td>ASSIGNMENTS_CURRENT <br> ASSIGNMENTS_DAILY_HISTORY <br> ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>TOEWIJZEN</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
      <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Wachtend op goedkeuring

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Wachtend op goedkeuring</td>
            <td>Wachtend op goedkeuring</td>
            <td>AWAPVL</td>
            <td>Wachtend op goedkeuring</td>
            <td>AWAITINGGOEDVALS_CURRENT <br> AWAITINGGOEDVALS_DAILY_HISTORY <br> AWAITINGGOEDVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSREQUESTID</td>
             <td>-</td>
             <td colspan="2">Toegangsaanvraagtabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>GOEDKEURINGSTEKEN</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>GOEDGEKEURD</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ONTBREKEN</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTIEF</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTIEF</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Basislijn

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Basislijn</td>
            <td>Basislijn</td>
            <td>BLIN</td>
            <td>Basislijn</td>
            <td>BASELINES_CURRENT <br> BASELINES_DAILY_HISTORY <br> BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Basislijntaak

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Basislijntaak</td>
            <td>Basislijntaak</td>
            <td>BSTSK</td>
            <td>Basislijntaak</td>
            <td>BASELINETASKS_CURRENT <br> BASELINETASKS_DAILY_HISTORY <br> BASELINETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
    </tbody>
</table>

### Factureringsgraad

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Factureringsgraad</td>
            <td>Snelheid of Override Rate</td>
            <td>TARIEF</td>
            <td>Factureringsgraad</td>
            <td>RATES_CURRENT <br> RATES_DAILY_HISTORY <br> RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIEËN_HUIDIGE</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRNT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Factureringsrecord

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Factureringsrecord</td>
            <td>Factureringsrecord</td>
            <td>BILL</td>
            <td>Factureringsrecord</td>
            <td>BILLINGRECORDS_CURRENT <br> BILLINGRECORDS_DAILY_HISTORY <br> BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICEID</td>
             <td>-</td>
             <td colspan="2">Factuurtabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Boking

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Boking</td>
            <td>Boking</td>
            <td>BOOKN</td>
            <td>Boking</td>
            <td>BOOKINGS_CURRENT <br> BOOKINGS_EVENT<br></td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIEËN_HUIDIGE</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op TOPOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld TOPOBJCODE wordt geïdentificeerd</td>
        </tr>
    </tbody>
</table>

### Bedrijfsprofiel

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Bedrijfsprofiel</td>
            <td>Bedrijfsprofiel</td>
            <td>BSNPRF</td>
            <td>BusinessProfile</td>
            <td>BUSINESSPROFILE_CURRENT <br> BUSINESSPROFILE_DAILY_HISTORY <br> BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Zakelijke regel

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Zakelijke regel</td>
            <td>Zakelijke regel</td>
            <td>BSNRUL</td>
            <td>Zakelijke regel</td>
            <td>BUSINESSRULE_CURRENT <br> BUSINESSRULE_DAILY_HISTORY <br> BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Categorie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categorie</td>
            <td>Aangepast formulier</td>
            <td>CTGIE</td>
            <td>Categorie</td>
            <td>CATEGORIEËN_CURRENT <br> CATEGORIEËN_DAILY_HISTORY <br> CATEGORIEËN_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Categorieparameter

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categorieparameter</td>
            <td>Aangepaste formuliervelden</td>
            <td>CTGYPA</td>
            <td>Categorieparameter</td>
            <td>CATEGORIESPARAMETERS_CURRENT <br> CATEGORIESPARAMETERS_DAILY_HISTORY <br> CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIESPARAMETERIA</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>PARAMETERS</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERS</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Klassificator

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Klassificator</td>
            <td>Locatie</td>
            <td>CLSF</td>
            <td>Locatie</td>
            <td>CLASSIFIER_CURRENT <br> CLASSIFIER_DAILY_HISTORY <br> CLASSIFIER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Bedrijf

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Bedrijf</td>
            <td>Bedrijf</td>
            <td>CMPY</td>
            <td>Bedrijf</td>
            <td>COMPANIES_CURRENT <br> COMPANIES_DAILY_HISTORY <br> COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Aangepast kwartaal

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Aangepast kwartaal</td>
            <td>Aangepast kwartaal</td>
            <td>CSTQRT</td>
            <td>Aangepast kwartaal</td>
            <td>CUSTOMQUARTERS_CURRENT <br> CUSTOMQUARTERS_DAILY_HISTORY <br> CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AANGEPAST</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Aangepaste Enum

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>CustomEnum</td>
            <td>Voorwaarde, Prioriteit, Prioriteit, Status</td>
            <td>CSTEM</td>
            <td>Aangepaste Enum</td>
            <td>CUSTOMENUMS_CURRENT <br> CUSTOMENUMS_DAILY_HISTORY <br> CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AANGEPAST</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Het type record wordt bepaald via de eigenschap `enumClass` . Het volgende is de verwachte types:<br>
><ul><li>CONDITION_OPTASK</li>
&gt;<li>CONDITION_PROJ</li>
&gt;<li>CONDITION_TASK</li>
&gt;<li>PRIORITY_OPTASK</li>
&gt;<li>PRIORITY_PROJ</li>
&gt;<li>PRIORITY_TASK</li>
&gt;<li>SEVERITY_OPTASK</li>
&gt;<li>STATUS_OPTASK</li>
&gt;<li>STATUS_PROJ</li>
&gt;<li>STATUS_TASK</li></ul>


### Document

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Document</td>
            <td>Document</td>
            <td>DOCU</td>
            <td>Document</td>
            <td>DOCUMENTS_CURRENT <br> DOCUMENTS_DAILY_HISTORY <br> DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCUMENTIEF</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>-</td>
             <td colspan="2">Documentaanvraagtabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>-</td>
             <td colspan="2">Geen versietabel momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op TOPOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld TOPOBJCODE wordt geïdentificeerd</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Documentgoedkeuring

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documentgoedkeuring</td>
            <td>Documentgoedkeuring</td>
            <td>DOCAPL</td>
            <td>Documentgoedkeuring</td>
            <td>DOCAPPROVALS_CURRENT <br> DOCAPPROVALS_DAILY_HISTORY <br> DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDGEKEURD</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTIEF</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTIEF</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>VERZOEKEN</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Documentgoedkeuring (NIEUW)

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documentgoedkeuring</td>
            <td>Goedkeuring</td>
            <td>NVT</td>
            <td>NVT</td>
            <td>GOEDKEURING_CURRENT <br> GOEDKEURING_DAILY_HISTORY <br> GOVAL_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">ONGELDIG</td>
             <td>PK</td>
             <td>-</td>
             <td>OPMERKING: dit is ook de id van het DOCUMENTVERSION-object waaraan de goedkeuring is gekoppeld.</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op ASSETTYPE</td>
             <td>De primaire sleutel/id van het object dat in het veld ASSETTYPE is geïdentificeerd</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">EAUTHTENANTID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td class="key">PRODUCTIEF</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td class="key">REALCREATORIE</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Werkgebied voor documentgoedkeuring (NIEUW)

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Werkgebied Documentgoedkeuring</td>
            <td>Goedkeuringsfase</td>
            <td>NVT</td>
            <td>NVT</td>
            <td>GOVAL_STAGE_CURRENT <br> GOVAL_STAGE_DAILY_HISTORY <br> GOVAL_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">ONGELDIG</td>
             <td>FK</td>
             <td>GOEDKEURING_CURRENT</td>
             <td>ONGELDIG</td>
        </tr>
        <tr>
             <td class="key">GOEDKEURINGSSTAGEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
    </tbody>
</table>

### Deelnemers aan werkgebied voor documentgoedkeuring (NIEUW)

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Deelnemer werkgebied voor documentgoedkeuring</td>
            <td>Goedkeuringsbesluiten</td>
            <td>NVT</td>
            <td>NVT</td>
            <td>GOVAL_STAGE_DEDEIPANT_CURRENT <br> GOEDKEURING_STAGE_DEILANT_DAILY_HISTORY <br> GOEDKEURING_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">ONGELDIG</td>
             <td>FK</td>
             <td>GOEDKEURING_CURRENT</td>
             <td>ONGELDIG</td>
        </tr>
        <tr>
             <td class="key">ERKVALSTAGEPARTIKIPANTID/td&gt;
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op ASSETTYPE</td>
             <td>De primaire sleutel/id van het object dat in het veld ASSETTYPE is geïdentificeerd</td>
        </tr>
        <tr>
             <td class="key">BESLISIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td class="key">DEELNEMERS</td>
             <td>FK</td>
             <td class="relatedtable">Variabele, gebaseerd op PARTICIPANTTYPE</td>
             <td>De primaire sleutel/id van het object dat in het veld PARTICIPANTTYPE is geïdentificeerd</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">VERZOEKEN</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">STAGEID</td>
             <td>FK</td>
             <td>GOEDKEURING_STAGE_CURRENT</td>
             <td>STAGEID</td>
        </tr>
    </tbody>
</table>

### Documentmap

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documentmap</td>
            <td>Documentmap</td>
            <td>DOCFLD</td>
            <td>DocsFolders</td>
            <td>DOCFOLDERS_CURRENT <br> DOCFOLDERS_DAILY_HISTORY <br> DOCFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Metagegevens van documentprovider

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Metagegevens van documentprovider</td>
            <td>Metagegevens van documentprovider</td>
            <td>DOCMET</td>
            <td>DocumentProviderMetadata</td>
            <td>DOCPROVIDERMETA_CURRENT <br> DOCPROVIDERMETA_DAILY_HISTORY <br> DOCPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Documentprovider

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documentprovider</td>
            <td>Documentprovider</td>
            <td>DOCPRO</td>
            <td>Documentprovider</td>
            <td>DOCPROVIDERS_CURRENT <br> DOCPROVIDERS_DAILY_HISTORY <br> DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Configuratie van documentprovider

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Configuratie van documentprovider</td>
            <td>Configuratie van documentprovider</td>
            <td>DOCCFG</td>
            <td>DocumentProviderConfig</td>
            <td>DOCPROVIDERCONFIG_CURRENT <br> DOCPROVIDERCONFIG_DAILY_HISTORY <br> DOCPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Documentversie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documentversie</td>
            <td>Documentversie</td>
            <td>DOCV</td>
            <td>Documentversie</td>
            <td>DOCUMENTVERSIONS_CURRENT <br> DOCUMENTVERSIONS_DAILY_HISTORY <br> DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTIEF</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTIEF</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">De externe id in het externe opslagsysteem</td>
        </tr>
        <tr>
             <td>PROOFAPPVALSTATUSID</td>
             <td>-</td>
             <td colspan="2">De tabel met de goedkeuringsstatus van proefdrukken wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>PROOFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">Proeftabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>PROOFOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFSTAGEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Proefwerkgebiedtabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Wisselkoers

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Wisselkoers</td>
            <td>Wisselkoers</td>
            <td>EXRATEN</td>
            <td>Wisselkoers</td>
            <td>EXCHANGERATES_CURRENT <br> EXCHANGERATES_DAILY_HISTORY <br> EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Kosten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Kosten</td>
            <td>Kosten</td>
            <td>EXPNS</td>
            <td>Kosten</td>
            <td>EXPENSES_CURRENT <br> EXPENSES_DAILY_HISTORY <br> EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>UITGAVEN</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>UITGAVEN</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>UITGAVEN</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op TOPBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het TOPBJCODE-veld wordt geïdentificeerd</td>
        </tr>
    </tbody>
</table>

### Type uitgave

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Type uitgave</td>
            <td>Type uitgave</td>
            <td>EXPTYP</td>
            <td>Type uitgave</td>
            <td>EXPENSETYPES_CURRENT <br> EXPENSETYPES_DAILY_HISTORY <br> EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UITGAVEN</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Groep

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Groep</td>
            <td>Groep</td>
            <td>GROEP</td>
            <td>Groep</td>
            <td>GROUPS_CURRENT <br> GROUPS_DAILY_HISTORY <br> GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSLEADERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Uur

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Uur</td>
            <td>Uur</td>
            <td>UUR</td>
            <td>Uur</td>
            <td>HOURS_CURRENT <br> HOURS_DAILY_HISTORY <br> HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDKEURINGSBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>DUPID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>-</td>
             <td colspan="2">Geen Workfront-relatie; wordt gebruikt voor integratie met externe systemen
Zelf</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>PROJECTOVERHEADID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
    </tbody>
</table>

### Uurtype

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Uurtype</td>
            <td>Uurtype</td>
            <td>HOURT</td>
            <td>Uurtype</td>
            <td>HOURTYPES_CURRENT <br> HOURTYPES_DAILY_HISTORY <br> HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Iteratie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Iteratie</td>
            <td>Iteratie</td>
            <td>ITRN</td>
            <td>Iteratie</td>
            <td>ITERATIONS_CURRENT <br> ITERATIONS_DAILY_HISTORY <br> ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Dagboekinvoer

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dagboekinvoer</td>
            <td>Dagboekinvoer</td>
            <td>JRNLE</td>
            <td>Dagboekinvoer</td>
            <td>JOURNALENTRIES_CURRENT <br> JOURNALENTRIES_DAILY_HISTORY <br> JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDKEURINGSTATUSID</td>
             <td>FK</td>
             <td>RESVERSTATUSES_CURRENT</td>
             <td>GOEDKEURINGSTATUSID</td>
        </tr>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Tabel met auditrecord wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTIEF</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTIEF</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>-</td>
             <td colspan="2">Tabel voor delen van document wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>UITGAVEN</td>
             <td>FK</td>
             <td>UITGAVEN_HUIDIGE</td>
             <td>UITGAVEN</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>HOURID</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>-</td>
             <td colspan="2">Initiatieftabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op SUBOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld SUBOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SUBSCRIBEID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op TOPOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld TOPOBJCODE wordt geïdentificeerd</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Gekoppelde map

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gekoppelde map</td>
            <td>Gekoppelde map</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT <br> LINKEDFOLDERS_DAILY_HISTORY <br> LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">De externe id in het externe opslagsysteem</td>
        </tr>
        <tr>
             <td>MAPPEN</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>MAPPEN</td>
        </tr>
        <tr>
             <td>LINKEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Mijlsteen

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Mijlsteen</td>
            <td>Mijlsteen</td>
            <td>MILE</td>
            <td>Mijlsteen</td>
            <td>MILESTONES_CURRENT <br> MILESTONES_DAILY_HISTORY <br> MILESTONES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Mijlpad

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Mijlpad</td>
            <td>Mijlpad</td>
            <td>MPATH</td>
            <td>Mijlpad</td>
            <td>MILESTONEPATHS_CURRENT <br> MILESTONEPATHS_DAILY_HISTORY <br> MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Niet-arbeidbron

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Niet-arbeidbron</td>
            <td>Bron voor niet-arbeid</td>
            <td>NLBR</td>
            <td>Bron voor niet-arbeid</td>
            <td>NONLABORRESOURCES_CURRENT <br> NONLABORRESOURCES_DAILY_HISTORY <br> NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIEËN_HUIDIGE</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Niet-arbeidsuitrustingscategorie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Niet-arbeidsuitrustingscategorie</td>
            <td>Niet-arbeidsuitrustingscategorie</td>
            <td>NLBRCY</td>
            <td>Broncategorie voor niet-arbeid</td>
            <td>NLBRCATEGORIES_CURRENT <br> NLBRCATEGORIES_DAILY_HISTORY <br> NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Onwerkdag

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Onwerkdag</td>
            <td>Uitzondering schema</td>
            <td>NONWKD</td>
            <td>Onwerkdag</td>
            <td>NONWORKDAYS_CURRENT <br> NONWORKDAYS_DAILY_HISTORY <br> NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Opmerking

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Opmerking</td>
            <td>Opmerking</td>
            <td>OPMERKING</td>
            <td>Opmerking</td>
            <td>NOTES_CURRENT <br> NOTES_DAILY_HISTORY <br> NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTIEF</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op ATTACHOBJCODE</td>
             <td>De primaire sleutel/id van het object dat wordt geïdentificeerd in de OBJCODE-ATTACHOBJCODE</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>WORKITEMS_CURRENT</td>
             <td>WORKPOID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Tabel in auditrecord wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTIEF</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTIEF</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>-</td>
             <td colspan="2">Geen Workfront-relatie; wordt gebruikt voor integratie met externe systemen</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op NOTEOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld NOTEOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTENDORSEMENTID</td>
             <td>-</td>
             <td colspan="2">Onderwerptabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>PROOFACTIONID</td>
             <td>-</td>
             <td colspan="2">Proefactietabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">Proeftabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>DREADID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op TOPOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld TOPOBJCODE wordt geïdentificeerd</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>


</table>

### Objectintegratie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Objectintegratie</td>
            <td>Objectintegratie</td>
            <td>OBJINT</td>
            <td>ObjectIntegration</td>
            <td>OBJECTINTEGRATION_CURRENT <br> OBJECTINTEGRATION_DAILY_HISTORY <br> OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op LINKEDOBJECTCODE</td>
             <td>De primaire sleutel/identiteitskaart van het voorwerp dat in het gebied LINKEDOBJECTCODE wordt geïdentificeerd</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>

</table>

### Objectcategorie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Objectcategorie</td>
            <td>Objectcategorieën</td>
            <td>OBJCAT</td>
            <td>Objectcategorie</td>
            <td>OBJECTSCATEGORIES_CURRENT <br> OBJECTSCATEGORIES_DAILY_HISTORY <br> OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### OpTask/Issue

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>OpTask</td>
            <td>Uitgave, verzoek</td>
            <td>OPTASK</td>
            <td>Probleem</td>
            <td>OPTASKS_CURRENT <br> OPTASKS_DAILY_HISTORY <br> OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>FK</td>
             <td>METHODES_CURRENT</td>
             <td>GOEDVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>METHOVALSTEPS_CURRENT</td>
             <td>GOEDGEKEURDE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">Kanban Board table momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">De tabel voor wachtrijdefinitie wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>-</td>
             <td colspan="2">De lijst van het Onderwerp van de Rij wordt momenteel niet gesteund</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op RESOLVINGOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld RESOLVINGOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op SOURCEOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld SOURCEOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Parameter

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parameter</td>
            <td>Aangepast veld</td>
            <td>PARAM</td>
            <td>Parameter</td>
            <td>PARAMETERS_CURRENT <br> PARAMETERS_DAILY_HISTORY <br> PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>-</td>
             <td colspan="2">Parameterfiltertabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>PARAMETERS</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Parametergroep

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parametergroep</td>
            <td>Formuliersectie</td>
            <td>PARAM</td>
            <td>Parametergroep</td>
            <td>PARAMETERGROUPS_CURRENT <br> PARAMETERGROUPS_DAILY_HISTORY <br> PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Parameteroptie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parameteroptie</td>
            <td>Parameteroptie</td>
            <td>POPT</td>
            <td>Parameteroptie</td>
            <td>PARAMETEROPTIONS_CURRENT <br> PARAMETEROPTIONS_DAILY_HISTORY <br> PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERS</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERS</td>
        </tr>
        <tr>
             <td>PARAMETEROPTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Portaalsectie/-rapport

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Poortsectie</td>
            <td>Rapport</td>
            <td>PTLSEC</td>
            <td>Rapport</td>
            <td>PORTALSECTIONS_CURRENT <br> PORTALSECTIONS_DAILY_HISTORY <br> PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>FILTERID</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>FILTERID</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUPBYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>VOORKEUR</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>VOORKEUR</td>
        </tr>
        <tr>
             <td>PUBLICRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>REPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>-</td>
             <td colspan="2">Geplande rapporttabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>VIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>VIEWID</td>
        </tr>
    </tbody>
</table>

### Portal, tabblad/dashboard

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portal, tabblad</td>
            <td>Dashboard</td>
            <td>PTLTAB</td>
            <td>Dashboard</td>
            <td>PORTALTABS_CURRENT <br> PORTALTABS_DAILY_HISTORY <br> PORTALTABS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Sectie tabblad Portal

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sectie tabblad Portal</td>
            <td>Sectie dashboard</td>
            <td>PRTBSC</td>
            <td>Sectie tabblad Portal</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT <br> PORTALTABSPORTALSECTIONS_DAILY_HISTORY <br> PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Sectie voor het kalenderportaal wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>-</td>
             <td colspan="2">De tabel Externe secties wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op PORTALSECTIONOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld PORTALSECTIONOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTABS_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Laatste viewer voor poortsectie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>PortalSectionLastViewer</td>
            <td>Laatste lezers rapporteren</td>
            <td>PLSLSV</td>
            <td>PortalSectionLastViewer</td>
            <td>REPORTLASTVIEWERS_CURRENT <br> REPORTLASTVIEWERS_DAILY_HISTORY <br> REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RAPPORTERING</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>RAPPORTERING</td>
        </tr>
        <tr>
             <td>REPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Portfolio

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portfolio</td>
            <td>Portfolio</td>
            <td>POORT</td>
            <td>Portfolio</td>
            <td>PORTFOLIOS_CURRENT <br> PORTFOLIOS_DAILY_HISTORY <br> PORTFOLIOS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Scorecard-tabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Voorkeur

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Voorkeur</td>
            <td>Weergeven, Filteren, Groeperen, Rapportdefinitie</td>
            <td>PROSET</td>
            <td>Voorkeur</td>
            <td>PREFERENCES_CURRENT <br> PREFERENCES_DAILY_HISTORY <br> PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>VOORKEUR</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Programma

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Programma</td>
            <td>Programma</td>
            <td>PRGM</td>
            <td>Programma</td>
            <td>PROGRAMMS_CURRENT <br> PROGRAMMS_DAILY_HISTORY <br> PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Project

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Project</td>
            <td>Project</td>
            <td>PROJ</td>
            <td>Project</td>
            <td>PROJECTS_CURRENT <br> PROJECTS_DAILY_HISTORY <br> PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Scorecard-tabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>FK</td>
             <td>METHODES_CURRENT</td>
             <td>GOEDVALPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>METHOVALSTEPS_CURRENT</td>
             <td>GOEDGEKEURDE</td>
        </tr>
        <tr>
             <td>LEVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Scorecard-tabel wordt momenteel niet ondersteund</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>-</td>
             <td colspan="2">Pop-accounttabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">De tabel voor wachtrijdefinitie wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SPONSORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Projectteamgebruiker

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Projectteamgebruiker</td>
            <td>Projectteamgebruiker</td>
            <td>PRTU</td>
            <td>Projectgebruiker</td>
            <td>PROJECTSUSERS_CURRENT <br> PROJECTSUSERS_DAILY_HISTORY <br> PROJECTSUSERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Gebruikersrol projectteam

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gebruikersrol projectteam</td>
            <td>Gebruikersrol projectteam</td>
            <td>PTEAM</td>
            <td>ProjectUserRole</td>
            <td>PROJECTSUSERSROLES_CURRENT <br> PROJECTSUSERSROLES_DAILY_HISTORY <br> PROJECTSUSERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Creditcard

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Creditcard</td>
            <td>Creditcard</td>
            <td>RTCRD</td>
            <td>Creditcard</td>
            <td>RATECARD_CURRENT <br> RATECARD_DAILY_HISTORY <br> RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op SECURITYOBJCODE</td>
             <td>De primaire sleutel/id van het object dat wordt geïdentificeerd in het veld SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op SOURCEOBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld SOURCEOBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>

</table>

### Rapportmap

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rapportmap</td>
            <td>Rapportmap</td>
            <td>RPTFDR</td>
            <td>Rapportmap</td>
            <td>REPORTFOLDERS_CURRENT <br> REPORTFOLDERS_DAILY_HISTORY <br> REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Statistisch aantal rapportweergave

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Statistisch aantal rapportweergave</td>
            <td>Statistisch aantal rapportweergave</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticInfo</td>
            <td>REPORTVIEWSTATISTICCOUNTS_CURRENT <br> REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY <br> REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RAPPORTERING</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>RAPPORTVIEWSTATISTICCOUNTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Te rapporteren begrotingsuren

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Te rapporteren begrotingsuren</td>
            <td>Te rapporteren begrotingsuren</td>
            <td>RPBGHR</td>
            <td>Budgeted Hour</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT <br> REPORTABLEBUDGETEDHOURS_DAILY_HISTORY <br> REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>REPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Gereserveerde tijd / PTO

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gereserveerde tijd</td>
            <td>(Persoonlijk) Tijd weg</td>
            <td>HERVATTEN</td>
            <td>Tijd uit</td>
            <td>RESERVEDTIMES_CURRENT <br> RESERVEDTIMES_DAILY_HISTORY <br> RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Resource Manager

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Resource Manager</td>
            <td>Resource Manager</td>
            <td>RESMGR</td>
            <td>Resource Manager</td>
            <td>RESOURCEMANAGERS_CURRENT <br> RESOURCEMANAGERS_DAILY_HISTORY <br> RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Bronpool

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Bronpool</td>
            <td>Bronpool</td>
            <td>RSPL</td>
            <td>Bronpool</td>
            <td>RSRCPOOLS_CURRENT <br> RSRCPOOLS_DAILY_HISTORY <br> RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### RTF-notitie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>RTF-notitie</td>
            <td>RTF-notitie</td>
            <td>RHNOTE</td>
            <td>RTF-notitie</td>
            <td>RESERVEDTEXTNOTES_CURRENT <br> RESERVEDTEXTNOTES_DAILY_HISTORY <br> RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Waarde van RTF-parameter

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Waarde van RTF-parameter</td>
            <td>Waarde van RTF-parameter</td>
            <td>RCHVAL</td>
            <td>RichTextParameterValue</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT <br> RICHTEXTPARAMETERVALUES_DAILY_HISTORY <br> RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>-</td>
             <td colspan="2">Parameterwaardetabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Risico

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Risico</td>
            <td>Risico</td>
            <td>RISICO</td>
            <td>Risico</td>
            <td>RISKS_CURRENT <br> RISKS_DAILY_HISTORY <br> RISKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>RISKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Type risico

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Type risico</td>
            <td>Type risico</td>
            <td>RSKTYP</td>
            <td>Type risico</td>
            <td>RISKTYPES_CURRENT <br> RISKTYPES_DAILY_HISTORY <br> RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Rol

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rol</td>
            <td>Functie</td>
            <td>ROL</td>
            <td>Functie</td>
            <td>ROLES_CURRENT <br> ROLES_DAILY_HISTORY <br> ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Lay-outsjabloontabel wordt niet ondersteund</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Schema

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Schema</td>
            <td>Schema</td>
            <td>GEPLAND</td>
            <td>Schema</td>
            <td>SCHEDULES_CURRENT <br> SCHEDULES_DAILY_HISTORY <br> SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Personeelsformatie

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Personeelsformatie</td>
            <td>Personeelsformatie</td>
            <td>STAFFP</td>
            <td>Personeelsformatie</td>
            <td>STAFFING_PLAN_CURRENT <br> STAFFING_PLAN_DAILY_HISTORY <br> STAFFING_PLAN_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE </td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>        
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>       
         <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID
</td>
        </tr>        
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID
</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Personeelsformatie

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Personeelsformatie</td>
            <td>Personeelsformatie</td>
            <td>STAFFR</td>
            <td>Personeelsformatie</td>
            <td>STAFFING_PLAN_RESOURCE_CURRENT <br> STAFFING_PLAN_RESOURCE_DAILY_HISTORY <br> STAFFING_PLAN_RESOURCE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>       
         <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>        
    </tbody>
</table>

### Stap fiatteur

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Stap fiatteur</td>
            <td>Stap fiatteur</td>
            <td>SPAPVR</td>
            <td>Stage-fiatteur</td>
            <td>STEPAPPROVERS_CURRENT <br> STEPAPPROVERS_DAILY_HISTORY <br> STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDGEKEURDE</td>
             <td>FK</td>
             <td>METHOVALSTEPS_CURRENT</td>
             <td>GOEDGEKEURDE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Taak

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Taak</td>
            <td>Taak</td>
            <td>TAAK</td>
            <td>Taak</td>
            <td>TASKS_CURRENT <br> TASKS_DAILY_HISTORY <br> TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>FK</td>
             <td>METHODES_CURRENT</td>
             <td>GOEDVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>METHOVALSTEPS_CURRENT</td>
             <td>GOEDGEKEURDE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">Kanban Board table momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Tabel met herhalingsregels wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Taakvoorganger

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Taakvoorganger</td>
            <td>Voorganger</td>
            <td>PRED</td>
            <td>Voorganger</td>
            <td>PREDECESSORS_CURRENT <br> PREDECESSORS_DAILY_HISTORY <br> PREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Team

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Team</td>
            <td>Team</td>
            <td>TEAMOB</td>
            <td>Team</td>
            <td>TEAMS_CURRENT <br> TEAMS_DAILY_HISTORY <br> TEAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Lay-outsjabloontabel wordt niet ondersteund</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REQUESTSVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Er zijn 3 teamtypes die in de de objecten van het Team lijsten worden opgeslagen: PROJECT, SJABLOON, en ADHOC. <br>
>Elk van deze teamtypen wordt samen weergegeven in de Data Connect-weergaven voor gegevens in het meer. Als u het specifieke type team wilt isoleren dat u wilt retourneren, moet u filteren op de kolom `teamtype` . Bijvoorbeeld, als u slechts de traditionele teams wilt die deel van uw organisatorische structuren uitmaken, die in het gebied van Teams van de toepassing worden gevormd, zou u een vraag kunnen hebben die iets als dit kijkt: <code> uitgezocht * van teams_current waar teamtype = &quot;ADHOC&quot;;</code>

### Teamlid

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Teamlid</td>
            <td>Overige teams, teamlid</td>
            <td>TEAMMB</td>
            <td>Teamlid</td>
            <td>TEAMMEMBERS_CURRENT <br> TEAMMEMBERS_DAILY_HISTORY <br> TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Functie teamlid

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Functie teamlid</td>
            <td>Functie teamlid</td>
            <td>TEAMMR</td>
            <td>Functie teamlid</td>
            <td>TEAMMEMBERROLES_CURRENT <br> TEAMMEMBERROLES_EVENT<br></td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Sjabloon

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sjabloon</td>
            <td>Sjabloon, projectsjabloon</td>
            <td>TMPL</td>
            <td>Sjabloon</td>
            <td>TEMPLATES_CURRENT <br> TEMPLATES_DAILY_HISTORY <br> TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>FK</td>
             <td>METHODES_CURRENT</td>
             <td>GOEDVALPROCESSID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>LEVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Afleverbare scorebordtabel wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">De tabel voor wachtrijdefinitie wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Toewijzing sjabloontaak

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Toewijzing sjabloontaak</td>
            <td>Sjabloontoewijzing</td>
            <td>TASSGN</td>
            <td>Sjabloontoewijzing</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT <br> TEMPLATEASSIGNMENTS_DAILY_HISTORY <br> TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Tijdlijnbare tabel voor team wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Sjabloontaak

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sjabloontaak</td>
            <td>Sjabloontaak</td>
            <td>TTSK</td>
            <td>Sjabloontaak</td>
            <td>TEMPLATETASKS_CURRENT <br> TEMPLATETASKS_DAILY_HISTORY <br> TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDVALPROCESSID</td>
             <td>FK</td>
             <td>METHODES_CURRENT</td>
             <td>GOEDVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Tabel met herhalingsregels wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Tijdlijnbare tabel voor team wordt momenteel niet ondersteund</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Sjabloontaakvoorganger

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sjabloontaakvoorganger</td>
            <td>Sjabloonvoorganger</td>
            <td>TPRED</td>
            <td>Voorganger</td>
            <td>TEMPLATEPREDECESSORS_CURRENT <br> TEMPLATEPREDECESSORS_DAILY_HISTORY <br> TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEPREDECESSORID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Tijd-gefaseerde Gecombineerde KPI

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tijd-gefaseerde Gecombineerde KPI</td>
            <td>Tijd-gefaseerde KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_COMBINED_CURRENT <br> TIMEPHASED_COMBINED_DAILY_HISTORY <br> TIMEPHASED_COMBINED_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
                <tr>
             <td>EVENT_ID    </td>
             <td>PK</td>
             <td>Dit is een natuurlijke sleutel voor de tijd-gefaseerde ingang van KPI</td>
             <td>-</td>
        </tr>
                        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
                        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>De METADATA-tabel is niet beschikbaar</td>
             <td>-</td>
        </tr>
                        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
                        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
                        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
                        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd
</td>
        </tr>
                        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>De SCHEMA-tabel wordt niet opgegeven; de waarde uit deze tabel wordt gegeven in de SCHEMANAME-kolom. Het SCHEMANAME identificeert de KPI (bv. SchedulHours, estiméHours, en actualHours) waarmee de record is verbonden.</td>
             <td>-</td>
        </tr>
                                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                                <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tijdgefaseerde PKI-valuta

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tijdgefaseerde PKI-valuta</td>
            <td>Tijd-gefaseerde KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_CURRENCY_CURRENT <br> TIMEPHASED_CURRENCY_DAILY_HISTORY <br> TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>De METADATA-tabel is niet beschikbaar</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>De SCHEMA-tabel wordt niet opgegeven; de waarde uit deze tabel wordt gegeven in de SCHEMANAME-kolom. Het SCHEMANAME identificeert de KPI (bv. scheduledRevenueRate, scheduledCostRate, actualRevenue, enz.) waarmee de record is verbonden.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
          <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tijd-gefaseerde Duur KPI

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tijd-gefaseerde Duur KPI</td>
            <td>Tijd-gefaseerde KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_DURATION_CURRENT <br> TIMEPHASED_DURATION_DAILY_HISTORY <br> TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>De METADATA-tabel is niet beschikbaar</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>De SCHEMA-tabel wordt niet opgegeven; de waarde uit deze tabel wordt gegeven in de SCHEMANAME-kolom. Het SCHEMANAME identificeert de KPI (bv. SchedulHours, estiméHours, en actualHours) waarmee de record is verbonden.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID </td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
           <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tijd-gefaseerde KPI Aantallen

Beperkte beschikbaarheid van klanten

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tijd-gefaseerde KPI Aantallen</td>
            <td>Tijd-gefaseerde KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_NUMBERS_CURRENT <br> TIMEPHASED_NUMBERS_DAILY_HISTORY <br> TIMEPHASED_NUMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
        <tr>
             <td>EVENT_ID</td>
             <td>PK</td>
             <td>Dit is een natuurlijke sleutel voor de tijd-gefaseerde ingang van KPI</td>
             <td>-</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>De METADATA-tabel is niet beschikbaar</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                <tr>
             <td>PROGRAMMA</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMMA</td>
        </tr>
                <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
                <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
                <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>De SCHEMA-tabel wordt niet opgegeven; de waarde uit deze tabel wordt gegeven in de SCHEMANAME-kolom. Het SCHEMANAME identificeert de KPI (bv. SchedulHours, estiméHours, en actualHours) waarmee de record is verbonden.</td>
             <td>-</td>
        </tr>
                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>TIMEPHASEDNUMBERSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tijdschema

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tijdschema</td>
            <td>Tijdschema</td>
            <td>TSHET</td>
            <td>Tijdschema</td>
            <td>TIMESHEETS_CURRENT <br> TIMESHEETS_DAILY_HISTORY <br> TIMESHEETS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDGEKEURD</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tijdbladprofiel

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tijdbladprofiel</td>
            <td>Tijdbladprofiel</td>
            <td>TSPRO</td>
            <td>Tijdbladprofiel</td>
            <td>TIMESHEETPROFILES_CURRENT <br> TIMESHEETPROFILES_DAILY_HISTORY <br> TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GOEDGEKEURD</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI-filter

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI-filter</td>
            <td>Filter</td>
            <td>UIFT</td>
            <td>Filter</td>
            <td>UIFILTERS_CURRENT <br> UIFILTERS_DAILY_HISTORY <br> UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>VOORKEUR</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>VOORKEUR</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UIFILTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI-groep door

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI-groep door</td>
            <td>Groepering</td>
            <td>UIGB</td>
            <td>Groepering</td>
            <td>UIGROUPBYS_CURRENT <br> UIGROUPBYS_DAILY_HISTORY <br> UIGROUPBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>VOORKEUR</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>VOORKEUR</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI-sjabloon

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI-sjabloon</td>
            <td>Lay-outsjabloon</td>
            <td>UITMPL</td>
            <td>Lay-outsjabloon</td>
            <td>UITEMPLATES_CURRENT <br> UITEMPLATES_DAILY_HISTORY <br> UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI-weergave

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI-weergave</td>
            <td>Weergave</td>
            <td>UIVIEW</td>
            <td>Weergave</td>
            <td>UIVIEWS_CURRENT <br> UIVIEWS_DAILY_HISTORY <br> UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>VOORKEUR</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>VOORKEUR</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Gebruiker

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gebruiker</td>
            <td>Gebruiker</td>
            <td>GEBRUIKER</td>
            <td>Gebruiker</td>
            <td>USERS_CURRENT <br> USERS_DAILY_HISTORY <br> USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>CATEGORIE</td>
             <td>FK</td>
             <td>CATEGORIEËN_HUIDIGE</td>
             <td>CATEGORIE</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>DELEGATIONTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMETEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Lay-outsjabloontabel wordt niet ondersteund</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">Poortprofielentabel wordt niet ondersteund</td>
        </tr>
        <tr>
             <td>PREFUIID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>UMUSERID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
    </tbody>
</table>

### Gebruikersdelegatie

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gebruikersdelegatie</td>
            <td>Gebruikersdelegatie</td>
            <td>USRDEL</td>
            <td>Gebruikersdelegatie</td>
            <td>USERDELEGATIONS_CURRENT <br> USERDELEGATIONS_DAILY_HISTORY <br> USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FROMUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Gebruikersgroep

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gebruikersgroep</td>
            <td>Overige groepen</td>
            <td>USRGPS</td>
            <td>Gebruikersgroep</td>
            <td>USERSGROUPS_CURRENT <br> USERSGROUPS_DAILY_HISTORY <br> USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Locatie gebruiker

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Locatie gebruiker</td>
            <td>Locatie gebruiker</td>
            <td>USRLOC</td>
            <td>UserLocation</td>
            <td>USERLOCATIONS_CURRENT <br> USERLOCATIONS_DAILY_HISTORY <br> USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Gebruikersrol

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gebruikersrol</td>
            <td>Andere rollen</td>
            <td>USRROL</td>
            <td>Gebruikersrol</td>
            <td>USERSROLES_CURRENT <br> USERSROLES_DAILY_HISTORY <br> USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Voorkeurswaarde gebruiker

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Waarde gebruikersvoorvoegsel</td>
            <td>Gebruikersvoorkeur</td>
            <td>USERPF</td>
            <td>Gebruikersvoorkeur</td>
            <td>USERPREFVALUES_CURRENT <br> USERPREFVALUES_DAILY_HISTORY <br> USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Gebruikersrolset

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UserRoleSet</td>
            <td>Gebruikersrolset</td>
            <td>URSET</td>
            <td>UserRoleSet</td>
            <td>USERROLESET_CURRENT <br> USERROLESET_DAILY_HISTORY <br> USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PRIMARYROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Gebruikersbeslissingen

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UsersDecisions</td>
            <td>Gebruikersbeslissingen</td>
            <td>USRDEC</td>
            <td>Gebruikersbeslissingen</td>
            <td>USERSDECISION_CURRENT <br> USERSDECISION_DAILY_HISTORY <br> USERSDECISION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERBESIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Werkitem

<table>
    <thead>
        <tr>
            <th>Naam Workfront-entiteit</th>
            <th>Interfaceverwijzingen</th>
            <th>API-naslag</th>
            <th>API-label</th>
            <th>Weergaven van datameer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>WorkItem</td>
            <td>Werkitem</td>
            <td>WRKITM</td>
            <td>WorkItem</td>
            <td>WORKITEMS_CURRENT <br> WORKITEMS_DAILY_HISTORY <br> WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primaire/buitenlandse sleutel</th>
            <th>Type</th>
            <th>Verwante tabel</th>
            <th>Verwant veld</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TOEWIJZEN</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TOEWIJZEN</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabele, gebaseerd op OBJCODE</td>
             <td>De primaire sleutel/id van het object dat in het veld OBJCODE is geïdentificeerd</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTIEF</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTIEF</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Geen relatie; wordt gebruikt voor interne toepassingen</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>WORKPOID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>
