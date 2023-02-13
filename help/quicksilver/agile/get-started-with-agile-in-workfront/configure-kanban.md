---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Kanban configureren
description: U kunt de volgende opties voor Kanban agile teams vormen tijdens of nadat het team wordt gecreeerd.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 0%

---

# Configureren [!UICONTROL Kanban]

U kunt de volgende opties voor mobiele teams vormen tijdens of nadat het team is gemaakt. U maakt een &#39;agile&#39; team (Kanban of Scrum) in [!DNL Adobe Workfront] zoals beschreven in [Een bestandsteam maken](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

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
   <td> <p>[!UICONTROL Work] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Configureer of artikelen worden geschat in punten of uren

U kunt artikelen configureren om te worden geschat aan de hand van punten of uren.

Om te vormen hoe de verhalen voor uw agile team worden geschat:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** selecteert u vervolgens een nieuw team in het keuzemenu of zoekt u naar een team in de zoekbalk.
1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.\
   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** in de **[!UICONTROL Estimate Stories in]** selecteert u of u punten of uren wilt gebruiken voor het schatten van de grootte (werkbelasting) van artikelen. Als u Punten selecteert, geeft u op hoeveel uren gelijk zijn aan 1 punt. (De standaardwaarde is 1 punt = 8 uur.) Dit is het aantal geplande uren dat aan het artikel wordt toegevoegd.

   **Voorbeeld:** Als u artikelen in punten en 1 punt wilt schatten, is dit gelijk aan 8 uur en een artikel wordt geschat op 3 punten, worden 24 geplande uren toegevoegd aan het artikel.

1. Klik op **[!UICONTROL Save changes]**.

## Statuskolommen configureren op de whiteboardlijst voor bestanden

U kunt de statussen bepalen die op de verhaalraad voor het flexibele team bestaan. Dit zijn de enige statussen die op het artikelbord worden weergegeven.

U definieert de statussen die beschikbaar zijn voor de artikelkaart die is gekoppeld aan het mobiele team:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!UICONTROL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** de sectie, bepaal de plaats van **[!UICONTROL Story Board]** gebied.

1. (Optioneel) Klik op **[!UICONTROL Add Column]** om een extra statuskolom toe te voegen aan het artikelbord.
1. (Optioneel) Sleep een statuskolom met de indicator voor slepen en neerzetten om de volgorde van de statuskolommen op het artikelbord te wijzigen. De eerste kolom kan niet worden verplaatst en u kunt geen andere kolom vóór de eerste kolom slepen.

   ![Slepen en neerzetten](assets/agile-story-card-drag-and-drop.png)

