---
product-area: projects
navigation-topic: convert-issues
title: Overzicht van conversie van problemen in Adobe Workfront
description: Als meer werk moet worden gedaan om een kwestie te voltooien nadat de kwestie wordt voorgelegd, kunt u de kwestie in een project of in een taak omzetten.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 586abc0babac2a9b3d6d22bebe841c217315b064
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# Overzicht van conversie van problemen in Adobe Workfront

Als meer werk moet worden gedaan om een kwestie te voltooien nadat de kwestie wordt voorgelegd, kunt u de kwestie in een project of in een taak omzetten.

Voor informatie over het omzetten van kwesties in taken, zie [ een kwestie in een taak in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issue-to-task.md) omzetten.

Voor informatie over het omzetten van kwesties in projecten, zie [ een kwestie in een project in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issue-to-project.md) omzetten.

## Overwegingen bij het converteren van problemen

* Wanneer het omzetten van kwesties in taken of projecten, meeste informatie van de uitgifteoverdrachten aan de taak of het project, tenzij anders gespecificeerd in dit artikel.
* Uw beheerder van Workfront of groepsbeheerder heeft reeds de voorkeur voor wat met een kwestie, zijn resolutie, en de toegang van zijn Primair Contact wanneer het in een project of een taak wordt omgezet, zoals die in [ wordt geschetst vormt systeembrede taak en geeft voorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) uit.
* Workfront verwijdert goedkeuringen die tijdens de conversie aan problemen zijn gekoppeld.
* Workfront overschrijft het Oplossende Voorwerp van de kwestie wanneer u het in een taak of een project omzet. De nieuwe taak of kwestie wordt het nieuwe Oplossende Voorwerp van de kwestie na omzetting.
* Overweeg het volgende:

   * Tijdens de conversie wordt u mogelijk gevraagd of u het probleem en de bijbehorende resolutie wilt koppelen aan het project of de taak die u maakt.
   * Als u de kwestie houdt, werken de status en het percentage volledig van het project of de taak automatisch de status en het percentage volledig van de kwestie bij wanneer om het even welke veranderingen op het project, de taak, of de kwestie voorkomen of wanneer Workfront de chronologie opnieuw berekent.

  >[!NOTE]
  >
  >   Nadat de status van de uitgave is afgesloten (als gevolg van het sluiten van de taak of het project), blijft de kwestie gesloten, ongeacht in welke status de taak of het project verandert nadat deze is gesloten.


* Wanneer het omzetten van een kwestie in een taak of een project, wordt de kwestie verwijderd uit het gebied van het Huis van de gebruiker die aan de kwestie wordt toegewezen.

* Bij het omzetten van een uitgave worden de machtigingen naar de oorspronkelijke uitgaven niet overgedragen naar het omgezette object (taak of project).

* Wanneer het omzetten van een kwestie in een project gebruikend een malplaatje, de meeste informatie van het malplaatje overdrachten aan het nieuwe project. Bepaalde informatie uit de uitgave kan echter ook naar het nieuwe project worden overgedragen. Voor meer informatie, zie het [ Overzicht van projectgebieden wanneer het omzetten van een kwestie in een project gebruikend een malplaatje ](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) sectie in dit artikel.
* Tijdens het converteren van een uitgave worden niet alle documenten of de bijbehorende gegevens verplaatst naar het nieuwe object waarnaar de uitgave wordt geconverteerd. De volgende items worden opgenomen wanneer u een uitgave converteert waaraan documenten of documentkoppelingen zijn gekoppeld:

   * Document
   * Het document is gekoppeld aan services van derden, zoals Google Drive of SharePoint.
   * Versies
   * De proef is inbegrepen slechts wanneer de optie **de originele kwestie houdt en zijn resolutie aan deze taak bindt** niet geselecteerd is.
   * Documentgoedkeuringen worden niet opgenomen wanneer u een uitgave converteert waaraan documenten en documentkoppelingen zijn gekoppeld.

