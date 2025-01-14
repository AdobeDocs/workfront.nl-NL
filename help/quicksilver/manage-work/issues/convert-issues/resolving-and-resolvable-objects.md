---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Overzicht van Oplossende en Oplosbare objecten
description: Een oplosbaar object is een probleem waarvan de resolutie is gekoppeld aan een oplosbaar object. Een oplossend Voorwerp is een project, een taak, of een andere kwestie.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1771'
ht-degree: 0%

---

# Overzicht van Oplossende en Oplosbare objecten

Een oplosbaar object is een probleem waarvan de resolutie is gekoppeld aan een oplosbaar object. Een oplossend Voorwerp is een project, een taak, of een andere kwestie.

Wanneer u een kwestie in een taak of een project omzet, wordt de kwestie het Oplosbare Voorwerp van de taak of het project.

U kunt een kwestie aan een het oplossen Voorwerp manueel ook verbinden, dat een taak, een project, of een kwestie kan zijn. Voor informatie, zie [ manueel de resolutie van een kwestie aan andere kwesties, taken, of projecten ](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md) binden.

De originele kwestie wordt het Resolvable Voorwerp van de taak, het project, of de kwestie, in dit scenario.

## Adobe Workfront instellen voor verwerking van oplosbare objecten {#set-up-adobe-workfront-to-handle-resolvable-objects}

Als Workfront-beheerder of groepsbeheerder kunt u bepalen hoe u de Oplosbare objecten in uw systeem of voor uw groep wilt verwerken.

U kunt selecteren om het Resolvable Voorwerp te houden aangezien u het in een taak of een project omzet, of het te schrappen zodra de taak of het project worden gecreeerd. U kunt deze instellingen wijzigen tijdens het converteren van uitgaven. Hiermee kan de gebruiker de uitgaven converteren en selecteren of de uitgave behouden of verwijderen tijdens het converteren.

>[!NOTE]
>
>Oplosbare objecten zijn altijd problemen waarvan de resolutie en status afhankelijk kunnen zijn van de resolutie en status van het object dat ze hebben opgelost. Het oplossen van Voorwerpen kan kwesties, taken, of projecten zijn.

