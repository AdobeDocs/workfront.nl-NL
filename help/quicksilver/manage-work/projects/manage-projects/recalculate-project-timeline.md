---
product-area: projects
navigation-topic: manage-projects
title: Projecttijdlijnen opnieuw berekenen
description: Door de tijdlijnen opnieuw te berekenen kunnen beheerders zien hoe verschillende factoren die met het project samenhangen, van invloed zijn op de tijdlijn van het project. De tijdlijn van een project verwijst naar geplande en geplande data.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 0%

---

# Projecttijdlijnen opnieuw berekenen

<!--Audited: 06/2025-->

Door de tijdlijnen opnieuw te berekenen kunnen beheerders zien hoe verschillende factoren die met het project samenhangen, van invloed zijn op de tijdlijn van het project. De tijdlijn van een project verwijst naar geplande en geplande data.

Het aanbrengen van veranderingen in programma&#39;s, personeelstijd weg, en andere punten buiten het werkingsgebied van een project beïnvloeden niet onmiddellijk de projectchronologie. De projecttijdlijn wordt beïnvloed wanneer de tijdlijn opnieuw wordt berekend. Externe invloeden hebben pas effect op uw project als de herberekening plaatsvindt.

In dit artikel worden de manieren beschreven waarop tijdlijnherberekening plaatsvindt.

De automatische chronologieherberekening gebeurt zonder speciale toegang voor om het even welke gebruikers betrokken bij het werken aan het project. Bovendien kunt u de tijdlijn handmatig opnieuw berekenen.

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
   <td> <p>Standard</p> 
    <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Systeembeheerder om de tijdlijn voor alle projecten in het systeem opnieuw te berekenen</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard </p> 
    <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Automatische herberekening

Door gebrek, worden de projectchronologie automatisch opnieuw berekend dagelijks wanneer het projectwerkingsgebied verandert of elke nacht. De beheerder van Workfront bepaalt of om chronologie elke nacht of met elke werkingsgebiedverandering automatisch te berekenen door de montages van Chronologie in het gebied van de Voorkeur van het Project van Opstelling te beheren. Voor meer informatie, zie [ chronologieherberekeningen voor projecten ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md) vormen.

>[!IMPORTANT]
>
>* Als de tijdlijn van een project langer is dan 15 jaar, wordt de automatische herberekening uitgeschakeld voor dat project en kunt u alleen een Handmatig updatetype selecteren. Als u de datums in het project wijzigt in minder dan 15 jaar, moet u de tijdlijn handmatig opnieuw berekenen voordat deze automatisch wordt berekend.
>* Voor de milieu&#39;s van de Sandbox van de Voorproef en van het Douane verfrissen, wordt de niight herberekening onbruikbaar gemaakt en de projectchronologie wordt niet automatisch opnieuw berekend. U moet de projectchronologie voor de Voorproef en de Douane manueel opnieuw berekenen vernieuwt Sandbox milieu&#39;s.
>* Als een project complex is, kan de automatische chronologieherberekening niet voorkomen.
> Een voorbeeld van een complex project zou een project met veelvoudige gebiedsdelen, groot aantal taken, verscheidene dwars-project predecessors, of veelvoudige taakinspringingen kunnen zijn.
> Workfront plaatst een waarschuwing rechts van de projectnaam op de projectpagina om gebruikers te adviseren dat de projectchronologie manueel moet worden opnieuw berekend. Alleen gebruikers met de machtiging Beheren voor het project kunnen de tijdlijn handmatig opnieuw berekenen.
>
>   ![ waarschuwing van het Project om chronologie ](assets/project-warning-to-manually-recalculate-timeline.png) opnieuw te berekenen
>

