---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configureer hoe informatie wordt weergegeven op het tabblad [!UICONTROL Gantt] Diagram
description: U kunt vormen welke informatie in zowel de Grafiek van Gantt van de Lijst van de Taak als de Grafiek van Gantt van de Lijst van het Project toont.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# Configureer hoe informatie wordt weergegeven op het tabblad [!UICONTROL Gantt Chart]

U kunt vormen welke informatie in beide Lijst van de Taak toont [!UICONTROL Gantt Chart] en de projectlijst [!UICONTROL Gantt Chart].

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel te volgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten en Taken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] of een betere toegang tot het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Weergaveopties begrijpen

In de volgende tabel worden de weergaveopties voor de [!UICONTROL Gantt chart]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actual Dates]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Actual Start Date] en [!UICONTROL Actual Completion Date] worden weergegeven met een driehoekje. Als de [!UICONTROL Actual Completion Date] is null, alleen de [!UICONTROL Actual Start Date] wordt weergegeven.</p> <p>Voor meer informatie over begin- en einddatums raadpleegt u <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overzicht van het project [!UICONTROL Actual Completion Date] </a> en <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overzicht van het project [!UICONTROL Actual Start Date] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="toewijzingen_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Hiermee geeft u taaktoewijzingen weer. Muis over de <strong>[!UICONTROL Details]</strong> link naast de naam van een toegewezen persoon om meer gedetailleerde informatie over de betrokkenen te zien, waaronder het percentage van hun toewijzing aan de taak.</p> <p>Toewijzingen worden niet weergegeven op de [!UICONTROL Gantt chart] wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF. Wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF, worden de toewijzingen alleen weergegeven in de takenlijst.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Een projectmomentopname die zeer belangrijke stukken van gegevens over het project inbegrepen in het aanvankelijke projectplan vertegenwoordigt. De basislijnen kunnen gedurende de gehele looptijd van het project worden genomen. Wanneer u basislijnen wilt weergeven in het dialoogvenster [!UICONTROL Gantt chart]selecteert u welke basislijn u wilt weergeven. U kunt slechts één basislijn weergeven op de [!UICONTROL Gantt chart] en wordt weergegeven in de vorm van een grijze balk.</p> <p>Zie voor meer informatie over basislijnen <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Projectbasislijnen maken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>De datum waarop een ontvanger zich ertoe verbindt wanneer de taak zal worden voltooid, wordt aangegeven met een markering in de [!UICONTROL Gantt chart]. </p> <p>Zie voor meer informatie over datums vastleggen <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date] overzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  Het percentage van de taak die wordt voltooid toont in de taaklijn.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critical Path]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>De taken die van invloed kunnen zijn op de tijdlijn van het project worden beschouwd als onderdeel van het kritieke pad en worden duidelijk rood gemarkeerd. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Ruiten</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Een ruitje wordt weergegeven na de taak die aan een mijlpaal is gekoppeld. Plaats de muis boven een mijlpaal om de naam en de datum van de mijlpaal te bekijken. De [!DNL Workfront] de beheerder bepaalt de kleur van elke milestone-ruit.</p> <p>Zie voor meer informatie over mijlpalen <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Een milestone-pad maken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Lijnen</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Een lijn toont na de taak die met een mijlpaal wordt geassocieerd. Plaats de muis boven een mijlpaal om de naam en de datum van de mijlpaal te bekijken. De [!DNL Workfront] de beheerder bepaalt de kleur van elke milestone-lijn.</p> <p> Zie voor meer informatie over mijlpalen  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Een milestone-pad maken</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessors]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Een lijn van één taak aan een andere die de voorgangersverhouding tussen de twee taken toont. Als u een afzonderlijke voorganger wilt markeren, plaatst u de muis erboven. Klik erop om het gemarkeerd te houden. U kunt slechts één voorganger per regel markeren.</p> <p>A <strong>[!UICONTROL Predecessor]</strong> het pictogram wordt getoond naast om het even welke taak die een voorgangersverhouding heeft die veelvoudige pagina's op de grafiek van Gantt of op om het even welke taak overspant die een dwars-projectvoorganger heeft.</p> <p>Klik op de knop <strong>[!UICONTROL Predecessor]</strong> pictogram om alle voorganger- en opvolgertaken weer te geven, evenals details over elke taak, zoals de naam van de taak, het type van de voorganger en de belangrijkste datums.</p> <p>Opmerking: De [!UICONTROL Gantt Chart] in een lijst van projecten toont informatie over dwars-project predecessors. Voor meer informatie over hoe te om voorgangersverhoudingen tussen verschillende projecten tot stand te brengen zie <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Predecessors voor meerdere projecten maken</a></p> <p>Voor meer informatie over predecessors raadpleegt u <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Voorgangers afdwingen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress Status]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__okt._2017.png"></p> <p>[!UICONTROL Behind]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind_okt._2017.png"></p> <p>[!UICONTROL At Risk]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Late        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>De status van de huidige voortgang van een bepaalde taak. </p> <p>Voor meer gedetailleerde informatie over elk [!UICONTROL Progress Status] tekst, zie <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Taak [!UICONTROL Progress Status] overzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projected Dates]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>De verwachte geprojecteerde tijdlijn die de [!UICONTROL Projected Start] en [!UICONTROL Completion dates] op basis van de voltooide werkzaamheden en het resterende werk. </p> <p>Zie voor meer informatie over de geplande afsluitdatums <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Overzicht van de [!UICONTROL Projected Completion Date] voor projecten, taken en kwesties</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Weergaveopties configureren

1. Ga naar de Taaklijst [!UICONTROL Gantt Chart] of de projectlijst [!UICONTROL Gantt Chart].\
   Voor meer informatie over waar [!UICONTROL Gantt chart] bevindt zich, zie [Aan de slag met de [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Optioneel) Selecteer de optie **[!UICONTROL Switch to Projected Dates]** instellen om de taken weer te geven op basis van [!UICONTROL Projected Dates]. Taken worden standaard weergegeven op basis van hun [!UICONTROL Planned Dates] in de [!UICONTROL Gantt chart].
1. Klik op het optiepictogram om het dialoogvenster **[!UICONTROL Options]** in.\
   ![Opties.png](assets/options-350x129.png)

1. Selecteer de configuratieopties die u wilt weergeven in het dialoogvenster [!UICONTROL Gantt chart].

   >[!NOTE]
   > Niet zijn alle configuratieopties beschikbaar in de Lijst van het Project [!UICONTROL Gantt Chart].

1. Klik ergens in het dialoogvenster [!UICONTROL Gantt chart] om de **[!UICONTROL Options]** in.
