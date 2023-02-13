---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Scrum configureren
description: U kunt de volgende opties voor de teams van het de agbestand van de Trommel tijdens of nadat het team wordt gecreeerd vormen.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1531'
ht-degree: 0%

---

# Configureren [!UICONTROL Scrum]

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

>[!NOTE]
>
>Deze instelling kan niet worden gewijzigd als het team herhalingen heeft die momenteel worden uitgevoerd.

U kunt artikelen configureren om te worden geschat aan de hand van punten of uren.

Om te vormen hoe de verhalen voor uw agile team worden geschat:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!UICONTROL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** selecteert u vervolgens een nieuw team in het keuzemenu of zoekt u naar een team in de zoekbalk.
1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.\
   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** in de **[!UICONTROL Estimate Stories in]** selecteert u of u punten of uren wilt gebruiken voor het schatten van de grootte (werkbelasting) van artikelen. Als u Punten selecteert, geeft u op hoeveel uren gelijk zijn aan 1 punt. (De standaardwaarde is 1 punt = 8 uur.) Dit is het aantal geplande uren dat aan het artikel wordt toegevoegd.

   **Voorbeeld:** Als u artikelen in punten en 1 punt wilt schatten, is dit gelijk aan 8 uur en een artikel wordt geschat op 3 punten, worden 24 geplande uren toegevoegd aan het artikel.

1. Klik op **[!UICONTROL Save changes]**.

## Statuskolommen configureren op de whiteboardlijst voor bestanden

U kunt vormen welke kolommen op het agile verhaalbord voor alle herhalingen worden getoond die aan uw team, of voor een bepaald project worden toegewezen.

