---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Informatie bijwerken in de Gantt-grafiek van de takenlijst
description: De van de taaklijst Gantt- Grafiek toont details over taken die op een project of een malplaatje zijn.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# Gegevens in de takenlijst bijwerken [!UICONTROL Gantt Chart]

De takenlijst [!UICONTROL Gantt Chart] toont details over taken die op een project of een malplaatje zijn.

In een malplaatje, de taaklijst [!UICONTROL Gantt Chart] weerspiegelt updates die in de de taaklijst van het malplaatje op het taakniveau worden gemaakt. U kunt de [!UICONTROL Gantt chart] gekoppeld aan een sjabloon.

In een project kunt u taakinformatie rechtstreeks in de takenlijst bijwerken [!UICONTROL Gantt Chart].

Dit artikel beschrijft de volgende acties die u direct in de Lijst van de Taak kunt uitvoeren [!UICONTROL Gantt Chart]:

* Taakduur wijzigen
* Vorige relaties maken of verwijderen
* Start- en einddatum van taak wijzigen
* Percentage bijwerken voltooid
* Niveau-projectbronnen

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
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>[!UICONTROL Edit] toegang tot projecten en taken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project en de taken </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Taakduur wijzigen

1. Ga naar het project u wilt wijzigen.
1. Klikken **[!UICONTROL Tasks]** in het linkerdeelvenster.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Klik op de knop **[!UICONTROL Gantt chart]** pictogram.

   ![Klik op het pictogram Gantt-diagram](assets/click-gantt-chart-icon.png)

   Alle wijzigingen worden automatisch opgeslagen wanneer de **[!UICONTROL Autosave]** is ingeschakeld. Deze optie is standaard ingeschakeld.

1. (Optioneel) Klik op de knop **[!UICONTROL Plan mode]** pictogram en selecteer **[!UICONTROL Manual save Standard]** of **[!UICONTROL Timeline Planning]** om uw wijzigingen handmatig op te slaan.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Houd de cursor boven de tijdlijn van een taak en sleep de tijdlijnindicator naar een andere datum.
1. Zet de indicator neer wanneer u de correcte nieuwe Datum van Voltooiing voor de taak hebt bereikt.
1. (Optioneel en voorwaardelijk) Als u de optie hebt geselecteerd om uw wijzigingen handmatig op te slaan, klikt u op de knop **[!UICONTROL Undo]** of &#x200B;**[!UICONTROL Redo]** als u een van de wijzigingen wilt annuleren of dupliceren.

   >[!TIP]
   >
   >U kunt de volgende sneltoetsen gebruiken om wijzigingen in het Gantt-diagram ongedaan te maken of opnieuw uit te voeren:
   >
   >   
   >   
   >   * [!DNL Mac]: Gebruiken [!UICONTROL Command + Z] om ongedaan te maken en [!UICONTROL Command + Shift + Z] om opnieuw uit te voeren.
   >   * [!DNL Windows]: Gebruiken [!UICONTROL Ctrl + Z] om ongedaan te maken en [!UICONTROL Ctrl + Y] om opnieuw uit te voeren.
   >   
   >

1. Klikken **[!UICONTROL Save]** in de rechterbovenhoek van het dialoogvenster [!UICONTROL Gantt chart].

## Vorige relaties maken of verwijderen

1. Ga naar het project u wilt wijzigen.
1. In de **[!UICONTROL Tasks]** gebied, klikt u op **[!UICONTROL Gantt chart]** pictogram.

   De **[!UICONTROL Autosave]** Deze optie is standaard geselecteerd. In dat geval worden alle wijzigingen automatisch opgeslagen.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Optioneel) Klik op de knop **[!UICONTROL Plan mode]** pictogram en selecteer **[!UICONTROL Manual save Standard]** of **[!UICONTROL Timeline Planning]** om uw wijzigingen handmatig op te slaan.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Als u een voorgaande relatie wilt maken, klikt u op het beginpunt van een taak en sleept u deze naar het eindpunt van de taak.
1. Als u een voorgaande relatie wilt verwijderen, klikt u op een voorgangerlijn die twee taken met elkaar verbindt om deze te selecteren en drukt u vervolgens op **[!UICONTROL Delete]** op uw toetsenbord.\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Optioneel en voorwaardelijk) Als u de wijzigingen handmatig wilt opslaan, klikt u op de knop **[!UICONTROL Undo]** of &#x200B;**[!UICONTROL Redo]** als u een van de wijzigingen wilt annuleren of dupliceren.

   >[!TIP]
   >
   >U kunt de volgende sneltoetsen gebruiken om wijzigingen in het Gantt-diagram ongedaan te maken of opnieuw uit te voeren:
   >
   >   
   >   
   >   * [!DNL Mac]: Gebruiken [!UICONTROL Command + Z] om ongedaan te maken en [!UICONTROL Command + Shift + Z] om opnieuw uit te voeren.
   >   * [!DNL Windows]: [!UICONTROL Use Ctrl + Z] om ongedaan te maken en [!UICONTROL Ctrl + Y] om opnieuw uit te voeren.
   >   
   >

