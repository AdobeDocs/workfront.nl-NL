---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 11
description: ReportBudgedHour is toegevoegd aan de Adobe Workfront API als bron voor Rapportage. Het kenmerkt verwijzingsgebieden, kerngebieden, en standaardgebieden die in BudgetedHour afwezig zijn.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 0%

---

# Nieuw in API-versie 11

* [Toegevoegde bronnen](#added-resources)
* [Verwijderde bronnen](#removed-resources)
* [Gewijzigde bronnen](#modified-resources)

## Toegevoegde bronnen {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [TeRapporableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessor</li> 
     <li style="font-weight: bold;">klant</li> 
     <li style="font-weight: bold;">user  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">klant  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">klant  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TeRapporableBudgetedHour {#reportablebudgetedhour}

ReportBudgedHour is toegevoegd aan de Adobe Workfront API als bron voor Rapportage. Het kenmerkt verwijzingsgebieden, kerngebieden, en standaardgebieden die in BudgetedHour afwezig zijn.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">assignDate </p> <p>De datum van de Toewijzing is de eerste dag (een Zondag) van de week waarvoor u de uren in de Planner van het Middel begroot.</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>De begrote Uren zijn uren dat de middelmanager voor het werk begrotingen dat de middelen aan projecten moeten voltooien begrotingen</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>De unieke Workfront-id die is toegewezen aan een specifiek Te Rapporteren Boedgeted Hour-object.</p> </li> 
     <li style="font-weight: bold;">scheduledBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>De unieke Workfront-id die aan een specifiek project is toegewezen.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>De unieke Workfront-id die aan een specifieke taakrol is toegewezen.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>De unieke Workfront-id die aan een specifieke gebruiker is toegewezen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">project</p> <p>Het project waaraan een Te RapporterenBudgetedHour is gekoppeld.</p> </li> 
     <li> <p style="font-weight: bold;">rol</p> <p>De Rol van de Baan die een Te RapporterenBudgetedHour wordt geassocieerd met.</p> </li> 
     <li> <p style="font-weight: bold;">user</p> <p>De gebruiker die een Te RapporterenBudgetedHour wordt geassocieerd met.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standaardvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Bewerkingen</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">TELLEN</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">RAPPORT </li> 
     <li style="font-weight: bold;">ZOEKEN</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Verwijderde bronnen {#removed-resources}

Er zijn geen bronnen verwijderd voor API v11.

## Gewijzigde bronnen {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Goedkeuring</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Toewijzing</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Categorie</a> </li> 
     <li><a href="#company" class="MCXref xref">Bedrijf</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Klant</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">Klantvoorkeuren</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Document</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iteratie</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Lay-outsjabloon</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Opmerking</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parameter</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programma</a> </li> 
     <li><a href="#project" class="MCXref xref">Project</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">Goedkeuring proef</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Risico</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Taak</a> </li> 
     <li><a href="#team" class="MCXref xref">Team</a> </li> 
     <li><a href="#template" class="MCXref xref">Sjabloon</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Tijdschema</a> </li> 
     <li><a href="#update" class="MCXref xref">Bijwerken</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">Werk </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Een AccessLevelPermissions-object vertegenwoordigt een set machtigingen. Deze reeks toestemmingen kan dan met een Niveau van de Toegang worden geassocieerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>In de volgende velden werd de mogelijke waarde BUDGETING_INFORMATIE toegevoegd. Hierdoor kunnen gebruikers met toestemming prioriteiten en begrotingstijden in de planner bewerken.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secundairActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Als een gebruiker in Workfront geen toegang heeft tot een object dat hij of zij nodig heeft, kan hij of zij toegang tot dat object aanvragen. Het AccessRequest-object vertegenwoordigt deze aanvraag.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">action</p> <p>Toegevoegd de mogelijke waarde BUDGETING_INFORMATIE. Hierdoor kunnen gebruikers met toestemming prioriteiten en begrotingstijden in de planner bewerken.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Een voorwerp AccessRule vertegenwoordigt een regel die in de niveaus van de douanetoegang wordt geplaatst die bepaalt hoe de gebruikers projecten kunnen delen zij tot stand brengen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>In de volgende velden werd de mogelijke waarde BUDGETING_INFORMATIE toegevoegd. Hierdoor kunnen gebruikers met toestemming prioriteiten en begrotingstijden in de planner bewerken.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secundairActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Goedkeuring {#approval}

Een bepaald het werkpunt, zoals een taak, een document, of een timesheet, kunnen vereisen dat een supervisor of een andere gebruiker weg op het het werkpunt ondertekent. Een voorwerp van de Goedkeuring vertegenwoordigt de actie van het ondertekenen van op een het werkpunt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Directe velden<p style="font-weight: normal;">In de volgende velden zijn de validators AT_DATE_BEFORE_YEAR en AT_DATE_AFTER_YEAR toegevoegd. Deze validators geven aan dat datums op gekoppelde objecten niet kunnen worden ingesteld voor het jaar 1900 of na 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">SchedulStartDate</li>
    </ul><p style="font-weight: normal;">De volgende velden zijn toegevoegd aan de openbare API voor transparantie bij het berekenen van de EAC (Schatting bij voltooiing).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Ook gekend als Geëiste Waarde, is de Begrotte Kosten van het Gepresteerde Werk (BCWP) metrisch van projectprestaties die de begrote kosten van het bedrag van de taak vertegenwoordigt die eigenlijk op het tijdstip van de berekening van deze metrisch is voltooid. Voor taken, BCWP = de Werkelijke Percentage Volledige x begroting van de Taak. Voor Projecten, BCWP = SUM (waarden BCWP van alle ouder en individuele taken).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Ook gekend als Geplande Waarde, is de Begrotte Kosten van Gepland Werk (BCWS) metrisch van projectprestaties die de begrote kosten van de hoeveelheid taak vertegenwoordigt die op het tijdstip zou moeten voltooid zijn dat deze metrisch wordt berekend. Voor taken, BCWS = Geplande Percentage Volledige x begroting van de Taak. Voor projecten, BCWS = SUM (waarden BCWS van alle ouder en individuele taken).</p></li>
    </ul><p style="font-weight: normal;">In de volgende velden is de mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">In de volgende velden is de markering VALUTA toegevoegd</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">De volgende velden zijn verwijderd uit het object Approval.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Het volgende veld is toegevoegd aan het object Approval.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Verwijderd uit het object Approval  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Toegevoegd aan het object Approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Een object ApprovalPath is een vertakking in een goedkeuringsproces. Goedkeuringspaden zijn gebaseerd op de status van het object waaraan het goedkeuringsproces is gekoppeld.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">De mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Een voorwerp ApprovalProcess is een multi-step Goedkeuring die met een Project, een Taak, of een Kwestie kan worden geassocieerd.

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

### Toewijzing {#assignment}

Een toewijzingsobject vertegenwoordigt de verbinding tussen een werkitem en de gebruiker, het team of de groep die is toegewezen aan het werken eraan.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">De mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

Basislijnen zijn momentopnamen van hoe de prestaties van een project er op een bepaald moment uitzagen. Ze slaan belangrijke informatie over het project op, zoals belangrijke data, voortgang, kosten en inkomstenwaarden. Wanneer u een basislijn maakt, worden de taakgegevens ook vastgelegd op de basislijntaken van die basislijn.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">De mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categorie {#category}

Een object Categorie is een aangepast formulier. U kunt rapporten voor dit voorwerp bouwen en u kunt het in andere objecten rapporten tonen, eveneens.

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

### Bedrijf {#company}

Een object Company vertegenwoordigt een organisatie die bestaat uit een verzameling personen. Bedrijven zijn gekoppeld aan een gebruiker of een project.

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

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p style="font-weight: normal;">De volgende acties zijn toegevoegd aan het object CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Zoekopdrachten</td> 
   <td> <p>De volgende query's zijn toegevoegd aan het object CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Klant {#customer}

Een object van de Klant vertegenwoordigt een organisatie die een instantie van Workfront gebruikt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarden: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Projectvoorwaarden)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Taakvoorwaarden)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Uitgavevoorwaarden)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p style="font-weight: normal;">De volgende acties zijn toegevoegd aan het object Customer</p> 
    <ul> 
     <li style="font-weight: bold;">targetEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Klantvoorkeuren {#customerpreferences}

Een object CustomerPreferences vertegenwoordigt de set voorkeuren die een klant heeft ingesteld voor hun exemplaar van Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarden:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Vereisten voor wachtwoordcomplexiteit)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Minimale Wachtwoordlengte)</li> 
       <li style="font-weight: normal;">wachtwoord:mobileSessionTimeout (mobiele sessietime-out)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (User Time Off)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.manualrole (Handmatige controlerende rol)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultnonontvangersRol) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proofhq.defaultnonreceientguestrol)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Handelingen</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Document {#document}

Een object Document vertegenwoordigt een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p>De volgende handelingen zijn toegevoegd aan het object Document.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Iteratie {#iteration}

Een Iteration-object vertegenwoordigt één Agile Iteration. Herhalingen zijn discrete tijdsperiodes die worden gebruikt om artikelen van het type Agile te plannen en te voltooien.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>De volgende velden zijn toegevoegd aan het object Iteration.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">Voltooide punten</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Lay-outsjabloon {#layout-template}

Een object Layout Sjabloon vertegenwoordigt een bepaalde rangschikking van lay-outelementen, zoals het hoofdmenu, het navigatievenster of het gebied Home. Lay-outsjablonen kunnen worden toegewezen aan gebruikers, teams, groepen of taakrollen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Dit veld is toegevoegd en is een Booleaanse parameter met de waarde true als een lay-outsjabloon is ingesteld op het weergeven van tijdstempels voor datums die zijn ingesteld op Tijdstempels in de werklijst en de kalender, en false als deze is ingesteld op het verbergen van tijdstempels.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standaardvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

Een mijlpaal is een markering op een taakindicatie dat het een cruciaal punt in het project is. In het algemeen gebruikt om een belangrijke gebeurtenis aan te duiden, zoals de voltooiing van een fase van het project of een reeks kritieke activiteiten. Een object MilestonePath is een verzameling mijlpalen.

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

### Opmerking {#note}

Een object Note is een opmerking of update die op een Workfront-object wordt uitgevoerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>De volgende velden zijn toegevoegd aan het object Note.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>leuk</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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
   <td colspan="2">Directe velden<p style="font-weight: normal;">In de volgende velden zijn de validators AT_DATE_BEFORE_YEAR en AT_DATE_AFTER_YEAR toegevoegd. Deze waarden geven aan dat datums op gekoppelde objecten niet kunnen worden ingesteld voor het jaar 1900 of na 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">SchedulStartDate</li>
    </ul><p style="font-weight: normal;">De volgende gebieden werden toegevoegd aan OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">De unieke Workfront-id van een Kanban Board-object.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Percentage voltooid is een parameter die de voltooide hoeveelheid van een uitgave, als percentage zal terugkeren.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">werk  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Zoeken in velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>werk</p> <p style="font-weight: normal;">Verwijderd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standaardvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p>De volgende acties zijn toegevoegd aan het OpTask-object</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Een object Parameter is een aangepast veld.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarde TYAH (Typeahead).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Dit veld is toegevoegd en verwijst naar de objectcode van een object waarnaar wordt verwezen. Objectcodes voor alle objecten vindt u in het dialoogvenster <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Een object Portfolio is een verzameling projecten die concurreren om dezelfde bronnen, meestal geld of mensen om deze te voltooien.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>beschrijving</p> <p style="font-weight: normal;">De validator MAX_LENGTH is toegevoegd, die aangeeft dat de beschrijving niet langer is dan 4000 tekens.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programma {#program}

Een programmaobject is een subset binnen een portfolio, waarin vergelijkbare projecten kunnen worden gegroepeerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>beschrijving</p> <p style="font-weight: normal;">De validator MAX_LENGTH is toegevoegd, die aangeeft dat de beschrijving niet langer is dan 4000 tekens.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dit veld is toegevoegd en is een Booleaanse parameter met de waarde true als een object actief is en false als dit niet het geval is. Objecten die zijn ingesteld op Actief, worden weergegeven in vervolgkeuzemenu's en keuzelijsten die kunnen worden gekoppeld aan andere objecten. Objecten die niet op Actief zijn ingesteld, zijn niet zichtbaar in vervolgkeuzemenu's en keuzelijsten die aan andere objecten moeten worden gekoppeld.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">De validator MAX_LENGTH is toegevoegd, waarmee wordt opgegeven dat de naam niet langer is dan 255 tekens.  </p> </li> 
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

### Project {#project}

Projecten zijn werkitems binnen Workfront en vormen een belangrijke bouwsteen voor de manier waarop Workfront mensen helpt om te werken. Een voorwerp van het Project vertegenwoordigt een groep taken met een gemeenschappelijk, specifiek doel.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Directe velden<p style="font-weight: normal;">In de volgende velden zijn de validators AT_DATE_BEFORE_YEAR en AT_DATE_AFTER_YEAR toegevoegd. Deze waarden geven aan dat datums op gekoppelde objecten niet kunnen worden ingesteld voor het jaar 1900 of na 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">SchedulStartDate</li>
    </ul><p style="font-weight: normal;">De volgende velden zijn toegevoegd aan de openbare API voor transparantie bij het berekenen van de EAC (Schatting bij voltooiing).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Ook gekend als Geëiste Waarde, is de Begrotte Kosten van het Gepresteerde Werk (BCWP) metrisch van projectprestaties die de begrote kosten van het bedrag van de taak vertegenwoordigt die eigenlijk op het tijdstip van de berekening van deze metrisch is voltooid. Voor taken, BCWP = de Werkelijke Percentage Volledige x begroting van de Taak. Voor Projecten, BCWP = SUM (waarden BCWP van alle ouder en individuele taken).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Ook gekend als Geplande Waarde, is de Begrotte Kosten van Gepland Werk (BCWS) metrisch van projectprestaties die de begrote kosten van de hoeveelheid taak vertegenwoordigt die op het tijdstip zou moeten voltooid zijn dat deze metrisch wordt berekend. Voor taken, BCWS = Geplande Percentage Volledige x begroting van de Taak. Voor projecten, BCWS = SUM (waarden BCWS van alle ouder en individuele taken).</p></li>
    </ul><p style="font-weight: normal;">In de volgende velden is de markering VALUTA toegevoegd</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Het volgende veld is verwijderd uit het object Project.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitDecision</p> <p style="font-weight: normal;">Dit veld is toegevoegd en is een Booleaanse parameter met de waarde true als een bewijs op een beslissing wacht en false als dit niet het geval is.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Een voorwerp QueueDef vertegenwoordigt een Rij, die een Project is dat aan het gebied van de Helpdesk is gepubliceerd om gebruikers toe te staan om Kwesties aan het voor te leggen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>In de volgende velden werd de mogelijke waarde BUDGETING_INFORMATIE toegevoegd. Hierdoor kunnen gebruikers met toestemming prioriteiten en begrotingstijden in de planner bewerken.</p> 
    <ul> 
     <li style="font-weight: bold;">aanvragerCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

Een voorwerp ReservedTime vertegenwoordigt dagen die op de Persoonlijke Tijd van een Gebruiker worden gespecificeerd, erop wijzend dat de Gebruiker niet voor het werk beschikbaar zal zijn.

Het middel ReservedTime voegde de vlag toe RAPPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>De volgende velden hebben de markering NOT_GROUPABLE verwijderd.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>Het volgende veld is verwijderd uit het object ReservedTime.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>taak</p> <p style="font-weight: normal;">Verwijderd  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Bewerkingen</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>BEWERKEN</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

Een voorwerp ResourcePlannerFilter is een reeks regels die bepalen welke punten in de Planner van het Middel zullen tonen.

De resource ResourcePlannerFilter heeft de markering SHARABLE toegevoegd. Er zijn geen andere wijzigingen aangebracht in het object.

### Risico {#risk}

Een object Risk vertegenwoordigt een mogelijke gebeurtenis die kan voorkomen dat een project op tijd of binnen het budget wordt voltooid. Er worden in de planningsfase risico&#39;s toegevoegd aan projecten om potentiële obstakels te identificeren voordat eventuele werkzaamheden worden goedgekeurd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p>De volgende velden zijn toegevoegd aan het object Risk:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">De id van de gebruiker die het object oorspronkelijk heeft gemaakt.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>De datum waarop een object door een gebruiker in Workfront is verzonden.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>De parameter Last Update Date retourneert de datum waarop de laatste update aan een object is uitgevoerd.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Laatst bijgewerkt op door-id is een parameter die de gebruikersnaam retourneert van de laatste gebruiker die het object heeft bijgewerkt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> <p style="font-weight: normal;">De volgende Referentievelden zijn toegevoegd aan het RIsk-object.</p> 
    <ul> 
     <li style="font-weight: bold;">enterBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Een voorwerp ScheduledReport vertegenwoordigt een rapport dat is gevormd om voor levering te gepland.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Een ScoreCardQuestion-object vertegenwoordigt een vraag die aan een Scorecard is toegevoegd. Deze vragen worden gewoonlijk bepaald door de manager van het Portfolio, en hun antwoorden staan de manager toe om te begrijpen hoe goed een project zich op de doelstellingen van de portefeuille richt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarde TYAH (Typeahead)  </p> </li> 
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
   <td colspan="2">Directe velden<p style="font-weight: normal;">In de volgende velden zijn de validators AT_DATE_BEFORE_YEAR en AT_DATE_AFTER_YEAR toegevoegd. Deze waarden geven aan dat datums op gekoppelde objecten niet kunnen worden ingesteld voor het jaar 1900 of na 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">SchedulStartDate</li>
    </ul><p style="font-weight: normal;">De volgende velden zijn toegevoegd aan de openbare API voor transparantie bij het berekenen van de EAC (Schatting bij voltooiing).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Ook gekend als Geëiste Waarde, is de Begrotte Kosten van het Gepresteerde Werk (BCWP) metrisch van projectprestaties die de begrote kosten van het bedrag van de taak vertegenwoordigt die eigenlijk op het tijdstip van de berekening van deze metrisch is voltooid. Voor taken, BCWP = de Werkelijke Percentage Volledige x begroting van de Taak. Voor Projecten, BCWP = SUM (waarden BCWP van alle ouder en individuele taken).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Ook gekend als Geplande Waarde, is de Begrotte Kosten van Gepland Werk (BCWS) metrisch van projectprestaties die de begrote kosten van de hoeveelheid taak vertegenwoordigt die op het tijdstip zou moeten voltooid zijn dat deze metrisch wordt berekend. Voor taken, BCWS = Geplande Percentage Volledige x begroting van de Taak. Voor projecten, BCWS = SUM (waarden BCWS van alle ouder en individuele taken).</p></li>
    </ul><p style="font-weight: normal;">In de volgende velden is de mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Het volgende veld is verwijderd uit het object Task.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Het volgende veld is toegevoegd aan het object Task.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Verwijderd  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Dit gebied werd toegevoegd aan het voorwerp van het Team. Het Type van Gelijke Schatting bepaalt hoe de het werklading van een verhaal wordt geschat. Als dit in uren wordt geschat, is dit het aantal geplande uren dat aan het artikel wordt toegevoegd. Indien geschat in punten, zal elk punt een aantal Geplande Uren aan het verhaal toevoegen dat op wordt gebaseerd hoe de punten worden geplaatst (gebrek is 8 uren). Mogelijke waarden voor het Beoordelingstype zijn:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (artikelpunten)</li> 
       <li style="font-weight: normal;">UREN (uren)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (uren als punten)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sjabloon {#template}

Een voorwerp van het Malplaatje vertegenwoordigt een patroon voor een Project. Projecten kunnen worden gemaakt met behulp van sjablonen om tijd te besparen. Een malplaatje bevat een Team en Taken, die aan een Project zullen worden gekopieerd wanneer het Malplaatje wordt gebruikt.

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
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allePrioriteiten</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">De mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Een voorwerp TemplateTask vertegenwoordigt een Taak die deel van een Malplaatje uitmaakt. De Taken van het malplaatje worden Taken in het Project waar het Malplaatje wordt gebruikt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p style="font-weight: normal;">In de volgende velden is de mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allePrioriteiten</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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
   <td>Kernvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Verwijderd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Bijwerken {#update}

Werkonderdelen in Workfront kunnen worden bijgewerkt om gebruikers op de hoogte te houden van de huidige status. Een object Update vertegenwoordigt een van deze updates. Updates kunnen door gebruikers worden ingevoerd of door het Workfront-systeem worden gemaakt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarde referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Zoekopdrachten</td> 
   <td> <p style="font-weight: normal;">De volgende query's zijn toegevoegd aan het object Update.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p style="font-weight: normal;">De volgende handelingen zijn toegevoegd aan het object User.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Zoekopdrachten</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p style="font-weight: normal;">De volgende handelingen zijn toegevoegd aan het object User.</p> 
    <ul> 
     <li style="font-weight: bold;">confirmMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledgedAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Zoekopdrachten</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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
   <td colspan="2">Directe velden<p style="font-weight: normal;">In de volgende velden zijn de validators AT_DATE_BEFORE_YEAR en AT_DATE_AFTER_YEAR toegevoegd. Deze waarden geven aan dat datums op gekoppelde objecten niet kunnen worden ingesteld voor het jaar 1900 of na 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">SchedulStartDate</li>
    </ul><p style="font-weight: normal;">De volgende velden zijn toegevoegd aan de openbare API voor transparantie bij het berekenen van de EAC (Schatting bij voltooiing).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Ook gekend als Geëiste Waarde, is de Begrotte Kosten van het Gepresteerde Werk (BCWP) metrisch van projectprestaties die de begrote kosten van het bedrag van de taak vertegenwoordigt die eigenlijk op het tijdstip van de berekening van deze metrisch is voltooid. Voor taken, BCWP = de Werkelijke Percentage Volledige x begroting van de Taak. Voor Projecten, BCWP = SUM (waarden BCWP van alle ouder en individuele taken).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Ook gekend als Geplande Waarde, is de Begrotte Kosten van Gepland Werk (BCWS) metrisch van projectprestaties die de begrote kosten van de hoeveelheid taak vertegenwoordigt die op het tijdstip zou moeten voltooid zijn dat deze metrisch wordt berekend. Voor taken, BCWS = Geplande Percentage Volledige x begroting van de Taak. Voor projecten, BCWS = SUM (waarden BCWS van alle ouder en individuele taken).</p></li>
    </ul><p style="font-weight: normal;">In de volgende velden is de mogelijke waarde ET toegevoegd. Deze waarde vertegenwoordigt de eenheid van tijd Verstreken Maanden, die naar maanden zonder met betrekking tot weekends of feestdagen verwijst.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Het volgende veld is verwijderd uit het object Work.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Het volgende veld is toegevoegd aan het object Work.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Verwijderd  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
