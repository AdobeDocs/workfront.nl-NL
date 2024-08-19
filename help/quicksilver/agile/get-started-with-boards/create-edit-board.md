---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Een kaart maken of bewerken
description: Vanuit het dashboard van [!UICONTROL boards] kunt u een nieuw board maken of een bestaand board bewerken.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: efe636e14964cc8705839c9f534a9947327803d7
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Een board maken of bewerken

<!-- Audited: 12/2023 -->

Vanuit het dashboard van [!UICONTROL boards] kunt u een nieuw board maken of een bestaand board bewerken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: Medewerker of hoger </p>
 <p>of</p> 
<p>Huidig: [!UICONTROL Request] of hoger </p> 
</td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een nieuw bord maken

{{step1-to-boards}}

1. Klik op **[!UICONTROL Add board]**.

1. Selecteer een sjabloon voor het bord.

   | Sjabloon | Beschrijving |
   |---------|----------|
   | Basisbord | Drie standaardkolommen worden verstrekt op het bord. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. <p>Drie standaardkolommen worden verstrekt op het bord. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. |
   | Kanban-bord | De volgende kolommen worden verstrekt op de raad: Achtergrond, Nieuw, Bezig, Voltooid, en op Greep. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen.<p>Als u de achterstand wilt gebruiken, moet u filters instellen voor de inlaatkolom. Voor informatie, zie [ een inlaatkolom aan een raad ](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md) toevoegen. <p>Om het standaardbeleid voor elke kolom te herzien, klik [!UICONTROL **Meer** menu ] op een kolom en selecteer [!UICONTROL **uitgeven**]. U kunt al deze vooraf ingestelde beleidsregels wijzigen. Voor informatie, zie [ de kolommen van het Beheer ](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospectief | De volgende kolommen staan aan boord: Wat is er goed gegaan? Wat zou verbeterd kunnen worden? Wie moeten we vieren? Wat kunnen we doen om sneller te gaan? U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. <p>Er worden geen kolombeleid toegepast. |
   | Dynamisch bord | De volgende kolommen worden verstrekt op de raad: Niet geselecteerd, Nieuw, Bezig, In Greep, en Volledig. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. (U kunt de naam van de niet-geselecteerde kolom wijzigen, maar de kolom niet verwijderen. Deze kolom bevat alle kaarten met een status die niet overeenkomt met een van de andere kolomstatussen.) <p>Het standaardkolombeleid wijst kaarten aan kolommen toe die op hun status worden gebaseerd. Voor informatie, zie [ de kolommen van het Beheer ](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Voer de stappen van de installatiewizard uit als u alleen een dynamisch board wilt gebruiken:

   1. Typ een naam voor de raad en klik [!UICONTROL **daarna**].
   1. Onderzoek naar en selecteer [!DNL Workfront] [!UICONTROL **Projecten**] om taken en kwesties op de raad te brengen.
   1. Onderzoek naar en selecteer [!UICONTROL **Taken**] om taken en kwesties op de raad te brengen.

      Alle objecten worden op het bord weergegeven als verbonden kaarten.

      De [!UICONTROL **Kaarten die worden toegevoegd**] teller toont hoeveel kaarten op de raad zullen zijn. Bijvoorbeeld, als u een project met 100 taken en kwesties selecteert, toont teller 100. Als u een gebruikerstaak toevoegt en die persoon aan 5 taken op het project wordt toegewezen, toont de teller 5.

      >[!NOTE]
      >
      >De kaartlimiet voor dynamische borden is 700 taken en 700 emissies, voor een totaal van 1.400 kaarten. Een groot aantal kaarten op het bord kan van invloed zijn op de prestaties van het bord. Alle gearchiveerde kaarten, zowel verborgen als zichtbaar, tellen voor deze limiet.

   1. (Facultatief) Uitgezocht [!UICONTROL **archiveer geen voltooide kaarten**] om voltooide taken en kwesties op de raad als zichtbare kaarten in de Voltooide kolom te brengen. Als deze optie niet is geselecteerd, worden voltooide kaarten op het moment van het maken van het bord als gearchiveerde kaarten op het bord geplaatst.

      >[!NOTE]
      >
      >Gearchiveerde kaarten worden standaard niet op het bord weergegeven. Als u gearchiveerde kaarten wilt weergeven, moet u een configuratie-instelling inschakelen en vervolgens het bord filteren om gearchiveerde kaarten weer te geven. Voor details, zie [ aanpassen welke gebieden op een kaart ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) en [ Filter en onderzoek in een raad ](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md) worden getoond.

   1. (Facultatief) klik [!UICONTROL **Geavanceerde filters van het Gebruik**] om extra filteropties te tonen.

      Dit is hetzelfde proces als het maken van een filter op een inlaatkolom. Voor meer informatie, zie [ een inlaatkolom aan een raad ](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md) toevoegen.

      Als u de filters op een dynamisch bord bijwerkt nadat deze zijn gemaakt, worden de kaartinstellingen die geen deel uitmaken van de Workfront-taak of -uitgave (zoals codes) opnieuw ingesteld.

   1. Na het toevoegen van de filters, klik [!UICONTROL **creeer raad**].

1. Typ een naam voor het bord in het veld **[!UICONTROL Board]** en druk op Enter.
1. Configureer de kaart naar wens.

   Voor informatie, zie [ leden toevoegen of verwijderen uit a raad ](../../agile/get-started-with-boards/add-members-to-board.md), [ beheer boardkolommen ](../../agile/get-started-with-boards/manage-board-columns.md), [ voeg een ad hoc kaart aan a raad ](../../agile/get-started-with-boards/add-card-to-board.md) toe, en [ Gebruik verbonden kaarten op raad ](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Klik op **[!UICONTROL All Boards]** om terug te keren naar het dashboard voor de gebieden.

   U kunt ook het vervolgkeuzemenu met de naam van het huidige board vinden en erop klikken om naar een ander bord te gaan.

   ![ Lijst van Borden ](assets/boards-button-list-of-boards-350x188.png)

## Een bestaand bord bewerken

{{step1-to-boards}}

1. Selecteer op het dashboard het board dat u wilt openen.
1. Bewerk het bord naar wens. U kunt op de naam van het tekengebied klikken om de naam te wijzigen.

   Voor informatie, zie [ leden toevoegen of verwijderen uit a raad ](../../agile/get-started-with-boards/add-members-to-board.md), [ beheer boardkolommen ](../../agile/get-started-with-boards/manage-board-columns.md), en [ voeg een kaart aan a raad ](../../agile/get-started-with-boards/add-card-to-board.md) toe.

1. Klik op **[!UICONTROL All Boards]** om terug te keren naar het dashboard voor de gebieden.

   U kunt ook het vervolgkeuzemenu met de naam van het huidige board vinden en erop klikken om naar een ander bord te gaan.