1. Klik op **[!UICONTROL Save]** .

## Start- en einddatum van taak wijzigen

1. Ga naar het project u wilt wijzigen.
1. In de **[!UICONTROL Tasks]** gebied, klikt u op **[!UICONTROL Gantt chart]** pictogram.

   Alle wijzigingen worden automatisch opgeslagen wanneer de **[!UICONTROL Autosave]** is ingeschakeld. Deze optie is standaard ingeschakeld.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Optioneel) Klik op de knop **[!UICONTROL Plan mode]** pictogram en selecteer **[!UICONTROL Manual save Standard]** of **[!UICONTROL Timeline Planning]** om uw wijzigingen handmatig op te slaan.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Houd de muisaanwijzer boven het midden van de taak en zoek de pijl met meerdere richtingen.
1. Klik en sleep de taak naar de gewenste datum.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. Als u de taakdatum wijzigt op een manier die invloed heeft op de taakbeperking, klikt u op **[!UICONTROL Accept]** om de verandering van de taakbeperking te erkennen.

   >[!NOTE]
   >
   >Als de taak een van de volgende beperkingen heeft, werkt het systeem de [!UICONTROL Task Constraint] tot [!UICONTROL Start No Earlier] Dan als het project van gepland is [!UICONTROL Start Date] of [!UICONTROL Finish No Later Than] als het project gepland is vanuit de [!UICONTROL Completion Date]:
   >
   >   
   >   
   >   * [!UICONTROL As Soon As Possible]
   >   * [!UICONTROL As Late As Possible]
   >   * [!UICONTROL Earliest Available Time]
   >   * [!UICONTROL Latest Available Time]
   >   
   >   
   >In sommige gevallen, zouden de voorgangersverhoudingen de taken kunnen verhinderen vroeger te beginnen, en de taakbeweging wordt niet toegestaan.

1. (Optioneel en voorwaardelijk) Als u de wijzigingen handmatig wilt opslaan, klikt u op de knop **[!UICONTROL Undo]** of &#x200B;**[!UICONTROL Redo]** als u een van de wijzigingen wilt annuleren of dupliceren.

   >[!TIP]
   >
   >U kunt de volgende sneltoetsen gebruiken om wijzigingen in het dialoogvenster [!UICONTROL Gantt chart]:
   >
   >   
   >   
   >   * [!DNL Mac]: Gebruiken [!UICONTROL Command + Z] om ongedaan te maken en [!UICONTROL Command + Shift + Z] om opnieuw uit te voeren.
   >   * [!DNL Windows]: Gebruiken [!UICONTROL Ctrl + Z] om ongedaan te maken en [!UICONTROL Ctrl + Y] om opnieuw uit te voeren.
   >   
   >

1. Klik op **[!UICONTROL Save]**.

## Percentage bijwerken voltooid

1. Ga naar het project u wilt wijzigen.
1. In de **[!UICONTROL Tasks]** gebied, klikt u op **[!UICONTROL Gantt chart]** pictogram.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   Alle wijzigingen worden automatisch opgeslagen wanneer de **[!UICONTROL Autosave]** is ingeschakeld. Deze optie is standaard ingeschakeld.

1. (Optioneel) Klik op de knop **[!UICONTROL Plan mode]** pictogram en selecteer **[!UICONTROL Manual save Standard]** of **[!UICONTROL Timeline Planning]** om uw wijzigingen handmatig op te slaan.
1. Dubbelklik op het percentagenummer in de taak en voer het getal in.

   >[!IMPORTANT]
   >
   >U moet [!UICONTROL % Complete] geselecteerd in het dialoogvenster [!UICONTROL Options] om het volledige percentage bij te werken. Om dit te doen, klik **[!UICONTROL Options]** pictogram en selecteer **[!UICONTROL % Complete]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Optioneel en voorwaardelijk) Als u de wijzigingen handmatig wilt opslaan, klikt u op de knop **[!UICONTROL Undo]** of &#x200B;**[!UICONTROL Redo]** als u een van de wijzigingen wilt annuleren of dupliceren.

   >[!TIP]
   >
   >U kunt de volgende sneltoetsen gebruiken om wijzigingen in het dialoogvenster [!UICONTROL Gantt chart]:
   >
   >   
   >   
   >   * [!DNL Mac]: Gebruiken [!UICONTROL Command + Z] om ongedaan te maken en [!UICONTROL Command + Shift + Z] om opnieuw uit te voeren.
   >   * [!DNL Windows]: Gebruiken [!UICONTROL Ctrl + Z] om ongedaan te maken en [!UICONTROL Ctrl + Y] om opnieuw uit te voeren.
   >   
   >

1. Klikken **[!UICONTROL Save]** in de rechterbovenhoek van het dialoogvenster [!UICONTROL Gantt chart].

## Niveau-projectmiddelen

U kunt de Lijst van de Taak gebruiken [!UICONTROL Gantt Chart] om uw bronnen op peil te houden.

Voor informatie over het nivelleren van bronnen in de [!UICONTROL Gantt chart], zie [Niveau-bronnen in het dialoogvenster [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