* [ Automatische herberekening van projectchronologie ](#automatic-recalculation-of-project-timelines)
* [Handelingen die een automatische herberekening van projecttijdlijnen activeren](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)



### Automatische herberekening van projecttijdlijnen {#automatic-recalculation-of-project-timelines}

Workfront herberekent dagelijks tijdlijnen alleen voor projecten waarbij aan alle volgende voorwaarden is voldaan:

* Huidige status hebben.
* Het updatetype van het project wordt geplaatst aan Automatisch of Automatisch en bij Verandering.

  Voor informatie, zie [ Overzicht van het Type van Update van het Project ](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Hebt u een datum voor laatste update in de afgelopen 3 maanden. Een Workfront-beheerder kan deze standaardfunctionaliteit wijzigen. Voor meer informatie, zie [ chronologieherberekeningen voor projecten ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md) vormen.

* De laatste berekeningsdatum van de projecttijdlijn valt niet binnen de huidige kalenderdag. Dit betekent dat de laatste berekeningsdatum van de projectchronologie vóór 00 :00 van de huidige dag is.

U kunt vormen hoe vaak de chronologie voor uw project wordt bijgewerkt. Wanneer de projectchronologie wordt bijgewerkt, wordt het opnieuw berekend gebaseerd op veranderingen die aan het project worden aangebracht.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Voor informatie, zie [ het Type van projectupdate ](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click  <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Handelingen die een automatische herberekening van projecttijdlijnen activeren {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Diverse bereikwijzigingen in de levensduur van een project berekenen de projecttijdlijn automatisch opnieuw, inclusief de volgende acties:

* Taakstatus wordt bijgewerkt.
* Een taak naar een ander project verplaatsen.
* De geplande datum of geplande einddatum van de taken bijwerken.
* Het bijwerken van het Type van Duur, de Beperking van de Taak, of het aantal wijzers op de taken.
* Het bijwerken van taak predecessor verhoudingen.
* Het toevoegen van een goedkeuring aan een taak die ook tijd aan de Geplande Datum van Voltooiing van de taak toevoegt.\
  Voor meer informatie over goedkeuringsmontages, zie [ globale goedkeuringsmontages ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md) vormen.

## Handmatige herberekening {#manual-recalculation}

Als projecteigenaar, kunt u de chronologie voor individuele projecten manueel opnieuw berekenen. De Workfront-beheerder kan alle tijdlijnen in Workfront handmatig opnieuw berekenen.

* [ herberekent chronologie voor individuele projecten of in bulk ](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [ manueel herberekent chronologie in bulk in het Edit vakje van Projecten ](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Tijdlijnen voor alle projecten in het systeem opnieuw berekenen (alleen voor Workfront-beheerders)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Tijdlijnen voor afzonderlijke projecten of bulksgewijs opnieuw berekenen {#recalculate-timelines-for-individual-projects-or-in-bulk}

U kunt de chronologie van een project in Workfront van de projectpagina of van een projectlijst of rapport opnieuw berekenen.

1. Ga naar het project u de chronologie voor wilt opnieuw berekenen en **Meer** pictogram ![ klikken Meer menu ](assets/qs-more-menu.png) links van de projectnaam.

   of

   Ga naar een projectlijst of een rapport en selecteer één of verscheidene projecten, dan klik **Meer** pictogram ![ Meer menu ](assets/qs-more-menu.png) bij de bovenkant van de lijst.

   ![ herberekenen uitdrukkingen chronologie met financiën drop-down ](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Afhankelijk van de complexiteit van uw projecten raden we u aan geen groot aantal projecten te selecteren wanneer u de tijdlijnen van de projecten bulksgewijs herberekent voor optimale prestaties. Sommige dingen die een project te complex zouden kunnen maken zouden veelvoudige gebiedsdelen of taken, of een groot aantal douanevelden kunnen zijn.

1. Klik **opnieuw berekenen Chronologie**. De tijdlijn wordt opnieuw berekend en er verschijnt een succesbericht op het scherm.

   >[!TIP]
   >
   >Voordat de tijdlijnherberekening is voltooid, worden sommige geplande of geprojecteerde datums mogelijk grijs weergegeven. Dit betekent dat de herberekening nog niet is voltooid en dat de data kunnen worden gewijzigd.

### Tijdlijnen in grote hoeveelheden handmatig opnieuw berekenen in het vak Projecten bewerken {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

U kunt de tijdlijnen van verschillende projecten handmatig opnieuw berekenen door ze bulksgewijs te bewerken.

>[!TIP]
>
>Afhankelijk van de complexiteit van uw projecten raden we u aan om geen groot aantal projecten te selecteren wanneer u deze in bulk bewerkt, zodat u optimale prestaties krijgt. Sommige dingen die een project te complex zouden kunnen maken zouden veelvoudige gebiedsdelen of taken, of een groot aantal douanevelden kunnen zijn.

1. Ga naar een lijst met projecten.
1. Selecteer verscheidene projecten in de lijst, dan klik **uitgeven**.
1. Klik **Montages**, dan selecteren **Tijdlijnen** opnieuw berekenen.

1. Klik **sparen Veranderingen**.

### Tijdlijnen voor alle projecten in het systeem opnieuw berekenen (alleen voor Workfront-beheerders) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront-beheerders kunnen de tijdlijndiagnose opnieuw berekenen om alle tijdlijnen in het Workfront-systeem onmiddellijk opnieuw te berekenen. Hierdoor kunnen alle projectbeheerders de invloed van externe wijzigingen direct zien op zowel geplande als geplande data.

Voor meer informatie over het opnieuw berekenen van chronologie voor de volledige plaats van Workfront, zie de sectie opnieuw berekende chronologie voor de volledige instantie van Workfront in [ vormen chronologieherberekeningen voor projecten ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong> This is the default setting. The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.  <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong> The project timeline is updated only when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
