---
content-type: reference
navigation-topic: notifications
title: 'Meldingen: Informatie over het werk dat aan mij is toegewezen'
description: De volgende meldingen waarschuwen u voor activiteiten die plaatsvinden op een werkitem dat aan u is toegewezen.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1870'
ht-degree: 0%

---

# Meldingen: Informatie over het werk dat aan mij is toegewezen

De volgende meldingen waarschuwen u voor activiteiten die plaatsvinden op een werkitem dat aan u is toegewezen.

Zie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) voor informatie over het configureren van welke meldingen u ontvangt.

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
   <td> <p><strong>Een voorloper van een taak die aan mijn team is toegewezen, is voltooid</strong> </p> <p>Het toegewezen team ontvangt een e-mailmelding wanneer een voorloper van een van hun taken is voltooid. </p> <p>Gebruikers met een licentie van [!UICONTROL Review] of [!UICONTROL Requestor] ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em> voltooid: &lt;Taaknaam&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> <p>Voorganger Taaknaam<br>Voorganger Taakproject<br>Voorganger Taakreferentienummer<br>Naam van de gebruiker die de voorgangerstaak<br>Status van de voorgangerstaak<br>Datum en tijd waarop de voorganger is voltooid<br>Vorige status van de voorgangerstaak<br><strong>Zie meer details</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voorgangers voltooid<br>*Taaknaam <br>*Naam van de gebruiker die de taak heeft voltooid <br>*Datum van het dagelijks overzicht </p> </td> 
   <td><strong>dagelijks</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Een voorloper van een van mijn taken is voltooid</strong> </p> <p>De toegewezen taak ontvangt een e-mailmelding wanneer een voorganger van een van hun taken is voltooid. </p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Complete]: &lt;Taaknaam&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> <p>Voorganger Taaknaam<br>Voorganger Taakproject<br>Voorganger Taakreferentienummer<br>Naam van de gebruiker die de voorganger taak<br>Status van de voorganger taak<br> Datum en tijd toen de voorganger voltooid<br>Vorige status van de voorganger taak<br><strong>[!UICONTROL See More Details]</strong> knop <br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voorgangers voltooid<br>*Taaknaam<br>*Naam van de gebruiker die de taak<br>*Datum van overzicht </p> </td> 
   <td><strong>dagelijks</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Een taak die ik heb voltooid, is goedgekeurd of afgewezen</strong> </p> <p>De toegewezen taak ontvangt een e-mailmelding wanneer de taak wordt goedgekeurd of afgewezen.</p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Complete]: &lt;taaknaam&gt; op &lt;projectnaam&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Naam van de gebruiker die de goedkeuring heeft verleend<br>Nieuwe taakstatus<br>Datum en tijd waarop de taak is goedgekeurd of afgewezen<br>Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal goedgekeurde of afgewezen taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak {<br>*Goedkeuringsbesluit ([!UICONTROL Approved]/ [!UICONTROL Rejected]})<br>*Datum heeft goedgekeurd of afgewezen van het dagelijks overzicht<br></td> 
   <td><strong>dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Een taak die ik toegewezen heb gekregen is voltooid</strong> </p> <p>De toegewezen taak ontvangt een e-mail melding wanneer de taak is voltooid.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Complete]: &lt;taaknaam&gt; op &lt;projectnaam&gt;</em></p> <p> <p>Opmerking: Als de taak wordt gewijzigd in een status die overeenkomt met [!UICONTROL Complete], wordt het onderwerp van de e-mail nog steeds "Voltooid" weergegeven.</p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> <p>Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Naam van de gebruiker die de taak heeft voltooid<br>Datum en tijd waarop de taak is voltooid<br>Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van het dagelijkse overzicht<br></p> </td> 
   <td><strong>dagelijks</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alle voorgangers van een taak die aan mijn team is toegewezen, zijn voltooid</strong> </p> <p>Het toegewezen team ontvangt een e-mailmelding wanneer een voorganger van een van hun taken is gemarkeerd als voltooid.</p> <p>Gebruikers met een licentie voor controleren of aanvragen ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>Taak voltooid: &lt;naam&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> Overzichtswerk aan u toegewezen &lt;Datum van dagelijkse overzichtsopname&gt; </em></p> </td> 
   <td> Taaknaam<br>Taakproject<br>Taakreferentienummer<br>Naam van de gebruiker die de voorgangstaak<br>Status van de voorgangstaak<br>Datum en tijd waarop de voorganger is voltooid<br>Vorige status van de voorgangstaak<br><strong>Zie meer informatie</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak <br>*Datum van het dagelijks overzicht heeft voltooid </td>
   <td><strong>Onmiddellijk </strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Alle voorgangers van mijn taken zijn voltooid</strong> </p> <p>De toegewezen taak ontvangt een e-mailmelding voor elke voorganger die is voltooid.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Complete]: &lt;taaknaam&gt;</em><br></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> Taaknaam<br>Taakproject<br>Taakreferentienummer<br>Naam van de gebruiker die de voorgangstaak<br>Status van de voorgangstaak<br>Datum en tijd waarop de voorganger voltooid was<br>Vorige status van de voorgangstaak <br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker de taak voltooid<br>*Datum van dagelijks overzicht </td> 
   <td><strong>Onmiddellijk </strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Een probleem dat ik oplos, is goedgekeurd of afgewezen</strong> </p> <p>De cessionaris van een probleem ontvangt een e-mailmelding wanneer een goedkeuringsbesluit wordt genomen (goedgekeurd of afgewezen).</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>Probleem in afwachting van goedkeuring: &lt;geplande startdatum&gt; &lt;referentienummer probleem&gt; - &lt;naam probleem&gt; in &lt;naam project&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> Overzichtswerk aan u toegewezen &lt;Datum van dagelijkse overzichtsopname&gt; </em></p> </td> 
   <td> Probleem Naam<br>Projectnaam<br>Referentienummer van afgifte<br>Naam van de gebruiker die het probleem heeft goedgekeurd of afgewezen<br>Goedkeuringsbesluit (goedgekeurd of afgewezen)<br>Afgiftestatus<br>Naam van de gebruiker die de goedkeuring heeft aangevraagd<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal problemen goedgekeurd of afgewezen<br>*Afgiftenaam<br>*Naam van de gebruiker die het probleem heeft goedgekeurd of afgewezen<br>*Goedkeuringsbesluit (goedgekeurd of afgewezen)<br>*Datum van het dagelijks overzicht<br></td> 
   <td><strong>dagelijks</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Een probleem waaraan ik ben toegewezen, is voltooid</strong> </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning] is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>Voltooid: &lt;probleemnaam&gt; op &lt;projectnaam&gt;</em></p> <p><em> Het onderwerp van de dagelijkse overzichtsmelding is: Overzichtswerk toegewezen aan u &lt;Datum van dagelijkse overzichtsopname&gt; </em> </p> </td> 
   <td> Probleemnaam<br>Projectnaam<br>Referentienummer <br>Naam van de gebruiker die het probleem heeft opgelost<br>Nieuwe probleemstatus<br>Datum en tijd waarop het probleem is opgelost<br>Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide problemen<br>*Naam van probleem<br>*Naam van de gebruiker die het probleem heeft voltooid<br> Datum van het dagelijks overzicht<br></td> 
   <td><strong>dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documenten worden geüpload of gewijzigd op aanvragen die ik heb toegewezen aan</strong> </p> <p>De toegewezen probleemontvanger ontvangt een e-mailmelding wanneer documenten worden geüpload of wanneer documentdetails worden gewijzigd in verband met een probleem dat hij of zij heeft toegevoegd.</p> <p>Er wordt geen e-mailmelding verzonden als de gebruiker die het probleem heeft geactiveerd, het probleem heeft toegewezen.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is en als het project is ingesteld als een Help-aanvraagwachtrij (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a>).</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Document added to] &lt;naam aanvraag&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> <p>Naam aanvraag<br>Projectnaam (naam aanvraagwachtrij)<br>Referentienummer document <br>Naam van de gebruiker die het document heeft geüpload<br>Naam document <br>Toegevoegd op datum<br>Documentdetails (formaat, grootte, versienummer)<br>Documentminiatuur<br><strong>[!UICONTROL Preview]</strong> en <strong>[!UICONTROL Download]</strong> knoppen<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal geüploade of gewijzigde<br>*Documentnaam<br>*Objectnaam<br>*Naam van de gebruiker die het document<br>*Datum van dagelijks overzicht heeft geüpload</p> </td> 
   <td><strong>dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De vervaldatum verandert bij een taak die ik toegewezen heb gekregen aan</strong> </p> <p>De toegewezen taak ontvangt een e-mailmelding wanneer [!UICONTROL Planned Completion Date] van de taak verandert, tenzij de gebruiker die de geplande voltooiingsdatum heeft gewijzigd ook de toegewezen taak is.</p> <p>Er wordt alleen een melding verzonden als de projectstatus iets anders is dan [!UICONTROL Planning].</p> <p>Er wordt geen melding verzonden over persoonlijke taken.</p> <p> Gebruikers met een licentie voor controleren of aanvragen ontvangen geen melding. </p> <p> Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Due Date has been changed.]</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Nieuwe vervaldatum ([!UICONTROL Planned Completion Date])<br> Datum en tijd waarop de vervaldatum werd gewijzigd<br>De naam van de gebruiker die de vervaldatum<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal taken waarbij de vervaldatum (geplande voltooiingsdatum)<br>*Taaknaam<br>*Nieuwe geplande voltooiingsdatum<br> Naam van de gebruiker die de vervaldatum<br>*Datum van dagelijkse samenvatting heeft gewijzigd </td> 
   <td> <p><strong>Onmiddellijk </strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De vervaldatum verandert bij een probleem dat ik heb toegewezen aan</strong> </p> <p>De probleemtoegewezen persoon ontvangt een e-mailmelding wanneer de [!UICONTROL Planned Completion Date] verandert, tenzij de gebruiker die de [!UICONTROL Planned Completion Date] heeft gewijzigd, ook de toegewezen persoon is.</p> <p>Er wordt alleen een melding verzonden als de projectstatus iets anders is dan [!UICONTROL Planning].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt;</em></p> </td> 
   <td> <p>Naam van uitgifte<br>Projectnaam<br>Referentienummer van uitgifte<br>Nieuwe vervaldatum ([!UICONTROL Planned Completion Date])<br> Datum en tijd waarop de vervaldatum werd gewijzigd<br>Naam van de gebruiker die de vervaldatum heeft gewijzigd<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal problemen waarbij de vervaldatum ([!UICONTROL Planned Completion Date])<br>*Naam van uitgifte<br>*Nieuwe [!UICONTROL Planned Completion Date]<br>*Naam van de gebruiker die de vervaldatum<br>*Datum van het dagelijks overzicht heeft gewijzigd<br></p> </td> 
   <td> <p><strong>Onmiddellijk </strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>De status verandert bij een taak die ik toegewezen heb gekregen aan</strong> <p>De Taaktoegewezen ontvangt een e-mail melding wanneer de status van de taak verandert, tenzij de gebruiker die de status heeft gewijzigd ook de toegewezen persoon is.</p> <p>Opmerking: Deze melding wordt niet verzonden wanneer de taakstatus verandert om te voltooien. Een afzonderlijke melding wordt gebruikt voor voltooide taken. Zie <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Een taak die ik toegewezen heb gekregen is voltooid</a>, hierboven.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>&lt;Taaknaam&gt; van &lt;projectnaam&gt; is &lt;nieuwe status&gt;</em></p> <p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Naam van de gebruiker die de status<br>Nieuwe status<br>Datum en tijd waarop de status werd gewijzigd<br>Voorbeeldstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal taken waarbij de status is gewijzigd<br>*Taaknaam<br>*Vorige Taakstatus<br>*Nieuwe Taakstatus<br>*Naam van de gebruiker die de status<br>*Datum van het dagelijks overzicht heeft gewijzigd<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De status verandert op een van mijn werkitems</strong> </p> <p>U ontvangt een e-mail wanneer de status verandert in een probleem waaraan u bent toegewezen, tenzij u de status zelf wijzigt. </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] licentie ontvangen geen melding.</p> <p>Het onderwerp van de direct-mailmelding is: <em>&lt;Naam probleem&gt; van &lt;Naam project&gt; is &lt;Nieuwe status&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;datum van dagelijkse overzichtsmelding&gt; </em></p> </td> 
   <td> Probleemnaam<br>Projectnaam<br>Uitgavenummer<br>Naam van de gebruiker die de status<br>Nieuwe status<br>Datum en tijd waarop de status werd gewijzigd<br>Vorige uitgiftestatus<br><strong>Zie meer informatie</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal problemen waarbij de status <br>*Taaknaam<br>*Vorige status is gewijzigd <br>*Nieuwe probleemstatus<br>*Naam van de gebruiker die de status<br>*Datum van dagelijks overzicht heeft gewijzigd </td> 
   <td><strong>dagelijks</strong> </td> 
  </tr> 
 </tbody> 
</table>
