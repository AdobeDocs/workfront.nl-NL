---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Niveaubronnen in de [!UICONTROL Gantt Chart]
description: Als dezelfde bron aan twee verschillende taken is toegewezen, kunt u de tijdlijn van de taken aanpassen door de resources nivelleren te gebruiken, zodat deze niet tegelijkertijd plaatsvinden. Dit artikel biedt informatie over hoe u resources in de Gantt-grafiek kunt nivelleren.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Niveaubronnen in de [!UICONTROL Gantt Chart]

<!--Audited: 08/2025-->

U kunt resourcepniveling gebruiken om de tijdlijn van de taken aan te passen zodat deze niet tegelijkertijd plaatsvinden, voor het geval dezelfde bronnen tegelijkertijd aan meerdere taken worden toegewezen.

Het Niveau van uw middelen op een project heeft twee doeleinden:

* De overtoewijzing van tijd voor toegewezen personen automatisch aanpassen.
* Om automatisch een realistisch taakprogramma voor een project tot stand te brengen.

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
   <td role="rowheader">[!DNL Workfront] licentie</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL Edit] toegang tot projecten</p></td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project</p>
</td> 
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
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects</p> <p><b>NOTE</b>

If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Overzicht van het Niveaus van Middelen

Als dezelfde bron aan twee verschillende taken is toegewezen, kunt u de tijdlijn van de taken aanpassen door de resources nivelleren te gebruiken, zodat deze niet tegelijkertijd plaatsvinden.

Overweeg het volgende wanneer het nivelleren van middelen op een project:

* Bronniveau is alleen van toepassing op één project, zodat bronnen in [!DNL Adobe Workfront] niet in meerdere projecten tegelijk op dezelfde hoogte worden gehouden.
* Als **[!UICONTROL Effort Driven]** is geselecteerd als een **[!UICONTROL Duration Type]** , zal [!DNL Workfront] de bronnen niet nivelleren.
* Wanneer meerdere gebruikers aan dezelfde taak zijn toegewezen, wordt nivelleren geannuleerd.
* Voorwaarden voor het type **[!UICONTROL Task Constraint]** hebben voorrang op het niveau van bronnen. Als **[!UICONTROL Fixed Dates]** bijvoorbeeld is geselecteerd als de [!UICONTROL Task Constraint] , worden de taakdatums niet gewijzigd door middel van nivelleren.
* Eerdere relaties hebben voorrang op bronnenniveau.
* **[!UICONTROL Resource Leveling]** moet voor het project worden ingesteld op **[!UICONTROL Manual]** om het niveau in de [!UICONTROL Gantt chart] aan te passen. Als u beheerdersmachtigingen voor het project hebt, kunt u ervoor zorgen dat het systeem bronnen automatisch op niveau brengt door deze instelling aan te passen op het project en **[!UICONTROL Automatic]** te selecteren in plaats van **[!UICONTROL Manual]** in het vak **[!UICONTROL Edit Project]** .

  ![&#x200B; het niveauwijze van het Middel &#x200B;](assets/resource-leveling-mode-350x177.png)

* Als projecteigenaar, of de taak toegewezen, kunt u een nivellerende vertraging voor een taak introduceren om erop te wijzen dat er een grote kans is dat de taak extra tijd zou kunnen vereisen. Voor informatie over het toevoegen van een nivellerende vertraging aan een taak, zie [&#x200B; de taak Levende Vertraging van de Update &#x200B;](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Bronniveaus toepassen in de [!UICONTROL Gantt Chart]

U kunt de Taaklijst [!UICONTROL Gantt Chart] gebruiken om uw middelen te nivelleren.

1. Ga naar het project u wilt vlakken.
1. Klik in het gebied **[!UICONTROL Tasks]** op het pictogram **[!UICONTROL Gantt chart]** .

   Alle wijzigingen worden automatisch opgeslagen wanneer de optie **[!UICONTROL Autosave]** is ingeschakeld. Deze optie is standaard ingeschakeld.

1. (Optioneel) Klik op het pictogram **[!UICONTROL Plan]mode** en selecteer **[!UICONTROL Manual save Standard]** of **[!UICONTROL Timeline Planning]** om de wijzigingen handmatig op te slaan.

   >[!TIP]
   >
   >U kunt resources niet in de [!UICONTROL Gantt Chart] nivelleren wanneer de optie [!UICONTROL Autosave] is ingeschakeld.

   ![&#x200B; Toegelaten het Handmatig plaatsen &#x200B;](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klik op de vervolgkeuzelijst **[!UICONTROL Level Resources]** .

   ![&#x200B; Level_resources.png &#x200B;](assets/level-resouces.png)

1. Selecteer een van de volgende opties:

   * **[!UICONTROL Level Now]**: past middelniveau op de geselecteerde taak toe.
   * **[!UICONTROL Clear Leveling]**: hiermee verwijdert u alle bronniveaus van de geselecteerde taak.

   >[!NOTE]
   >
   >Uw middelen zouden kunnen worden oververdeeld als zij aan veelvoudige taken worden toegewezen die tijdens het zelfde tijdkader voorkomen.

1. (Optioneel en voorwaardelijk) Als u de optie Automatisch opslaan hebt uitgeschakeld, klikt u op het pictogram **[!UICONTROL Undo]** of **[!UICONTROL Redo]** als u een van de wijzigingen wilt annuleren of dupliceren.

   >[!TIP]
   >
   >U kunt de volgende sneltoetsen gebruiken om wijzigingen in de [!UICONTROL Gantt Chart] ongedaan te maken of opnieuw uit te voeren:
   >
   >* [!DNL Mac]: gebruik [!UICONTROL Command + Z] om ongedaan te maken en [!UICONTROL Command + Shift + Z] om opnieuw uit te voeren.
   >* Windows: gebruik [!UICONTROL Ctrl + Z] om ongedaan te maken en [!UICONTROL Ctrl + Y] om opnieuw uit te voeren.


1. Klik op **[!UICONTROL Save]** in de rechterbovenhoek van [!UICONTROL Gantt chart] .

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
