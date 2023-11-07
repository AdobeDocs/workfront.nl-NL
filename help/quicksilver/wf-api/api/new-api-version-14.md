---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 14
description: Adobe Workfront heeft API-versie 14 uitgebracht op 9 september 2021. API-versie 14 heeft de volgende wijzigingen ten opzichte van versie 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# Nieuwe functies in API-versie 14

Adobe Workfront heeft API-versie 14 uitgebracht op 9 september 2021. API-versie 14 heeft de volgende wijzigingen ten opzichte van versie 14.

## Toegevoegde bronnen

Er zijn geen bronnen toegevoegd voor API-versie 14.

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 14.

## Gewijzigde bronnen

De volgende bronnen zijn gewijzigd voor API-versie 14.

* [Factureringsrecord (BILL)](#billingrecord-bill)
* [Categorie (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Klant (CUST)](#customer-cust)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Groep (GROEP)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Project (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Brontoewijzing (RSALLO)](#resource-allocation-rsallo)
* [Rol (ROLE)](#role-role)
* [Sjabloon (TMPL)](#template-tmpl)
* [Tijdschema (TSHET)](#timesheet-tshet)

### Factureringsrecord (BILL) {#billingrecord-bill}

Een object BillingRecord registreert de inkomsten, uren of kosten die in rekening kunnen worden gebracht. Deze informatie kan worden gebruikt om facturen op te stellen in een extern boekhoudsysteem.

Voor meer informatie over factureringsverslagen raadpleegt u [Factureringsrecords maken](../../manage-work/projects/project-finances/create-billing-records.md).

Het object BillingRecord heeft de vlag toegevoegd **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Toegevoegd. Een categorie is een aangepast formulier. Deze parameter is toegevoegd ter ondersteuning van de mogelijkheid om aangepaste Forms toe te voegen aan objecten BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referentievelden</td> 
   <td> 
    <ul> 
     <li> <p><b>categorie</b> </p> <p>Toegevoegd. Een categorie is een aangepast formulier. Deze parameter is toegevoegd ter ondersteuning van de mogelijkheid om aangepaste formulieren toe te voegen aan objecten BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Toegevoegd. Dit vertegenwoordigt een inzameling van Categorieën (douaneformulieren) verbonden aan het voorwerp BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Toegevoegd. Met deze handeling worden de expressies in aangepaste formuliervelden opnieuw berekend.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categorie (CTGY) {#category-ctgy}

Een object Categorie is een aangepast formulier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Toegevoegde mogelijke waarde:</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>Deze waarde is toegevoegd ter ondersteuning van de mogelijkheid om aangepaste formulieren toe te voegen aan objecten BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Deze actie neemt de parameters objID en objCode, en keert boolean terug.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

Het object CustomEnum helpt bij het omzetten van statuscodes in leesbare tekst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Zoekopdrachten</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Toegevoegd. Deze query ondersteunt de mogelijkheid om statussen voor groepen en subgroepen te maken en te beheren. </p> <p>Zie voor meer informatie <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Groepsstatussen beheren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Klant (CUST) {#customer-cust}

Een object van de Klant vertegenwoordigt een organisatie die een instantie van Workfront gebruikt.

Dit is een intern object.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Een object CustomerPreferences vertegenwoordigt de set voorkeuren die een klant heeft ingesteld voor hun exemplaar van Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Toegevoegde mogelijke waarde:</p> 
      <ul> 
       <li> <p>Gebruikers toestaan afbeeldingen toe te voegen in updates (updates:images.toggle)</p> </li> 
      </ul> <p>Deze parameter ondersteunt de mogelijkheid om afbeeldingen toe te voegen aan updates van werkitems. </p> <p>Zie voor meer informatie <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Werk bijwerken</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Een object DocumentVersion vertegenwoordigt een specifieke versie van een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

Zie voor meer informatie over documentversies [Een nieuwe versie van een document uploaden](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Toegevoegd. In dit veld worden de datum en het tijdstip vastgelegd van de laatste callback van Workfront Proof, als de versie aan een proefdruk is gekoppeld.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groep (GROEP) {#group-group}

Een object Group vertegenwoordigt een set gebruikers en teams. Groepen vertegenwoordigen vaak de afdelingsstructuur.

Zie voor meer informatie over groepen [Groepen versus teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Toegevoegd. Deze actie neemt een serie van groupIDs en voegt die groepen als subgroups aan de gespecificeerde groep toe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Een object NoteTag vertegenwoordigt de handeling waarbij een gebruiker of team wordt gelabeld in een update van een tijdelijk item.

Voor meer informatie over het labelen in updates raadpleegt u [Andere tags toepassen op updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bewerkingen</td> 
   <td> <p>De volgende bewerkingen zijn toegevoegd aan het object NoteTag:</p> 
    <ul> 
     <li> <p><b>TELLEN</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>RAPPORT</b> </p> </li> 
     <li> <p><b>ZOEKEN</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Project (PROJ) {#project-proj}

Projecten zijn werkitems binnen Workfront en vormen een belangrijke bouwsteen voor de manier waarop Workfront mensen helpt om te werken. Een voorwerp van het Project vertegenwoordigt een groep taken met een gemeenschappelijk, specifiek doel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Toegevoegd.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Een voorwerp QueueDef vertegenwoordigt een Rij, die een project is dat aan het gebied van de Desk van de Hulp is gepubliceerd om gebruikers toe te staan om kwesties aan het voor te leggen.

Zie voor meer informatie over Request Queuws [Een aanvraagwachtrij maken](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Toegevoegd. Deze actie steunt de capaciteit om verzoeken te vinden door de weg door de verzoekrij en onderwerpgroepen te gebruiken.</p> <p>Voor meer informatie bij het zoeken van verzoekrijen door weg, zie <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Verzoeken maken en concepten genereren in de Workfront-webapp</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Adobe Workfront-aanvragen maken en verzenden</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Brontoewijzing (RSALLO) {#resource-allocation-rsallo}

Een voorwerp van de Toewijzing van het Middel vertegenwoordigt de raming van middelen nodig voor een bepaald project. Dit object wordt alleen gebruikt in de verouderde bronnenplanner. Voor het overeenkomstige gebied in de nieuwe Planner van het Middel, gebruik Boedgeted Uur (BGHR).

Het object Resource Allocation heeft de markering verwijderd **RAPPORTAGE**.

### Rol (ROLE) {#role-role}

Een object Role (taakrol) vertegenwoordigt een functionele capaciteit of een vaardigheid die een gebruiker zou kunnen opvullen, zoals Designer of Product Manager.

Zie voor informatie over taakrollen [Overzicht van de taakrol](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Toegevoegd. Dit is een Booleaanse parameter die de waarde true heeft als een object Actief is en false als dit niet het geval is. Objecten die zijn ingesteld op Actief, worden weergegeven in vervolgkeuzemenu's en keuzelijsten die kunnen worden gekoppeld aan andere objecten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standaardvelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sjabloon (TMPL) {#template-tmpl}

Een voorwerp van het Malplaatje vertegenwoordigt een patroon voor een project. Projecten kunnen worden gemaakt op basis van sjablonen om tijd te besparen. Een malplaatje bevat een team en taken, die aan om het even welk project zullen worden gekopieerd dat van het malplaatje wordt gecreeerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Toegevoegd. Dit veld is toegevoegd ter ondersteuning van de mogelijkheid om groepen te koppelen aan sjablonen.</p> <p style="font-weight: normal;">Zie voor meer informatie <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Projectsjablonen bewerken</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groep</p> <p style="font-weight: normal;">Toegevoegd. Dit veld is toegevoegd ter ondersteuning van de mogelijkheid om groepen te koppelen aan sjablonen.</p> <p style="font-weight: normal;">Zie voor meer informatie <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Projectsjablonen bewerken</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
