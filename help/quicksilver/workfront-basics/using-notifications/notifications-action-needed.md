---
content-type: reference
navigation-topic: notifications
title: 'Meldingen: actie nodig'
description: Met de volgende meldingen kunt u zien of u actie moet ondernemen met betrekking tot een werkitem. Zie Uw eigen e-mailmeldingen wijzigen voor informatie over het configureren van welke meldingen u ontvangt.
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 0%

---

# Meldingen: [!UICONTROL Action needed]

Met de volgende meldingen kunt u zien of u actie moet ondernemen met betrekking tot een werkitem. Zie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) voor informatie over het configureren van de meldingen die u ontvangt.

Zie ook [gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th> <p>Inclusief velden </p> <p> *Alleen dagelijkse overzichtsvelden</p> </th> 
   <th>Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Ik krijg een nieuw werkverzoek</strong> </p> <p>De toegewezen persoon van het werkitem ontvangt een e-mailmelding, tenzij de gebruiker die het verzoek indient ook de toegewezen persoon is. </p> <p>Er wordt geen melding verzonden als de taakstatus [!UICONTROL Complete] is of de probleemstatus [!UICONTROL Closed] is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL New Work Request]: &lt;naam aanvraag&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is: <em>[!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> <p>Taaknaam</p> <p>[!UICONTROL Planned Completion Date]</p> <p>Ouders</p> <p>Toegewezen door</p> <p>Toegewezen aan</p> <p>[!UICONTROL Status]</p> <p>[!UICONTROL Description]</p> <p>[!UICONTROL View] knop<br>Optie om toe te voegen aan het dagelijks overzicht</p> <br> </td> 
   <td><strong>Onmiddellijk en </strong> <strong> per dag</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een document goedkeuren</strong> </p> <p>De goedkeurder van een document ontvangt een melding wanneer deze als de goedkeurder worden vermeld.</p> <p>Het onderwerp van de direct-mailmelding is: <em>&lt;Naam van de gebruiker die de goedkeuring heeft ingediend&gt; [!UICONTROL asked you to approve a document in [!DNL Adobe Workfront].]</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> Projectnaam<br>Naam Portfolio<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>Documentnaam<br>Referentienummer<br>Datum en tijd van goedkeuring aangevraagd<br>Documentdetails (formaat, grootte, versienummer)<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal in behandeling zijnde documentgoedkeuringen<br>*Koppeling naar <strong>[!UICONTROL Document Approvals</strong>*<strong>See All Approvals]</strong> knop<br>*Datum van het dagelijks overzicht<br></td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een project goedkeuren</strong> </p> <p>Bij goedkeuringen van taakrollen is het afhankelijk van de vraag welke gebruikers een e-mailmelding voor deze gebeurtenis ontvangen of de instelling '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' is ingeschakeld (zoals beschreven in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren</a>). </p> <p><strong>Als deze optie is ingeschakeld </strong>, wordt een e-mailmelding verzonden naar alle gebruikers in het systeem met de taakrol die aan de goedkeuring is gekoppeld. </p> <p><strong>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de taakrol die is gekoppeld aan het goedkeuringsproces een e-mailmelding.</p> <p>Als de goedkeuring is gekoppeld aan een gebruiker, ontvangt die gebruiker de melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Project Pending Approval]: &lt;projectnaam&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;datum van het dagelijkse overzicht&gt; </em></p> </td> 
   <td> <p>Projectnaam<br>goedkeuringsnaam<br>projectreferentienummer<br>naam van de gebruiker die de Portfolio heeft ingediend<br>in afwachting van goedkeuringsstatus<br>datum en tijd van goedkeuring aangevraagd<br>projectprioriteit<br>goedkeuringsstap in afwachting van goedkeuring<br>aantal beslissingen die wachten op goedkeuring<br>naam van de goedkeurder (alleen gebruikers)<br>[!UICONTROL Project Planned Completion Date] <br><strong>[!UICONTROL Make Approval Decision]</strong> knop <br>*totaal aantal in behandeling zijnde projectgoedkeuringen <br>*koppeling naar <strong>[!UICONTROL Project Approvals]</strong><br>*<strong>[!UICONTROL See All Approvals]</strong> knop<br>*datum van de dag overzicht</p> </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een taak goedkeuren</strong> </p> <p>Bij goedkeuringen van taakrollen is het afhankelijk van de vraag welke gebruikers een e-mailmelding voor deze gebeurtenis ontvangen of de instelling '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' is ingeschakeld (zoals beschreven in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren </a>). </p> <p><strong> Als deze optie is ingeschakeld </strong>, wordt een e-mailmelding verzonden naar alle gebruikers in het systeem met de taakrol die aan de goedkeuring is gekoppeld. </p> <p><strong>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de taakrol die is gekoppeld aan het goedkeuringsproces een e-mailmelding.</p> <p>Als de goedkeuring is gekoppeld aan een gebruiker, ontvangt die gebruiker de melding. </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Task Pending Approval]: &lt;Taaknaam&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;datum van het dagelijkse overzicht&gt; </em></p> </td> 
   <td> <p>Taaknaam<br>Projectnaam<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>In behandeling zijnde goedkeuringsstatus<br>Datum en tijd van goedkeuring aangevraagd<br>Taakprioriteit<br>Naam goedkeuringsfase<br>Naam goedkeurder<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal in behandeling zijnde taakgoedkeuringen<br>*Koppeling naar knop<strong>[!UICONTROL Task Approvals *See All Approvals]</strong><strong></strong>*Datum van het dagelijkse overzicht<br></p> </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een timesheet</strong> goedkeuren </p> <p>De Timesheet-goedkeurder ontvangt een e-mailmelding wanneer een timesheet wordt verzonden die moet worden goedgekeurd, tenzij de gebruiker die de timesheet heeft ingediend ook de Timesheet-goedkeurder is.</p> <p>Er wordt alleen een melding verzonden als de status van het timesheet [!UICONTROL Submitted] is.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Timesheet Submitted]: &lt;Timesheet Owner&gt;, &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;datum van het dagelijkse overzicht&gt; </em></p> </td> 
   <td> Naam van de gebruiker die de urenlijst ter goedkeuring heeft ingediend<br>Datum en tijdstip waarop de urenlijst is ingediend<br>Status van de urenlijst<br>Begin- en einddatum van de urenlijst<br>Aantal uren geregistreerd op de urenlijst<br>Aantal overuren geregistreerd op de urenlijst<br><strong>[!UICONTROL Review]</strong> en <strong>[!UICONTROL Approve]</strong> knoppen<br>*Totaal aantal openstaande urenbladen<br>*Link naar <strong>[!UICONTROL Timesheet Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop<br>*Datum van het dagelijks overzicht </td> 
   <td><strong>Onmiddellijk en </strong> <strong>Dagelijks</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een probleem goedkeuren</strong> </p> <p>Bij goedkeuringen van taakrollen is het afhankelijk van welke gebruikers een e-mailmelding voor deze gebeurtenis ontvangen of de instelling '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' is ingeschakeld (zoals beschreven in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configure global approval] instellingen </a>). </p> <p><strong>Als deze optie is ingeschakeld </strong>, wordt een e-mailmelding verzonden naar alle gebruikers in het systeem met de taakrol die aan de goedkeuring is gekoppeld. </p> <p><strong>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de taakrol die is gekoppeld aan het goedkeuringsproces een e-mailmelding.</p> <p>Als de goedkeuring is gekoppeld aan een gebruiker, ontvangt die gebruiker de melding. </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Issue Pending Approval]: &lt;naam van probleem&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;datum van het dagelijkse overzicht&gt; </em></p> </td> 
   <td> Naam van probleem<br>Projectnaam<br>Referentienummer van probleem<br>Naam van de gebruiker die het probleem ter goedkeuring heeft ingediend<br> In behandeling zijnde goedkeuringsstatus<br> Datum en tijd van goedkeuring aangevraagd<br>Prioriteit van probleem<br>Goedkeuringsfase<br>Naam van de goedkeurder<br>[!UICONTROL Issue Planned Completion Date]<br>[!UICONTROL Primary Contact]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop <br>*Totaal aantal in behandeling zijnde goedkeuringsprocedures<br>*Link naar <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop <br> Datum van het dagelijks overzicht </td> 
   <td><strong>Onmiddellijk en </strong> <strong> per dag</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een projectgoedkeuring controleren die ik heb gedelegeerd</strong> </p> <p>Er is een projectgoedkeuring aan u gedelegeerd en u moet deze beoordelen.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Delegated Project Approval - Please Review] &lt;projectnaam&gt;</em></p> <p><em>Het onderwerp van de dagelijkse overzichtsmelding is: [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em> </p> </td> 
   <td> Projectnaam <br>naam Portfolio<br>projectreferentienummer<br>naam van de gebruiker die om goedkeuring heeft gevraagd<br>naam van de gebruiker namens wie u het project goedkeurt<br>status in behandeling<br>datum en tijd van goedkeuring aangevraagd<br>projectprioriteit<br>goedkeuringsstap<br>namen van goedkeurders<br>[!UICONTROL Project Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*totaal aantal in behandeling zijnde projectgoedkeuringen<br>*koppeling <strong>[!UICONTROL Project Approvals *See All Approvals]</strong> knop <br>*Datum van het dagelijks overzicht </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een taakgoedkeuring controleren die ik heb gedelegeerd</strong> </p> <p>Een taakgoedkeuring is aan u gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Delegated Task Approval - Please Review ]&lt;Taaknaam&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> De Naam van het Project van de taak {<br> Naam van het Referentienummer van 1} Taak <br> van de gebruiker die om goedkeuring <br> Naam van de gebruiker vroeg namens wie u de Taak <br> goedkeurt Hangende de Status van de Goedkeuring <br> Datum en Tijd van Goedkeuring verzocht <br> de Prioriteit van de Taak {<br> Namen van het Stadium van de Goedkeuring <br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knoop <br>*Totaal aantal van wachtende taakgoedkeurende taakgoedkeuringen <br>*1} aan <br> <br> knop <br>*Datum van de dagelijkse samenvatting<strong>[!UICONTROL Task Approvals *See All Approvals]</strong> </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een probleemgoedkeuring bekijken die ik heb gedelegeerd</strong> </p> <p>Een probleemgoedkeuring is aan u gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Delegated Issue Approval - Please Review] &lt;naam van probleem&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> Naam van probleem<br>Projectnaam<br>Referentienummer van probleem<br>Naam van de gebruiker die om goedkeuring heeft gevraagd<br>Naam van de gebruiker namens wie u het probleem goedkeurt<br>Status van goedkeuring in behandeling<br>Datum en tijd van goedkeuring aangevraagd<br>Prioriteit van probleem <br>Goedkeuringsfase<br>Naam van de goedkeurder<br>Datum van voltooiing gepland probleem<br>Primair contact<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal openstaande probleemgoedkeuringen<br>*Koppeling naar <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop<br>*Datum van het dagelijks overzicht<br></td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik ben toegewezen aan een probleem</strong> </p> <p>De toegewezen probleemmelding ontvangt een e-mailmelding. De toegewezen probleemmelding ontvangt geen e-mail als de status van het probleem is of gelijk is aan [!UICONTROL Closed].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL New Work Request]: &lt;naam van probleem&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> <p>Probleemnaam<br>Projectnaam<br>[!UICONTROL Issue Reference Number]<br>Uw naam<br>Vervaldatum probleem ([!UICONTROL Planned Completion Date])<br>Naam van de gebruiker die het probleem aan u heeft toegewezen<br><strong>[!UICONTROL Work On It]</strong> knop<br>*Totaal aantal opdrachten<br>*Totaal aantal taken en problemen dat aan u is toegewezen<br>*Koppeling naar <strong>[!UICONTROL Work Requests]</strong><br>*Datum van het dagelijks overzicht<br></p> </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik ben ingesteld als de primaire toegewezen persoon voor een taak</strong> </p> <p>De Toegewezen Taak ontvangt een e-mail melding als hij of zij de primaire toewijzer is van de taak, tenzij de Toegewezen Taak de gebruiker is die de toewijzing heeft gedaan.</p> <p>Er wordt een melding verzonden als de projectstatus [!UICONTROL Current] is en de taak niet gemarkeerd [!UICONTROL Complete] is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL New Work Request]: &lt;taaknaam&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Uw naam<br>Taakvervaldatum ([!UICONTROL Planned Completion Date])<br>Naam van de gebruiker die de taak aan u heeft toegewezen<br><strong>[!UICONTROL Work On It]</strong> knop<br>*Totaal aantal taken en problemen dat aan u is toegewezen<br>*Koppeling naar <strong>[!UICONTROL Work Requests]</strong>*Datum van het dagelijks overzicht </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn team krijgt een nieuw werkverzoek</strong> </p> <p>Teamleden ontvangen een e-mail melding wanneer het team een nieuw werkverzoek ontvangt. (De gebruiker die de aanvraag heeft ingediend, ontvangt geen melding als hij of zij lid is van het team.)</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is en de werkaanvraagstatus [!UICONTROL New] is.</p> <p>Gebruikers met een [!UICONTROL Review] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL New Work Request]: &lt;naam aanvraag&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is: <em>[!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> <p> Naam probleem<br>Projectnaam (naam aanvraagwachtrij)<br>Referentienummer probleem<br>Teamnaam<br>Vervaldatum probleem (geplande voltooiingsdatum)<br>Naam van de gebruiker die de aanvraag heeft ingediend<br><strong>[!UICONTROL Work On It]</strong> knop <br>*Totaal aantal aanvragen dat is toegewezen aan uw team</p> <p>*Naam werkaanvraag</p> <p>[!UICONTROL *Planned Completion Date]</p> <p>*Naam van de gebruiker die de aanvraag heeft ingediend<br>*Link naar <strong>[!UICONTROL Team Requests]</strong><br>*Datum van het dagelijks overzicht </p> <p><span class="preview">*Teamtoewijzingen</span> </p> </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn timesheet is opnieuw geopend</strong> </p> <p>De Timesheet Eigenaar ontvangt een e-mail melding wanneer de Timesheet opnieuw wordt geopend, tenzij de gebruiker die de Timesheet opnieuw heeft geopend ook de eigenaar van de Timesheet is.</p> <p>Een e-mailmelding wordt alleen verzonden als de tijdbladstatus [!UICONTROL Open] is.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Timesheet Re-opened]: &lt;begindatum werkblad&gt; - &lt;einddatum werkblad&gt;</em></p> <p>Opmerking: U kunt deze melding niet configureren voor een dagelijkse overzichtsmail.</p> </td> 
   <td> Naam van de gebruiker die de urenlijst<br>Datum en tijd waarop de urenlijst werd heropend<br>Status van de urenlijst ([!UICONTROL Re-opened])<br>Aantal geregistreerde uren op de urenlijst<br>Aantal geregistreerde overuren op de urenlijst<br><strong>[!UICONTROL Review]</strong> </td> 
   <td><strong>Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn timesheet is afgewezen</strong> </p> <p>De Timesheet Eigenaar ontvangt een e-mail melding wanneer de timesheet wordt afgewezen, tenzij de gebruiker die de timesheet heeft afgewezen ook de eigenaar is.</p> <p>Een e-mailmelding wordt alleen verzonden als de tijdbladstatus [!UICONTROL Rejected] is.</p> <p>Het onderwerp van de direct-mail-melding is: <em>[!UICONTROL Timesheet Rejected]:&lt;Startdatum van de timesheet&gt; - &lt;Einddatum van de timesheet&gt;</em></p> <p>Opmerking: U kunt deze melding niet configureren voor een dagelijkse overzichtsmail.</p> </td> 
   <td> Naam van de gebruiker die de Timesheet<br>Status van de Timesheet ([!UICONTROL Rejected])<br>Datum en tijd waarop de Timesheet is afgewezen<br><strong>[!UICONTROL Review]</strong> knop heeft afgewezen </td> 
   <td><strong>Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand vraagt toegang tot mij</strong> </p> <p>Ik vraag om iets te doen, dus zet het aan.</p> <p>De persoon die het project maakt, krijgt toegang tot het project.</p> <p>Hierdoor krijgt de gebruiker de melding wanneer iemand toegang aanvraagt.</p> <p>Het onderwerp van de direct-mailmelding is: <em>&lt;Naam van de gebruiker die toegang heeft aangevraagd&gt; [!UICONTROL needs access to] &lt;Objectnaam&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;datum van de dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> <p>Objectnaam <br> Naam bovenliggend object <br> Objectreferentienummer<br>Naam van de gebruiker die toegang heeft aangevraagd<br>Het type toegang dat de gebruiker aanvraagt<br><strong>[!UICONTROL Grant] &lt;Naam van de gevraagde toegang&gt; Toegang</strong> en <strong>[!UICONTROL Grant different access]</strong> knoppen<br>*Totaal aantal openstaande goedkeuringen voor toegangsverzoeken<br>*Koppeling naar <strong>[!UICONTROL Access Request]</strong> goedkeuringen<br>*Datum van dagelijkse samenvatting</p> </td> 
   <td><strong>Onmiddellijk en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand vraagt me om een document te uploaden</strong> </p> <p>De aanvrager van het document ontvangt een e-mailmelding wanneer een gebruiker een aanvraag ontvangt om een document te uploaden.</p> <p>Het onderwerp van de direct-mailmelding is: <em>&lt;Naam van de gebruiker die het document aanvraagt&gt; [!UICONTROL needs a document from you in [!DNL Workfront].]</em></p> <p> <p>Opmerking: U kunt deze melding niet configureren voor een dagelijkse overzichtsmail.</p> </p> </td> 
   <td> Naam van de gebruiker die het document<br>Naam van het object aanvraagt waar het document moet worden geüpload<br><strong>[!UICONTROL Attach it here]</strong> link </td> 
   <td><strong>Onmiddellijk </strong> </td> 
  </tr> 
 </tbody> 
</table>
