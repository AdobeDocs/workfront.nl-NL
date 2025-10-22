---
product-area: reporting
navigation-topic: using-built-in-reports
title: Ingebouwde statuspictogrammen in weergaven
description: U kunt het veld Ingebouwde statuspictogrammen als een kolom in uw weergaven toevoegen om de zichtbaarheid te vergroten in belangrijke punten van uw objecten.
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# Ingebouwde statuspictogrammen in weergaven

<!-- Audited: 11/2024 -->

<!--(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.)-->

U kunt het veld Ingebouwde statuspictogrammen als een kolom in uw weergaven toevoegen om de zichtbaarheid te vergroten in belangrijke punten van uw objecten. Met Statuspictogrammen kunt u in één oogopslag zien wanneer de volgende voorwaarden bestaan:

* Een object bevat documenten
* Een object is gekoppeld aan een goedkeuringsproces
* Aan een object zijn aanvullende notities gekoppeld
* Een last is factureerbaar of terugbetaalbaar
* Een taak bevindt zich op een kritiek pad
* Een gebruiker behoort tot een bedrijf, een team, of persoonlijk gevestigd in een verschillende tijdzone

Overweeg het volgende:

* De meeste indicatoren in het veld Statuspictogrammen zijn snelle koppelingen naar het werkelijke object of gebied van het object dat ze vertegenwoordigen.

* Als een van de items die door de pictogrammen worden vertegenwoordigd, niet aanwezig is in het object, wordt het pictogram dat het ontbrekende item vertegenwoordigt, grijs weergegeven in de kolom Statuspictogrammen in plaats van in een gekleurde afbeelding.

  ![ task_status_icons.png ](assets/task-status-icons.png)

  Voor meer informatie, zie het [ Overzicht van de Pictogrammen van de Status en sectie van Vlaggen ](#overview-of-status-icons-and-flags) in dit artikel.

* In sommige meningen, wordt het **gebied van de Pictogrammen van de Status 0} genoemd** Vlaggen **of** Pictogrammen van de Mening **.**\
  U kunt de vormgeving van de pictogrammen in het veld Statuspictogrammen niet aanpassen.

* U kunt het aantal pictogrammen niet bewerken in het veld Statuspictogrammen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Medewerker of hoger</p>
      <p>Aanvraag of hoger</p>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om kolommen aan een rapport toe te voegen</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een bestaande weergave</p> <p>Rechten beheren aan een rapport om er kolommen aan toe te voegen</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het veld Statuspictogrammen toevoegen aan een weergave

In sommige ingebouwde weergaven en rapporten is het veld Statuspictogrammen al opgenomen.

U kunt het veld Statuspictogrammen niet aan alle weergaven toevoegen.

Het veld Statuspictogrammen toevoegen aan een aangepaste weergave die u vanaf nul maakt:

