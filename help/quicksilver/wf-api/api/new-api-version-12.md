---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 12
description: Workfront heeft API-versie 12 uitgebracht op 12 november 2020. API-versie 12 bevat de volgende wijzigingen ten opzichte van versie 11
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 0%

---

# Nieuwe functies in API-versie 12

Workfront heeft API-versie 12 uitgebracht op 12 november 2020. API-versie 12 bevat de volgende wijzigingen ten opzichte van versie 11

## Toegevoegde bronnen

De volgende bronnen zijn nieuw in Workfront API versie 12.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Een BreadCrumb-object vertegenwoordigt een element in de boven-/onderliggende hiërarchie van een Adobe Workfront-werkitem. Broodkruimels wijzen erop hoe een het werkpunt in de grotere structuur van Portfolio&#39;s, Projecten, Projecten, en Taken past.

Voor meer informatie over de Broodkruimels in Workfront raadpleegt u [Overzicht van Broodkruimels in de nieuwe Adobe Workfront-ervaring](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Handeling</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

Rijke tekstvelden zijn nu beschikbaar voor meer objecten. Het RichTextParameterValue-object is toegevoegd aan Workfront ter ondersteuning van deze beschikbaarheid.

Zie voor meer informatie [Rijke tekstvelden in de Adobe Workfront API](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 12.

## Gewijzigde bronnen

De volgende bronnen zijn gewijzigd voor Workfront API versie 12.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AankondigingBijlage</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Goedkeuring</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Bedrijf</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Klant</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">Klantvoorkeuren</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Document</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Groep </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parameter</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programma</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Taak</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Tijdschema</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Gebruiker</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Werk </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

Een voorwerp AccessLevel wordt geassocieerd met gebruikers, en beschrijft de reeks van AccessLevelPermissions die bepalen wat de gebruiker tot toegang heeft.

Voor meer informatie over toegangsniveaus, zie [Hoe de toegangsniveaus werken](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

Een AccessLevelPermissions-object vertegenwoordigt een specifieke machtiging om een Workfront-object te openen, maken of wijzigen. Deze toestemmingen kunnen dan met een Niveau van de Toegang worden geassocieerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan geplande uren in de Balancer van de Werkbelasting bijwerken.</p> <p>Zie voor meer informatie <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Taak geplande uren bijwerken bij het beheren van gebruikerstoewijzingen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Een gebruiker met een toegangsniveau dat deze machtiging bevat, kan velden toevoegen aan aangepaste formulieren.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan een douane gebied systeem-brede met de toegang van de Schrapping delen.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Delen voor aangepaste velden en widgets configureren</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secundairActions</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">action</p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan geplande uren in de Balancer van de Werkbelasting bijwerken.</p> <p>Zie voor meer informatie <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Taak geplande uren bijwerken bij het beheren van gebruikerstoewijzingen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Een gebruiker met een toegangsniveau dat deze machtiging bevat, kan velden toevoegen aan aangepaste formulieren.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan een douane gebied systeem-brede met de toegang van de Schrapping delen.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Delen voor aangepaste velden en widgets configureren</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan geplande uren in de Balancer van de Werkbelasting bijwerken.</p> <p>Zie voor meer informatie <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Taak geplande uren bijwerken bij het beheren van gebruikerstoewijzingen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Een gebruiker met een toegangsniveau dat deze machtiging bevat, kan velden toevoegen aan aangepaste formulieren.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan een douane gebied systeem-brede met de toegang van de Schrapping delen.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Delen voor aangepaste velden en widgets configureren</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secundairActions</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Een ActivityLog-object is een volledige lijst met alle activiteiten die hebben plaatsgevonden in een bepaalde Workfront Proof-account.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Bewerkingen</p> </td> 
   <td> <p>De volgende bewerking is verwijderd uit het object ActivityLog:</p> 
    <ul> 
     <li> <p><strong>ADD</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AankondigingBijlage {#announcementattachment}

Een object NoticeAttachment vertegenwoordigt een bestand dat aan een Workfront-aankondiging is gekoppeld.

Zie voor meer informatie over aankondigingsbijlagen [Aankondigingen verzenden](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Toegevoegde mogelijke waarden:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>De volgende markeringen zijn verwijderd:</p> 
      <ul> 
       <li> <p>DYNAMISCH</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>De volgende markeringen toegevoegd</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISCH</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workinspannt</strong> </p> <p>Dit veld is toegevoegd en geeft aan of een gebruiker een kleine, middelgrote of grote dagelijkse inspanning nodig heeft om een taak te voltooien. Mogelijke waarden zijn:</p> 
      <ul> 
       <li> <p>1 (klein)</p> </li> 
       <li> <p>2 (gemiddeld)</p> </li> 
       <li> <p>3 (Groot)</p> </li> 
      </ul> <p>Voor meer informatie over de Werkinspanning in Workfront raadpleegt u <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Overzicht van de werkprestaties</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

Een agendapunt is een kalenderrapport.

Zie voor meer informatie over kalenderrapporten [Overzicht van kalenderrapporten](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> <p style="font-weight: normal;">De volgende velden zijn toegevoegd aan het object CalendarSection ter ondersteuning van de nieuwe functionaliteit voor het gebruik van aangepaste datums in kalenderrapporten. </p> <p style="font-weight: normal;">Zie voor meer informatie <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Aangepaste datumvelden gebruiken in een kalenderrapport</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Bedrijf {#company}

Een object Company vertegenwoordigt een organisatie die bestaat uit een verzameling personen.

Zie voor meer informatie over bedrijven [Bedrijven maken en bewerken](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">De id van de groep waaraan het bedrijf is gekoppeld.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groep</p> <p style="font-weight: normal;">De groep waarmee het bedrijf is verbonden. Het associëren van een bedrijf met een groep staat de groepsbeheerder toe om groepstoegang en toestemmingen tot het bedrijf uit te breiden.</p> </li> 
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
  <tr> 
   <td>Handelingen</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Deze actie neemt een argument CustomerProductTypeEnum en keert een booleaanse die erop wijst of die klant een rekening voor dat product heeft. </p> </li> 
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
       <li style="font-weight: normal;">wachtwoord:zoomIntegrationEnabled (Zoom-integratie inschakelen in de updatestream)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Toegevoegd</p> </li> 
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
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Mogelijke waarde verwijderd:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>bewijsBesluit</strong> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Handelingen</td> 
   <td> <p>De volgende handelingen zijn toegevoegd aan het object Document.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Deze actie neemt het documentVersonID-argument (tekenreeks) en retourneert een kaart die de beslissing van de controleur aangeeft.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Deze handeling voert de volgende argumenten uit:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (tekenreeks)</p> </li> 
       <li> <p>revisorDecision (tekenreeks)</p> </li> 
       <li> <p>opmerking (tekenreeks)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groep  {#group}

Een object Group vertegenwoordigt een set gebruikers en teams. Groepen vertegenwoordigen vaak de afdelingsstructuur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">De id van de Business Leader die aan de groep is toegewezen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">De bedrijfsleider die aan de groep wordt toegewezen. Een bedrijfsleider is iemand die bedrijfsbesluiten voor de groep neemt.</p> <p style="font-weight: normal;">Voor meer informatie over bedrijfsleiders, zie <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Overzicht van Business Leader</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Handelingen</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Deze handeling voert de volgende argumenten uit:</p> 
      <ul> 
       <li> <p>userID's (tekenreeks[])</p> </li> 
       <li> <p>roleID's (tekenreeks[])</p> </li> 
       <li> <p>teamID (tekenreeks)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMember</strong> </p> </li> 
     <li> <p><strong>updateMemberList</strong> </p> <p>Deze handeling voert de volgende argumenten uit:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Mogelijke waarde verwijderd:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Directe velden</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>De orde wijst op de positie van een taak of verhaal op de Agile backlog.</p> <p>In dit veld zijn de volgende markeringen verwijderd:
       <ul>
        <li>DYNAMISCH</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> <p>Deze acties voegden de argumentstatus toe om de nieuwe de knoopfunctionaliteit van het Begin te steunen, die de status van een het werkpunt verandert wanneer een gebruiker de knoop klikt om erop te wijzen dat zij met het werk aan het punt zijn begonnen.</p> <p>Zie voor meer informatie <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Een object Parameter is een aangepast veld.

Het middel van de Parameter voegde de vlag SHARABLE toe.

Zie voor meer informatie over aangepaste velden [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Toegevoegde mogelijke waarde:</p> 
      <ul> 
       <li> <p>RICH (RTF)</p> <p>Zie voor meer informatie <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rijke tekstvelden in de Adobe Workfront API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Toegevoegde mogelijke waarde:</p> 
      <ul> 
       <li> <p>RICH (Tekstveld met opmaak)</p> <p>Zie voor meer informatie <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rijke tekstvelden in de Adobe Workfront API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>label</strong> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Verzamelingsvelden</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standaardvelden</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>label</strong> </p> <p>Toegevoegd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Een object Portfolio is een verzameling projecten die concurreren om dezelfde bronnen, meestal geld of mensen om deze te voltooien.

Zie voor meer informatie over portfolio&#39;s [Overzicht van Portfolio&#39;s in Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">De id van de groep waaraan het portfolio is gekoppeld.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groep</p> <p style="font-weight: normal;">De groep waaraan de portfolio is gekoppeld. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programma {#program}

Een programmaobject is een subset van projecten binnen een portfolio, waarin vergelijkbare projecten kunnen worden gegroepeerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">De id van de groep waaraan het programma is gekoppeld.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referentievelden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groep</p> <p style="font-weight: normal;">De groep waaraan het programma is gekoppeld. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Een voorwerp QueueDef vertegenwoordigt een Rij, die een Project is dat aan het gebied van de Helpdesk is gepubliceerd om gebruikers toe te staan om Kwesties aan het voor te leggen.

Zie voor meer informatie over Request Queuws [Een aanvraagwachtrij maken](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li><strong>aanvragerCoreAction</strong> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan geplande uren in de Balancer van de Werkbelasting bijwerken.</p> <p>Zie voor meer informatie <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Taak geplande uren bijwerken bij het beheren van gebruikerstoewijzingen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Een gebruiker met een toegangsniveau dat deze machtiging bevat, kan velden toevoegen aan aangepaste formulieren.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Een gebruiker met een toegangsniveau dat deze toestemming omvat kan een douane gebied systeem-brede met de toegang van de Schrapping delen.</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Delen voor aangepaste velden en widgets configureren</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Een voorwerp ScheduledReport vertegenwoordigt een rapport dat is gevormd om voor levering te gepland.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Toegevoegde mogelijke waarden:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Een ScoreCardQuestion-object vertegenwoordigt een vraag die aan een Scorecard is toegevoegd. Deze vragen worden gewoonlijk bepaald door de manager van het Portfolio, en hun antwoorden staan de manager toe om te begrijpen hoe goed een project zich op de doelstellingen van de portefeuille richt.

Voor meer informatie over Scorecard-vragen raadpleegt u [Een scorecard maken](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Toegevoegde mogelijke waarde RICH (Tekstveld met opmaak) </p> <p style="font-weight: normal;">Zie voor meer informatie <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rijke tekstvelden in de Adobe Workfront API</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Taak {#task}

Een voorwerp van de Taak vertegenwoordigt een het werkpunt dat als stap naar het bereiken van een definitief doel (het voltooien van een Project) moet worden uitgevoerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>workinspannt</strong> </p> <p>Dit veld is toegevoegd en geeft aan of een gebruiker een kleine, middelgrote of grote dagelijkse inspanning nodig heeft om een taak te voltooien. Mogelijke waarden zijn:</p> 
      <ul> 
       <li> <p>1 (klein)</p> </li> 
       <li> <p>2 (gemiddeld)</p> </li> 
       <li> <p>3 (Groot)</p> </li> 
      </ul> <p>Voor meer informatie over de Werkinspanning in Workfront raadpleegt u <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Overzicht van de werkprestaties</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> <p>Deze acties voegden de argumentstatus toe om de nieuwe de knoopfunctionaliteit van het Begin te steunen, die de status van een het werkpunt verandert wanneer een gebruiker de knoop klikt om erop te wijzen dat zij met het werk aan het punt zijn begonnen.</p> <p>Zie voor meer informatie <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Een voorwerp van het Team is een inzameling van Gebruikers die aan een het werkpunt kunnen worden toegewezen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> <p>De volgende gebieden werden toegevoegd aan het middel van het Team:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Dit veld geeft het aantal dagen weer dat een voltooide kaart op de Kanban-kaart achterblijft.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Dit gebied associeert een team met een groep. Dit identificeert het team als deel van de groep en staat de Beheerder van de Groep toe om de teams te beheren.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Dit is een booleaanse parameter die erop wijst of het Werk van het team aan het knoop is gevormd als knoop van het Begin. Wanneer een lid van het team een knoop van het Begin klikt om met het werk aan een het werkpunt te beginnen, verandert de status van het punt van Nieuw in een status die in de teammontages wordt gevormd.</p> </li> 
     <li> <p>In de volgende velden kunt u aangepaste statussen voor de knop Start opgeven voor de afzonderlijke werkitems.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Ga voor meer informatie over de knop Start naar <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referentievelden</td> 
   <td> <p>Het volgende gebied werd toegevoegd aan het middel van het Team:</p> 
    <ul> 
     <li> <p><strong>groep</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Een voorwerp TemplateTask vertegenwoordigt een Taak die deel van een Malplaatje uitmaakt. De Taken van het malplaatje worden Taken in het Project waar het Malplaatje wordt gebruikt.

Voor meer informatie over de Taken van het Malplaatje, zie [Een sjabloontaak bewerken](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>workinspannt</strong> </p> <p>Dit veld is toegevoegd en geeft aan of een gebruiker een kleine, middelgrote of grote dagelijkse inspanning nodig heeft om een taak te voltooien. Mogelijke waarden zijn:</p> 
      <ul> 
       <li> <p>1 (klein)</p> </li> 
       <li> <p>2 (gemiddeld)</p> </li> 
       <li> <p>3 (Groot)</p> </li> 
      </ul> <p>Voor meer informatie over de Werkinspanning in Workfront raadpleegt u <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Overzicht van de werkprestaties</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tijdschema {#timesheet}

Een voorwerp Timesheet vertegenwoordigt virtuele timecard dat Gebruikers toestaat om werkelijk gewerkte uren voor Taken, Projecten, en de Types van uren van overheaduren in te gaan.

Voor meer informatie over Timesheets, zie [Overzicht van tijdbladen](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Kernvelden</td> 
   <td> <p>Het volgende veld is verwijderd uit de tijdlijnbron:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Bijwerken

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>De volgende mogelijke waarden zijn toegevoegd:</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeAdd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeEdit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Zie voor meer informatie over initiatieven <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Overzicht van initiatieven in het scenario Planner</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gebruiker {#user}

Een object User vertegenwoordigt een persoon met een account in Workfront die zich kan aanmelden en met het systeem kan communiceren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Directe velden</td> 
   <td> <p>De volgende gebieden werden toegevoegd aan het middel van de Gebruiker:</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>Dit staat voor de datum en tijd waarop een gebruiker is gedeactiveerd.</p> <p>Voor meer informatie over gedeactiveerde Gebruikers raadpleegt u <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>In dit veld wordt de toegang van de gebruiker tot Workfront Goals weergegeven. Mogelijke waarden zijn:</p> 
      <ul> 
       <li> <p>Geen toegang</p> </li> 
       <li> <p>Weergave</p> </li> 
       <li> <p>Bewerken</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Handelingen</td> 
   <td> <p>De volgende actie werd toegevoegd aan het middel van de Gebruiker:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Deze handeling voert de volgende argumenten uit</p> 
      <ul> 
       <li> <p>id (tekenreeks)</p> </li> 
       <li> <p>objCode (tekenreeks)</p> </li> 
      </ul> </li> 
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
   <td>Directe velden</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>De orde wijst op de positie van een taak of verhaal op de Agile backlog.</p> <p>In dit veld zijn de volgende markeringen verwijderd:</p> 
      <ul> 
       <li> <p>DYNAMISCH</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>In dit veld zijn de volgende markeringen toegevoegd:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISCH</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workinspannt</strong> </p> <p>Dit veld is toegevoegd en geeft aan of een gebruiker een kleine, middelgrote of grote dagelijkse inspanning nodig heeft om een taak te voltooien. Mogelijke waarden zijn:</p> 
      <ul> 
       <li> <p>1 (klein)</p> </li> 
       <li> <p>2 (gemiddeld)</p> </li> 
       <li> <p>3 (Groot)</p> </li> 
      </ul> <p>Voor meer informatie over de Werkinspanning in Workfront raadpleegt u <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Overzicht van de werkprestaties</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
