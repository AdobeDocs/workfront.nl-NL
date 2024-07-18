---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Een team deactiveren
description: U kunt teams deactiveren die u niet meer gebruikt, terwijl de bijbehorende historische gegevens behouden blijven. Adobe Workfront-beheerders kunnen een team op elk gewenst moment vanuit het gedeelte Teams in Setup opnieuw activeren.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Een team deactiveren

U kunt teams deactiveren die u niet meer gebruikt, terwijl de bijbehorende historische gegevens behouden blijven. [!DNL Adobe Workfront] beheerders kunnen een team op elk ogenblik van het gebied van Teams in Opstelling opnieuw activeren. Als u een team deactiveert, wordt het team niet meer weergegeven op de volgende gebieden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Typeahead-velden in aangepaste formulieren</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Dialoogvenster voor delen van objecten</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Hoofd keuzemenu van de selectie in het gebied [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Assignments] typeahead</p> </li> 
     <li> <p>[!UICONTROL Add to Kanban] de dialoog van de raad in een project</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

De gedeactiveerde teams verschijnen niet wanneer u naar een team zoekt, maar zullen nog in [!UICONTROL Home Team] en Andere Teams tonen als de gebruiker aan het team voorafgaand aan deactivatie werd toegewezen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan of vergunningstype u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een team deactiveren

Alle werk dat voorafgaand aan deactivering aan het team is toegewezen, blijft toegewezen. We raden u aan het werk opnieuw toe te wijzen voordat u het team deactiveert.

>[!TIP]
>
>U kunt een rapport maken om te filteren op taken of problemen waarvoor het gedeactiveerde team nog steeds is toegewezen.

Wanneer het gebruiken van verzoekrijen, als u een team deactiveert dat als standaardteam in een verpletterende regel wordt toegewezen, blijft het team en de verzoeken nog verpletterd aan het gedeactiveerde team. Wij adviseren het bijwerken verpletterend regels met actieve teams alvorens u het team deactiveert.

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront en klik vervolgens op **[!UICONTROL Teams]** .
1. Klik op het pictogram **[!DNL Switch team]** en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   ![](assets/edit-team-settings-350x205.png)

1. Schakel het selectievakje **[!UICONTROL Is Active]** uit.
1. Klik op **[!UICONTROL Save changes]**.

## Bekende beperkingen

Gedetactiveerde teams worden weergegeven in de volgende gebieden:

* Het veld Eigenaar in [!DNL Workfront Goals] . Hiervoor is een extra licentie vereist voor [!DNL Adobe Workfront Goals] . Voor meer informatie, zie [ begonnen worden met  [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