Voor informatie over vestiging voorkeur voor de behandeling van Oplosbare Voorwerpen, zie [ de taak van het hele systeem vormen en voorkeur uitgeven ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Verwerk het oplosbare object tijdens de conversie naar een project of een taak

Afhankelijk van de manier waarop de Workfront of de groepsbeheerder de systeem- of groepsniveauvoorkeuren heeft geconfigureerd, kunt u het oplosbare object mogelijk afhandelen tijdens de conversie van een probleem naar een project of taak.

De volgende scenario&#39;s bestaan:

* Als de Workfront of de groepsbeheerder de **originele kwestie heeft behouden en zijn resolutie aan de taak** en **binden houd de originele kwestie en verbind zijn resolutie aan het geselecteerde project** en **staan deze montages toe om tijdens omzetting** worden veranderd niet geselecteerd, zult u niet deze montages kunnen veranderen aangezien u kwesties in taken of projecten omzet.\
  ![](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Als Workfront of de groepsbeheerder de **originele kwestie heeft behouden en zijn resolutie aan de taak** binden en **de originele kwestie houden en zijn resolutie aan het project** of geselecteerde of unselected en **toestaan deze montages om tijdens geselecteerde omzetting** worden veranderd, zult u deze montages kunnen veranderen aangezien u kwesties in taken of projecten omzet.\
  ![](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

Voor meer informatie over het omzetten van kwesties in taken en projecten, zie [ Overzicht van het omzetten van kwesties in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p>  </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## De status van het verwijderbare object synchroniseren met die van het oplosbare object {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [ synchroniseer statussen wanneer het Resolving Voorwerp een kwestie ](#synchronize-statuses-when-the-resolving-object-is-an-issue) is
* [Synchroniseer statussen wanneer het Oplossende Voorwerp een taak of een project is](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### Statussen synchroniseren wanneer het oplossen van object een probleem is {#synchronize-statuses-when-the-resolving-object-is-an-issue}

Wanneer een uitgave handmatig aan een andere uitgave is gekoppeld, wordt door de status van de tweede uitgave (Object oplossen) een wijziging in de status van de eerste uitgave (Oplosbaar object) veroorzaakt. De status van de eerste uitgave komt overeen met de status waarnaar de tweede uitgave wordt gewijzigd. Dit geldt zowel voor de standaardstatus als voor de aangepaste uitgiftestatus.

### Synchroniseer statussen wanneer het Oplossende Voorwerp een taak of een project is {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

Wanneer een kwestie het Oplosbare Voorwerp van een taak of een project is, brengen de veranderingen in het statuut van de taken en de projecten veranderingen in het statuut van de kwestie teweeg. Standaardstatussen worden anders geactiveerd dan aangepaste statussen, in dit geval.

Wanneer de status van de projectdouane aan een standaardstatus evenaart die geen verandering in de uitgiftestatus teweegbrengt, brengt het geen verandering in status voor de kwestie teweeg.

* [ synchroniseer de Standaardstatus van het Resolving Voorwerp met de StandaardStatus van het Resolvable Voorwerp ](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [Synchroniseer de Status van de Douane van het Resolving Voorwerp met de Status van de Douane van het Oplosbare Voorwerp](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### Synchroniseer de Standaardstatus van het Oplossende Voorwerp met de Standaardstatus van het Oplosbare Voorwerp {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

Ongeacht of de status van het probleem &quot;Automatically update Resolvable Issue status when the status of the Resolving Object changes&quot; option is geselecteerd, verandert telkens als de standaardstatus verandert in de Resolving Objects (projects or tasks) de status van het object dat kan worden opgelost (issues) dienovereenkomstig. Alleen standaardstatussen worden al toegewezen om een dergelijke wijziging te activeren.

De volgende standaardstatussen voor taken activeren de volgende wijzigingen in de standaardstatussen voor uitgaven, wanneer de kwestie als het het oplossen van voorwerp van een taak wordt geplaatst:

| **STATUS VAN DE TAAK** | **STATUS VAN DE UITGAVE** |
|---|---|
| Nieuw | Nieuw |
| In uitvoering | In uitvoering |
| Voltooid | Gesloten |

De volgende standaardstatussen voor projecten brengen de volgende veranderingen in de standaardstatus voor kwesties teweeg, wanneer de kwestie als Resolvable Voorwerp van een project wordt geplaatst. Sommige statussen van projecten brengen geen veranderingen in de status van de kwesties teweeg. De kwesties blijven in de status verkeren die zij hadden voordat het project in een van deze statussen werd omgezet:

| **STATUS VAN HET PROJECT** | **STATUS VAN DE UITGAVE** |
|---|---|
| Planning | Nieuw |
| Huidig | In uitvoering |
| In de wachtstand | In de wachtstand |
| Gevraagd | Hiermee wordt geen wijziging in de emissiestatus veroorzaakt |
| Goedgekeurd | Hiermee wordt geen wijziging in de emissiestatus veroorzaakt |
| Geweigerd | Hiermee wordt geen wijziging in de emissiestatus veroorzaakt |
| Idea | Hiermee wordt geen wijziging in de emissiestatus veroorzaakt |
| Dead | Gesloten |
| Voltooid | Gesloten |

>[!NOTE]
>
>Nadat de status van de uitgave is afgesloten (als gevolg van het sluiten van de taak of het project), blijft de kwestie gesloten, ongeacht in welke status de taak of het project verandert nadat deze is gesloten.

#### Synchroniseer de Status van de Douane van het Resolving Voorwerp met de Status van de Douane van het Oplosbare Voorwerp {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

Wanneer u de status van de taak of het project wijzigt in een aangepaste status, verandert de status van de uitgave alleen in de status van een aangepaste uitgave als aan de volgende twee voorwaarden is voldaan:

* De optie &quot;Probleemstatus automatisch bijwerken wanneer de status van de optie Oplossend object verandert&quot; is geselecteerd. Voor meer informatie over hoe te om dit het plaatsen toe te laten, zie [ Opstelling Adobe Workfront om Oplosbare Voorwerpen ](#set-up-adobe-workfront-to-handle-resolvable-objects) te behandelen.

* De douanestatus van het project of de taak heeft de zelfde drie lettercode zoals de douanestatus van de kwestie.

U kunt aangepaste statussen maken met dezelfde sleutel voor zowel uitgaven als projecten of taken. Wanneer het project of de taak (als Oplossend Voorwerp) in de douanestatus worden veranderd, weerspiegelt de verandering ook op de status van de kwestie. De statussleutel moet gelijk zijn voor de uitgave en project- of taakstatus.

Maak bijvoorbeeld een aangepaste status voor een project met de naam &quot;Launched&quot; met de drielettercode &quot;LCD&quot; die gelijk is aan &quot;Current&quot; (Huidig). Maak ook een aangepaste status voor uitgave met de naam Project Launched, ook met de lettercode LCD die gelijk is aan &quot;In uitvoering&quot;. Wanneer u het project als &quot;Gelanceerd&quot;markeert, zal de kwestie automatisch de status in &quot;Project Gelanceerd&quot;veranderen. Als &quot;
Werk automatisch de status van het opgeloste probleem bij wanneer de status van de instelling van het Oplossende object verandert&quot; niet is ingeschakeld, verandert de status van het probleem in &quot;In uitvoering&quot; (de standaardstatus).

Voor meer informatie over het creëren van een douanestatus, zie [ een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

## Synchroniseer het percentage voltooide van een Oplossend Voorwerp met dat van het Oplosbare Voorwerp

Als een probleem door een taak of een project wordt opgelost, werkt het percentage voltooide van de kwestie over de oplosbare kwestie bij wanneer om het even welke volgende dingen voorkomen: 

* Wanneer iemand een wijziging in de taak of het project opslaat.
* De tijdlijn van het project wordt opnieuw berekend.

Als en het probleem wordt opgelost door een ander probleem, wordt het percentage bijgewerkt wanneer een van de problemen wordt bijgewerkt.

## Zoek het oplosbare object op een taak of een project

Het vinden van het het oplossen van voorwerp is identiek voor taken en projecten.

1. Navigeer naar een project of een taak die u creeerde door een kwestie in het project of de taak om te zetten.
1. Klik het **pictogram van de Details van het Project** of **Details van de Taak** en klik om het uit te breiden.
1. Klik **Overzicht**.
1. Bij de bodem van het lusje, bepaal de plaats van aan **Dit lost** gebied op: de kwestie die het Oplosbare Voorwerp van het project of de taak is vermeld op dit gebied.

   >[!NOTE]
   >
   >Uitgaven kunnen niet naar andere uitgaven worden geconverteerd, maar ze kunnen handmatig aan een Probleem oplossen worden gekoppeld. Een project, taak of kwestie kan veelvoudige kwesties als Oplosbare Voorwerpen hebben. Wanneer het project, de taak, of de kwestie oplossen, lost het Oplosbare Voorwerp (kwestie) ook op. Het Oplossbare probleem blijft gesloten, zelfs als het project, de taak of het probleem dat het oplost opnieuw wordt geopend.

## Probleem identificeren met een oplossend object in een lijst

In een lijst van kwesties, kunt u kwesties identificeren die als het oplossen van voorwerpen via statuspictogrammen door dit pictogram in de **pictogrammen van de Status** of **kolommen van Vlaggen** worden geëtiketteerd:

![](assets/ro1.png)

## De informatie van Objecten van de mening Oplosbaar en van het Oplossen in een rapport

U kunt informatie over de Oplosbare of Oplossende Voorwerpen in de mening of het rapport voor projecten, taken, of kwesties tonen.\
In de volgende tabel wordt aangegeven welke velden u kunt weergeven en in welke weergaven u deze kunt weergeven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Gebied in Mening </strong> </th> 
   <th><strong> Mening van de Uitgave </strong> </th> 
   <th><strong> Mening van de Taak </strong> </th> 
   <th><strong> Mening van het Project </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong> heeft Resolvables </strong>: Toont a <strong> Ware </strong> waarde als het project of de taak Oplosbare Kwesties verbonden aan hen heeft, en a <strong> Vals </strong> waarde als zij niet.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong> Oorspronkelijke Naam van de Uitgave, de Oorspronkelijke Datum van de Ingang van de Uitgave, de Naam van de Afgever </strong>: Toont de naam en ingangsdatum van de originele kwestie, evenals de naam van de gebruiker die de kwestie in een tekst-wijze aangepaste mening creeerde.<br> voor meer informatie over de bouw van een de douanemening van de tekstwijze voor een project of een taakrapport of lijst om informatie over de originele kwestie te tonen, zie <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref"> Mening: toon originele uitgifteinformatie over taak of projectlijsten </a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong> Resolvables:</strong> toont een lijst van alle Resolvable Voorwerpen op een de douanemening van de tekstwijze voor een project of taakrapport of een lijst.</p> <p>Voor meer informatie over de bouw van deze mening, zie <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref"> Mening: De oplosbare Voorwerpen in een taak of projectrapport </a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong> Bekeerde de Hervormer van de Uitgave </strong>: De informatie van vertoningen over de gebruiker die oorspronkelijk de kwestie opende die later in de taak werd omgezet. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong> los Project </strong> op: De informatie van vertoningen over het Oplossende Project dat of van de originele kwestie werd omgezet, of manueel als Oplossend Voorwerp van een kwestie werd aangewezen.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong> los Taak </strong> op: De informatie van vertoningen over de Resolving Taak die of van de originele kwestie werd omgezet, of manueel als het Oplossen Voorwerp van een kwestie wordt aangewezen.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong> los Uitgave </strong> op: De informatie van vertoningen over het Oplossen Uitgave die manueel als het Oplossen Voorwerp van een kwestie werd aangewezen.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
