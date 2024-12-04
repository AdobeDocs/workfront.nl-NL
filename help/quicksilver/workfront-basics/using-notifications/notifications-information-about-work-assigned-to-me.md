---
content-type: reference
navigation-topic: notifications
title: 'Meldingen: Informatie over werk dat aan mij is toegewezen'
description: In de volgende meldingen wordt u gewaarschuwd voor activiteiten die plaatsvinden op een werkitem dat aan u is toegewezen.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1870'
ht-degree: 0%

---

# Meldingen: Informatie over werk dat aan mij is toegewezen

In de volgende meldingen wordt u gewaarschuwd voor activiteiten die plaatsvinden op een werkitem dat aan u is toegewezen.

Voor informatie over het vormen van welke berichten u ontvangt, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong> een voorganger van een taak die aan mijn team wordt toegewezen wordt voltooid </strong> </p> <p>Het toegewezen team ontvangt een e-mailbericht wanneer een voorganger van een van zijn taken is voltooid. </p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van het onmiddellijke bericht e-mail is: <em> Voltooid: &lt;Taaknaam&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Voorganger Taaknaam<br>Voorganger Taakproject<br>Voorganger Taakreferentienummer<br>Naam van de gebruiker die de voorgangerstaak<br>Status van de voorgangerstaak<br>Datum en tijd waarop de voorganger is voltooid<br>Vorige status van de voorgangerstaak<br><strong>Zie meer details</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voorgangers voltooid<br>*Taaknaam <br>*Naam van de gebruiker die de taak heeft voltooid <br>*Datum van het dagelijks overzicht </p> </td> 
   <td><strong> Dagelijks </strong> </td>
  </tr>
  <tr> 
   <td> <p><strong> een voorganger van één van mijn taken wordt voltooid </strong> </p> <p>De toegewezen taak ontvangt een e-mailbericht wanneer een voorganger van een van zijn taken is voltooid. </p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Complete]: &lt;Taaknaam&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Voorganger Taaknaam<br>Voorganger Taakproject<br>Voorganger Taakreferentienummer<br>Naam van de gebruiker die de voorganger taak<br>Status van de voorganger taak<br> Datum en tijd toen de voorganger voltooid<br>Vorige status van de voorganger taak<br><strong>[!UICONTROL See More Details]</strong> knop <br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voorgangers voltooid<br>*Taaknaam<br>*Naam van de gebruiker die de taak<br>*Datum van overzicht </p> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong> de taak van A wordt I voltooide goedgekeurd of verworpen </strong> </p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de taak wordt goedgekeurd of afgewezen.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Complete]: &lt;Taaknaam&gt; op &lt;Projectnaam&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Naam van de gebruiker die de goedkeuring heeft verleend<br>Nieuwe taakstatus<br>Datum en tijd waarop de taak is goedgekeurd of afgewezen<br>Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal goedgekeurde of afgewezen taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak {<br>*Goedkeuringsbesluit ([!UICONTROL Approved]/ [!UICONTROL Rejected]})<br>*Datum heeft goedgekeurd of afgewezen van het dagelijks overzicht<br></td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong> de taak van A wordt I toegewezen aan wordt voltooid </strong> </p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de taak is voltooid.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Complete]: &lt;Task Name&gt; op &lt;Project name&gt; </em></p> <p> <p>Opmerking: als de taak is gewijzigd in een status die gelijk is aan [!UICONTROL Complete] , wordt voor het onderwerp van de e-mail nog steeds ''Voltooid'' weergegeven.</p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Naam van de gebruiker die de taak heeft voltooid<br>Datum en tijd waarop de taak is voltooid<br>Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van het dagelijkse overzicht<br></p> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong> Alle predecessors van een taak die aan mijn team wordt toegewezen wordt voltooid </strong> </p> <p>Het toegewezen team ontvangt een e-mailbericht wanneer een voorganger van een van zijn taken als voltooid is gemarkeerd.</p> <p>Gebruikers met een licentie voor een revisie of aanvrager ontvangen geen melding.</p> <p>Het onderwerp van het onmiddellijke bericht e-mail is: <em> Volledige Taak: &lt;Name&gt; </em></p> <p> Het onderwerp van het dagelijkse samenvattingsbericht is: <em> Overzicht van werkzaamheden toegewezen aan u &lt;Datum van dagelijkse samenvatting&gt; </em></p> </td> 
   <td> Taaknaam<br>Taakproject<br>Taakreferentienummer<br>Naam van de gebruiker die de voorgangstaak<br>Status van de voorgangstaak<br>Datum en tijd waarop de voorganger is voltooid<br>Vorige status van de voorgangstaak<br><strong>Zie meer informatie</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak <br>*Datum van het dagelijks overzicht heeft voltooid </td>
   <td><strong> Onmiddellijk </strong> </td> 
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
   <td> <p><strong> Alle predecessors van mijn taken worden voltooid </strong> </p> <p>De toegewezen taak ontvangt een e-mailbericht voor elke voorganger die is voltooid.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Complete]: &lt;Taaknaam&gt; </em><br></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Taaknaam<br>Taakproject<br>Taakreferentienummer<br>Naam van de gebruiker die de voorgangstaak<br>Status van de voorgangstaak<br>Datum en tijd waarop de voorganger voltooid was<br>Vorige status van de voorgangstaak <br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker de taak voltooid<br>*Datum van dagelijks overzicht </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong> Een kwestie ik oplos wordt goedgekeurd of verworpen </strong> </p> <p>De ontvanger van een afgifte ontvangt een e-mailkennisgeving wanneer een goedkeuringsbesluit wordt genomen (goedgekeurd of afgewezen).</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em> Kwestie in afwachting van Goedkeuring: &lt;Planned Datum van het Begin&gt; &lt;Issue Reference Number&gt; - &lt;Issue Name&gt; in &lt;Project Name&gt; </em></p> <p> Het onderwerp van het dagelijkse samenvattingsbericht is: <em> Overzicht van werkzaamheden toegewezen aan u &lt;Datum van dagelijkse samenvatting&gt; </em></p> </td> 
   <td> Probleem Naam<br>Projectnaam<br>Referentienummer van afgifte<br>Naam van de gebruiker die het probleem heeft goedgekeurd of afgewezen<br>Goedkeuringsbesluit (goedgekeurd of afgewezen)<br>Afgiftestatus<br>Naam van de gebruiker die de goedkeuring heeft aangevraagd<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal problemen goedgekeurd of afgewezen<br>*Afgiftenaam<br>*Naam van de gebruiker die het probleem heeft goedgekeurd of afgewezen<br>*Goedkeuringsbesluit (goedgekeurd of afgewezen)<br>*Datum van het dagelijks overzicht<br></td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong> Een kwestie I wordt toegewezen aan wordt voltooid </strong> </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning] is.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van het onmiddellijke bericht e-mail is: <em> Voltooid: &lt;Issue Name&gt; op &lt;Project Name&gt; </em></p> <p><em> Het onderwerp van de dagelijkse overzichtsmelding is: Overzicht van het werk dat aan u is toegewezen &lt;Datum van dagelijkse controlesamenvatting&gt; </em> </p> </td> 
   <td> Probleemnaam<br>Projectnaam<br>Referentienummer <br>Naam van de gebruiker die het probleem heeft opgelost<br>Nieuwe probleemstatus<br>Datum en tijd waarop het probleem is opgelost<br>Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide problemen<br>*Naam van probleem<br>*Naam van de gebruiker die het probleem heeft voltooid<br> Datum van het dagelijks overzicht<br></td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de Documenten worden geupload of veranderd op verzoeken ik aan </strong> wordt toegewezen </p> <p>De uitgevers ontvangen een e-mailbericht wanneer documenten worden geüpload of documentgegevens worden gewijzigd over een uitgave die hij of zij heeft toegevoegd.</p> <p>Er wordt geen e-mailbericht verzonden als de gebruiker die de uitgave heeft geactiveerd, de uitgevende instelling is.</p> <p>Een bericht wordt verzonden slechts als de projectstatus [!UICONTROL Current] is en als het project opstelling als Rij van het Verzoek van de Hulp (zoals die in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> wordt beschreven creeer een Rij van het Verzoek </a>).</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Document added to] &lt;Naam van het Verzoek&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Naam aanvraag<br>Projectnaam (naam aanvraagwachtrij)<br>Referentienummer document <br>Naam van de gebruiker die het document heeft geüpload<br>Naam document <br>Toegevoegd op datum<br>Documentdetails (formaat, grootte, versienummer)<br>Documentminiatuur<br><strong>[!UICONTROL Preview]</strong> en <strong>[!UICONTROL Download]</strong> knoppen<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal geüploade of gewijzigde<br>*Documentnaam<br>*Objectnaam<br>*Naam van de gebruiker die het document<br>*Datum van dagelijks overzicht heeft geüpload</p> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de verouderde datumveranderingen op een taak ik aan </strong> wordt toegewezen </p> <p>De toegewezen taak ontvangt een e-mailbericht wanneer [!UICONTROL Planned Completion Date] van de taak verandert, tenzij de gebruiker die de Geplande Datum van Voltooiing veranderde ook de Toegewezen Taak is.</p> <p>Er wordt alleen een melding verzonden als de projectstatus iets anders is dan [!UICONTROL Planning] .</p> <p>Er wordt geen melding verzonden met betrekking tot persoonlijke taken.</p> <p> Gebruikers met een licentie voor een revisie of aanvrager ontvangen geen melding. </p> <p> Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Due Date has been changed.]</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Taakreferentienummer<br>Nieuwe vervaldatum ([!UICONTROL Planned Completion Date])<br> Datum en tijd waarop de vervaldatum werd gewijzigd<br>De naam van de gebruiker die de vervaldatum<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal taken waarbij de vervaldatum (geplande voltooiingsdatum)<br>*Taaknaam<br>*Nieuwe geplande voltooiingsdatum<br> Naam van de gebruiker die de vervaldatum<br>*Datum van dagelijkse samenvatting heeft gewijzigd </td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de verouderde datumveranderingen op een kwestie ik aan </strong> wordt toegewezen </p> <p>De uitgevers ontvangen een e-mailmelding wanneer de [!UICONTROL Planned Completion Date] verandert, tenzij de gebruiker die [!UICONTROL Planned Completion Date] heeft gewijzigd ook de ontvanger is.</p> <p>Er wordt alleen een melding verzonden als de projectstatus iets anders is dan [!UICONTROL Planning] .</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> Het onderwerp van het dagelijkse samenvattingsbericht is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Naam van uitgifte<br>Projectnaam<br>Referentienummer van uitgifte<br>Nieuwe vervaldatum ([!UICONTROL Planned Completion Date])<br> Datum en tijd waarop de vervaldatum werd gewijzigd<br>Naam van de gebruiker die de vervaldatum heeft gewijzigd<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal problemen waarbij de vervaldatum ([!UICONTROL Planned Completion Date])<br>*Naam van uitgifte<br>*Nieuwe [!UICONTROL Planned Completion Date]<br>*Naam van de gebruiker die de vervaldatum<br>*Datum van het dagelijks overzicht heeft gewijzigd<br></p> </td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong> de statusveranderingen op een taak ik aan </strong> wordt toegewezen <p>De taakontvanger ontvangt een e-mailbericht wanneer de status van de taak verandert, tenzij de gebruiker die de status heeft gewijzigd ook de ontvanger is.</p> <p>Opmerking: deze melding wordt niet verzonden wanneer de taakstatus wordt gewijzigd in voltooid. Een afzonderlijke melding wordt gebruikt voor voltooide taken. Zie <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref"> een taak I wordt toegewezen aan wordt voltooid </a>, hierboven.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Task Name&gt; van &lt;Project Name&gt; is &lt;New Status&gt; </em></p> <p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> De Naam van het project van de taak <br> Naam van de Taak {<br> Naam van de gebruiker die de status <br> Nieuwe Status <br> Datum en Tijd veranderde toen de status <br> de Status van de Voorproef <br><strong>[!UICONTROL See More Details]</strong> knoop <br>*De Naam van het Project <br>*Het Aantal van de Verwijzing van het Project <br>*Totaal aantal taken waar de Status <br>*Naam van de Taak <br>*Vorige Taak*Taak Status <br> <br> Nieuwe Taak taak  Van de Naam van het Project taak  veranderde Status <br>*Naam van de gebruiker die de Status <br>*Datum van de dagelijkse samenvatting veranderde<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de statusveranderingen op één van mijn werkpunten </strong> </p> <p>U ontvangt een e-mailmelding wanneer de status verandert in een uitgave waaraan u bent toegewezen, tenzij u de status zelf wijzigt. </p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Gebruikers met een [!UICONTROL Review] - of [!UICONTROL Requestor] -licentie ontvangen geen melding.</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Issue Name&gt; van &lt;Project Name&gt; is &lt;New Status&gt; </em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> De Naam van het uitgeven van de Naam <br> Naam van het Project {<br> Naam van de Verwijzing van de Uitgave van de gebruiker die de status <br> Nieuwe Status <br> veranderde Datum en Tijd toen de status <br> Vorige Status van de Uitgave <br><strong> Meer Details </strong> knoop <br> * Naam van het Project <br>*Het Aantal van de Verwijzing van het Project <br>*Totaal aantal kwesties waar de Status <br>*Naam van de Taak 112} veranderde*De vorige Status van de Uitgave <br>*Nieuwe Status van de Uitgave <br>*Naam van de gebruiker die de Status <br>*Datum van dagelijkse samenvatting veranderde<br><br> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
 </tbody> 
</table>
