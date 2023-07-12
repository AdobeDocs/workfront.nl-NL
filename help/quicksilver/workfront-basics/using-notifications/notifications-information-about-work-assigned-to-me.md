---
content-type: reference
navigation-topic: notifications
title: "Meldingen: Informatie over werk dat aan mij is toegewezen"
description: In de volgende meldingen wordt u gewaarschuwd voor activiteiten die plaatsvinden op een werkitem dat aan u is toegewezen.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 901605917347297a1ee077f00905b03427582650
workflow-type: tm+mt
source-wordcount: '1872'
ht-degree: 0%

---

# Meldingen: Informatie over werk dat aan mij is toegewezen

In de volgende meldingen wordt u gewaarschuwd voor activiteiten die plaatsvinden op een werkitem dat aan u is toegewezen.

Voor informatie over het vormen van welke berichten u ontvangt, zie [Uw eigen gebeurtenismeldingen activeren of deactiveren](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Een voorganger van een taak die aan mijn team wordt toegewezen wordt voltooid</strong> </p> <p>Het toegewezen team ontvangt een e-mailbericht wanneer een voorganger van een van zijn taken is voltooid. </p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Voltooid: &lt;task name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Naam van vorige taak<br>Predecessor Taakproject<br>Referentienummer vorige taak<br>Naam van de gebruiker die de voorgangstaak heeft voltooid<br>Status van de voorgaande taak<br>Datum en tijd waarop de voorganger is voltooid<br>Eerdere status van de vorige taak<br><strong>Meer informatie</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide voorgangers<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van de dagelijkse samenvatting </p> </td> 
   <td><strong>Dagelijks</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Een voorganger van een van mijn taken is voltooid</strong> </p> <p>De toegewezen taak ontvangt een e-mailbericht wanneer een voorganger van een van zijn taken is voltooid. </p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Naam van vorige taak<br>Predecessor Taakproject<br>Referentienummer vorige taak<br>Naam van de gebruiker die de voorgangstaak heeft voltooid<br>Status van de voorgaande taak<br>Datum en tijd waarop de voorganger is voltooid<br>Eerdere status van de vorige taak<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide voorgangers<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van de dagelijkse samenvatting </p> </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Een taak die ik voltooi, is goedgekeurd of afgewezen</strong> </p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de taak wordt goedgekeurd of afgewezen.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Complete]: &lt;task name=""&gt; op &lt;project name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Naam van de gebruiker die de goedkeuring heeft verleend<br>Nieuwe taakstatus<br>Datum en tijdstip waarop de taak is goedgekeurd of afgewezen<br>Status vorige taak<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal goedgekeurde of geweigerde taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft goedgekeurd of geweigerd<br>*Goedkeuringsbesluit ([!UICONTROL Approved]/ [!UICONTROL Rejected])<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Een taak waaraan ik ben toegewezen, is voltooid</strong> </p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de taak is voltooid.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Complete]: &lt;task name=""&gt; op &lt;project name=""&gt;</em></p> <p> <p>Opmerking: Als de taak is gewijzigd in een status die overeenkomt met [!UICONTROL Complete]In het onderwerp van de e-mail staat nog steeds ''Voltooid''.</p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Naam van de gebruiker die de taak heeft voltooid<br>Datum en tijd waarop de taak is voltooid<br>Status vorige taak<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van de dagelijkse samenvatting<br></p> </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alle voorgangers van een taak die aan mijn team is toegewezen, zijn voltooid</strong> </p> <p>Het toegewezen team ontvangt een e-mailbericht wanneer een voorganger van een van zijn taken als voltooid is gemarkeerd.</p> <p>Gebruikers met een licentie voor een revisie of aanvrager ontvangen geen melding.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Taak voltooid: &lt;name&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> Overzicht van het werk dat aan u is toegewezen &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Taaknaam<br>Taakproject<br>Referentienummer taak<br>Naam van de gebruiker die de voorgangstaak heeft voltooid<br>Status van de voorgaande taak<br>Datum en tijd waarop de voorganger is voltooid<br>Eerdere status van de vorige taak<br><strong>Meer informatie</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van de dagelijkse samenvatting </td>
   <td><strong>Meteen</strong> </td> 
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
   <td> <p><strong>Alle voorgangers van mijn taken zijn voltooid</strong> </p> <p>De toegewezen taak ontvangt een e-mailbericht voor elke voorganger die is voltooid.</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em><br></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Taaknaam<br>Taakproject<br>Referentienummer taak<br>Naam van de gebruiker die de voorgangstaak heeft voltooid<br>Status van de voorgaande taak<br>Datum en tijd waarop de voorganger is voltooid<br>Eerdere status van de vorige taak<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide taken<br>*Taaknaam<br>*Naam van de gebruiker die de taak heeft voltooid<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Meteen</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Een probleem dat ik heb opgelost, is goedgekeurd of verworpen</strong> </p> <p>De ontvanger van een afgifte ontvangt een e-mailkennisgeving wanneer een goedkeuringsbesluit wordt genomen (goedgekeurd of afgewezen).</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Uitgeven in afwachting van goedkeuring: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> Overzicht van het werk dat aan u is toegewezen &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die het probleem heeft goedgekeurd of afgewezen<br>Goedkeuringsbesluit (goedgekeurd of afgewezen)<br>Status van afgifte<br>Naam van de gebruiker die de goedkeuring heeft aangevraagd<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal goedgekeurde of afgewezen kwesties<br>*Naam van uitgave<br>*Naam van de gebruiker die het probleem heeft goedgekeurd of afgewezen<br>*Goedkeuringsbesluit (goedgekeurd of afgewezen)<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Een probleem waaraan ik ben toegewezen, is voltooid</strong> </p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Voltooid: &lt;issue name=""&gt; op &lt;project name=""&gt;</em></p> <p><em> Het onderwerp van de dagelijkse overzichtsmelding is: Overzicht van het werk dat aan u is toegewezen &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die de uitgave heeft voltooid<br>Status nieuwe uitgave<br>Datum en tijdstip waarop de afgifte is voltooid<br>Status vorige taak<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide uitgaven<br>*Naam van uitgave<br>*Naam van de gebruiker die de uitgave heeft voltooid<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documenten worden geüpload of gewijzigd op aanvragen waaraan ik ben toegewezen</strong> </p> <p>De uitgevers ontvangen een e-mailbericht wanneer documenten worden geüpload of documentgegevens worden gewijzigd over een uitgave die hij of zij heeft toegevoegd.</p> <p>Er wordt geen e-mailbericht verzonden als de gebruiker die de uitgave heeft geactiveerd, de uitgevende instelling is.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current] en als het project opstelling is als Rij van het Verzoek van de Hulp (zoals die in wordt beschreven <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a>).</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Document added to] &lt;request name=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Naam aanvraag<br>Projectnaam (naam wachtrij aanvragen)<br>Referentienummer document <br>Naam van de gebruiker die het document heeft geüpload<br>Documentnaam <br>Toegevoegd op datum<br>Documentdetails (formaat, grootte, versienummer)<br>Documentminiatuur<br><strong>[!UICONTROL Preview]</strong> en <strong>[!UICONTROL Download]</strong> knoppen<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal geüploade of gewijzigde documenten<br>*Documentnaam<br>*Objectnaam<br>*Naam van de gebruiker die het document heeft geüpload<br>*Datum van de dagelijkse samenvatting</p> </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De wijzigingen op de vervaldatum in een taak waaraan ik ben toegewezen</strong> </p> <p>De taakontvanger ontvangt een e-mailbericht wanneer de [!UICONTROL Planned Completion Date] van de taak verandert, tenzij de gebruiker die de Geplande Datum van Voltooiing veranderde ook de Taak Toegewezen is.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus iets anders is dan [!UICONTROL Planning].</p> <p>Er wordt geen melding verzonden met betrekking tot persoonlijke taken.</p> <p> Gebruikers met een licentie voor een revisie of aanvrager ontvangen geen melding. </p> <p> Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Due Date has been changed.]</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Nieuwe vervaldatum ([!UICONTROL Planned Completion Date])<br>Datum en tijdstip waarop de vervaldatum is gewijzigd<br>De naam van de gebruiker die de vervaldatum heeft gewijzigd<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal taken waarbij de vervaldatum (geplande uitvoeringsdatum) is gewijzigd<br>*Taaknaam<br>*Nieuwe geplande afsluitdatum<br>*Naam van de gebruiker die de vervaldatum heeft gewijzigd<br>*Datum van de dagelijkse samenvatting </td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De wijzigingen op de vervaldatum van een uitgave waaraan ik ben toegewezen</strong> </p> <p>De uitgevende instelling ontvangt een e-mailbericht wanneer de [!UICONTROL Planned Completion Date] wijzigt, tenzij de gebruiker die de [!UICONTROL Planned Completion Date] is ook de ontvanger.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus iets anders is dan [!UICONTROL Planning].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Nieuwe vervaldatum ([!UICONTROL Planned Completion Date])<br>Datum en tijdstip waarop de vervaldatum is gewijzigd<br>Naam van de gebruiker die de vervaldatum heeft gewijzigd<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal emissies waarvoor de vervaldatum geldt ([!UICONTROL Planned Completion Date]) gewijzigd<br>*Naam van uitgave<br>*Nieuw [!UICONTROL Planned Completion Date]<br>*Naam van de gebruiker die de vervaldatum heeft gewijzigd<br>*Datum van de dagelijkse samenvatting<br></p> </td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>De status verandert op een taak waaraan ik ben toegewezen</strong> <p>De taakontvanger ontvangt een e-mailbericht wanneer de status van de taak verandert, tenzij de gebruiker die de status heeft gewijzigd ook de ontvanger is.</p> <p>Opmerking: Dit bericht wordt niet verzonden wanneer de taakstatus wordt gewijzigd in voltooid. Een afzonderlijke melding wordt gebruikt voor voltooide taken. Zie <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Een taak waaraan ik ben toegewezen, is voltooid</a>, hierboven.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;task name=""&gt; van &lt;project name=""&gt; is &lt;new status=""&gt;</em></p> <p> </p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Naam van de gebruiker die de status heeft gewijzigd<br>Nieuwe status<br>Datum en tijd waarop de status is gewijzigd<br>Voorvertoningsstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal taken waar de Status veranderde<br>*Taaknaam<br>*Status vorige taak<br>*Nieuwe taakstatus<br>*Naam van de gebruiker die de status heeft gewijzigd<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De status verandert op een van mijn werkitems</strong> </p> <p>U ontvangt een e-mailmelding wanneer de status verandert in een uitgave waaraan u bent toegewezen, tenzij u de status zelf wijzigt. </p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Gebruikers met een [!UICONTROL Review] of [!UICONTROL Requestor] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;issue name=""&gt; van &lt;project name=""&gt; is &lt;new status=""&gt;</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die de status heeft gewijzigd<br>Nieuwe status<br>Datum en tijd waarop de status is gewijzigd<br>Status van vorige uitgave<br><strong>Meer informatie</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal uitgaven waarvoor de status is gewijzigd<br>*Taaknaam<br>*Status van vorige uitgave<br>*Status nieuwe uitgave<br>*Naam van de gebruiker die de status heeft gewijzigd<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
 </tbody> 
</table>
