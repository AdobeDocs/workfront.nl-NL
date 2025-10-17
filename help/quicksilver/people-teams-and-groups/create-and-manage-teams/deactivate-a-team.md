---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Een team deactiveren of verwijderen
description: U kunt teams deactiveren die u niet meer gebruikt, terwijl de bijbehorende historische gegevens behouden blijven. Adobe Workfront-beheerders kunnen een team op elk gewenst moment vanuit het gedeelte Teams in Setup opnieuw activeren.
author: Jenny
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Een team deactiveren of verwijderen

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

Gedetactiveerde teams worden niet weergegeven wanneer u naar een team zoekt, maar worden wel weergegeven in [!UICONTROL Home Team] en Overige teams als de gebruiker aan het team was toegewezen voordat het team werd gedeactiveerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-pakket</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr>
   <td>Configuraties op toegangsniveau</td>
   <td><p>Voor het deactiveren van een team zijn geen configuraties vereist.</p>
   <p>Om een team te schrappen, moet u een beheerder van het Systeem zijn.</p></td>
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een team deactiveren

Alle werk dat voorafgaand aan deactivering aan het team is toegewezen, blijft toegewezen. We raden u aan het werk opnieuw toe te wijzen voordat u het team deactiveert.

>[!TIP]
>
>U kunt een rapport maken om te filteren op taken of problemen waarvoor het gedeactiveerde team nog steeds is toegewezen.

Wanneer het gebruiken van verzoekrijen, als u een team deactiveert dat als standaardteam in een verpletterende regel wordt toegewezen, blijft het team en de verzoeken nog verpletterd aan het gedeactiveerde team. Wij adviseren het bijwerken verpletterend regels met actieve teams alvorens u het team deactiveert.

{{step1-to-team}}

1. Klik op het pictogram **[!DNL Switch team]** en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   ![](assets/edit-team-settings.png)

1. Schakel het selectievakje **[!UICONTROL Is Active]** uit in de teaminstellingen.
1. Klik op **[!UICONTROL Save changes]**.

## Bekende beperkingen om een team te deactiveren

Gedetactiveerde teams worden weergegeven in de volgende gebieden:

* Het veld Eigenaar in [!DNL Workfront Goals] . Hiervoor is een extra licentie vereist voor [!DNL Adobe Workfront Goals] . Voor meer informatie, zie [&#x200B; begonnen worden met  [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Een team verwijderen

Alleen een systeembeheerder kan een team verwijderen. Als u een teameigenaar bent (maar geen beheerder) en u probeert om een team te schrappen, zult u een foutenmelding zien.

Een team verwijderen:

{{step1-to-team}}

1. Klik op het pictogram **[!DNL Switch team]** en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Delete]** .

   ![](assets/edit-team-settings.png)

1. Klik [!UICONTROL **bevestigen**] op het bevestigingsbericht om het team permanent te schrappen. Verwijderde teams kunnen niet worden hersteld.
