---
product-area: projects
navigation-topic: manage-tasks
title: Overzicht van het Opslaan van Gelijktijdige Veranderingen binnen een Lijst van de Taak
description: Wanneer u taken in een lijst bewerkt, kunt u afzonderlijke opslaginstellingen gebruiken om aan te geven of de wijzigingen automatisch moeten worden opgeslagen wanneer u taken in een lijst bewerkt.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Overzicht van het opslaan van gelijktijdige wijzigingen in een takenlijst

Wanneer u taken in een lijst bewerkt, kunt u afzonderlijke opslaginstellingen gebruiken om aan te geven of de wijzigingen automatisch moeten worden opgeslagen wanneer u taken in een lijst bewerkt.

Voor informatie over het uitgeven van taken in een taaklijst, zie het artikel [&#x200B; taken in een lijst &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) uitgeven.

Soms kunnen conflicten optreden als twee gebruikers wijzigingen aanbrengen in dezelfde taken.

Houd rekening met het volgende wanneer u taken in een takenlijst bewerkt:

* Adobe Workfront slaat de wijzigingen die u aanbrengt in taken direct op wanneer u ervoor kiest om uw wijzigingen automatisch op te slaan als het type projectupdate Automatisch of Automatisch of bij Wijzigen is. Voor informatie over het Type van projectupdate, zie [&#x200B; het Type van projectupdate &#x200B;](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.
* Workfront werkt de informatie op de lijst bij u aan elke minuut met veranderingen werkt die andere gebruikers overal anders in het systeem zouden kunnen aanbrengen. Dit zorgt ervoor dat u altijd de recentste informatie over de taken krijgt.

De volgende scenario&#39;s bestaan wanneer de veelvoudige gebruikers de zelfde taken uitgeven:

* **één gebruiker bewaart automatisch de veranderingen in een taaklijst en een andere manueel**: Als een gebruiker (Gebruiker A) veranderingen manueel opslaat terwijl Gebruiker B de zelfde taken uitgeeft maar zij sparen hun veranderingen automatisch, worden de levende veranderingen die door Gebruiker B worden aangebracht bijgewerkt op de lijst voor Gebruiker A elke minuut. Als er conflicten zijn tussen de wijzigingen die door de twee gebruikers zijn aangebracht, wordt voor het handmatig opslaan van de gebruiker (gebruiker A) een waarschuwingsbericht weergegeven voordat de gebruikers hun wijzigingen kunnen opslaan. Het waarschuwingsbericht geeft de items weer die conflicterende wijzigingen hebben. Op dit ogenblik, kan Gebruiker A verkiezen of zij hun veranderingen zouden moeten houden (die de veranderingen door Gebruiker B worden aangebracht) overschrijft, of hen verwerpen (die de veranderingen houdt die door Gebruiker B worden aangebracht).

>[!NOTE]
>
>Wanneer u ervoor kiest om de aangebrachte wijzigingen te verwijderen, geldt dit voor alle wijzigingen en niet alleen voor wijzigingen die een conflict hebben met de bewerkingen die door een andere gebruiker zijn aangebracht.

* **Verscheidene gebruikers bewaren manueel de veranderingen in een taaklijst**: Als verscheidene gebruikers die veranderingen in taken in een lijst aanbrengen manueel tezelfdertijd sparen, slaat Workfront de veranderingen op die door de gebruiker worden aangebracht die eerst bewaart. Als u deze wijzigingen opslaat, treden er geen conflicten op. Workfrontthen vergelijkt de veranderingen die door alle andere gebruikers met de informatie worden aangebracht die het reeds bewaarde en toont een waarschuwing over de conflicterende veranderingen aan de andere gebruikers alvorens zij hun informatie kunnen bewaren.

>[!IMPORTANT]
>
>Wanneer u ervoor kiest om uw wijzigingen bij alle andere wijzigingen te houden, worden alle wijzigingen opgeslagen, tenzij de taken waarvoor u wijzigingen hebt aangebracht, door een andere gebruiker zijn verwijderd. In dit geval wordt u via het waarschuwingsbericht geïnformeerd dat de wijzigingen die u hebt aangebracht in de verwijderde taken, verloren gaan.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
