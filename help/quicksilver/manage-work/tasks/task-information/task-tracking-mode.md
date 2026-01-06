---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van de modus Taken bijhouden
description: U kunt de instelling van de modus Tekstspatiëring van een taak aanpassen wanneer u een taak maakt of bewerkt om te bepalen hoe en wanneer de voortgangsstatusindicatoren van een taak worden weergegeven. Adobe Workfront geeft voortgangsstatusvlaggen weer wanneer u bepaalde instellingen configureert voor het bijhouden van de voortgang van taken.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Overzicht van de modus Taken bijhouden

<!-- Audited: 01/2024 -->

U kunt de instelling van de modus Tekstspatiëring van een taak aanpassen wanneer u een taak maakt of bewerkt om te bepalen hoe en wanneer de voortgangsstatusindicatoren van een taak worden weergegeven. Adobe Workfront geeft voortgangsstatusvlaggen weer wanneer u bepaalde instellingen configureert voor het bijhouden van de voortgang van taken.

Voor meer informatie over de Voortgangsstatus van taken, zie [ Overzicht van de Status van de Voortgang van de Taak ](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click <strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the <strong>Settings</strong> section, use the <strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Opties voor trackingmodus {#tracking-mode-options}

Als taakeigenaar of projectmanager kunt u bepalen hoe Workfront de status van de voortgang van elke taak aangeeft. Voor informatie over hoe te om het Volgen Wijze op uw taken te plaatsen, zie [ Reeks het Volgen Wijze voor taken ](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

U kunt uit de volgende opties selecteren:

* [ Gebruiker moet ](#user-must-update) bijwerken
* [ veronderstel op Tijd ](#assume-on-time)
* [ negeer Late Waarschuwingen ](#ignore-late-warnings)
* [ Auto Volledig ](#auto-complete)
* [Voorganger](#predecessor)

### Gebruiker moet bijwerken {#user-must-update}

Als deze optie is geselecteerd, gebruikt Workfront het programma Procent voltooid en Werkelijke uren om de status van de voortgang van de taak te bepalen. Dit is de standaardoptie.

### Veronderstellen op tijd {#assume-on-time}

Workfront gaat ervan uit dat een taak op tijd wordt voltooid, ongeacht de huidige voltooiingsstatus. Als de taak niet op tijd (op de Geplande VoltooiingsDatum) wordt voltooid, dan neemt Workfront automatisch een Geplande VoltooiingsDatum van de volgende werkdag over. U moet nog aangeven wanneer de taak is voltooid. Gebruik deze optie als gebruikers hun taken niet regelmatig bijwerken.

### Te late waarschuwingen negeren {#ignore-late-warnings}

De status van de Voortgang van een taak zal op Tijd zijn tot het te laat wordt. Bijvoorbeeld, als u een taak plant om 10 dagen te nemen en op de dag het moet worden voltooid toont de taak een Percentage Voltooid van 60%, dan werkt Workfront de Geprojecteerde Datum van Voltooiing door vier dagen toe te voegen en de Status van de Voortgang van de taak wordt Te laat.

### Automatisch aanvullen {#auto-complete}

Workfront gaat ervan uit dat de taken volgens planning zullen worden voltooid en markeert ze als voltooid op de vervaldatum of de geplande datum van voltooiing. Tot dat, gebruikt Workfront het programma van de Uren van de Percentage Volledige en Werkelijke die Uren om de Status van de Voortgang te bepalen. Ongeacht de status van de voortgang vóór de geplande voltooiingsdatum markeert Workfront echter nog steeds de voltooide taak.

De volgende uitzonderingen bestaan:

* Als de taak onvolledige voorgangers heeft, zal het niet automatisch worden voltooid tot al zijn voordecessors worden voltooid. Voorgangers moeten worden afgedwongen.
* Als de taak een beperking van Vaste Datum heeft, voltooit de taak altijd op de Geplande Datum van Voltooiing, ongeacht of zijn predecessors worden voltooid.

>[!IMPORTANT]
>
>Als u wilt dat taken automatisch worden voltooid, markeert u de taak Voltooien wanneer de projecttijd opnieuw wordt berekend. Als het Type van Update van het project aan Automatisch of Automatisch en bij Verandering wordt geplaatst, wordt de projectchronologie dagelijks berekend. Voor informatie over chronologieherberekeningen over projecten, zie [ projectchronologie ](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.
>
>De tijd van de datum van daadwerkelijke voltooiing is middernacht van de dag wanneer de chronologie automatisch wordt berekend. De tijd die wordt gebruikt om deze tijdstempel te genereren is de tijdzone van uw systeem zoals die door uw Workfront-beheerder in het gedeelte Klantgegevens van Setup is gedefinieerd. Voor informatie over het plaatsen van de tijdzone van uw systeem, zie [ basisinformatie voor uw systeem ](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

### Voorganger {#predecessor}

Workfront raamt de voorspelde voltooiingsdatum van een taak op basis van zijn eerdere relatie. De status van de voortgang van een taak wordt bepaald op basis van deze schatting. Bijvoorbeeld, heeft Taak B een Duur van 1 Dag en is gepland om twee dagen na zijn voorganger, Taak A te voltooien, die vijf dagen zou moeten nemen. Een gebruiker werkt dan Taak B aan 50% volledig bij, maar predecessor, Taak A, is nog niet begonnen. Workfront plant afhankelijke Taak B zes dagen na de begindatum van de voorgangertaak, die 5 dagen voor Taak A en 1 dag voor Taak B toestaat.
