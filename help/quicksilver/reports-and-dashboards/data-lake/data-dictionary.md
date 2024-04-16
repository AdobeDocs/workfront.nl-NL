---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Data Lake data dictionary
description: Deze pagina bevat informatie over de structuur en inhoud van de gegevens in het gegevenspMeer van Workfront.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 912f46c87170d6b678d885ccc1fb0170526578df
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Gegevenswoordenboek van Workfront-gegevensmeergegevens

Deze pagina bevat informatie over de structuur en inhoud van de gegevens in het gegevenspMeer van Workfront.

>[!NOTE]
>
>De gegevens in het Workfront data Lake verfrissen zich om de vier uur, zodat recente veranderingen mogelijk niet direct worden weerspiegeld.

## Tabeltypen

Er zijn een aantal tabeltypen die u kunt gebruiken om uw Workfront-gegevens op een manier te bekijken die het meest inzicht biedt.

### Huidige tabel

De tabel Huidig bevat gegevens die ongeveer overeenkomen met de status in Workfront, elk object en de huidige status. U kunt er echter veel minder latentie aan toevoegen dan in Workfront.

### Gebeurtenistabel

De gebeurtenissentabel houdt elke veranderingsverslag in Workfront bij: namelijk telkens als een voorwerp staat verandert, wordt een verslag gecreeerd dat toont wanneer de verandering gebeurde, die de verandering aanbracht, en wat werd veranderd. Daarom is deze lijst nuttig voor punt-in-tijd vergelijkingen. Deze tabel bevat alleen gegevens van de afgelopen drie jaar.

### Tabel met dagelijkse historie

De tabel Dagelijkse historie bevat een verkorte versie van de tabel Gebeurtenis, in die zin dat de status van elk object dagelijks wordt weergegeven in plaats van wanneer elke afzonderlijke gebeurtenis zich heeft voorgedaan. Daarom is deze tabel nuttig voor trendanalyse.

<!-- Custom table -->

## Terminologie tabel

De volgende tabel correleert de objectnamen in Workfront (en hun namen in de interface en API) met hun equivalente naam in het datumpomeer.

