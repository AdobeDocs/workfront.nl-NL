---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Vorm hoe de Informatie op de [!UICONTROL Gantt] Grafiek toont
description: U kunt vormen welke informatie in zowel de Grafiek van Gantt van de Lijst van de Taak als de Grafiek van Gantt van de Lijst van het Project toont.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Configureer hoe informatie wordt weergegeven op de [!UICONTROL Gantt Chart]

<!-- Audited: 5/2025 -->

U kunt vormen welke informatie in zowel de Grafiek van Gantt van de Lijst van de Taak als Grafiek van Gantt van de Lijst van het Project toont.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> 
   <p>[!UICONTROL Light] of hoger<p>
   <p>[!UICONTROL Review] of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten en Taken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] of een betere toegang tot het project en de taken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Light<p>
   <p>Or</p>
   <p>Current: Review</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Weergaveopties begrijpen

In de volgende tabel worden de weergaveopties voor de [!UICONTROL Gantt chart] weergegeven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Werkelijke datums</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Actual Start Date] en [!UICONTROL Actual Completion Date] worden weergegeven met een driehoekje. Als de waarde van [!UICONTROL Actual Completion Date] null is, wordt alleen de waarde van [!UICONTROL Actual Start Date] weergegeven.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref"> Overzicht van het project [!UICONTROL Actual Completion Date] </a> en <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref"> Overzicht van het project [!UICONTROL Actual Start Date] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="toewijzingen_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Hiermee geeft u taaktoewijzingen weer. Houd de link Details naast de naam van de ontvanger aan om meer gedetailleerde informatie over de gegevens te zien, waaronder het percentage van hun toewijzing aan de taak.</p> <p>Toewijzingen worden niet weergegeven op de [!UICONTROL Gantt chart] wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF. Wanneer de [!UICONTROL Gantt chart] naar PDF wordt geëxporteerd, worden de toewijzingen alleen weergegeven in de takenlijst.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Een projectmomentopname die zeer belangrijke stukken van gegevens over het project inbegrepen in het aanvankelijke projectplan vertegenwoordigt. De basislijnen kunnen door de chronologie van het project worden genomen. Wanneer u de optie inschakelt om basislijnen weer te geven in de [!UICONTROL Gantt chart] , selecteert u welke basislijn u wilt weergeven. U kunt slechts één basislijn tegelijk weergeven op de [!UICONTROL Gantt chart] en deze wordt weergegeven in de vorm van een grijze balk.</p> <p>Voor meer informatie over basislijnen, zie <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref"> projectbasislijnen </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>De datum die een ontvanger opgeeft als zijn verplichting om te bepalen wanneer de taak wordt voltooid, wordt weergegeven met een markering in de [!UICONTROL Gantt chart] . </p> <p>Zie <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date] overview </a> voor meer informatie over datums vastleggen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  Het percentage van de taak die wordt voltooid toont in de taaklijn.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critical Path]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>De taken die de tijdslijn van het project zouden kunnen beïnvloeden worden beschouwd als deel van de Kritieke Weg en duidelijk duidelijk in rood gemerkt. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Ruiten</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Een ruitje wordt weergegeven na de taak die aan een mijlpaal is gekoppeld. Houd een mijlpaal boven om de naam en de datum van de mijlpaal te bekijken. De beheerder [!DNL Workfront] bepaalt de kleur van elke milestone-ruitje.</p> <p>Voor meer informatie over mijlpalen, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref"> een milestone weg </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Lijnen</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Een lijn wordt weergegeven na de taak die aan een mijlpaal is gekoppeld. Houd een mijlpaal boven om de naam en de datum van de mijlpaal te bekijken. De beheerder [!DNL Workfront] bepaalt de kleur van elke milestone-lijn.</p> <p> Zie voor meer informatie over mijlpalen  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref"> creeer een milestone weg </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessors]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Een lijn van één taak aan een andere die de voorgangersverhouding tussen de twee taken toont. Houd de muisaanwijzer boven een afzonderlijke voorganger om deze te markeren. Klik erop om het gemarkeerd te houden. U kunt slechts één voorganger per regel markeren.</p> <p>Er wordt een pictogram [!UICONTROL Predecessor] weergegeven naast elke taak die een eerdere relatie heeft die meerdere pagina's beslaat op de Gantt-grafiek of op elke taak die een voorganger voor meerdere projecten heeft.</p> <p>Klik op het pictogram [!UICONTROL Predecessor] om alle voorgangers- en opvolgertaken en hun details weer te geven, zoals de naam van de taak, het type van de voorganger en de belangrijkste datums.</p> <p>Opmerking: [!UICONTROL Gantt Chart] in een lijst met projecten bevat informatie over voordecessors voor meerdere projecten. Voor meer informatie over hoe te om voorgangersverhoudingen tussen verschillende projecten tot stand te brengen zie <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref"> dwars-project voorgangers </a> creëren</p> <p>Voor meer informatie over predecessors, zie <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref"> predecessors </a> afdwingen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress Status]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__okt._2017.png"></p> <p>[!UICONTROL Behind]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind_okt._2017.png"></p> <p>[!UICONTROL At Risk]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Late        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>De status van de huidige voortgang van een bepaalde taak. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref"> overzicht van de Taak 0&rbrace; [!UICONTROL Progress Status].</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Geprojecteerde datums</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>De verwachte tijdlijn die de geplande begin- en einddatum markeert, gebaseerd op de voltooide werkzaamheden en het resterende werk. </p> <p>Voor meer informatie over voorgenomen voltooiingsdata, zie <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref"> Overzicht van de Verwachte Datum van de Voltooiing voor projecten, taken, en kwesties </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Weergaveopties configureren

1. Ga naar de **Gantt Grafiek van de Lijst van de Taak** of de **Gantt Grafiek van de Lijst van het Project**.\
   Voor meer informatie over waar één van beide grafiek van Gantt wordt gevestigd, zie [&#x200B; begonnen worden met [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Facultatief) selecteer de **Schakelaar aan Geprojecteerde Datums** plaatsen om de taken door hun Geprojecteerde Datums te tonen. Taken worden standaard weergegeven op basis van de geplande datums.
1. Klik het **pictogram van Opties**. Het **de dialoogvakje van Opties** opent.\
   ![&#x200B; Options.png &#x200B;](assets/options-350x129.png)

1. Selecteer de configuratieopties die u in [!UICONTROL Gantt chart] wilt weergeven.

   >[!NOTE]
   >
   > Niet alle configuratieopties zijn beschikbaar in de Projectlijst [!UICONTROL Gantt Chart].

1. Klik overal in de grafiek van Gantt om het **de dialoogvakje van Opties** te sluiten.