1. Ga naar een lijst met een van de volgende objecten:

   * Taken
   * Problemen
   * Projecten
   * Sjabloontaken
   * Sjablonen
   * Uitgaven
   * Documenten
   * Gebruikers\
     Slechts hebben deze voorwerpen het **beschikbare gebied van de Pictogrammen van de Status 0} {.**\
     Voor informatie over objecten lijsten, zie [ begonnen worden met lijsten in Adobe Workfront ](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. Klik **toevoegen Kolom**.
1. In **toon in deze kolom** doos, begin om het even welke volgende gebiedsnamen te typen, dan het te selecteren wanneer het in de lijst verschijnt:

   * *Pictogrammen van de Status*
   * *Vlaggen*
   * *Pictogrammen van de Mening* (slechts in de meningen van het Document).

   De ingebouwde pictogrammen staan onder een van deze namen.\
   Een mening van het Malplaatje bevat zowel de **Pictogrammen van de Status** als de **Vlaggen** gebieden. In dit geval bevatten de twee kolommen identieke pictogrammen.\
   De meningen van het document bevatten a **gebied van de Pictogrammen van de a** Mening.

1. Klik **sparen Mening**.
1. (Facultatief) specificeer een nieuwe naam voor uw mening, dan klik **sparen Mening**.\
   Dit voegt de **pictogrammen van de Status** kolom aan uw Mening toe.
1. (Optioneel) Plaats de muisaanwijzer op een pictogram om te begrijpen wat het vertegenwoordigt.
1. (Optioneel) Klik op een pictogram om naar het gebied van het object te gaan dat wordt weergegeven.\
   Niet alle pictogrammen zijn koppelingen naar objecten.\
   Voor een volledige lijst van attributen voor elk pictogram, zie het [ Overzicht van de Pictogrammen van de Status en sectie van Vlaggen ](#overview-of-status-icons-and-flags).

## Overzicht van statuspictogrammen en vlaggen {#overview-of-status-icons-and-flags}

In de volgende tabel worden alle statuspictogrammen weergegeven die beschikbaar zijn in Workfront, het type objecten dat eraan kan worden gekoppeld en wat er gebeurt wanneer u erop klikt.

U moet over machtigingen beschikken om de objecten ten minste weer te geven, zodat u op een aantal van de volgende pictogrammen kunt klikken en deze objecten kunt openen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Pictogram van de Status of Vlag </strong> </th> 
   <th><strong> Beschrijving </strong> </th> 
   <th><strong> Voorwerp </strong> </th> 
   <th>Bij klikken</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">of <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon_in_problem.png" style="width: 29;height: 26;"> of <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> of <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Geeft aan dat de voorwaarde van het project On Target (groen), In Trouble (rood) of At Risk (geel) is.<br> voor informatie over projectvoorwaarde, zie <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref"> Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project </a>.</td> 
   <td>Projecten</td> 
   <td>Klik om de takenlijst van het project te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Geeft aan dat voor het object notities (updates) zijn opgenomen op het tabblad Updates.</td> 
   <td> <p>De projecten <br> van Taken <br> Malplaatjes <br> Taken van het Malplaatje<br></p> </td> 
   <td> <p>Klik om het tabblad Updates van het object te openen. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">of <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Geeft aan dat aan het object documenten zijn gekoppeld. </td> 
   <td> De projecten <br> van Taken <br> Malplaatjes <br> Taken van het Malplaatje<br> </td> 
   <td>Klik om het tabblad Documenten van het object te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">of <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Geeft aan dat er openstaande problemen zijn met het project of de taak.</td> 
   <td> Projecten <br> Taken </td> 
   <td>Klik om het object te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> of <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Geeft aan dat er goedkeuring is voor het object.</td> 
   <td> De projecten <br> van Taken <br> Malplaatjes <br> Taken van het Malplaatje<br> </td> 
   <td>Klik om het object te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="uitgaven_pictogram.png" style="width: 52;height: 40;"> </td> 
   <td> <p>U kunt een kolom van het pictogram van Uitgaven in uw mening toevoegen om dit pictogram te tonen. Dit wijst erop dat het project of de taak uitgaven verbonden aan hen heeft.</p> </td> 
   <td> <p>Projecten</p> <p>Taken</p> </td> 
   <td>Klik om het tabblad Uitgaven van het project of de taak te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Geeft aan dat de status van voortgang van een taak een van de volgende is:</p> 
    <ul> 
     <li>Op tijd (groen vierkant)</li> 
     <li>Late (rode cirkel)</li> 
     <li>Risico (blauwe ruit)</li> 
     <li>Achter (gele driehoek)</li> 
    </ul> <p>Voor informatie over de Voortgangsstatus van taken, zie <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref"> Overzicht van de Status van de Voortgang van de Taak </a>.</p> </td> 
   <td>Taken</td> 
   <td>Klik om de taak te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="taak_kritiek_pad_pictogram.png" style="width: 36;height: 35;"> of <img src="assets/new-critical-path-icon-34x34.png" alt="new_kritiek_pad_pictogram.png" style="width: 34;height: 34;"></td> 
   <td>Geeft aan dat de taak zich momenteel op het kritieke pad bevindt. <br> voor informatie over taken op een Kritieke Weg van het project, zie <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref"> Overzicht van het project Kritieke Weg </a>.</td> 
   <td>Taken</td> 
   <td>Klik om de taak te openen.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Geeft aan dat de taak aan een mijlpaal is gekoppeld. Uw systeembeheerder kan de kleur van de ruit in uw milieu aanpassen.<br> voor informatie over mijlpalen, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref"> een milestone weg </a> creëren.</td> 
   <td>Taken</td> 
   <td>Klik om de taak te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Koppeling naar het bronobject van een uitgave. Het bronobject van een uitgave is het object waarin de uitgave is vastgelegd. Een taak of een project kan bronvoorwerpen voor kwesties zijn. </td> 
   <td>Problemen</td> 
   <td>Klik om het bronobject (taak of project) van een uitgave te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Geeft aan dat er een object is dat het probleem uiteindelijk verhelpt. In dit geval kunt u het probleem niet voltooien. De bewerking wordt voltooid wanneer het object dat het omzetten uitvoert, is voltooid. <br> voor informatie over het oplossen van voorwerpen, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</td> 
   <td>Problemen</td> 
   <td>Klik om het oplossende voorwerp van de kwestie te openen. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Een document weergeven.</td> 
   <td>Documenten</td> 
   <td>Klik om het document te downloaden.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Download een document.</td> 
   <td>Documenten</td> 
   <td>Klik om het document te downloaden.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Geeft het type document aan.</td> 
   <td>Documenten</td> 
   <td>Klik om het document te downloaden.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_behoort_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Wijst erop dat de gebruiker met een Bedrijf wordt geassocieerd. </td> 
   <td>Gebruikers</td> 
   <td>Niet beschikbaar</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Wijst erop dat de gebruiker met een Team wordt geassocieerd.</td> 
   <td>Gebruikers</td> 
   <td>Klik om het gebruikersprofiel te openen.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Sneltoets naar het tabblad Toewijzing van de gebruiker. </td> 
   <td>Gebruikers</td> 
   <td>Klik om het tabblad Toewijzing van de gebruiker te openen en te leren aan welke werkitems de gebruiker heeft toegewezen.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Geeft aan dat de gebruiker zich in een andere tijdzone bevindt dan die van het systeem.</td> 
   <td>Gebruikers</td> 
   <td>Niet beschikbaar</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_last_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Geeft aan dat een uitgave factureerbaar is.<br> voor informatie over uitgaven, zie <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref"> projectuitgaven beheren </a>.</td> 
   <td>Uitgaven</td> 
   <td>Niet beschikbaar</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="last_restitusable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> Geeft aan dat een uitgave terugbetaalbaar is.<br> voor informatie over uitgaven, zie <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref"> projectuitgaven beheren </a>.</td> 
   <td>Uitgaven</td> 
   <td>Niet beschikbaar</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="vergoed_uitgave_pictogram.png" style="width: 44;height: 43;"></td> 
   <td> Geeft aan dat een uitgave is vergoed.<br> voor informatie over uitgaven, zie <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref"> projectuitgaven beheren </a>.</td> 
   <td>Uitgaven</td> 
   <td>Niet beschikbaar</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
