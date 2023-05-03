---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Gebeurtenismeldingen beschikbaar in Adobe Workfront
description: Gebeurtenismeldingen worden geactiveerd door verschillende typen gebeurtenissen op objecten, zoals projecten, taken en problemen, zoals wordt uitgelegd in gebeurtenismeldingen.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 25625291f691f7858634d9961fccb4465008dc3c
workflow-type: tm+mt
source-wordcount: '5008'
ht-degree: 0%

---

# Gebeurtenismeldingen beschikbaar in Adobe Workfront

Gebeurtenismeldingen worden geactiveerd door verschillende typen gebeurtenissen op objecten, zoals projecten, taken en problemen, zoals wordt uitgelegd in [Gebeurtenismeldingen](../../../workfront-basics/using-notifications/event-notifications.md).

Deze meldingen kunnen op systeem- en groepsniveau worden geconfigureerd:

* Voor informatie over het configureren van gebeurtenismeldingen op systeemniveau raadpleegt u [Gebeurtenismeldingen configureren voor iedereen in het systeem](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Voor informatie over het configureren van gebeurtenismeldingen op groepsniveau raadpleegt u [Gebeurtenismeldingen voor een groep weergeven en configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Individuele gebruikers kunnen hun individuele gebeurtenismeldingen ook in hun afzonderlijke profiel activeren en deactiveren. Zie voor meer informatie [Uw eigen gebeurtenismeldingen activeren of deactiveren](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

In de volgende tabellen staan alle Adobe Workfront-gebeurtenismeldingen, een korte beschrijving van de gebeurtenis en of de gebeurtenis standaard actief of inactief is.

## Actie vereist

Zie ook [Meldingen: Actie vereist](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th>Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Gebruiker</p> </td> 
   <td> <p>Verzoek om toegang tot gebruiker</p> </td> 
   <td> <p>Iemand vraagt toegang van mij.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> <p> </p> </td> 
   <td> <p>Document-aanvraag toevoegen aan aanvrager</p> </td> 
   <td> <p>Vraag me om documenten te uploaden.</p> <p>De documentaanvrager ontvangt een e-mailbericht wanneer deze een aanvraag ontvangt om een document te uploaden.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document in afwachting van goedkeuring aan fiatteurs</p> </td> 
   <td> <p>Ik moet een document goedkeuren.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Toewijzing van uitgave aan uitgave toegewezen aan</p> </td> 
   <td> <p>Ik ben toegewezen aan een probleem.</p> <p>De uitgever ontvangt alleen een e-mailkennisgeving als de status van het project Actief is en de status van de uitgave niet Gesloten is of iets dat overeenkomt met Gesloten.</p> <p>Gebruikers met een licentie voor revisie of aanvragen ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Afgifte in afwachting van goedkeuring aan fiatteurs</p> </td> 
   <td> <p>Ik moet een kwestie goedkeuren.</p> <p>Welke gebruikers een e-mailbericht voor deze gebeurtenis ontvangen hangt af van of "Approver niet vereist om op het projectteam (voor goedkeuringsprocessen te zijn die een rol omvatten)"het plaatsen wordt toegelaten (zoals die in wordt beschreven <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren</a>). </p> <p>Als deze optie is ingeschakeld</strong>, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de functie "fiatteur".</p> <p>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de functie "fiatteur" een e-mailbericht.</p> <p>Een bericht wordt verzonden als het project in de Planning of Huidige status is. </p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Afgeven in afwachting van goedkeuring aan gedelegeerde fiatteur</p> </td> 
   <td> <p>Ik moet een goedkeuring van een kwestie herzien ik ben gedelegeerd.</p> <p>Wanneer iemand een uitgavecontrole aan een andere gebruiker delegeert, wordt die gebruiker op de hoogte gebracht. </p> <p>Een bericht wordt verzonden slechts wanneer het project in de Huidige status is.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project in afwachting van goedkeuring aan fiatteurs</p> </td> 
   <td> <p>Ik moet een project goedkeuren.</p> <p>Welke gebruikers een e-mailbericht voor deze gebeurtenis ontvangen hangt af van of "Approver niet vereist om op het projectteam (voor goedkeuringsprocessen te zijn die een baanrol omvatten)"het plaatsen wordt toegelaten (zoals die in wordt beschreven <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren</a>).</p> <p>Als deze optie is ingeschakeld</strong>, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de functie "fiatteur".</p> <p>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de functie "fiatteur" een e-mailbericht.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Project in afwachting van goedkeuring aan gedelegeerde fiatteur</td> 
   <td> <p>Ik moet een projectgoedkeuring bekijken die ik ben gedelegeerd.</p> </td> 
   <td> Actief</td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taaktoewijzing aan taak toegewezen aan</p> </td> 
   <td> <p>Ik ben ingesteld als de primaire ontvanger van een taak.</p> <p>De taakontvanger ontvangt een e-mailbericht als hij of zij de primaire ontvanger van de taak is, tenzij de ontvanger de gebruiker is die de taak heeft uitgevoerd.</p> <p>Er wordt een melding verzonden als de projectstatus Huidig is en de taak niet is gemarkeerd als Voltooid.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak in afwachting van goedkeuring aan fiatteurs</p> </td> 
   <td> <p>Ik moet een taak goedkeuren.</p> <p>Welke gebruikers een e-mailbericht voor deze gebeurtenis ontvangen hangt af van of "Approver niet vereist om op het projectteam (voor goedkeuringsprocessen te zijn die een rol omvatten)"het plaatsen wordt toegelaten (zoals die in wordt beschreven <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren</a>). </p> <p>Als deze optie is ingeschakeld</strong>, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de functie "fiatteur".</p> <p>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de functie "fiatteur" een e-mailbericht.</p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is op het moment van de aanvraag.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak in afwachting van goedkeuring aan gedelegeerde fiatteur</p> </td> 
   <td> <p>Ik moet een taakgoedkeuring bekijken die ik ben gedelegeerd.</p> <p>Wanneer iemand een uitgavecontrole aan een andere gebruiker delegeert, wordt die gebruiker op de hoogte gebracht. </p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is op het moment van de aanvraag.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tijdschema</p> </td> 
   <td> <p>Tijdschema opnieuw geopend voor gebruiker</p> </td> 
   <td> <p>Mijn tijdspagina wordt opnieuw geopend.</p> <p>De eigenaar van de tijdpagina ontvangt een e-mailbericht wanneer de tijdpagina opnieuw wordt geopend, tenzij de gebruiker die de tijdpagina opnieuw heeft geopend ook de eigenaar van de tijdpagina is.</p> <p>Er wordt alleen een e-mailmelding verzonden als de status van het tijdschrift Open is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tijdschema</p> </td> 
   <td> <p>Afwijzing tijdpagina naar gebruiker</p> </td> 
   <td> <p>Mijn tijdschema wordt verworpen.</p> <p>De eigenaar van de tijdpagina ontvangt een e-mailbericht wanneer de tijdpagina wordt afgewezen, tenzij de gebruiker die de tijdpagina heeft afgewezen ook de eigenaar is.</p> <p>Er wordt alleen een e-mailmelding verzonden als de status van het tijdschrift is geweigerd.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tijdschema</p> </td> 
   <td> <p>Tijdschema-indiening bij fiatteur</p> </td> 
   <td> <p>Ik moet een tijdschema goedkeuren.</p> <p>De Tijdopmaakfiatteur ontvangt een e-mailbericht wanneer een timesheet wordt voorgelegd dat zij moeten goedkeuren, tenzij de gebruiker die timesheet indiende ook de fiatteur van de Tijdopmaak is.</p> <p>Een bericht wordt verzonden slechts als de status van timesheet wordt voorgelegd.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Toewijzing</p> </td> 
   <td> <p>Aanvraag voor werkitem naar team</p> </td> 
   <td> <p>Mijn team krijgt een nieuwe werkaanvraag.</p> <p>De Leden van het team ontvangen een e-mailbericht wanneer het team een nieuw het werkverzoek ontvangt. (De gebruiker die het verzoek heeft ingediend, ontvangt geen melding als hij of zij lid is van het team.)</p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is op het moment dat het werkverzoek wordt gedaan en de status van het werkverzoek Nieuw is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Toewijzing</p> </td> 
   <td> <p>Aanvraag voor tijdelijk item om te werken aan toegewezen persoon</p> </td> 
   <td> <p>Ik krijg een nieuw verzoek om werk.</p> <p>De ontvanger van het werkitem ontvangt een e-mailbericht, tenzij de gebruiker die het verzoek indient ook de ontvanger is. </p> <p>Er wordt geen melding verzonden als de taakstatus Voltooid is of als de uitgiftestatus Gesloten is.</p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is op het moment van de aanvraag.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verzoeken die ik heb ingediend

Zie ook [Meldingen: Verzoeken die ik heb ingediend](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Status van documentgoedkeuring wijzigen in aanvrager</p> </td> 
   <td> <p>Er is een aanvraag voor documentgoedkeuring voltooid.</p> <p>De aanvrager van het document ontvangt een e-mailbericht wanneer de aanvraag voor documentgoedkeuring is voltooid.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Documentaanvraag voltooid voor aanvrager</p> </td> 
   <td> <p>Er is voldaan aan een aanvraag voor het uploaden van documenten.</p> <p>De aanvrager van het document ontvangt een e-mailbericht wanneer aan een aanvraag voor het uploaden van een document is voldaan.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Probleem toevoegen aan primaire contactpersoon bij afgifte</p> </td> 
   <td> <p>Ik voeg een kwestie aan een project toe.</p> <p>Het primaire contact op een kwestie ontvangt een bericht wanneer zij een kwestie in een project toevoegen.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td>Probleem</td> 
   <td>Toewijzing van probleem aan primaire contactpersoon</td> 
   <td> <p>Iemand wordt toegewezen aan een kwestie waarvoor ik het primaire contact ben.</p> <p>Het primaire contact op een kwestie ontvangt een bericht wanneer de kwestie aan een gebruiker wordt toegewezen. </p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> Inactief</td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Probleemoplossing voor primaire contactpersoon</p> </td> 
   <td> <p>Een kwestie waarvoor ik het primaire contact ben wordt voltooid.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Wijziging projectstatus in ingevoerd door</p> </td> 
   <td> <p>De status verandert in een project dat ik heb gemaakt.</p> <p>De gebruiker die het project creeerde ontvangt een e-mailbericht wanneer de projectstatus verandert.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Verzoek om toevoegen aan primaire contactpersoon bij afgifte</p> </td> 
   <td> <p>Ik verzend een verzoek (bevestiging).</p> <p>De primaire contactpersoon voor de uitgave ontvangt een e-mailbericht wanneer deze een uitgave indient.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het project "Is de Mening van de Helpdesk"gebruikt.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Toewijzing aanvragen aan primaire contactpersoon</p> </td> 
   <td> <p>Er is iemand toegewezen aan mijn verzoek.</p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer een gebruiker aan de uitgave wordt toegewezen, tenzij de primaire contactpersoon en de toegewezen gebruiker dezelfde gebruiker zijn.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het project "Is de Mening van de Helpdesk"gebruikt.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Aanvraag gesloten voor primaire contactpersoon</p> </td> 
   <td> <p>Mijn aanvraag is gesloten (bevestiging).</p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer de aanvraag wordt gesloten.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het project "Is de Mening van de Helpdesk"gebruikt.</p> <p>Als de meldingen voor 'Aflevering voltooien' zijn ingeschakeld, worden ze altijd geactiveerd in plaats van 'Aanvraag gesloten voor Primaire contactpersoon afgifte'. Als u wilt dat dit bericht wordt geactiveerd, moet u de meldingen voor het voltooien van de uitgave deactiveren.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document aanvragen Toevoegen aan primaire contactpersoon voor afgifte</p> </td> 
   <td> <p>Een document wordt gewijzigd of geüpload op een probleem waarvoor ik de primaire contactpersoon ben.</p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer een document wordt geüpload of gewijzigd tijdens de uitgave, tenzij de gebruiker die het document heeft geüpload of gewijzigd ook de primaire contactpersoon is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het project "publiceer als Rij van het Verzoek van de Hulp"heeft die op het lusje van de Opstelling van de Rij wordt toegelaten.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Statuswijziging aanvragen voor primaire contactpersoon</p> </td> 
   <td> <p>De status verandert op mijn verzoek.</p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer de status van de uitgave verandert, tenzij de gebruiker die de status heeft gewijzigd ook de primaire contactpersoon is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en het project "Is de Mening van de Helpdesk"gebruikt.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Communicatie

Zie ook [Meldingen: Communicatie](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Opmerking over document naar documenteigenaar</p> </td> 
   <td> <p>Er wordt een opmerking toegevoegd aan mijn document.</p> <p>De eigenaar van een document in Workfront ontvangt een e-mailbericht wanneer een opmerking in het document wordt geplaatst, tenzij de gebruiker die de opmerking heeft geplaatst ook de eigenaar van het document is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is. </p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Opmerking over &lt;request name=""&gt; op &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is:<em> Samenvatting van communicatie &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Actief </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Opmerking</p> </td> 
   <td> <p>Opmerking toevoegen bij aanvraag voor primaire contactpersoon</p> </td> 
   <td> <p>Als er een opmerking op een aanvraag wordt geplaatst, stuurt u een e-mail naar de primaire contactpersoon voor de uitgave.</p> <p>De primaire contactpersoon voor een kwestie ontvangt een e-mailbericht wanneer een commentaar op een verzoek wordt gepost, tenzij de gebruiker die de opmerking heeft geplaatst ook de primaire contactpersoon voor de kwestie is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gebruiker</p> </td> 
   <td>Gerichte update naar gebruiker</td> 
   <td> <p>Iemand neemt mij op een geleide update.</p> <p>Een geleide update is wanneer een gebruiker specifiek een andere gebruiker in een update omvat, zoals die in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere tags toepassen op updates</a>.</p> <p>In dit geval ontvangt de gebruiker die is opgenomen in de gestuurde update een e-mailmelding over de update.</p> <p>Het e-mailbericht wordt alleen verzonden als de gebruiker toegangsrechten heeft voor het object en als deze ingeschakeld blijft in het profiel.  </p> <p>Deze gebeurtenismelding wordt standaard geactiveerd en kan niet worden gedeactiveerd.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Directe update naar team</p> </td> 
   <td> <p>Iemand neemt mijn team op een geleide update.</p> <p>Een geleide update is wanneer een gebruiker specifiek een andere gebruiker in een update omvat, zoals die in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere tags toepassen op updates</a>.</p> <p>In dit geval ontvangt elk lid van het team dat is opgenomen in de gestuurde update een e-mailmelding over de update.</p> <p>Het e-mailbericht wordt alleen verzonden naar gebruikers die toegangsrechten hebben voor het object van de update.</p> <p>Als de gebruiker die de gestuurde update verzendt lid is van het team dat wordt opgenomen, ontvangt de gebruiker die de update verzendt geen e-mailbericht.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Opmerking</p> </td> 
   <td> <p>Commentaar van het Punt van het werk aan de Deelnemers van de draad</p> </td> 
   <td> <p>Iemand reageert op een thread waar ik in zit.</p> <p>De deelnemers in de draad en de gebruikers die in een direct bericht inbegrepen zijn ontvangen een e-mailbericht wanneer een gebruiker een commentaar in de draad aanbrengt.</p> <p>Gebruikers moeten toegang tot de weergave hebben om een melding te ontvangen.</p> <p>De volgende gebruikers ontvangen geen melding:</p> 
    <ul> 
     <li> <p>Teams die zijn opgenomen in een direct bericht</p> </li> 
     <li> <p>De eigenaar van de notitie</p> </li> 
     <li> <p>De primaire contactpersoon</p> </li> 
    </ul> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Opmerking</p> </td> 
   <td> <p>Opmerking voor werkitem om item toe te wijzen</p> </td> 
   <td> <p>Iemand reageert op een van mijn werkitems.</p> <p>De ontvanger van het werkitem ontvangt een e-mailbericht wanneer een gebruiker een update aan een werkitem toevoegt, tenzij de gebruiker die de update toevoegt ook de ontvanger is.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Opmerking</p> </td> 
   <td> <p>Antwoord op verzoek van werk naar werkaanvrager</p> </td> 
   <td> <p>Iemand beantwoordt mijn verzoek.</p> <p>Nadat een gebruiker een aanvraag heeft ingediend en een andere gebruiker op die aanvraag heeft geantwoord, ontvangt de gebruiker die het verzoek heeft verzonden een e-mailbericht.</p> <p>Er wordt geen e-mailmelding verzonden als:</p> 
    <ul> 
     <li> <p>De gebruiker die antwoordt is de zelfde gebruiker die het verzoek indiende</p> </li> 
     <li> <p>De gebruiker heeft geen toegang om de notitie te zien</p> </li> 
    </ul> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Goedkeuringsinformatie

Zie ook [Meldingen: Goedkeuringsinformatie](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Gebruiker</p> </td> 
   <td> <p>Goedkeuringsdelegatie voor een andere gebruiker</p> </td> 
   <td> <p>Ik ben gedelegeerd als fiatteur.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Wijziging van goedkeuringsstatus van gedelegeerde afgifte</p> </td> 
   <td> <p>Er is een verzoek tot goedkeuring van een gedelegeerde uitgave voltooid. </p> <p>Wanneer u een afgiftegoedkeuring aan iemand anders delegeert, ontvangt u een e-mailbericht wanneer deze de goedkeuring heeft voltooid (of zij de goedkeuring van de uitgave goedkeuren of verwerpen). </p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Wijziging van status van projectgoedkeuring</p> </td> 
   <td> <p>Een gedelegeerd verzoek tot goedkeuring van een project is voltooid.</p> <p>Wanneer u een projectgoedkeuring aan iemand anders delegeert, ontvangt u een e-mailbericht wanneer zij die goedkeuring (of zij goedkeuren of de projectgoedkeuring verwerpen) beëindigen.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Status van gedelegeerde taak wijzigen</p> </td> 
   <td> <p>Een gedelegeerde status voor taakgoedkeuring is voltooid.</p> <p>Wanneer u een taakgoedkeuring aan iemand anders delegeert, ontvangt u een e-mailbericht wanneer zij die goedkeuring beëindigen (of zij de taakgoedkeuring goedkeuren of verwerpen).</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Goedkeuring van document annuleren bij fiatteur</p> </td> 
   <td> <p>Een aanvraag voor documentgoedkeuring wordt geannuleerd.</p> <p>De documentfiatteur van het document ontvangt een e-mailbericht wanneer het verzoek om documentgoedkeuring wordt geannuleerd.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tijdschema</p> </td> 
   <td> <p>Goedkeuring tijdpagina voor gebruiker</p> </td> 
   <td> <p>Mijn tijdschema is goedgekeurd.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informatie over werk dat aan mij is toegewezen

Zie ook [Meldingen: Informatie over werk dat aan mij is toegewezen](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Taak</td> 
   <td>Alle Voltooiing van de Taak van de Predecessor aan Taak Afhankelijken op Toegewezen Team</td> 
   <td> <p>Alle voorgangers van de taken van het team worden voltooid.</p> <p>De taakwijzers (alle leden van het team) ontvangen een e-mailbericht.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td>Inactief</td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Alle Afwikkelingen van de Taak van de Predecessor aan Taak Afhankelijke</p> </td> 
   <td> <p>Alle voorgangers van mijn taken zijn voltooid.</p> <p>De toegewezen taak ontvangt een e-mailbericht.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Goedkeuringsbesluit toegewezen aan</p> </td> 
   <td> <p>Een kwestie die ik heb opgelost, wordt goedgekeurd of verworpen.</p> <p>De ontvanger van een afgifte ontvangt een e-mailkennisgeving wanneer een goedkeuringsbesluit wordt genomen (goedgekeurd of afgewezen).</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Goedkeuringsbesluit voor taak toegewezen aan</p> </td> 
   <td> <p>Een taak die ik heb voltooid, wordt goedgekeurd of afgewezen.</p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de taak wordt goedgekeurd of afgewezen.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Probleemoplossing toegewezen aan</p> </td> 
   <td> <p>Een probleem waaraan ik ben toegewezen, is voltooid.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Geplande afsluitdatum van uitgave gewijzigd</p> </td> 
   <td> <p>De wijzigingen op de vervaldatum in een uitgave waaraan ik ben toegewezen.</p> <p>De uitgeversidentificatie ontvangt een e-mailbericht wanneer de Geplande Datum van Voltooiing verandert, tenzij de gebruiker die de Geplande Datum van Voltooiing veranderde ook de ontvanger is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus om het even wat buiten Planning is.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Status van uitgave wijzigen in uitgave toegewezen aan</p> </td> 
   <td> <p>De status verandert op een van mijn werkitems.</p> <p>De ontvanger van de uitgave ontvangt een e-mailbericht wanneer de status verandert, tenzij de gebruiker die de status heeft gewijzigd ook de ontvanger is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document aanvragen voor toevoegen aan probleem toegewezen aan</p> </td> 
   <td> <p>Documenten worden geüpload of gewijzigd op aanvragen waaraan ik toegewezen ben.</p> <p>De uitgevers ontvangen een e-mailbericht wanneer documenten worden geüpload of gewijzigd in een uitgave die zij hebben toegevoegd.</p> <p>Er wordt geen e-mailbericht verzonden als de gebruiker die de uitgave heeft ingevoerd, de uitgever is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het project "publiceer als Rij van het Verzoek van de Hulp"heeft die op het lusje van de Opstelling van de Rij wordt toegelaten.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak Voltooien aan Taak Toegewezen aan</p> </td> 
   <td> <p>Een taak waaraan ik ben toegewezen, is voltooid.</p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de taak is voltooid. Meldingen worden niet verzonden wanneer een persoonlijke taak is voltooid.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> <p>Gebruikers met een licentie voor een revisie of aanvrager ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak Voltooien aan Van de Taak afhankelijke</p> </td> 
   <td> <p>Een voorganger van een van mijn taken is voltooid.</p> <p>De toegewezen taak ontvangt een e-mailbericht wanneer een van de voorgangers van hun taak is voltooid.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Geplande voltooiingsdatum van taak gewijzigd</p> </td> 
   <td> <p>De vervaldatum wijzigt in een taak waaraan ik ben toegewezen.</p> <p>De toegewezen Taak ontvangt een e-mailbericht wanneer de Geplande Datum van Voltooiing van de taak verandert, tenzij de gebruiker die de Geplande Datum van Voltooiing veranderde ook de Toegewezen Taak is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus om het even wat buiten Planning is.</p> <p>Er wordt geen melding verzonden met betrekking tot persoonlijke taken.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taakstatus wijzigen in Taak toegewezen aan</p> </td> 
   <td> <p>De status verandert op een taak waaraan ik ben toegewezen.</p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de status van de taak verandert, tenzij de gebruiker die de status heeft gewijzigd ook de ontvanger is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding. </p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informatie over projecten die ik op

Zie ook [Meldingen: Informatie over projecten die ik op](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Huidige verandering van de Status van het Project in het Team van het Project</p> </td> 
   <td> <p>Een project dat ik aan zet, wordt actief.</p> <p>De gebruikers op het project ontvangen een e-mailbericht wanneer het project actief wordt.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document toevoegen aan projectteam</p> </td> 
   <td> <p>Er wordt een document toegevoegd aan een project waarop ik sta.</p> <p>De gebruikers op het projectteam ontvangen een e-mailbericht wanneer een document aan het project, behalve de gebruiker wordt toegevoegd die het document toevoegde.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en het document niet Privé is. </p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Probleem toevoegen aan projectteam</p> </td> 
   <td> <p>Een kwestie wordt toegevoegd aan een project ik op ben.</p> <p>De gebruikers in een project ontvangen een e-mailbericht wanneer een kwestie aan het project wordt toegevoegd.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Voltooiing van probleem aan het Team van het Project</p> </td> 
   <td> <p>Een kwestie wordt voltooid over een project waar ik aan sta.</p> <p>Om het even welke gebruiker op het project ontvangt een bericht.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Voltooiing van de Taak van de mijlpaal aan het Team van het Project</p> </td> 
   <td> <p>Een mijlpaal-taak is voltooid voor een project waar ik mee bezig ben.</p> <p>Alle gebruikers op het Team van het Project ontvangen een bericht wanneer een milestone taak wordt voltooid. </p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Voltooiing van project voor projectteam</p> </td> 
   <td> <p>Een project dat ik heb, is voltooid.</p> <p>De gebruikers op een projectteam ontvangen een e-mailbericht wanneer de projectstatus Voltooid is.</p> <p>Tip: Als projecten regelmatig worden voltooid, kan het toelaten van deze optie tot veel e-mail voor gebruikers leiden die een beperkt aantal taken op vele projecten hebben. </p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Verandering van de Status van het project in het Team van het Project</p> </td> 
   <td> <p>De status verandert in een project waar ik aan sta.</p> <p>De gebruikers op het Team van het Project ontvangen een e-mailbericht wanneer de status van het project verandert. </p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projectgebruiker</p> </td> 
   <td> <p>Projectgebruiker toevoegen aan projectgebruiker</p> </td> 
   <td> <p>Ik ben toegevoegd aan een project.</p> <p>De gebruiker die aan het project werd toegevoegd ontvangt een e-mailbericht wanneer zij worden toegevoegd, tenzij de gebruiker zelf-toegevoegd aan het project was.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak Voltooien aan het Team van het Project</p> </td> 
   <td> <p>Een taak is voltooid voor een project waar ik mee bezig ben.</p> <p>De leden van het projectteam ontvangen een e-mailbericht.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Niet toegewezen Uitgave die aan het Team van het Project wordt toegevoegd</p> </td> 
   <td> <p>Een niet toegewezen kwestie wordt toegevoegd aan een project ik op ben.</p> <p>De gebruikers op een project ontvangen een e-mailbericht wanneer een niet toegewezen kwestie aan het project wordt toegevoegd.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informatie over projecten die ik bezit

Zie ook [Meldingen: Informatie over projecten die ik bezit](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document toevoegen aan projecteigenaar</p> </td> 
   <td> <p>Een document wordt toegevoegd aan een project dat ik bezit.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer een document aan het project wordt toegevoegd, tenzij de gebruiker die het document heeft toegevoegd ook de eigenaar van het project is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en het document niet Privé is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Probleem toevoegen aan projecteigenaar</p> </td> 
   <td> <p>Een kwestie wordt toegevoegd aan een project ik bezit.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer een uitgave aan het project wordt toegevoegd.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Datum van uitgave vastleggen wijzigen in projecteigenaar</p> </td> 
   <td> <p>De datum van het vastleggen verandert voor een kwestie over één van mijn projecten.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer de Datum van het Vastleggen voor een kwestie op het project verandert, tenzij de gebruiker die de Datum van het Vastleggen verandert de zelfde gebruiker is zoals de Eigenaar van het Project.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Voltooiing van probleem aan projecteigenaar</p> </td> 
   <td> <p>Een kwestie wordt voltooid over een project dat ik bezit.</p> <p>De eigenaar van het project ontvangt een e-mailbericht.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Mijlpaal taak Voltooien naar projecteigenaar</p> </td> 
   <td> <p>Een mijlpaal is een project dat ik heb.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Toewijzing projecteigenaar aan projecteigenaar</p> </td> 
   <td> <p>Ik ben de eigenaar van een nieuw project.</p> <p>Wanneer een gebruiker als eigenaar van een project wordt toegewezen, ontvangt die gebruiker een e-mailbericht.</p> <p>Als de eigenaar van het project dezelfde gebruiker is die de toewijzing heeft uitgevoerd, wordt geen e-mailmelding verzonden</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Voortgangswijziging van project in projecteigenaar</p> </td> 
   <td> <p>Een project dat ik heb loopt achter.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer het project achter schema ligt.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak Datumwijziging vastleggen in projecteigenaar</p> </td> 
   <td> <p>De datum van het plegen verandert voor een taak op één van mijn projecten.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer de datum vastleggen verandert voor een taak in het project, tenzij de gebruiker die de datum heeft gewijzigd, ook de eigenaar van het project is.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak Voltooien aan de Eigenaar van het Project</p> </td> 
   <td> <p>Een taak is voltooid voor een project dat ik bezit.</p> <p>De eigenaar van het project ontvangt een kennisgeving. </p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Voortgangswijziging taak in projecteigenaar</p> </td> 
   <td> <p>Een taak voor een project dat ik heb, loopt achter.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer een taak in het project achterloopt op schema.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Niet-toegewezen probleem toevoegen aan projecteigenaar</p> </td> 
   <td> <p>Een niet toegewezen kwestie wordt toegevoegd aan een project I bezit.</p> <p>De eigenaar van het project ontvangt een e-mailbericht wanneer een niet-toegewezen uitgave aan het project wordt toegevoegd.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informatie over door mij gefinancierde projecten

Zie ook [Meldingen: Informatie over door mij gefinancierde projecten](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document toevoegen aan projectsponsor</p> </td> 
   <td> <p>Een document wordt toegevoegd aan een project dat ik sponsor.</p> <p>De projectsponsor ontvangt een e-mailbericht wanneer een document aan het project wordt toegevoegd, tenzij het document wordt toegevoegd door de projectsponsor.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het document niet Privé is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Probleem toevoegen aan projectsponsor</p> </td> 
   <td> <p>Er wordt een probleem toegevoegd aan een project dat ik sponsor.</p> <p>De projectsponsor ontvangt een e-mailbericht wanneer een uitgave aan het project wordt toegevoegd.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Voltooiing van probleem aan projectsponsor</p> </td> 
   <td> <p>Er is een probleem met een project dat ik sponsor.</p> <p>De projectsponsor ontvangt een e-mailkennisgeving.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Mijlpaal taak Voltooien naar projectsponsor</p> </td> 
   <td> <p>Een mijlpalettaak is voltooid voor een project dat ik sponsor.</p> <p>De projectsponsor ontvangt een e-mailbericht wanneer een mijlpaal taak wordt voltooid voor een project dat hij of zij financiert.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Voortgangswijziging project naar projectsponsor</p> </td> 
   <td> <p>Een project dat ik sponsor, loopt achter.</p> <p>De projectsponsor ontvangt een e-mailbericht wanneer het project achterloopt op schema.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Projectsponsor toewijzen aan projectsponsor</p> </td> 
   <td> <p>Ik ben de sponsor van een project.</p> <p>De projectsponsor ontvangt een e-mailkennisgeving wanneer deze wordt ingesteld als de sponsor van een project.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak Voltooien naar projectsponsor</p> </td> 
   <td> <p>Een taak is voltooid voor een project dat ik sponsor.</p> <p>De projectsponsor ontvangt een e-mailkennisgeving.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Voortgangswijziging taak naar projectsponsor</p> </td> 
   <td> <p>Een taak voor een project dat ik sponsor, loopt achter.</p> <p>De projectsponsor ontvangt een e-mailbericht wanneer een taak in het project achterloopt op schema.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Niet-toegewezen probleem toevoegen aan projectsponsor</p> </td> 
   <td> <p>Er wordt een niet-toegewezen uitgave toegevoegd aan een project dat ik sponsor.</p> <p>De projectsponsor ontvangt een e-mailbericht wanneer een niet-toegewezen uitgave aan het project wordt toegevoegd.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overige informatie

Zie ook [Meldingen: Overige informatie](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objecttype</th> 
   <th>Gebeurtenis</th> 
   <th>Beschrijving</th> 
   <th> Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aankondiging</td> 
   <td> <p>Aankondiging toegevoegd</p> </td> 
   <td> <p>Er wordt een bericht verzonden naar het Aankondigingscentrum.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Verzoek om document Annuleren aan gezochte persoon</p> </td> 
   <td> <p>Annuleer een aanvraag voor het uploaden van documenten van mij.</p> <p>De documentaanvrager ontvangt een e-mailbericht wanneer een documentverzoek wordt geannuleerd.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Foutmelding</p> </td> 
   <td> <p>Er is een fout gevonden die uw aandacht vereist.</p> <p>Er wordt een e-mailbericht gegenereerd nadat Workfront een poging heeft gedaan en geen verbinding met een POP-account heeft gemaakt. Na 25 pogingen, maakt Workfront de verbinding aan POP rekening onbruikbaar om middelen te bewaren en het verzendt een bericht. </p> <p>Het e-mailbericht wordt verzonden naar de eigenaar van het project, als de POP-e-mail is gekoppeld aan een aanvraagwachtrij, of naar de Workfront-beheerders als de POP-account is gekoppeld aan de functie "Incoming Mail" in E-mailinstelling.
   </p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem</p> </td> 
   <td> <p>Uitgave toewijzen aan eigenaar van bron</p> </td> 
   <td> <p>Een wijziging in de toewijzing van uitgaven is van invloed op een van mijn mensen.</p> <p>De manager van de Ontvanger van de Uitgave ontvangt een e-mailbericht wanneer een verandering een gebruiker beïnvloedt zij leiden.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gebruiker</p> </td> 
   <td> <p>Nieuwe gebruiker aan Gebruiker</p> </td> 
   <td> <p>Verzend de gebruiker via e-mail wanneer een nieuwe gebruiker in Workfront wordt gemaakt.</p> <p>Nadat de nieuwe gebruiker is gemaakt, ontvangt de gebruiker een e-mailuitnodiging, waarin hij of zij aangeeft dat een Workfront-account is gemaakt en waarin hij of zij wordt gevraagd hun wachtwoord in te stellen.</p> <p>Wanneer gebruikers een nieuwe gebruiker maken, kunnen ze de optie "E-mail voor een uitnodiging naar deze persoon verzenden" selecteren (zoals beschreven in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Gebruikers toevoegen</a><span style="font-weight: 400;">). Wanneer de optie Nieuwe gebruiker naar gebruiker echter is ingeschakeld, ontvangen alle nieuwe gebruikers de e-mailuitnodiging, ongeacht of de optie "E-mailuitnodiging verzenden naar deze persoon" is geselecteerd.</span></p> </td> 
   <td> Inactief </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Object delen naar team</p> </td> 
   <td> <p>Iemand deelt een object met mijn team.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gebruiker</p> </td> 
   <td> <p>Object delen over gebruiker</p> </td> 
   <td> <p>Iemand deelt een object met mij.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projectgebruiker</p> </td> 
   <td> <p>Projectgebruiker toevoegen aan Resource Owner</p> </td> 
   <td> <p>Een van mijn mensen is toegevoegd aan een project.</p> <p>Een manager ontvangt een e-mailbericht wanneer een van zijn of haar directe rapporten aan een project wordt toegevoegd.</p> <p>Gebruikers met een Revisielicentie ontvangen geen melding.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project toegevoegd aan een portfolio of programma</p> </td> 
   <td> <p>Iemand voegt een project toe aan een portfolio of programma waarvan ik eigenaar ben.</p> </td> 
   <td> <p>Actief</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak</p> </td> 
   <td> <p>Taak toewijzen aan Resource Owner</p> </td> 
   <td> <p>Een wijziging in de taaktoewijzing is van invloed op een van mijn mensen.</p> <p>De manager van de Taak van de Ontvanger ontvangt een e-mailbericht.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> </td> 
   <td> <p>Inactief</p> </td> 
  </tr> 
  <tr> 
   <td> Project <br>Taak <br>Probleem</td> 
   <td>Nieuwe update voor abonnee </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Er wordt een e-mail verzonden wanneer er een update wordt uitgevoerd naar een taak, uitgave of project waarop ik ben geabonneerd.</span> </p> </td> 
   <td>Actief</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Delegatie

Zie ook [Meldingen: Delegatie](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Objecttype | Gebeurtenis | Beschrijving | Standaardstatus |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Taken en problemen | Taak en delegatie aan de verkrijger | Ik delegeer mijn taken en problemen (bevestiging) | Actief |
| Taken en problemen | Taak beëindigen en delegatie aan de toegewezen persoon afgeven | Ik stop de delegatie van mijn taken en kwesties (bevestiging) | Actief |
| Taken en problemen | Taak en afgifte van delegatie | Iemand delegeert zijn taken en kwesties aan mij | Actief |
| Taken en problemen | Taken stoppen en delegeren aan gedelegeerde personen afgeven | Iemand stopt de delegatie van zijn taken en kwesties aan mij | Actief |
