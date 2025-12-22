---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Kanban configureren
description: U kunt de volgende opties voor Kanban Agile-teams configureren tijdens of nadat het team is gemaakt.
author: Jenny
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# Configureren [!UICONTROL Kanban]

<!--Audited: 12/2023-->

U kunt een team van de Gelijkheid in [!DNL Adobe Workfront] tot stand brengen zoals die in [&#x200B; wordt beschreven leidt tot een team van de Gelijkheid &#x200B;](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Terwijl het creëren van een team van de Gelijkheid kunt u de methodologie kiezen die het team gebruikt om hun werk te voltooien. U kunt uit de volgende opties kiezen:

* Schuiven
* Kanban

Dit artikel beschrijft hoe te om de montages voor een team te vormen Kanban. Nadat u een Agile-team hebt gemaakt en de Kanban-methode hebt gekozen, kunt u naar dit artikel verwijzen om de volgende instellingen bij te werken:

* Of artikelen worden geschat in punten of uren
* De statuskolommen op het artikel in het artikel
* Extra velden die op artikelkaarten op het artikel van het artikel van het artikel van het artikel worden weergegeven
* De limiet voor lopende werkzaamheden (WIP)
* Hoe te om verhalen van de achterstand automatisch toe te voegen
* Hoe lang kaarten op de Kanban-kaart blijven

Voor informatie over het vormen van een team van het Trommel, zie [&#x200B; Scrum &#x200B;](../get-started-with-agile-in-workfront/configure-scrum.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot teams bewerken</p>  </td> 
  </tr>

</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configureer of artikelen worden geschat in punten of uren

U kunt artikelen configureren om te worden geschat aan de hand van punten of uren.

Om te vormen hoe de verhalen voor uw team van Agile worden geschat:

{{step1-to-team}}

1. Klik op het pictogram **[!UICONTROL Switch Teams]** ![](assets/switch-team-icon.png) en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team in het zoekvak.
1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het **[!UICONTROL More]** menu ![](assets/more-menu.png) en selecteer vervolgens **[!UICONTROL Edit]** .

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Selecteer in de sectie **[!UICONTROL Agile]** in het gebied **[!UICONTROL Estimate Stories in]** of u punten of uren wilt gebruiken om de grootte (werklast) van artikelen te schatten. Als u Punten selecteert, geeft u op hoeveel uren gelijk zijn aan 1 punt. (De standaardwaarde is 1 punt = 8 uur.) Dit is het aantal geplande uren dat aan het artikel wordt toegevoegd.

   **Voorbeeld:** als u hebt geselecteerd om verhalen in punten en 1 punt te schatten evenaart 8 uren, en een verhaal wordt geschat op 3 punten, worden 24 Geplande Uren toegevoegd aan het verhaal.

1. Klik op **[!UICONTROL Save Changes]**.

## Statuskolommen configureren op de whitepaper

U kunt de statussen definiëren die op de whiteboard voor het team van Agile staan. Dit zijn de enige statussen die op het artikelbord worden weergegeven.

U definieert de statussen die beschikbaar zijn voor de artikelkaart die is gekoppeld aan het team van Agile:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch Teams]** pictogram ![&#x200B; pictogram van de Teams van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Zoek in de sectie **[!UICONTROL Agile]** het **[!UICONTROL Story Board]** -gebied.

1. (Optioneel) Klik op **[!UICONTROL Add Column]** om een extra statuskolom aan het artikelbord toe te voegen.
1. (Optioneel) Sleep een statuskolom met de indicator voor slepen en neerzetten om de volgorde van de statuskolommen op het artikelbord te wijzigen. De eerste kolom kan niet worden verplaatst en u kunt geen andere kolom vóór de eerste kolom slepen.

   ![&#x200B; belemmering en daling &#x200B;](assets/agile-story-card-drag-and-drop.png)

1. Selecteer taakstatussen.

   >[!IMPORTANT]
   >
   >Alleen vergrendelde statussen voor het hele systeem kunnen worden geselecteerd. U kunt geen groepsspecifieke statussen selecteren. De status van de eerste kolom komt altijd overeen met **[!UICONTROL New]** .

   U kunt aangepaste statussen toevoegen als de [!DNL Workfront] -beheerder deze heeft geconfigureerd. Voor meer informatie, zie [&#x200B; een status &#x200B;](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

1. Klik op **[!UICONTROL Save Changes]**.

## Aanvullende velden configureren voor weergave op artikelkaarten op de whitepaper

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

U configureert als volgt artikelkaarten die zijn toegewezen aan het Agile-team om extra velden weer te geven:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch Teams]** pictogram ![&#x200B; pictogram van de Teams van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Typ in de sectie **[!UICONTROL Agile]** een veldnaam om deze te zoeken.

   ![&#x200B; Extra gebieden &#x200B;](assets/agile-additional-fields-kanban.png)

1. Selecteer de naam van het veld dat u wilt toevoegen.
1. Typ de **[!UICONTROL Display name]** voor het veld dat moet worden weergegeven op het artikel of de uitgiftekaart.
1. Klik op **[!UICONTROL Save Changes]**.

## De WIP-limiet (werk in uitvoering) configureren

Wanneer u de grens van het KLOOFJE van een team bepaalt Kanban, kunt u het aantal punten controleren het team momenteel werkt door het aantal taken te beperken die in [!UICONTROL New] of de [!UICONTROL In Progress] kolom op de [!UICONTROL Kanban] raad kunnen verschijnen.

Nadat u de grens van het KLOOFJE voor een team vormt Kanban, kunt u de grens van het KLOOFJE bekijken en het van de [!UICONTROL Kanban] Gelijke verhaalraad bijwerken, zoals die in [&#x200B; wordt beschreven beheert het werk lopend (WIP) grens op de [!UICONTROL Kanban] raad &#x200B;](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Om WIP voor uw team van Kanban te beperken:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch Teams]** pictogram ![&#x200B; pictogram van de Teams van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het Kanban-team dat u wilt beheren.
1. Klik op het **[!UICONTROL More]** menu ![](assets/more-menu.png) en selecteer vervolgens **[!UICONTROL Edit]** .

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Controleer in de sectie **[!UICONTROL Agile]** in de sectie **[!UICONTROL Methodology]** of Kanban is geselecteerd.

1. Geef in de sectie **[!UICONTROL Story Board]** in het veld **[!UICONTROL WIP Limit]** het maximum aantal items op dat is toegestaan in elke kolom van het [!UICONTROL Kanban] artikel. U kunt voor elke kolom een andere limiet instellen. De maximumgrens u voor elke kolom kunt plaatsen is 100.
Als deze optie is ingesteld, wordt op het [!UICONTROL Kanban] artikel een waarschuwingsbericht weergegeven wanneer de limiet voor een kolom op het artikelbord wordt overschreden. Dit waarschuwingsbericht wordt alleen weergegeven wanneer de WIP-limiet voor het eerst wordt overschreden. Dit waarschuwingsbericht wordt niet weergegeven in kolommen met een status die gelijk is aan [!UICONTROL Complete] .
De grens van het KLOOFJE is eenvoudig een visuele waarschuwing en beperkt uw team niet om meer punten in één enkele kolom te hebben dan de grens u plaatst.

   ![&#x200B; grens van het WIP &#x200B;](assets/wip-limit-350x193.png)

1. Klik **sparen Veranderingen**.

## Automatisch artikelen toevoegen vanaf de achtergrond configureren

<!-- this functionality needs to be verified-->

U kunt artikelen vanaf de achtergrond configureren en deze direct na het verplaatsen van een item uit die kolom automatisch toevoegen aan de eerste kolom op de [!UICONTROL Kanban] -board.

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch Teams]** pictogram ![&#x200B; pictogram van de Teams van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het Kanban-team dat u wilt beheren.
1. Klik op het **[!UICONTROL More]** menu ![](assets/more-menu.png) en selecteer vervolgens **[!UICONTROL Edit]** .

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Selecteer **[!UICONTROL Automatically add next story from backlog]** om te configureren dat het volgende item in de backlog automatisch wordt toegevoegd aan de kolom **[!UICONTROL New]** wanneer een item uit de kolom **[!UICONTROL In Progress]** wordt verplaatst.

   De gebruikers moeten **tonen Achtergrond** plaatsen op de [!UICONTROL Kanban] raad voor deze functionaliteit toelaten om van kracht te worden. Wanneer gebruikers de instelling [!UICONTROL Show Backlog] inschakelen op de [!UICONTROL Kanban Board] , vindt de volgende functionaliteit plaats:

   Telkens wanneer een artikel van de kolom [!UICONTROL In Progress] wordt verplaatst naar een kolom op het artikelbord die een [!UICONTROL Complete] status (of een status die gelijk is aan [!UICONTROL Complete] ) vertegenwoordigt, wordt een artikel uit de kolom Backlog automatisch verplaatst naar de [!UICONTROL New] kolom van [!UICONTROL Kanban Board] .
Als het artikel met de hoogste prioriteit vanaf de achtergrond wordt toegevoegd aan het artikelbord.

1. Klik op **[!UICONTROL Save Changes]**.

## Configureer hoe lang kaarten op de kaart van [!UICONTROL Kanban] blijven

U kunt kiezen hoe lang voltooide kaarten op de [!UICONTROL Kanban] -kaart blijven staan. Taken die buiten de [!UICONTROL Kanban] -board vallen, zijn nog steeds toegankelijk in het oorspronkelijke project.

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch Teams]** pictogram ![&#x200B; pictogram van de Teams van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team Kanban van het drop-down menu of onderzoek naar een team in de onderzoeksbar.
1. Selecteer het Kanban-team.
1. Klik op het **[!UICONTROL More]** menu ![](assets/more-menu.png) en selecteer vervolgens **[!UICONTROL Edit]** .

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Selecteer een waarde in de vervolgkeuzelijst **[!UICONTROL Number of days Completed cards stay on the Kanban board]** .

   U kunt een aantal van 1 tot 30 dagen kiezen.
1. Klik op **[!UICONTROL Save Changes]**.