1. Selecteer taakstatussen.

   >[!IMPORTANT]
   >
   >Alleen vergrendelde statussen voor het hele systeem kunnen worden geselecteerd. u kunt geen groepsspecifieke statussen selecteren. Bovendien komt de status van de eerste kolom altijd overeen met **[!UICONTROL New]**.

   U kunt aangepaste statussen toevoegen als uw [!DNL Workfront] de beheerder heeft deze geconfigureerd; aangepaste statussen kunnen worden geconfigureerd zoals wordt beschreven in [Een status maken of bewerken](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klik op **[!UICONTROL Save changes]**.

## Aanvullende velden configureren voor weergave op artikelkaarten op de kaart van het gegenereerde artikel

Wanneer u velden toevoegt aan artikelkaarten, zijn velden alleen-weergeven en alleen-weergeven wanneer het veld is gevuld.

Standaard worden de volgende gegevenstypen op de artikelkaart weergegeven voor taken en uitgaven:

* Artikelnaam met een koppeling die rechtstreeks naar de taak of uitgave verwijst
* De projectnaam met een verbinding direct aan het project
* Deze koppeling wordt alleen weergegeven voor artikelen, niet voor subtaken
* De taak of uitgiftebeschrijving
* Huidige verplichting
* Het percentage voltooide bewerkingen weergeven en bewerken door het percentage aan te passen dat is voltooid of door het aantal punten of uren aan te passen dat is voltooid
* Toegewezen gebruikers

U kunt aanvullende gegevens (inclusief aangepaste gegevens) weergeven op artikelkaarten. U wilt mogelijk om een aantal redenen extra velden weergeven op artikelkaarten. Bijvoorbeeld, zou u identiteitskaart van de Klant kunnen willen tonen als u aan verhalen voor veelvoudige klanten binnen de herhaling werkt, of u zou de Datum van het Begin van het Project of de Datum van de Voltooiing van het Project kunnen willen tonen.

>[!NOTE]
>
>Als u een aangepast veld op een artikelkaart gebruikt, kan dit geen punt of punt in de naam bevatten.

U kunt als volgt artikelkaarten configureren die aan het mobiele team zijn toegewezen om extra velden weer te geven:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** -sectie, typt u een veldnaam om deze te zoeken.

   ![Aanvullende velden](assets/agile-additional-fields-kanban.png)

1. Selecteer de naam van het veld dat u wilt toevoegen.
1. Typ de **[!UICONTROL Display name]** voor het veld dat wordt weergegeven op het artikel of de uitgiftekaart.
1. Klik op **[!UICONTROL Save changes]**.

## De WIP-limiet (werk in uitvoering) configureren

Kanban in [!DNL Workfront] staat u toe om de hoeveelheid werk te controleren het team momenteel werkt door het aantal taken te beperken die in kan verschijnen [!UICONTROL In Progress] kolom op de [!UICONTROL Kanban] bord.

Als de WIP-limiet is geconfigureerd, kunt u de WIP-limiet weergeven of deze zelfs bijwerken vanuit de [!UICONTROL Kanban] agile story board, zoals beschreven in [De WIP-limiet (work in progress) beheren voor de [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Om WIP voor uw Kanban team te beperken:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het Kanban-team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** in de **[!UICONTROL Methodology]** selecteert, zorgt u ervoor dat Kanban is geselecteerd.

1. In de **[!UICONTROL Story Board]** in de **[!UICONTROL WIP LIMIT]** veld, geeft u het maximum aantal items op dat in elke kolom van het [!UICONTROL Kanban] &#39;agile story board&#39;. U kunt voor elke kolom een andere limiet instellen. De maximale limiet die u voor elke kolom kunt instellen, is 100.\
   Als deze optie is ingesteld, verschijnt er een waarschuwingsbericht op de knop [!UICONTROL Kanban] Op elk gewenst moment wordt de limiet voor elke kolom op het artikelbord overschreden. Dit waarschuwingsbericht wordt alleen weergegeven wanneer de WIP-limiet voor het eerst wordt overschreden. Dit waarschuwingsbericht wordt niet weergegeven in kolommen met een status die gelijk is aan [!UICONTROL Complete].\
   De grens van het KLOOFJE is eenvoudig een visuele waarschuwing en beperkt uw team niet om meer punten in één enkele kolom te hebben dan de grens u plaatst.

   ![WIP-limiet](assets/wip-limit-350x193.png)

1. Klikken **Wijzigingen opslaan**.

## Artikelen configureren die automatisch worden toegevoegd vanaf de achtergrond

U kunt verhalen van de achterstand vormen die automatisch aan de eerste kolom op worden toegevoegd [!UICONTROL Kanban] board onmiddellijk nadat een item uit die kolom wordt verplaatst.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het Kanban-team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. Selecteren **[!UICONTROL Automatically add next story from backlog]** om verhalen te vormen die automatisch van de backlog aan de eerste kolom op moeten worden toegevoegd [!UICONTROL Kanban] artikelbord.

   Dit gebeurt telkens wanneer een artikel wordt verplaatst naar een kolom op het artikelbord die de status Voltooid vertegenwoordigt (een status die gelijk is aan Voltooien). Als het artikel met de hoogste prioriteit vanaf de achtergrond wordt toegevoegd aan de artikellijst, selecteert u deze optie om het volgende item vanaf de achtergrond automatisch toe te voegen aan de lijst **[!UICONTROL In Progress]** kolom wanneer een item uit het deelvenster **[!UICONTROL In Progress]** kolom.

1. Klik op **[!UICONTROL Save changes]**.

## Configureer hoe lang kaarten op de [!UICONTROL Kanban] board

U kunt kiezen hoe lang voltooide kaarten op de [!UICONTROL Kanban] bord. Taken die buiten de [!UICONTROL Kanban] het bord kan nog steeds worden geopend in hun oorspronkelijke project .

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw Kanban-team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Selecteer het Kanban-team.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **Edhet**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Number of days Completed cards stay on the Kanban board]** Selecteer een waarde in de vervolgkeuzelijst.
1. Klik op **[!UICONTROL Save changes]**.
