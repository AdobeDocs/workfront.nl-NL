---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: De kaartlijst gebruiken
description: U kunt een kaartlijst op een werkstroom tot stand brengen en de kaarten toevoegen aan herhalingen.
author: Lisa
feature: Agile
source-git-commit: 8c02f5364154bdc343512416d0c7e38ef563a170
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# De kaartlijst gebruiken

U kunt een kaartlijst op een werkstroom tot stand brengen en de kaarten toevoegen aan herhalingen.

De kaartlijst kan als achterhoede werk voor de werkstroom functioneren.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

## Kaarten toevoegen aan de kaartlijst

{{step1-to-boards}}

1. Als u een werkstroom wilt openen, klikt u op [!UICONTROL **Werkstroom weergeven**].
1. Klik op de knop [!UICONTROL **Kaartlijst**] tab.
1. Klikken [!UICONTROL **Kaart toevoegen**].
1. In de [!UICONTROL **Kaart maken/bewerken**] voegt u de volgende informatie toe:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>De naam van de kaart.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>Een beschrijving van de kaart.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>Het geschatte aantal uren dat de kaart moet worden ingevuld. Dit is alleen een handmatige invoer.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Selecteer een status voor de kaart.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Selecteer een herhaling waaraan u de kaart wilt toewijzen.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>Als u de kaart wilt toewijzen, typt u een naam in het zoekveld en selecteert u de naam wanneer deze in de lijst wordt weergegeven. U kunt zowel personen als teams toevoegen en u kunt meerdere personen of teams toewijzen aan een kaart.</p><p>Toewijzingen moeten leden zijn in de werkstroom of worden niet weergegeven in de selectielijst.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Klikken [!UICONTROL **Opslaan**].
1. Ga door met het toevoegen van kaarten totdat u de kaartlijst hebt gemaakt.

## Kaarten weergeven

Als u alle kaarten voor de werkstroom in één lijst wilt weergeven, klikt u op [!UICONTROL **Lijstweergave**] op het tabblad Kaartlijst.

Klik op [!UICONTROL **Weergave herhaling**]. Niet-geplande kaarten worden in hun eigen groep weergegeven.

Als u een bestaande kaart wilt bewerken, selecteert u deze in de lijst en klikt u op [!UICONTROL **Bewerken**].

Als u een kaart wilt verwijderen, selecteert u deze in de lijst en klikt u op [!UICONTROL **Verwijderen**].

### Filterkaarten

Kaarten kunnen alleen worden gearchiveerd vanaf het iteratiebord. Wanneer een kaart wordt gearchiveerd, wordt deze niet weergegeven in de kaartlijst, tenzij u filtert om gearchiveerde kaarten weer te geven. Voor informatie over het archiveren van een kaart raadpleegt u [Een kaart van een kaart verwijderen of archiveren](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Open de kaartlijst voor de werkstroom.
1. Klikken [!UICONTROL **Filter**] en selecteert u [!UICONTROL **Alles**], [!UICONTROL **Actieve kaarten**], of [!UICONTROL **Gearchiveerde kaarten**].

   Wanneer een ander filter dan het gebrek op de kaartlijst wordt toegepast, wordt een indicator getoond op het filterpictogram ![Toegepast filter](assets/boards-filterapplied-30x30.png).

### Zoeken in de kaartlijst

1. Open de kaartlijst voor de werkstroom.
1. Klikken [!UICONTROL **Zoeken**] en typ een zoekterm. Druk vervolgens op Enter.

   Alle kaarten die de zoekterm bevatten, worden weergegeven.
Klik op de X om de zoekopdracht te wissen.

   ![Kaarten in een kaart zoeken](assets/boards-searchbox.png)

## Kaarten aan een herhaling toevoegen

>[!NOTE]
>
>U moet een herhaling maken voordat u er kaarten aan kunt toevoegen. Zie voor meer informatie [Een herhaling in een werkstroom maken](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Open de kaartlijst voor de werkstroom.
1. Selecteer [!UICONTROL **Weergave herhaling**] om te zien welke kaarten aan een herhaling worden toegewezen en welke niet gepland zijn.
1. Selecteer een ongeplande kaart in de lijst en klik op [!UICONTROL **Bewerken**].
1. Selecteer een herhaling in het dialoogvenster [!UICONTROL **Herhalingen**] veld.
1. Als u artikelpunten gebruikt, voert u een waarde in het dialoogvenster [!UICONTROL **Schatting**] veld.
1. Klikken [!UICONTROL **Opslaan**].

   De kaart wordt verplaatst naar de iteratie en de iteratiemetriek geeft het aantal kaarten en punten aan.

   U kunt een kaart ook slepen en neerzetten vanuit de groep Niet-geplande kaarten naar de herhaling of op [!UICONTROL **Kaart toevoegen**] om een nieuwe kaart aan de iteratie toe te voegen.

>[!TIP]
>
>Als u een herhalingsprocesboard hebt gemaakt, worden alle ongeplande kaarten in de kaartlijst weergegeven in [!UICONTROL Backlog] kolom. Wanneer een kaart naar een andere kolom wordt verplaatst, wordt deze onderdeel van de actieve herhaling. Kaarten die u toevoegt aan de iteratie in de kaartlijst, worden op basis van hun status toegevoegd aan een kolom.

