---
content-type: reference
navigation-topic: notifications
title: "Meldingen: Actie vereist"
description: In de volgende meldingen wordt u geïnformeerd of u actie moet ondernemen voor een tijdelijk onderdeel. Zie Uw eigen e-mailmeldingen wijzigen voor informatie over het configureren van de berichten die u ontvangt.
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 0%

---

# Meldingen: [!UICONTROL Action needed]

In de volgende meldingen wordt u geïnformeerd of u actie moet ondernemen voor een tijdelijk onderdeel. Voor informatie over het vormen van welke berichten u ontvangt, zie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [Gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th> <p>Inclusief velden </p> <p> *Alleen velden voor dagelijkse samenvatting</p> </th> 
   <th>Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Ik krijg een nieuw verzoek voor werk</strong> </p> <p>De ontvanger van het werkitem ontvangt een e-mailbericht, tenzij de gebruiker die het verzoek indient ook de ontvanger is. </p> <p>Er wordt geen melding verzonden als de taakstatus [!UICONTROL Complete] of de uitgiftestatus [!UICONTROL Closed].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL New Work Request]: &lt;request name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is: <em>[!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Taaknaam</p> <p>[!UICONTROL Planned Completion Date]</p> <p>Ouders</p> <p>Toegewezen door</p> <p>Toegewezen aan</p> <p>[!UICONTROL Status]</p> <p>[!UICONTROL Description]</p> <p>[!UICONTROL View] knop<br>Optie om toe te voegen aan de dagelijkse samenvatting</p> <br> </td> 
   <td><strong>Direct en</strong> <strong>Dagelijks</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een document goedkeuren</strong> </p> <p>De fiatteur van een document ontvangt een melding wanneer deze als fiatteur wordt vermeld.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [!UICONTROL asked you to approve a document in [!DNL Adobe Workfront].]</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Projectnaam<br>Naam Portfolio<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>Documentnaam<br>Referentienummer document<br>Datum en tijdstip van de aangevraagde erkenning<br>Documentdetails (formaat, grootte, versienummer)<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal goedkeuringen voor documenten die in behandeling zijn<br>*Koppeling naar <strong>[!UICONTROL Document Approvals</strong>*<strong>See All Approvals]</strong> knop<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een project goedkeuren</strong> </p> <p>Welke gebruikers een e-mailmelding ontvangen voor deze gebeurtenis, is afhankelijk van het feit of de code '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' instelling is ingeschakeld (zoals beschreven in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren</a>). </p> <p><strong>Als deze optie is ingeschakeld</strong>, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de taakrol die aan de goedkeuring is gekoppeld. </p> <p><strong>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de taakrol die is gekoppeld aan het goedkeuringsproces een e-mailmelding.</p> <p>Als de goedkeuring aan een gebruiker wordt geassocieerd, ontvangt die gebruiker het bericht.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Project Pending Approval]: &lt;project name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projectnaam<br>Naam Portfolio<br>Projectreferentienummer<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>In afwachting van goedkeuringsstatus<br>Datum en tijdstip van de aangevraagde erkenning<br>Projectprioriteit<br>Goedkeuringsstap in afwachting van goedkeuring<br>Aantal beslissingen dat op goedkeuring wacht<br>Naam fiatteurs (alleen gebruikers)<br>[!UICONTROL Project Planned Completion Date] <br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal goedkeuringen voor lopende projecten <br>*Koppeling naar <strong>[!UICONTROL Project Approvals]</strong><br>*<strong>[!UICONTROL See All Approvals]</strong> knop<br>*Datum van de dagelijkse samenvatting</p> </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een taak goedkeuren</strong> </p> <p>Welke gebruikers een e-mailmelding ontvangen voor deze gebeurtenis, is afhankelijk van het feit of de code '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' instelling is ingeschakeld (zoals beschreven in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Algemene goedkeuringsinstellingen configureren</a>). </p> <p><strong>Als deze optie is ingeschakeld</strong>, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de taakrol die aan de goedkeuring is gekoppeld. </p> <p><strong>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de taakrol die is gekoppeld aan het goedkeuringsproces een e-mailmelding.</p> <p>Als de goedkeuring aan een gebruiker wordt geassocieerd, ontvangt die gebruiker het bericht. </p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Task Pending Approval]: &lt;task name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Taaknaam<br>Projectnaam<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>In afwachting van goedkeuringsstatus<br>Datum en tijdstip van de aangevraagde erkenning<br>Taakprioriteit<br>Naam goedkeuringswerkgebied<br>Namen van fiatteurs<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal lopende taakgoedkeuringen<br>*Koppeling naar<strong>[!UICONTROL Task Approvals *See All Approvals]</strong> knop<strong></strong>*Datum van de dagelijkse samenvatting<br></p> </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een tijdschema goedkeuren</strong> </p> <p>De Tijdopmaakfiatteur ontvangt een e-mailbericht wanneer een timesheet wordt voorgelegd dat zij moeten goedkeuren, tenzij de gebruiker die timesheet indiende ook de fiatteur van de Tijdopmaak is.</p> <p>Een bericht wordt slechts verzonden als de status van timesheet is [!UICONTROL Submitted].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Timesheet Submitted]: &lt;timesheet owner=""&gt;, &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> Naam van de gebruiker die het tijdspad ter goedkeuring heeft ingediend<br>Datum en tijd waarop het tijdschema is ingediend<br>Status van het tijdschema<br>Begin- en einddatum van de tijdlijn<br>Aantal uren die op timesheet worden geregistreerd<br>Aantal overuren die op timesheet worden geregistreerd<br><strong>[!UICONTROL Review]</strong> en <strong>[!UICONTROL Approve]</strong> knoppen<br>*The total number of pending timesheet goedkeuringen<br>*Koppeling naar <strong>[!UICONTROL Timesheet Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Direct en</strong> <strong>Dagelijks</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een kwestie goedkeuren</strong> </p> <p>Welke gebruikers een e-mailmelding ontvangen voor deze gebeurtenis, is afhankelijk van het feit of de code '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' instelling is ingeschakeld (zoals beschreven in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configure global approval] instellingen</a>). </p> <p><strong>Als deze optie is ingeschakeld</strong>, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de taakrol die aan de goedkeuring is gekoppeld. </p> <p><strong>Als deze optie is uitgeschakeld</strong>, ontvangen alleen projectteamleden met de taakrol die is gekoppeld aan het goedkeuringsproces een e-mailmelding.</p> <p>Als de goedkeuring aan een gebruiker wordt geassocieerd, ontvangt die gebruiker het bericht. </p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Issue Pending Approval]: &lt;issue name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die de afgifte ter goedkeuring heeft ingediend<br>In afwachting van goedkeuringsstatus<br>Datum en tijdstip van de aangevraagde erkenning<br>Probleemprioriteit<br>Goedkeuringsfase<br>Namen van fiatteurs<br>[!UICONTROL Issue Planned Completion Date]<br>[!UICONTROL Primary Contact]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Het totale aantal goedkeuringen voor nog niet afgegeven certificaten<br>*Koppeling naar <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Direct en</strong> <strong>Dagelijks</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een projectgoedkeuring bekijken die ik ben gedelegeerd</strong> </p> <p>U hebt een projectgoedkeuring gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Delegated Project Approval - Please Review] &lt;project name=""&gt;</em></p> <p><em>Het onderwerp van de dagelijkse overzichtsmelding is: [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Projectnaam<br>Naam Portfolio<br>Projectreferentienummer<br>Naam van de gebruiker die goedkeuring heeft aangevraagd<br>Naam van de gebruiker namens wie u het Project goedkeurt<br>In afwachting van goedkeuringsstatus<br>Datum en tijdstip van de aangevraagde erkenning<br>Projectprioriteit<br>Goedkeuringsstap<br>Namen van fiatteurs<br>[!UICONTROL Project Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal goedkeuringen voor lopende projecten<br>*Koppeling naar <strong>[!UICONTROL Project Approvals *See All Approvals]</strong> knop <br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een taakgoedkeuring bekijken die ik ben gedelegeerd</strong> </p> <p>U hebt een taakgoedkeuring gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Delegated Task Approval - Please Review ]&lt;task name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Naam van de gebruiker die goedkeuring heeft aangevraagd<br>Naam van de gebruiker namens wie u de Taak goedkeurt<br>In afwachting van goedkeuringsstatus<br>Datum en tijdstip van de aangevraagde erkenning<br>Taakprioriteit<br>Goedkeuringsfase<br>Namen van fiatteurs<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop <br>*Totaal aantal lopende taakgoedkeuringen<br>*Koppeling naar <strong>[!UICONTROL Task Approvals *See All Approvals]</strong> knop<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik moet een goedkeuring van een probleem controleren als ik ben gedelegeerd</strong> </p> <p>U hebt een goedkeuring van een uitgave gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Delegated Issue Approval - Please Review] &lt;issue name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die goedkeuring heeft aangevraagd<br>Naam van de gebruiker namens wie u de kwestie goedkeurt<br>In afwachting van goedkeuringsstatus<br>Datum en tijdstip van de aangevraagde erkenning<br>Probleemprioriteit<br>Goedkeuringsfase<br>Namen van fiatteurs<br>Geplande afsluitdatum<br>Primaire contactpersoon<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal goedkeuringen voor afgifte in behandeling<br>*Koppeling naar <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik ben toegewezen aan een probleem</strong> </p> <p>De uitgever ontvangt een e-mailbericht. De uitgever ontvangt geen e-mail als de status van de uitgifte gelijk is aan [!UICONTROL Closed].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL New Work Request]: &lt;issue name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Naam van uitgave<br>Projectnaam<br>[!UICONTROL Issue Reference Number]<br>Uw naam<br>Vervaldatum van afgifte ([!UICONTROL Planned Completion Date])<br>Naam van de gebruiker die de uitgave aan u heeft toegewezen<br><strong>[!UICONTROL Work On It]</strong> knop<br>*Totaal aantal toewijzingen<br>*Totaal aantal taken en problemen toegewezen aan u<br>*Koppeling naar <strong>[!UICONTROL Work Requests]</strong><br>*Datum van de dagelijkse samenvatting<br></p> </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik ben ingesteld als de primaire taakontvanger</strong> </p> <p>De taakontvanger ontvangt een e-mailbericht als hij of zij de primaire ontvanger van de taak is, tenzij de ontvanger de gebruiker is die de taak heeft uitgevoerd.</p> <p>Een kennisgeving wordt verzonden als de projectstatus [!UICONTROL Current] en de taak is niet gemarkeerd [!UICONTROL Complete].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL New Work Request]: &lt;task name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Uw naam<br>Einddatum taak ([!UICONTROL Planned Completion Date])<br>Naam van de gebruiker die de taak aan u heeft toegewezen<br><strong>[!UICONTROL Work On It]</strong> knop<br>*Totaal aantal taken en problemen toegewezen aan u<br>*Koppeling naar <strong>[!UICONTROL Work Requests]</strong>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn team krijgt een nieuwe werkaanvraag</strong> </p> <p>De Leden van het team ontvangen een e-mailbericht wanneer het team een nieuw het werkverzoek ontvangt. (De gebruiker die het verzoek indiende ontvangt geen bericht als hij of zij een lid van het team is.)</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current] en de status van de werkaanvraag is [!UICONTROL New].</p> <p>Gebruikers met een [!UICONTROL Review] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL New Work Request]: &lt;request name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is: <em>[!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> Naam van uitgave<br>Projectnaam (naam wachtrij aanvragen)<br>Referentienummer van uitgave<br>Teamnaam<br>Vervaldatum afgifte (geplande afsluitdatum)<br>Naam van de gebruiker die het verzoek heeft ingediend<br><strong>[!UICONTROL Work On It]</strong> knop<br>*Totaal aantal aanvragen toegewezen aan uw team</p> <p>*Naam werkaanvraag</p> <p>[!UICONTROL *Planned Completion Date]</p> <p>*Naam van gebruiker die het verzoek heeft ingediend<br>*Koppeling naar <strong>[!UICONTROL Team Requests]</strong><br>*Datum van de dagelijkse samenvatting </p> <p><span class="preview">*Teamtoewijzingen</span> </p> </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn timesheet is opnieuw geopend</strong> </p> <p>De eigenaar van de tijdpagina ontvangt een e-mailbericht wanneer de tijdpagina opnieuw wordt geopend, tenzij de gebruiker die de tijdpagina opnieuw heeft geopend ook de eigenaar van de tijdpagina is.</p> <p>Een e-mailbericht wordt alleen verzonden als de status van het tijdblad is [!UICONTROL Open].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Timesheet Re-opened]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> Naam van de gebruiker die de tijdpagina opnieuw heeft geopend<br>Datum en tijd waarop de tijdpagina opnieuw is geopend<br>Status van het tijdschrift ([!UICONTROL Re-opened])<br>Aantal totale uren dat op de tijdkaart is aangemeld<br>Aantal overuren dat op de tijdspagina is aangemeld<br><strong>[!UICONTROL Review]</strong> knop </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn timesheet is afgewezen</strong> </p> <p>De eigenaar van de tijdpagina ontvangt een e-mailbericht wanneer de tijdpagina wordt afgewezen, tenzij de gebruiker die de tijdpagina heeft afgewezen ook de eigenaar is.</p> <p>Een e-mailbericht wordt alleen verzonden als de status van het tijdblad is [!UICONTROL Rejected].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Timesheet Rejected]:&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> Naam van de gebruiker die de tijdpagina heeft afgewezen<br>Status van het tijdschrift ([!UICONTROL Rejected])<br>Datum en tijdstip waarop het tijdschrift is afgewezen<br><strong>[!UICONTROL Review]</strong> knop </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand vraagt mij om toegang</strong> </p> <p>Ik verzoek me iets te doen, dus zet het aan.</p> <p>De persoon die het project creeert krijgt toegang tot het.</p> <p>Dit maakt de gebruiker het bericht krijgen wanneer iemand toegang aanvraagt.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [!UICONTROL needs access to] &lt;object name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Objectnaam<br>Naam bovenliggend object<br>Objectreferentienummer<br>Naam van de gebruiker die de toegang heeft aangevraagd<br>Het type toegang dat de gebruiker aanvraagt<br><strong>[!UICONTROL Grant] &lt;name of="" the="" access="" requested=""&gt; Toegang</strong> en <strong>[!UICONTROL Grant different access]</strong> knoppen<br>*Totaal aantal goedkeuringen voor toegangsaanvragen in behandeling<br>*Koppeling naar <strong>[!UICONTROL Access Request]</strong> Goedkeuringen<br>*Datum van de dagelijkse samenvatting</p> </td> 
   <td><strong>Direct en dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand vraagt mij een document te uploaden</strong> </p> <p>De documentaanvrager ontvangt een e-mailbericht wanneer een gebruiker een verzoek ontvangt om een document te uploaden.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; [!UICONTROL needs a document from you in [!DNL Workfront].]</em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Naam van de gebruiker die het document aanvraagt<br>Naam van het object waar het document moet worden geüpload<br><strong>[!UICONTROL Attach it here]</strong> link </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
 </tbody> 
</table>