<table>
<thead>
  <tr>
    <th>Naam Workfront-entiteit</th>
    <th>Interfaceverwijzingen</th>
    <th>API-naslag | Label</th>
    <th>Gegevens Meer tabellen</th>
    <th>Notities</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Toewijzing</td>
    <td>Toewijzing</td>
    <td>ASSGN | Toewijzing</td>
    <td>ASSIGNMENTS_CURRENT<br>     ASSIGNMENTS_DAILY_HISTORY<br>     ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Voorwaarde, Prioriteit, Prioriteit, Status</td>
    <td>CSTEM | Aangepaste Enum</td>
    <td>CUSTOMENUMS_CURRENT<br>     CUSTOMENUMS_DAILY_HISTORY<br>     CUSTOMENUMS_EVENT</td>
    <td>Het type record wordt geïdentificeerd via de eigenschap ` enumClass`. De volgende typen worden verwacht:<br>     CONDITION_OPTASK<br>     CONDITION_PROJ<br>     CONDITION_TASK<br>     PRIORITY_OPTASK<br>     PRIORITY_PROJ<br>     PRIORITY_TASK<br>     SEVERITY_OPTASK<br>     STATUS_OPTASK<br>     STATUS_PROJ<br>     STATUS_TASK</td>
  </tr>
  <tr>
    <td>Document</td>
    <td>Document</td>
    <td>DOCU | Document</td>
    <td>DOCUMENTS_CURRENT<br>     DOCUMENTS_DAILY_HISTORY<br>     DOCUMENTS_EVENT<br>     <br>     DOCUMENTS_CUSTOM_VALUE_CURRENT<br>     DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>     DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Documentversie</td>
    <td>DOCV | Documentversie</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>     DOCUMENTVERSIONS_DAILY_HISTORY<br>     DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Groep</td>
    <td>Groep</td>
    <td>GROEP | Groep</td>
    <td>GROUPS_CURRENT<br>     GROUPS_DAILY_HISTORY<br>     GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Uur</td>
    <td>Uur</td>
    <td>UUR | Uur</td>
    <td>HOURS_CURRENT<br>     HOURS_DAILY_HISTORY<br>     HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Uurtype</td>
    <td>Uurtype</td>
    <td>HOURT | Uurtype</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Mijlsteen</td>
    <td>Mijlsteen</td>
    <td>MILE | Mijlsteen</td>
    <td>MILESTONES_CURRENT<br>     MILESTONES_DAILY_HISTORY<br>     MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>Mijlpad</td>
    <td>MPATH | Mijlpad</td>
    <td>MILESTONEPATHS_CURRENT<br>     MILESTONEPATHS_DAILY_HISTORY<br>     MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Opmerking</td>
    <td>Opmerking</td>
    <td>OPMERKING | Opmerking</td>
    <td>NOTES_CURRENT<br>     NOTES_DAILY_HISTORY<br>     NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Uitgave, verzoek</td>
    <td>OPTASK | Probleem</td>
    <td>OPTASKS_CURRENT<br>     OPTASKS_DAILY_HISTORY<br>     OPTASKS_EVENT<br>     <br>     OPTASKS_CUSTOM_VALUE_CURRENT<br>     OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>POORT | Portfolio</td>
    <td>PORTFOLIO'S_CURRENT<br>     PORTFOLIO'S_DAILY_HISTORY<br>     PORTFOLIO'S_EVENT<br>     <br>     PORTFOLIO'S_CUSTOM_VALUE_CURRENT<br>     PORTFOLIO'S_CUSTOM_VALUE_DAILY_HISTORY<br>     PORTFOLIO'S_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programma</td>
    <td>Programma</td>
    <td>PRGM | Programma</td>
    <td>PROGRAMS_CURRENT<br>     PROGRAMMS_DAILY_HISTORY<br>     PROGRAMMS_EVENT<br>     <br>     PROGRAMMS_CUSTOM_VALUE_CURRENT<br>     PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Project</td>
    <td>Project</td>
    <td>PROJ | Project</td>
    <td>PROJECTS_CURRENT<br>     PROJECTS_DAILY_HISTORIE<br>     PROJECTS_EVENT<br>     <br>     PROJECTS_CUSTOM_VALUE_CURRENT<br>     PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Rol</td>
    <td>Functie</td>
    <td>ROL | Functie</td>
    <td>ROLES_CURRENT<br>     ROLES_DAILY_HISTORY<br>     ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Schema</td>
    <td>Schema</td>
    <td>GEPLAND | Schema</td>
    <td>SCHEDULES_CURRENT<br>     SCHEDULES_DAILY_HISTORY<br>     SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Taak</td>
    <td>Taak</td>
    <td>TAAK | Taak</td>
    <td>TASKS_CURRENT<br>     TASKS_DAILY_HISTORY<br>     TASKS_EVENT<br>     <br>     TASKS_CUSTOM_VALUE_CURRENT<br>     TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAMS_CURRENT<br>     TEAMS_DAILY_HISTORY<br>     TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tijdschema</td>
    <td>Tijdschema</td>
    <td>TSHET | Tijdschema</td>
    <td>TIMESHEETS_CURRENT<br>     TIMESHEETS_DAILY_HISTORY<br>     TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Gebruiker</td>
    <td>Gebruiker</td>
    <td>GEBRUIKER | Gebruiker</td>
    <td>USERS_CURRENT<br>     USERS_DAILY_HISTORY<br>     USERS_EVENT<br>     <br>     USERS_CUSTOM_VALUE_CURRENT<br>     USERS_CUSTOM_VALUE_DAILY_HISTORY<br>     USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