* [Statuskolommen voor herhalingen configureren](#configure-status-columns-for-iterations)
* [Statuskolommen configureren voor projecten](#configure-status-columns-for-projects)

### Statuskolommen voor herhalingen configureren {#configure-status-columns-for-iterations}

U kunt de statussen bepalen die op de verhaalraad voor het flexibele team bestaan. Dit zijn de enige statussen die op het artikelbord worden weergegeven.

U definieert de statussen die beschikbaar zijn voor de artikelkaart die is gekoppeld aan het mobiele team:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** de sectie, bepaal de plaats van **[!UICONTROL Story Board]** gebied.

1. (Optioneel) Klik op **[!UICONTROL Add Column]** om een extra statuskolom toe te voegen aan het artikelbord.
1. (Optioneel) Sleep een statuskolom met de indicator voor slepen en neerzetten om de volgorde van de statuskolommen op het artikelbord te wijzigen. De eerste kolom kan niet worden verplaatst en u kunt geen andere kolom vóór de eerste kolom slepen.

   ![Slepen en neerzetten](assets/agile-story-card-drag-and-drop.png)

1. Selecteer zowel taak- als uitgavestatus. De status van de taak wordt getoond als kolomtitel voor elke kolom op de verhaalraad. De uitgiftestatus die u selecteert, wordt toegewezen aan de taakstatus. Dit betekent dat wanneer u een uitgave naar een andere kolom van het artikelbord verplaatst, de status van de uitgave verandert in de hier weergegeven uitgiftestatus en niet in de naam van de kolom op het artikelbord (die de taakstatus weerspiegelt).

   >[!IMPORTANT]
   >
   >Alleen vergrendelde statussen voor het hele systeem kunnen worden geselecteerd. u kunt geen groepsspecifieke statussen selecteren. Bovendien komt de status van de eerste kolom altijd overeen met **[!UICONTROL New]**.

   U kunt aangepaste statussen toevoegen als uw [!DNL Workfront] de beheerder heeft deze geconfigureerd; aangepaste statussen kunnen worden geconfigureerd zoals wordt beschreven in [Een status maken of bewerken](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Bij het selecteren van uitgiftestatussen wordt de derde kolom altijd standaard ingesteld op [!UICONTROL Closed]. Als u meer dan drie kolommen hebt, moet u de kolommen handmatig bijwerken om de juiste status te weerspiegelen.

1. Klik op **[!UICONTROL Save changes]**.

### Statuskolommen configureren voor projecten {#configure-status-columns-for-projects}

Voor informatie over hoe te om statuskolommen voor een project te vormen, zie de sectie [Een [!UICONTROL Agile] weergave](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) in het artikel [Weergaven maken of bewerken in [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

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

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!UICONTROL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** -sectie, typt u een veldnaam om deze te zoeken.

   ![Aanvullende velden](assets/agile-additional-fields-scrum.png)

1. Selecteer de naam van het veld dat u wilt toevoegen.
1. Typ de **[!UICONTROL Display name]** voor het veld dat wordt weergegeven op het artikel of de uitgiftekaart.
1. Klik op **[!UICONTROL Save changes]**.

## Configureer hoe kleurindicatoren worden gebruikt voor artikelen op de agile-artikelkaart

Standaard worden artikelbordelementen in een flexibele herhaling gekleurd volgens het project waaraan het artikel is gekoppeld. Aan elk project wordt willekeurig een kleur toegewezen op het artikelbord. U kunt dit standaardgedrag voor elk agile team veranderen. Kleuren voor flexibele artikelen kunnen worden gekoppeld aan de prioriteit van het artikel, aan de eigenaar enzovoort.

U wijzigt als volgt het gedrag van de manier waarop kleuren worden toegewezen aan artikelen voor een bestandsteam:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het flexibele team dat u wilt beheren.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.

   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.

   ![Team bewerken](assets/edit-team-settings-350x205.png)

1. In de [!UICONTROL Agile] in de [!UICONTROL Associate Card Color to] selecteert u een van de volgende opties:

   * **[!UICONTROL Project]**: Kleuren worden gekoppeld aan het project waaraan het artikel is gekoppeld. (Wanneer een artikel wordt gemaakt, moet het worden gekoppeld aan een project, zoals wordt beschreven in [Een flexibel artikel maken](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Alle taken van hetzelfde project worden met dezelfde kleur weergegeven.
   * **[!UICONTROL Free Form]**: Alle kaarten worden standaard als blauw weergegeven totdat een gebruiker de kleur handmatig wijzigt, zoals wordt beschreven in [[!UICONTROL Categorize stories by color] op het trommelbord](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Priority]**: Kleuren worden als volgt gekoppeld aan de prioriteit van het artikel:

      * Hoog = rood
      * Normaal = geel
      * Laag = Groen\

         Als uw systeembeheerder aangepaste prioriteiten voor uw [!DNL Workfront] -systeem, de hoogste prioriteit is rood, de op één na hoogste geel en de op twee na hoogste groen.
   * **[!UICONTROL Task Owner]**: Alle artikelen met dezelfde primaire toewijzing hebben dezelfde kleur. De primaire ontvanger is de gebruiker die voor het eerst aan de taak is toegewezen.


1. Klik op **[!UICONTROL Save changes]**.

## Configureer hoe datums worden toegepast bij het toevoegen van werkitems aan een herhaling

Wanneer u een tijdelijk item toevoegt aan een scrubherhaling, worden de geplande begindatum en de geplande voltooiingsdatum voor het werkitem standaard gewijzigd zodat deze overeenkomen met de begin- en einddatum van de herhaling. U kunt ervoor kiezen om de oorspronkelijke datums op alle werkitems voor het team te houden.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront, klik vervolgens op **[!UICONTROL Teams]**.
1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw scrubteam in het keuzemenu of zoek naar een team op de zoekbalk.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.
1. In de [!UICONTROL Agile] in de [!UICONTROL When a Work Item is Added to an Iteration] selecteert u een van de volgende opties:

   * **[!UICONTROL Modify the Planned Start Date and Planned Completion Date to match the iteration start and end dates]**: Wanneer de het werkpunten aan een herhaling worden toegevoegd, worden de data van het het werkpunt veranderd in de iteratiedata.\

      Zie de sectie voor meer informatie over de manier waarop de datums worden gewijzigd [Begrijp hoe het toevoegen van artikelen takendatums beïnvloedt](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) in het artikel [Artikelen toevoegen aan een bestaande herhaling](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Do not modify the Planned Start Date and Planned Completion Date to match the iteration start and end dates]**: Wanneer de het werkpunten aan een herhaling worden toegevoegd, behouden de het werkpunten hun originele data.

   Als u de datumoptie wijzigt, worden de datums voor de werkitems die zich al in de herhaling bevinden, niet aangepast.

   Deze opties kunnen datums beïnvloeden wanneer de teams het werkpunten aan elkaars herhalingen toewijzen. Bijvoorbeeld, wijzigt team A de data van het werkpunt aan de iteratiedata en team B wijzigt het de data van het werkpunt niet. Als team B een het werkpunt aan de herhaling van team A toewijst, zullen de data van het het werkpunt worden veranderd. Nochtans, als team A een het werkpunt aan de herhaling van team B toewijst, zullen de data niet veranderen.

1. Klik op **[!UICONTROL Save changes]**.
