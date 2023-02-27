---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 13
description: Adobe Workfront heeft API-versie 13 uitgebracht op 22 april 2021. API-versie 13 bevat de volgende wijzigingen ten opzichte van versie 12.
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 0%

---

# Nieuwe functies in API-versie 13

Adobe Workfront heeft API-versie 13 uitgebracht op 22 april 2021. API-versie 13 bevat de volgende wijzigingen ten opzichte van versie 12.

## Toegevoegde bronnen

Er zijn geen bronnen toegevoegd voor API-versie 13.

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 13.

## Gewijzigde bronnen

De volgende bronnen zijn gewijzigd voor API-versie 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">Klantvoorkeuren</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Groep </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Project</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">Goedkeuring proef</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Taak</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Tijdschema</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">Gebruikersdelegatie</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Werk </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

Een voorwerp AccessLevel wordt geassocieerd met gebruikers, en beschrijft de reeks van AccessLevelPermissions die bepalen wat de gebruiker tot toegang heeft.

Voor meer informatie over toegangsniveaus, zie [Hoe de toegangsniveaus werken](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beschrijving</b> </p> <p>De validator MAX_LENGTH is toegevoegd, die aangeeft dat de beschrijving niet langer is dan 4000 tekens.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Een BreadCrumb-object vertegenwoordigt een element in de boven-/onderliggende hiërarchie van een Workfront-werkitem. Broodkruimels wijzen erop hoe een het werkpunt in de grotere structuur van Portfolio, Projecten, Projecten, en Taken past.

Voor meer informatie over broodkruimels, zie [Overzicht van Broodkruimels in de nieuwe Adobe Workfront-ervaring](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Objectcodes vindt u in het dialoogvenster <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Een object BurndownEvent vertegenwoordigt een object dat de bundown van een herhaling wijzigt.

Voor meer informatie over burndown, zie [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> <p>De volgende velden zijn verwijderd uit de flag NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Klantvoorkeuren {#customerpreferences}

Een object CustomerPreferences vertegenwoordigt de set voorkeuren die een klant heeft ingesteld voor hun exemplaar van Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarden:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p>De volgende acties werden toegevoegd aan het middel CustomerPreferences.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Neemt het argument:</p> 
      <ul> 
       <li> <p>voorkeuren (kaart)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Een object DocumentVersion vertegenwoordigt een specifieke versie van een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

Zie voor meer informatie over documentversies [Een nieuwe versie van een document uploaden](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Toegevoegde mogelijke waarde:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Toegevoegde markering NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groep  {#group}

Een object Group vertegenwoordigt een set gebruikers en teams. Groepen vertegenwoordigen vaak de afdelingsstructuur.

Zie voor meer informatie over groepen [Groepen versus teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Handelingen</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Deze actie retourneert een array van de bovenliggende groepen van de groep (groepen waarvan de opgegeven groep een subgroep is).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

Het object JournalEntry kan worden ingesteld om informatie over specifieke objectvelden te registreren wanneer deze velden worden gewijzigd. Wanneer een gebied opstelling is om als deel van het voorwerp van de Ingang van het Dagboek worden geregistreerd, zal een overeenkomstig Ingang van het Dagboek worden gecreeerd telkens als dat gebied wordt gewijzigd.

De middelen JournalEntry voegde de vlag toe RAPPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> <p>De volgende velden hebben de markering NOT_GROUPABLE verwijderd:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>In de volgende velden is de markering NOT_FILTERABLE toegevoegd:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Adobe Workfront-beheerders of groepsbeheerders kunnen sjablonen maken om de lay-outelementen in Adobe Workfront aan te passen. Het object LayoutTemplate is specifiek voor Adobe Workfront Classic.

Voor het object dat lay-outsjablonen in de nieuwe Adobe Workfront-ervaring vertegenwoordigt, raadpleegt u [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beschrijving</b> </p> <p>De validator MAX_LENGTH is toegevoegd, die aangeeft dat de beschrijving niet langer is dan 4000 tekens.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Een object LinkedFolder vertegenwoordigt een map die is gekoppeld vanuit een externe documentprovider, zoals Google Drive of Dropbox.

Voor meer informatie over Gekoppelde mappen raadpleegt u [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Toegevoegde mogelijke waarde:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Zoeken in velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favorByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Project {#project}

Projecten zijn werkitems binnen Workfront en vormen een belangrijke bouwsteen voor de manier waarop Workfront mensen helpt om te werken. Een voorwerp van het Project vertegenwoordigt een groep taken met een gemeenschappelijk, specifiek doel.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Goedkeuring proef {#proofapproval}

Een ProofApproval-object vertegenwoordigt een goedkeuring die rechtstreeks is verbonden met een proefdruk.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> <p>De volgende gebieden werden toegevoegd aan het middel ProofApproval.</p> 
    <ul> 
     <li> <p><b>ApproverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Een voorwerp QueueDef vertegenwoordigt een Rij, die een Project is dat aan het gebied van de Helpdesk is gepubliceerd om gebruikers toe te staan om Kwesties aan het voor te leggen.

Voor meer informatie over de Queuges van het Verzoek, zie [Een aanvraagwachtrij maken](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Toegevoegd. Mogelijke waarden zijn:</p> 
      <ul> 
       <li> <p>0 (Na aangepaste formulieren)</p> </li> 
       <li> <p>1 (Voor aangepaste formulieren)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Taak {#task}

Een voorwerp van de Taak vertegenwoordigt een het werkpunt dat als stap naar het bereiken van een definitief doel (het voltooien van een Project) moet worden uitgevoerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Zoeken in velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favorByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Een voorwerp van het Team is een inzameling van Gebruikers die aan een het werkpunt kunnen worden toegewezen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dit veld is toegevoegd en is een Booleaanse parameter met de waarde true als een object actief is en false als dit niet het geval is. Objecten die zijn ingesteld op Actief, worden weergegeven in vervolgkeuzemenu's en keuzelijsten die kunnen worden gekoppeld aan andere objecten. Objecten die niet op Actief zijn ingesteld, zijn niet zichtbaar in vervolgkeuzemenu's en keuzelijsten die aan andere objecten moeten worden gekoppeld.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standaardvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tijdschema {#timesheet}

Een voorwerp Timesheet vertegenwoordigt virtuele timecard dat Gebruikers toestaat om werkelijk gewerkte uren voor Taken, Projecten, en de Types van uren van overheaduren in te gaan.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernvelden</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Verwijderd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

Een voorwerp Timesheet vertegenwoordigt virtuele timecard dat Gebruikers toestaat om werkelijk gewerkte uren voor Taken, Projecten, en de Types van uren van overheaduren in te gaan.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standaardvelden</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront-beheerders of groepsbeheerders kunnen sjablonen maken om de lay-outelementen in Adobe Workfront aan te passen. Het object LayoutTemplate is specifiek voor de nieuwe Adobe Workfront-ervaring.

Voor het object dat lay-outsjablonen in Adobe Workfront Classic vertegenwoordigt, raadpleegt u [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> <p>De volgende acties werden toegevoegd aan het middel UITemplate.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Neemt het argument:</p> 
      <ul> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Neemt de argumenten:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gebruikersdelegatie {#userdelegation}

Een voorwerp UserDelegatie vertegenwoordigt de handeling van het delegeren van het werk van één gebruiker aan een andere voor een specifieke periode.

Het object UserDelegation heeft de markering REPORTABLE toegevoegd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> <p>De volgende velden zijn verwijderd uit de flag NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standaardvelden</td> 
   <td> <p>De volgende velden zijn toegevoegd:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Werk  {#work}

Een voorwerp van het Werk is een gemeenschappelijke interface die zowel Taak als OpTask erft, en gemeenschappelijke code tussen twee deelt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Zoeken in velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favorByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
