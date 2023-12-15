---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Kanban configureren
description: U maakt een Kanban- of Scrum agile-team in [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 0%

---

# Configureren [!UICONTROL Kanban]

U kunt een flexibel team maken in [!DNL Adobe Workfront] zoals beschreven in [Een bestandsteam maken](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Tijdens het creëren van een flexibel team kunt u de methodologie kiezen die het team gebruikt om hun werk te voltooien. U kunt uit de volgende opties kiezen:

* Schuiven
* Kanban

Dit artikel beschrijft hoe te om de montages voor een team te vormen Kanban. Nadat u een nieuw team hebt gemaakt en de Kanban-methode hebt gekozen, kunt u naar dit artikel verwijzen om de volgende instellingen bij te werken:

* Of artikelen worden geschat in punten of uren
* De statuskolommen op het &#39;agile story board&#39;
* Extra velden die op artikelkaarten op het karton voor een artikel worden weergegeven
* De limiet voor lopende werkzaamheden (WIP)
* Hoe te om verhalen van de achterstand automatisch toe te voegen
* Hoe lang kaarten op de Kanban-kaart blijven

Voor informatie over het vormen van een team van het Trommel, zie [Scrum configureren](../get-started-with-agile-in-workfront/configure-scrum.md).

## Toegangsvereisten

<!--Audited: 12/2023-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p> 
   of
   <p>Huidige: [!UICONTROL Work] of hoger</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>Toegang tot teams bewerken</p>  </td> 
  </tr>

</tbody> 
</table>

*Neem contact op met uw [!DNL Workfront] beheerder.

## Configureer of artikelen worden geschat in punten of uren

U kunt artikelen configureren om te worden geschat aan de hand van punten of uren.

Om te vormen hoe de verhalen voor uw agile team worden geschat:

{{step1-to-team}}

1. Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team in het zoekvak.
1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu ![](assets/more-menu.png) selecteert u vervolgens **[!UICONTROL Edit]**.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** in de **[!UICONTROL Estimate Stories in]** selecteert u of u punten of uren wilt gebruiken voor het schatten van de grootte (werkbelasting) van artikelen. Als u Punten selecteert, geeft u op hoeveel uren gelijk zijn aan 1 punt. (De standaardwaarde is 1 punt = 8 uur.) Dit is het aantal geplande uren dat aan het artikel wordt toegevoegd.

   **Voorbeeld:** Als u artikelen in punten en 1 punt wilt schatten, is dit gelijk aan 8 uur en een artikel wordt geschat op 3 punten, worden 24 geplande uren toegevoegd aan het artikel.

1. Klik op **[!UICONTROL Save Changes]**.

## Statuskolommen configureren op de whiteboardlijst voor bestanden

U kunt de statussen bepalen die op de verhaalraad voor het flexibele team bestaan. Dit zijn de enige statussen die op het artikelbord worden weergegeven.

U definieert de statussen die beschikbaar zijn voor de artikelkaart die is gekoppeld aan het mobiele team:

{{step1-to-team}}

1. Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![Pictogram Teams wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** de sectie te zoeken **[!UICONTROL Story Board]** gebied.

1. (Optioneel) Klik op **[!UICONTROL Add Column]** om een extra statuskolom toe te voegen aan het artikelbord.
1. (Optioneel) Sleep een statuskolom met de indicator voor slepen en neerzetten om de volgorde van de statuskolommen op het artikelbord te wijzigen. De eerste kolom kan niet worden verplaatst en u kunt geen andere kolom vóór de eerste kolom slepen.

   ![Slepen en slepen](assets/agile-story-card-drag-and-drop.png)

1. Selecteer taakstatussen.

   >[!IMPORTANT]
   >
   >Alleen vergrendelde statussen voor het hele systeem kunnen worden geselecteerd. U kunt geen groepsspecifieke statussen selecteren. De status van de eerste kolom komt altijd overeen met **[!UICONTROL New]**.

   U kunt aangepaste statussen toevoegen als uw [!DNL Workfront] de beheerder heeft hen gevormd. Zie voor meer informatie [Een status maken of bewerken](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klik op **[!UICONTROL Save Changes]**.

## Aanvullende velden configureren voor weergave op artikelkaarten op de kaart van het gegenereerde artikel

Wanneer u velden toevoegt aan artikelkaarten, zijn velden alleen-weergeven en alleen weergeven wanneer het veld is gevuld.

Standaard worden de volgende gegevenstypen op de artikelkaart weergegeven voor taken en uitgaven:

* Artikelnaam met een koppeling die rechtstreeks naar de taak of uitgave verwijst
* De projectnaam met een verbinding direct aan het project
* Deze koppeling wordt alleen weergegeven voor artikelen, niet voor subtaken
* De taak of uitgiftebeschrijving
* Huidige verplichting
* Het percentage voltooide bewerkingen weergeven en bewerken door het percentage aan te passen dat is voltooid of door het aantal punten of uren aan te passen
* Toegewezen gebruikers

U kunt aanvullende gegevens (inclusief aangepaste gegevens) weergeven op artikelkaarten. U wilt mogelijk om een aantal redenen extra velden weergeven op artikelkaarten. Bijvoorbeeld, zou u identiteitskaart van de Klant kunnen willen tonen als u aan verhalen voor veelvoudige klanten binnen de herhaling werkt, of u zou de Datum van het Begin van het Project of de Datum van de Voltooiing van het Project kunnen willen tonen.

>[!NOTE]
>
>Als u een aangepast veld op een artikelkaart gebruikt, kan dit geen punt (punt) in de naam bevatten.

U kunt als volgt artikelkaarten configureren die aan het mobiele team zijn toegewezen om extra velden weer te geven:

{{step1-to-team}}

1. Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![Pictogram Teams wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** -sectie, typt u een veldnaam om deze te zoeken.

   ![Aanvullende velden](assets/agile-additional-fields-kanban.png)

1. Selecteer de naam van het veld dat u wilt toevoegen.
1. Typ de **[!UICONTROL Display name]** voor het veld dat wordt weergegeven op het artikel of de uitgiftekaart.
1. Klik op **[!UICONTROL Save Changes]**.

## De WIP-limiet (werk in uitvoering) configureren

Wanneer u de grens van het WIP van een team van Kanban bepaalt, kunt u het aantal punten controleren het team momenteel werkt door het aantal taken te beperken die in kunnen verschijnen [!UICONTROL New] of de [!UICONTROL In Progress] kolom op de [!UICONTROL Kanban] bord.

Nadat u de grens van het WIP voor een team Kanban vormt, kunt u de grens van het WIP bekijken en het van bijwerken [!UICONTROL Kanban] agile story board, zoals beschreven in [De WIP-limiet (work in progress) beheren voor de [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Om WIP voor uw team van Kanban te beperken:

{{step1-to-team}}

1. Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![Pictogram Teams wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het Kanban-team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu ![](assets/more-menu.png)selecteert u vervolgens **[!UICONTROL Edit]**.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** in de **[!UICONTROL Methodology]** selecteert, zorgt u ervoor dat Kanban is geselecteerd.

1. In de **[!UICONTROL Story Board]** in de **[!UICONTROL WIP Limit]** veld, geeft u het maximum aantal items op dat in elke kolom van het [!UICONTROL Kanban] agile verhaalbord. U kunt voor elke kolom een andere limiet instellen. De maximumgrens u voor elke kolom kunt plaatsen is 100.\
   Als deze optie is ingesteld, verschijnt er een waarschuwingsbericht op de knop [!UICONTROL Kanban] Op elk gewenst moment wordt de limiet voor elke kolom op het artikelbord overschreden. Dit waarschuwingsbericht wordt alleen weergegeven wanneer de WIP-limiet voor het eerst wordt overschreden. Dit waarschuwingsbericht wordt niet weergegeven in kolommen met een status die gelijk is aan [!UICONTROL Complete].\
   De grens van het KLOOFJE is eenvoudig een visuele waarschuwing en beperkt uw team niet om meer punten in één enkele kolom te hebben dan de grens u plaatst.

   ![WIP-limiet](assets/wip-limit-350x193.png)

1. Klikken **Wijzigingen opslaan**.

## Automatisch artikelen toevoegen vanaf de achtergrond configureren

<!-- this functionality needs to be verified-->

U kunt verhalen van de achterstand vormen die automatisch aan de eerste kolom op worden toegevoegd [!UICONTROL Kanban] board onmiddellijk nadat een item uit die kolom wordt verplaatst.

{{step1-to-team}}

1. Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![Pictogram Teams wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het Kanban-team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu ![](assets/more-menu.png)selecteert u vervolgens **[!UICONTROL Edit]**.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. Selecteren **[!UICONTROL Automatically add next story from backlog]** om te vormen dat het volgende punt van de backlog automatisch aan wordt toegevoegd **[!UICONTROL New]** kolom wanneer een item uit het deelvenster **[!UICONTROL In Progress]** kolom.

   Gebruikers moeten de **Achtergrond tonen** instellen op de [!UICONTROL Kanban] Deze functionaliteit kan van kracht worden. Wanneer de gebruikers toelaten [!UICONTROL Show Backlog] instellen op de [!UICONTROL Kanban Board], vindt de volgende functionaliteit plaats:

   Elke keer dat een artikel wordt verplaatst van het dialoogvenster [!UICONTROL In Progress] in een kolom op het artikelbord die een [!UICONTROL Complete] status (of een status die gelijk is aan [!UICONTROL Complete]), wordt een artikel uit de kolom Achtergrond automatisch naar de [!UICONTROL New] kolom van de [!UICONTROL Kanban Board].
Als het artikel met de hoogste prioriteit vanaf de achtergrond wordt toegevoegd aan het artikelbord.

1. Klik op **[!UICONTROL Save Changes]**.

## Configureer hoe lang kaarten op de [!UICONTROL Kanban] board

U kunt kiezen hoe lang voltooide kaarten op de [!UICONTROL Kanban] bord. Taken die buiten de [!UICONTROL Kanban] het bord kan nog steeds worden geopend in hun oorspronkelijke project .

{{step1-to-team}}

1. (Optioneel) Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![Pictogram Teams wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw Kanban-team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Selecteer het Kanban-team.
1. Klik op de knop **[!UICONTROL More]** menu ![](assets/more-menu.png) selecteert u vervolgens **[!UICONTROL Edit]**.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Number of days Completed cards stay on the Kanban board]** Selecteer een waarde in de vervolgkeuzelijst.

   U kunt een aantal van 1 tot 30 dagen kiezen.
1. Klik op **[!UICONTROL Save Changes]**.
