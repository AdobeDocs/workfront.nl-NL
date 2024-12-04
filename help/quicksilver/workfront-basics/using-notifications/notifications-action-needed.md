---
content-type: reference
navigation-topic: notifications
title: 'Meldingen: Actie vereist'
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

In de volgende meldingen wordt u geïnformeerd of u actie moet ondernemen voor een tijdelijk onderdeel. Voor informatie over het vormen van welke berichten u ontvangt, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [ de berichten van de Gebeurtenis ](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong> ik krijg een nieuw het werkverzoek </strong> </p> <p>De ontvanger van het werkitem ontvangt een e-mailbericht, tenzij de gebruiker die het verzoek indient ook de ontvanger is. </p> <p>Er wordt geen melding verzonden als de taakstatus [!UICONTROL Complete] is of als de uitgiftestatus [!UICONTROL Closed] is.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe melding-e-mail is: <em>[!UICONTROL New Work Request]: &lt;Naam van verzoek&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is: <em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Taaknaam</p> <p>[!UICONTROL Planned Completion Date]</p> <p>Ouders</p> <p>Toegewezen door</p> <p>Toegewezen aan</p> <p>[!UICONTROL Status]</p> <p>[!UICONTROL Description]</p> <p>[!UICONTROL View] knoop <br> Optie om aan de dagelijkse samenvatting toe te voegen</p> <br> </td> 
   <td><strong>Onmiddellijk en </strong> <strong> per dag</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een document goedkeuren </strong> </p> <p>De fiatteur van een document ontvangt een melding wanneer deze als fiatteur wordt vermeld.</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Naam van de gebruiker die de goedkeuring&gt; [!UICONTROL asked you to approve a document in [!DNL Adobe Workfront] indiende.] </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> Projectnaam<br>Naam Portfolio<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>Documentnaam<br>Referentienummer<br>Datum en tijd van goedkeuring aangevraagd<br>Documentdetails (formaat, grootte, versienummer)<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal in behandeling zijnde documentgoedkeuringen<br>*Koppeling naar <strong>[!UICONTROL Document Approvals</strong>*<strong>See All Approvals]</strong> knop<br>*Datum van het dagelijks overzicht<br></td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een project goedkeuren </strong> </p> <p>In het geval van de goedkeuringen van de baanrol, die de gebruikers een e-mailbericht voor deze gebeurtenis ontvangen hangt af van of het plaatsen "[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]"wordt toegelaten (zoals die in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref"> wordt beschreven vormt globale goedkeuringsmontages </a>). </p> <p><strong> als deze optie </strong> wordt toegelaten, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de baanrol verbonden aan de goedkeuring. </p> <p><strong> als deze optie </strong> gehandicapt is, slechts ontvangen de leden van het projectteam met de baanrol verbonden aan het goedkeuringsproces een e-mailbericht.</p> <p>Als de goedkeuring aan een gebruiker wordt geassocieerd, ontvangt die gebruiker het bericht.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Project Pending Approval]: &lt;de Naam van het Project&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Projectnaam<br>goedkeuringsnaam<br>projectreferentienummer<br>naam van de gebruiker die de Portfolio heeft ingediend<br>in afwachting van goedkeuringsstatus<br>datum en tijd van goedkeuring aangevraagd<br>projectprioriteit<br>goedkeuringsstap in afwachting van goedkeuring<br>aantal beslissingen die wachten op goedkeuring<br>naam van de goedkeurder (alleen gebruikers)<br>[!UICONTROL Project Planned Completion Date] <br><strong>[!UICONTROL Make Approval Decision]</strong> knop <br>*totaal aantal in behandeling zijnde projectgoedkeuringen <br>*koppeling naar <strong>[!UICONTROL Project Approvals]</strong><br>*<strong>[!UICONTROL See All Approvals]</strong> knop<br>*datum van de dag overzicht</p> </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een taak goedkeuren </strong> </p> <p>In het geval van de goedkeuringen van de baanrol, die de gebruikers een e-mailbericht voor deze gebeurtenis ontvangen hangt af van of het plaatsen "[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]"wordt toegelaten (zoals die in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref"> wordt beschreven vormt globale goedkeuringsmontages </a>). </p> <p><strong> als deze optie </strong> wordt toegelaten, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de baanrol verbonden aan de goedkeuring. </p> <p><strong> als deze optie </strong> gehandicapt is, slechts ontvangen de leden van het projectteam met de baanrol verbonden aan het goedkeuringsproces een e-mailbericht.</p> <p>Als de goedkeuring aan een gebruiker wordt geassocieerd, ontvangt die gebruiker het bericht. </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Task Pending Approval]: &lt;Taaknaam&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Taaknaam<br>Projectnaam<br>Naam van de gebruiker die de goedkeuring heeft ingediend<br>In behandeling zijnde goedkeuringsstatus<br>Datum en tijd van goedkeuring aangevraagd<br>Taakprioriteit<br>Naam goedkeuringsfase<br>Naam goedkeurder<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*Totaal aantal in behandeling zijnde taakgoedkeuringen<br>*Koppeling naar knop<strong>[!UICONTROL Task Approvals *See All Approvals]</strong><strong></strong>*Datum van het dagelijkse overzicht<br></p> </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een timesheet goedkeuren </strong> </p> <p>De Tijdopmaakfiatteur ontvangt een e-mailbericht wanneer een timesheet wordt voorgelegd dat zij moeten goedkeuren, tenzij de gebruiker die timesheet indiende ook de fiatteur van de Tijdopmaak is.</p> <p>Er wordt alleen een melding verzonden als de status van de tijdpagina [!UICONTROL Submitted] is.</p> <p>Het onderwerp van de e-mail van de directe melding is: <em>[!UICONTROL Timesheet Submitted]: &lt;Timesheet Owner&gt;, &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> De naam van de gebruiker die timesheet voor goedkeuring <br> Datum en Tijd voorlegde toen timesheet <br> Status van timesheet <br> Begin en Eind Dates van de Tijdopmaak <br> Aantal uren die op timesheet <br> worden geregistreerd Aantal overuren die op timesheet <br><strong>[!UICONTROL Review]</strong> en <strong>[!UICONTROL Approve]</strong> knopen <br>*Het totale aantal van hangende timesheet goedkeuringen <br> worden geregistreerd aan <strong>[!UICONTROL Timesheet Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop <br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong> Onmiddellijk en </strong> <strong> Dagelijks </strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een kwestie goedkeuren </strong> </p> <p>In het geval van de goedkeuringen van de baanrol, die de gebruikers een e-mailbericht voor deze gebeurtenis ontvangen hangt van af of het plaatsen "[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]"wordt toegelaten (zoals die in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configure global approval] montages </a> wordt beschreven). </p> <p><strong> als deze optie </strong> wordt toegelaten, wordt een e-mailbericht verzonden naar alle gebruikers in het systeem met de baanrol verbonden aan de goedkeuring. </p> <p><strong> als deze optie </strong> gehandicapt is, slechts ontvangen de leden van het projectteam met de baanrol verbonden aan het goedkeuringsproces een e-mailbericht.</p> <p>Als de goedkeuring aan een gebruiker wordt geassocieerd, ontvangt die gebruiker het bericht. </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Issue Pending Approval]: &lt;Naam van Uitgave&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> Naam van probleem<br>Projectnaam<br>Referentienummer van probleem<br>Naam van de gebruiker die het probleem ter goedkeuring heeft ingediend<br> In behandeling zijnde goedkeuringsstatus<br> Datum en tijd van goedkeuring aangevraagd<br>Prioriteit van probleem<br>Goedkeuringsfase<br>Naam van de goedkeurder<br>[!UICONTROL Issue Planned Completion Date]<br>[!UICONTROL Primary Contact]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop <br>*Totaal aantal in behandeling zijnde goedkeuringsprocedures<br>*Link naar <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knop <br> Datum van het dagelijks overzicht </td> 
   <td><strong> Onmiddellijk en </strong> <strong> Dagelijks </strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een projectgoedkeuring herzien ik </strong> ben afgevaardigd </p> <p>U hebt een projectgoedkeuring gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Delegated Project Approval - Please Review] &lt;Projectnaam&gt; </em></p> <p><em> het onderwerp van het dagelijkse samenvattingsbericht is: [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em> </p> </td> 
   <td> Projectnaam <br>naam Portfolio<br>projectreferentienummer<br>naam van de gebruiker die om goedkeuring heeft gevraagd<br>naam van de gebruiker namens wie u het project goedkeurt<br>status in behandeling<br>datum en tijd van goedkeuring aangevraagd<br>projectprioriteit<br>goedkeuringsstap<br>namen van goedkeurders<br>[!UICONTROL Project Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop<br>*totaal aantal in behandeling zijnde projectgoedkeuringen<br>*koppeling <strong>[!UICONTROL Project Approvals *See All Approvals]</strong> knop <br>*Datum van het dagelijks overzicht </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een taakgoedkeuring herzien ik </strong> ben afgevaardigd </p> <p>U hebt een taakgoedkeuring gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de onmiddellijke bericht e-mail is: <em>[!UICONTROL Delegated Task Approval - Please Review ] &lt;Task Name&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Naam van de gebruiker die om goedkeuring heeft gevraagd<br>Naam van de gebruiker namens wie u de taak {<br>} In behandeling zijnde goedkeuringsstatus<br>Datum en tijd van goedkeuring aangevraagd<br>Taakprioriteit <br>Goedkeuringsfase <br>Naam van de goedkeurder<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knop <br>*Totaal aantal in behandeling zijnde taakgoedkeuringen <br>*Koppeling naar <strong>[!UICONTROL Task Approvals *See All Approvals]</strong> knop <br>*Datum van het dagelijks overzicht </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik moet een probleemgoedkeuring herzien ik ben afgevaardigd </strong> </p> <p>U hebt een goedkeuring van een uitgave gedelegeerd en u moet deze controleren.</p> <p>Het onderwerp van de e-mail van de onmiddellijke melding is: <em>[!UICONTROL Delegated Issue Approval - Please Review] &lt;Naam van Uitgave&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> De Naam van het Uitgeven van de Naam van het Project <br> het Aantal van de Verwijzing van de Kwestie <br> Naam van de gebruiker die om goedkeuring <br> Naam van de gebruiker verzocht van de gebruiker namens wie u de Kwestie <br> goedkeurde Datum en de Tijd van Goedkeuring <br> Gevraagde 6} Prioriteit van de Uitgave {<br> Namen van het Stadium van de Goedkeuring <br> Uitgave Geplande Datum van de Voltooiing 1110} Primaire Contact 11} 1} 1} 1} 1} 1} 1} 1} goedkeurings knoop <br>*Totaal aantal hangende kwesties goedkeurt <br>*Verbinding aan <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knoop <br>*Datum van de dagelijkse samenvatting<br><br><br><br><br><strong>[!UICONTROL Make Approval Decision]</strong><br></td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> I wordt toegewezen aan een kwestie </strong> </p> <p>De uitgever ontvangt een e-mailbericht. De uitgifteontvanger ontvangt geen e-mail als de status van de uitgave gelijk is aan of gelijk is aan [!UICONTROL Closed] .</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL New Work Request]: &lt;Naam van Uitgave&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Probleemnaam<br>Projectnaam<br>[!UICONTROL Issue Reference Number]<br>Uw naam<br>Vervaldatum probleem ([!UICONTROL Planned Completion Date])<br>Naam van de gebruiker die het probleem aan u heeft toegewezen<br><strong>[!UICONTROL Work On It]</strong> knop<br>*Totaal aantal opdrachten<br>*Totaal aantal taken en problemen dat aan u is toegewezen<br>*Koppeling naar <strong>[!UICONTROL Work Requests]</strong><br>*Datum van het dagelijks overzicht<br></p> </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> I wordt geplaatst als primaire ontvanger van een taak </strong> </p> <p>De taakontvanger ontvangt een e-mailbericht als hij of zij de primaire ontvanger van de taak is, tenzij de ontvanger de gebruiker is die de taak heeft uitgevoerd.</p> <p>Er wordt een melding verzonden als de projectstatus [!UICONTROL Current] is en de taak niet is gemarkeerd met [!UICONTROL Complete] .</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL New Work Request]: &lt;Taaknaam&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> De Naam van het project van de taak <br> Naam van het Project {<br> Uw Naam <br> Verdachte Datum van de Taak ([!UICONTROL Planned Completion Date]) <br> Naam van de gebruiker die de taak aan u <br><strong>[!UICONTROL Work On It]</strong> knoop <br>*Totaal aantal taken en kwesties toewezen aan u <br>*Verbinding aan <strong>[!UICONTROL Work Requests]</strong>*Datum van de dagelijkse samenvatting toewees<br> </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Mijn team krijgt een nieuw het werkverzoek </strong> </p> <p>De Leden van het team ontvangen een e-mailbericht wanneer het team een nieuw het werkverzoek ontvangt. (De gebruiker die het verzoek indiende ontvangt geen bericht als hij of zij een lid van het team is.)</p> <p>Een melding wordt alleen verzonden als de projectstatus [!UICONTROL Current] is en de werkaanvraagstatus [!UICONTROL New] is.</p> <p>Gebruikers met een [!UICONTROL Review] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe melding-e-mail is: <em>[!UICONTROL New Work Request]: &lt;Naam van verzoek&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is: <em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p> Naam probleem<br>Projectnaam (naam aanvraagwachtrij)<br>Referentienummer probleem<br>Teamnaam<br>Vervaldatum probleem (geplande voltooiingsdatum)<br>Naam van de gebruiker die de aanvraag heeft ingediend<br><strong>[!UICONTROL Work On It]</strong> knop <br>*Totaal aantal aanvragen dat is toegewezen aan uw team</p> <p>*Naam werkaanvraag</p> <p>[!UICONTROL *Planned Completion Date]</p> <p>*Naam van gebruiker die het verzoek <br>*Verbinding aan <strong>[!UICONTROL Team Requests]</strong><br>*Datum van de dagelijkse samenvatting voorlegde </p> <p><span class="preview">*Teamtoewijzingen </span> </p> </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Mijn timesheet is opnieuw geopend </strong> </p> <p>De eigenaar van de tijdpagina ontvangt een e-mailbericht wanneer de tijdpagina opnieuw wordt geopend, tenzij de gebruiker die de tijdpagina opnieuw heeft geopend ook de eigenaar van de tijdpagina is.</p> <p>Er wordt alleen een e-mailmelding verzonden als de status van het tijdschrift [!UICONTROL Open] is.</p> <p>Het onderwerp van de e-mail van de directe melding is: <em>[!UICONTROL Timesheet Re-opened]: &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt; </em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> De naam van de gebruiker die de Tijdopname <br> Datum en Tijd heropende toen de Tijdopnemer <br> Status van de Tijdopnemer ([!UICONTROL Re-opened]) <br> Aantal Totale Uren die op het 4} Aantal uren van de Tijdopnemer {worden geregistreerd die op de Chronologie <br><strong>[!UICONTROL Review]</strong> knoop wordt geregistreerd<br> </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Mijn timesheet wordt verworpen </strong> </p> <p>De eigenaar van de tijdpagina ontvangt een e-mailbericht wanneer de tijdpagina wordt afgewezen, tenzij de gebruiker die de tijdpagina heeft afgewezen ook de eigenaar is.</p> <p>Er wordt alleen een e-mailmelding verzonden als de status van het tijdschrift [!UICONTROL Rejected] is.</p> <p>Het onderwerp van de directe melding-e-mail is: <em>[!UICONTROL Timesheet Rejected]:&lt;Start Date of the Timesheet&gt; - &lt;End Date of the Timesheet&gt; </em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> De naam van de gebruiker die de Status van de Tijdopnemer <br> van de Tijdopnemer ([!UICONTROL Rejected]) verwierp <br> Datum en Tijd van toen de Chronologie <br><strong>[!UICONTROL Review]</strong> knoop werd verworpen </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Iemand vraagt toegang van me </strong> </p> <p>Ik verzoek me iets te doen, dus zet het aan.</p> <p>De persoon die het project creeert krijgt toegang tot het.</p> <p>Dit maakt de gebruiker het bericht krijgen wanneer iemand toegang aanvraagt.</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Naam van gebruiker die de toegang&gt; [!UICONTROL needs access to] &lt;Naam van Voorwerp&gt; </em> vroeg</p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Objectnaam <br> Naam bovenliggend object <br> Objectreferentienummer<br>Naam van de gebruiker die toegang heeft aangevraagd<br>Het type toegang dat de gebruiker aanvraagt<br><strong>[!UICONTROL Grant] &lt;Naam van de gevraagde toegang&gt; Toegang</strong> en <strong>[!UICONTROL Grant different access]</strong> knoppen<br>*Totaal aantal openstaande goedkeuringen voor toegangsverzoeken<br>*Koppeling naar <strong>[!UICONTROL Access Request]</strong> goedkeuringen<br>*Datum van dagelijkse samenvatting</p> </td> 
   <td><strong> Onmiddellijk en Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Iemand verzoekt me om een document </strong> te uploaden </p> <p>De documentaanvrager ontvangt een e-mailbericht wanneer een gebruiker een verzoek ontvangt om een document te uploaden.</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Naam van de gebruiker die het document verzoekt&gt; [!UICONTROL needs a document from you in [!DNL Workfront].] </em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Naam van de gebruiker die het document <br> verzoekt Naam van het voorwerp waar het document <br><strong>[!UICONTROL Attach it here]</strong> verbinding zou moeten worden geupload </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
 </tbody> 
</table>