* Als u hebt besloten de uitgave bij de conversie te houden en er documenten aan zijn gekoppeld, worden het document en de versies ervan naar het project of de taak gekopieerd. De proefdrukken en de documentgoedkeuringen worden niet gekopieerd naar het project of de taak.
* Als u hebt besloten de uitgave niet bij de conversie te houden en er documenten aan zijn gekoppeld, worden het document, de versies en de proefdrukken naar het project of de taak overgedragen. De documentgoedkeuringen worden niet overgedragen naar het project of de taak.
* Als er documenten en mappen zijn gekoppeld aan de oorspronkelijke uitgave bij externe services, zoals Google Drive, worden deze koppelingen naar het nieuwe object gekopieerd, ongeacht of u de uitgave bewaart of niet tijdens de conversie.
* Opmerkingen bij uitgaven worden ook gekopieerd naar de taak of het project dat vanuit de uitgave is geconverteerd, maar gelabelde gebruikers worden niet overgedragen.
* Als u de informatie van de douaneformulier van de kwestie naar het project of de taak wilt overbrengen u het in zet, zorg ervoor u een project of een vorm van de taakdouaneformulier hebt die de zelfde gebieden omvat u van de kwestie wilt overbrengen. Voor meer informatie, zie [ de gegevens van de douanevorm van de Overdracht wanneer het omzetten van een voorwerp ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Overzicht van projectgebieden wanneer het omzetten van een kwestie in een project gebruikend een malplaatje {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

Wanneer het omzetten van een kwestie in een project, kunt u of het in een leeg project omzetten of een malplaatje gebruiken.

Voor informatie, zie [ Bekeerling een kwestie in een project in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

Wanneer het gebruiken van een malplaatje, sommige gebieden die op de malplaatjeoverdracht aan het project worden bevolkt dat van de omgezette kwestie wordt gecreeerd. Andere gebieden brengen naar het project van de omgezette kwestie over.

De volgende lijst maakt een lijst van projectinformatie en of het van het malplaatje of van de kwestie overbrengt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Beschrijving</td> 
   <td> <p>De beschrijving van de uitgifteoverdracht naar het nieuwe project. </p> <p> Als er geen beschrijving over de kwestie is, brengt de Beschrijving van het malplaatje naar het project over. </p> <p>Als het veld Beschrijving zowel voor de uitgave als voor de sjabloon leeg is, is het veld in het project leeg. </p> </td> 
  </tr> 
  <tr> 
   <td>Status</td> 
   <td>Standaardstatus geselecteerd voor de groep op de sjabloon. Als het malplaatje niet met de groep wordt geassocieerd, wordt de projectstatus geplaatst aan de standaardstatus die door de beheerder van Workfront op het gebied van de Voorkeur van het Project van Opstelling wordt geplaatst. Voor informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</td> 
  </tr> 
  <tr> 
   <td>Prioriteit</td> 
   <td><p>Overdrachten van de uitgifte.</p>
   <p>Wanneer u een malplaatje voor het omgezette project gebruikt, hebt u de optie om de Prioriteit manueel te veranderen. Als u ervoor kiest deze instelling niet te wijzigen, wordt de prioriteit van de uitgave aan het project overgedragen. 
    </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>De URL van de uitgave wordt overgedragen naar het nieuwe project. </p> <p> Als er geen URL is gespecificeerd op de kwestie, brengt URL van het malplaatje naar het project over. </p> <p>Als het veld URL zowel voor de uitgave als voor de sjabloon leeg is, is het veld in het project leeg. </p> </td> 
  </tr> 
  <tr> 
   <td>Type projectvoorwaarde</td> 
   <td>Overdrachten uit de sjabloon.</td> 
  </tr> 
  <tr> 
   <td>Projectvoorwaarde</td> 
   <td>Komt overeen met de standaardvoorkeur op systeemniveau zoals bepaald door de Workfront-beheerder in het gedeelte Setup. Voor informatie, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref"> plaats een douanetoewijzing als gebrek voor projecten </a></td> 
  </tr> 
  <tr> 
   <td>Schema vanuit</td> 
   <td>Overdrachten uit de sjabloon.</td> 
  </tr> 
  <tr> 
   <td>Projectdatums</td> 
   <td> 
    <ul> 
     <li> <p><b> Geplande Datum van het Begin </b>: De dichtstbijzijnde arbeidstijd die op de het werktijd van het malplaatjeprogramma wordt gebaseerd zou, volgens de tijdzone van het programma van het malplaatje vooraf moeten worden geselecteerd. Dit veld is uitgeschakeld als het veld Planning van wordt ingesteld op Van voltooiing. </p> </li> 
     <li> <p><b> Geplande Datum van de Voltooiing </b>: De dichtstbijzijnde die arbeidstijd op de de werktijd van het malplaatjeprogramma wordt gebaseerd zou, volgens de tijdzone van het programma van het malplaatje vooraf moeten worden geselecteerd. Dit veld is uitgeschakeld als het veld Planning van wordt ingesteld op Van begin. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Overdrachten uit de sjabloon. Anders is dit veld leeg.</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>Overdrachten uit de sjabloon. Anders is dit veld leeg.</td> 
  </tr> 
  <tr> 
   <td>Groep</td> 
   <td><p> De volgende scenario's bestaan:</p>
     <ul><li>Als een groep tijdens de omzetting wordt gespecificeerd, wordt dat de groep van het project</li>
     <li>Als u in een project omzet gebruikend een malplaatje, en er een groep op het malplaatje is, en tijdens de omzetting u geen groep specificeert, dan wordt de groep van het malplaatje de groep van het nieuwe project</li>
      <li> Als er geen groep op het malplaatje is en u geen groep tijdens de omzetting specificeert, dan wordt de groep van het oorspronkelijke project van de kwestie de groep van het nieuwe project</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>Bedrijf</td>    
   <td>  Overdrachten uit de sjabloon. Anders is dit veld leeg.</td>

</tr> 
  <tr> 
   <td>Projecteigenaar</td> 
   <td>Overdrachten van het gebied van de Eigenaar van het Malplaatje op het malplaatje. Anders, wordt het geplaatst aan het programma geopende gebruiker die de omzetting uitvoert. </td> 
  </tr> 
  <tr> 
   <td>Projectsponsor</td> 
   <td>Overschrijvingen van het veld Sjabloonsponsor op de sjabloon. Anders is dit veld leeg.</td> 
  </tr> 
  <tr> 
   <td>Resource Manager</td> 
   <td>Overdrachten uit de sjabloon. Anders is dit veld leeg.</td> 
  </tr> 
  <tr> 
   <td>Taakinstellingen</td> 
   <td>Overdracht van de sjabloon.</td> 
  </tr> 
  <tr> 
   <td>Instellingen van uitgave</td> 
   <td>Overdracht van de sjabloon. </td> 
  </tr> 
  <tr> 
   <td>Toegang</td> 
   <td> <p>Overdrachten van de sectie van de Toegang op het malplaatje. </p> </td> 
  </tr> 
  <tr> 
   <td>Goedkeuringen</td> 
   <td>Overdracht van de sjabloon. De goedkeuringen die bij de uitgave horen, worden tijdens de conversie verwijderd. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p>  </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p>  </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## Originele informatie over projecten en taken weergeven {#view-original-issue-information-on-projects-and-tasks}

U kunt de originele uitgifteinformatie in project en taaklijsten en rapporten of in het gebied van de Details van het Project bekijken. Voor informatie over de bouw van rapporten, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

In de volgende tabel wordt aangegeven welke velden zichtbaar zijn van de omgezette projecten en taken.

| Probleemvelden | Project- of taakveld | Projectlijst of -rapport | Het gebied Projectdetails | Taaklijst of rapport | Taakdetails, gebied |
|---|---|---|---|---|---|
| Naam van uitgave | Omgezette uitgeversnaam | ✔ | ✔ | ✔ | ✔ |
| Primaire contactpersoon | Naam van initiator van geconverteerde uitgave | ✔ | `✔` | ✔ |  |
| Invoerdatum | Invoerdatum van geconverteerde uitgave | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Als de Primaire Contact van een kwestie verandert of als de kwestie van het project of de taak los wordt nadat de kwestie is omgezet, werkt de Omgezette Naam van de Ontvanger van de Uitgave niet bij en het toont de originele Primaire Contact van de kwestie op het tijdstip dat de kwestie werd omgezet.
