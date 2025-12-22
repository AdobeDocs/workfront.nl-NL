---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Scrum configureren
description: U kunt de volgende opties voor de teams van de Hulpmiddelen van de Trommel tijdens of nadat het team wordt gecreeerd vormen.
author: Jenny
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 0%

---

# Configureren [!UICONTROL Scrum]

U kunt een team van de Gelijkheid in [!DNL Adobe Workfront] tot stand brengen zoals die in [&#x200B; wordt beschreven leidt tot een team van de Gelijkheid &#x200B;](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Terwijl het creëren van een team van de Gelijkheid kunt u de methodologie kiezen die het team gebruikt om hun werk te voltooien. U kunt uit de volgende opties kiezen:

* Schuiven
* Kanban

In dit artikel wordt beschreven hoe u de instellingen voor een scrubteam configureert. Nadat u een Agile-team hebt gemaakt en de methode Scrum hebt gekozen, kunt u naar dit artikel verwijzen om de volgende instellingen bij te werken:

* Of artikelen worden geschat in punten of uren
* De statuskolommen in het artikel van het artikel van het artikel van het element voor herhalingen en projecten
* Extra velden die op artikelkaarten op het artikel van het artikel van het artikel van het artikel worden weergegeven
* De manier waarop kleurindicatoren worden gebruikt voor artikelen op de whitelepaper
* Hoe datums worden toegepast bij het toevoegen van werkitems aan een herhaling

Voor informatie over het vormen van een team Kanban, zie [&#x200B; Kanban &#x200B;](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md) vormen.

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

>[!NOTE]
>
>Deze instelling kan niet worden gewijzigd als het team herhalingen heeft die momenteel worden uitgevoerd.

U kunt artikelen configureren om te worden geschat aan de hand van punten of uren.

Om te vormen hoe de verhalen voor uw team van Agile worden geschat:

{{step1-to-team}}

1. Klik op het pictogram **[!UICONTROL Switch team]** en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   Deze optie wordt alleen weergegeven voor teamleden met een licentie [!UICONTROL Standard] , [!UICONTROL Plan] of [!UICONTROL Work] .
   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Selecteer in de sectie **[!UICONTROL Agile]** in het gebied **[!UICONTROL Estimate Stories in]** of u punten of uren wilt gebruiken om de grootte (werklast) van artikelen te schatten. Als u Punten selecteert, geeft u op hoeveel uren gelijk zijn aan 1 punt. (De standaardwaarde is 1 punt = 8 uur.) Dit is het aantal geplande uren dat aan het artikel wordt toegevoegd.

   **Voorbeeld:** als u hebt geselecteerd om verhalen in punten en 1 punt te schatten evenaart 8 uren, en een verhaal wordt geschat op 3 punten, worden 24 Geplande Uren toegevoegd aan het verhaal.

1. Klik op **[!UICONTROL Save changes]**.

## Statuskolommen configureren op de whitepaper

U kunt vormen welke kolommen op de het verhaalraad van de Gelijkheid voor alle herhalingen worden getoond die aan uw team, of voor een bepaald project worden toegewezen.

* [Statuskolommen voor herhalingen configureren](#configure-status-columns-for-iterations)
* [Statuskolommen configureren voor projecten](#configure-status-columns-for-projects)

### Statuskolommen voor herhalingen configureren {#configure-status-columns-for-iterations}

U kunt de statussen definiëren die op de whiteboard voor het team van Agile staan. Dit zijn de enige statussen die op het artikelbord worden weergegeven.

U definieert de statussen die beschikbaar zijn voor de artikelkaart die is gekoppeld aan het team van Agile:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch team]** pictogram van het pictogram ![&#x200B; team van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   Deze optie wordt alleen weergegeven voor teamleden met een [!UICONTROL Plan] - of [!UICONTROL Work] -licentie.

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Zoek in de sectie **[!UICONTROL Agile]** het **[!UICONTROL Story Board]** -gebied.

1. (Optioneel) Klik op **[!UICONTROL Add Column]** om een extra statuskolom aan het artikelbord toe te voegen.
1. (Optioneel) Sleep een statuskolom met de indicator voor slepen en neerzetten om de volgorde van de statuskolommen op het artikelbord te wijzigen. De eerste kolom kan niet worden verplaatst en u kunt geen andere kolom vóór de eerste kolom slepen.

   ![&#x200B; belemmering en daling &#x200B;](assets/agile-story-card-drag-and-drop.png)

1. Selecteer zowel taak- als uitgavestatus. De status van de taak wordt getoond als kolomtitel voor elke kolom op de verhaalraad. De uitgiftestatus die u selecteert, wordt toegewezen aan de taakstatus. Dit betekent dat wanneer u een uitgave naar een andere kolom van het artikelbord verplaatst, de status van de uitgave verandert in de hier weergegeven uitgiftestatus en niet in de naam van de kolom op het artikelbord (die de taakstatus weerspiegelt).

   >[!IMPORTANT]
   >
   >Alleen vergrendelde statussen voor het hele systeem kunnen worden geselecteerd. U kunt geen groepspecifieke statussen selecteren. Bovendien komt de status van de eerste kolom altijd overeen met **[!UICONTROL New]** .

   U kunt douanestatus toevoegen als uw [!DNL Workfront] beheerder hen heeft gevormd; de douanestatus kan worden gevormd zoals die in [&#x200B; wordt beschreven creeer of geef een status &#x200B;](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) uit.

   >[!NOTE]
   >
   >Wanneer u uitgavestatussen selecteert, wordt de derde kolom altijd standaard ingesteld op [!UICONTROL Closed] . Als u meer dan drie kolommen hebt, moet u de kolommen handmatig bijwerken om de juiste status te weerspiegelen.

1. Klik op **[!UICONTROL Save changes]**.

### Statuskolommen configureren voor projecten {#configure-status-columns-for-projects}

Voor informatie over hoe te om statuskolommen voor een project te vormen, zie de sectie [&#x200B; creëren of aanpassen een [!UICONTROL Agile] mening &#x200B;](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) in het artikel [&#x200B; creeert of geeft meningen in  [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md) uit.

## Aanvullende velden configureren voor weergave op artikelkaarten op de whitepaper

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

U configureert als volgt artikelkaarten die zijn toegewezen aan het Agile-team om extra velden weer te geven:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch team]** pictogram van het pictogram ![&#x200B; team van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .
Deze optie wordt alleen weergegeven voor teamleden met een [!UICONTROL Plan] - of [!UICONTROL Work] -licentie.

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Typ in de sectie **[!UICONTROL Agile]** een veldnaam om deze te zoeken.

   ![&#x200B; Extra gebieden &#x200B;](assets/agile-additional-fields-scrum.png)

1. Selecteer de naam van het veld dat u wilt toevoegen.
1. Typ de **[!UICONTROL Display name]** voor het veld dat moet worden weergegeven op het artikel of de uitgiftekaart.
1. Klik op **[!UICONTROL Save changes]**.

## Configureer hoe kleurindicatoren worden gebruikt voor artikelen op de whitepaper

Standaard worden artikelbordelementen in een letterlijke herhaling gekleurd volgens het project waaraan het artikel is gekoppeld. Aan elk project wordt willekeurig een kleur toegewezen op het artikelbord. U kunt dit standaardgedrag voor elk team van Agile veranderen. Kleuren voor eenvoudige artikelen kunnen worden gekoppeld aan de prioriteit van het artikel, aan de eigenaar enzovoort.

U wijzigt als volgt het gedrag van de manier waarop kleuren worden toegewezen aan artikelen voor een Agile-team:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch team]** pictogram van het pictogram ![&#x200B; team van de Schakelaar &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het gangbare team dat u wilt beheren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   Deze optie wordt alleen weergegeven voor teamleden met een [!UICONTROL Plan] - of [!UICONTROL Work] -licentie.

   ![&#x200B; geef team &#x200B;](assets/edit-team-settings-350x205.png) uit

1. Selecteer in de sectie [!UICONTROL Agile] in het gebied [!UICONTROL Associate Card Color to] een van de volgende opties:

   * **[!UICONTROL Project]**: kleuren zijn gekoppeld aan het project waaraan het artikel is gekoppeld. (Wanneer een verhaal wordt gecreeerd, moet het met een project worden geassocieerd, zoals die in [&#x200B; wordt beschreven leidt tot een Artikel van de Gelijkheid &#x200B;](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Alle taken van hetzelfde project worden met dezelfde kleur weergegeven.
   * **[!UICONTROL Free Form]**: Alle kaarten worden standaard als blauw weergegeven totdat een gebruiker de kleur handmatig wijzigt, zoals wordt beschreven in [[!UICONTROL Categorize stories by color] op het Klembord &#x200B;](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md) .
   * **[!UICONTROL Priority]**: Kleuren worden als volgt gekoppeld aan de prioriteit van het artikel:

      * Hoog = rood
      * Medium = geel
      * Laag = groen

        Als uw systeembeheerder douaneprioriteiten voor uw [!DNL Workfront] systeem heeft gevormd, is de hoogste prioriteit rood, is het op één na hoogste geel, en het derde hoogste groen.
   * **[!UICONTROL Task Owner]**: alle artikelen met dezelfde primaire toewijzing hebben dezelfde kleur. De primaire ontvanger is de gebruiker die voor het eerst aan de taak is toegewezen.


1. Klik op **[!UICONTROL Save changes]**.

## Configureer hoe datums worden toegepast bij het toevoegen van werkitems aan een herhaling

Wanneer u een tijdelijk item toevoegt aan een scrubherhaling, worden de geplande begindatum en de geplande voltooiingsdatum voor het werkitem standaard aangepast aan de begin- en einddatum van de herhaling. U kunt ervoor kiezen om de oorspronkelijke datums op alle werkitems voor het team te houden.

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![&#x200B; Schakelaar teampictogram &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .
Deze optie wordt alleen weergegeven voor teamleden met een [!UICONTROL Plan] - of [!UICONTROL Work] -licentie.
1. Selecteer in de sectie [!UICONTROL Agile] in het gebied [!UICONTROL When a Work Item is Added to an Iteration] een van de volgende opties:

   * **[!UICONTROL Modify the Planned Start Date and Planned Completion Date to match the iteration start and end dates]**: Wanneer werkitems aan een herhaling worden toegevoegd, worden de datums van het werkitem gewijzigd in de herhalingsdatums.

     Voor meer informatie over hoe de data worden gewijzigd, zie de sectie [&#x200B; begrijpen hoe het toevoegen van verhalen taakdata &#x200B;](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understand-how-adding-stories-affects-task-dates) in het artikel [&#x200B; beïnvloedt verhalen aan een bestaande herhaling &#x200B;](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) toevoegen.
   * **[!UICONTROL Do not modify the Planned Start Date and Planned Completion Date to match the iteration start and end dates]**: Wanneer werkitems aan een herhaling worden toegevoegd, behouden de werkitems hun oorspronkelijke datums.

   Als u de datumoptie wijzigt, worden de datums voor de werkitems die zich al in de herhaling bevinden, niet aangepast.

   Deze opties kunnen datums beïnvloeden wanneer de teams het werkpunten aan elkaars herhalingen toewijzen. Bijvoorbeeld, wijzigt team A de data van het werkpunt aan de iteratiedata en team B wijzigt het de data van het werkpunt niet. Als team B een het werkpunt aan de herhaling van team A toewijst, zullen de data van het het werkpunt worden veranderd. Nochtans, als team A een het werkpunt aan de herhaling van team B toewijst, zullen de data niet veranderen.

1. Klik op **[!UICONTROL Save changes]**.
