---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Een board maken of bewerken
description: Van de [!UICONTROL boards] kunt u een nieuw board maken of een bestaand board bewerken.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 38715b9571206fd3621b5c078c3eebe380297e9b
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Een board maken of bewerken

<!-- Audited: 12/2023 -->

Van de [!UICONTROL boards] kunt u een nieuw board maken of een bestaand board bewerken.

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Medewerker of hoger </p>
 <p>of</p> 
<p>Huidige: [!UICONTROL Request] of hoger </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een nieuw bord maken

{{step1-to-boards}}

1. Klik op **[!UICONTROL Add board]**.

1. Selecteer een sjabloon voor het bord.

   | Sjabloon | Beschrijving |
   |---------|----------|
   | Basisbord | Drie standaardkolommen worden verstrekt op het bord. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. <p>Drie standaardkolommen worden verstrekt op het bord. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. |
   | Kanban-bord | De volgende kolommen worden verstrekt op de raad: Achtergrond, Nieuw, Bezig, Voltooid, en op Greep. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen.<p>Als u de achterstand wilt gebruiken, moet u filters instellen voor de inlaatkolom. Zie voor meer informatie [Een inlaatkolom aan een bord toevoegen](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Als u het standaardbeleid voor elke kolom wilt bekijken, klikt u op de knop [!UICONTROL **Meer** menu] op een kolom en selecteer [!UICONTROL **Bewerken**]. U kunt al deze vooraf ingestelde beleidsregels wijzigen. Zie voor meer informatie [Bordkolommen beheren](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospectief | De volgende kolommen staan aan boord: Wat is er goed gegaan? Wat zou verbeterd kunnen worden? Wie moeten we vieren? Wat kunnen we doen om sneller te gaan? U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. <p>Er worden geen kolombeleid toegepast. |
   | Dynamisch bord | De volgende kolommen worden verstrekt op de raad: Niet geselecteerd, Nieuw, Bezig, In Greep, en Volledig. U kunt nieuwe kolommen toevoegen en de standaardkolommen hernoemen of verwijderen. (U kunt de naam van de niet-geselecteerde kolom wijzigen, maar de kolom niet verwijderen. Deze kolom bevat alle kaarten met een status die niet overeenkomt met een van de andere kolomstatussen.) <p>Het standaardkolombeleid wijst kaarten aan kolommen toe die op hun status worden gebaseerd. Zie voor meer informatie [Bordkolommen beheren](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Voer de stappen van de installatiewizard uit als u alleen een dynamisch board wilt gebruiken:

   1. Zoeken naar en selecteren [!DNL Workfront] [!UICONTROL **Projecten**] taken en kwesties op de agenda te zetten.
   1. Zoeken naar en selecteren [!UICONTROL **Toewijzingen**] taken en kwesties op de agenda te zetten.

      Alle objecten worden op het bord weergegeven als verbonden kaarten.

      De [!UICONTROL **Kaarten die worden toegevoegd**] de teller laat zien hoeveel kaarten er op het bord staan . Bijvoorbeeld, als u een project met 100 taken en kwesties selecteert, toont teller 100. Als u een gebruikerstaak toevoegt en die persoon aan 5 taken op het project wordt toegewezen, toont de teller 5.

   1. (Optioneel) Selecteer [!UICONTROL **Voltooid werk opnemen als gearchiveerde kaarten**] om voltooide taken en kwesties als gearchiveerde kaarten aan de raad van bestuur te onderwerpen.

      >[!NOTE]
      >
      >Gearchiveerde kaarten worden standaard niet op het bord weergegeven. Als u gearchiveerde kaarten wilt weergeven, moet u een configuratie-instelling inschakelen en vervolgens het bord filteren om gearchiveerde kaarten weer te geven. Zie voor meer informatie [Aanpassen welke velden worden weergegeven op een kaart](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) en [Filteren en zoeken in een board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).
      >
      >Als deze optie niet is geselecteerd, worden voltooide kaarten op het moment van het maken van het bord niet op het bord weergegeven. Kaarten die later als volledig zijn gemarkeerd, blijven in de kolom Voltooid op het bord en worden alleen gearchiveerd als u de kaart hebt uitgeschakeld. Zie voor meer informatie [Afvalfunctie van kaart configureren](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

   1. (Optioneel) Klik op [!UICONTROL **Geavanceerde filters gebruiken**] om extra filteropties weer te geven.

      Dit is hetzelfde proces als het maken van een filter op een inlaatkolom. Zie voor meer informatie [Een inlaatkolom aan een bord toevoegen](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. Klik op [!UICONTROL **Tekengebied maken**].

1. Typ een naam voor het toetsenbord in het dialoogvenster **[!UICONTROL Board]** en drukt u op Enter.
1. Configureer de kaart naar wens.

   Zie voor meer informatie [Leden toevoegen aan of verwijderen uit een board](../../agile/get-started-with-boards/add-members-to-board.md), [Bordkolommen beheren](../../agile/get-started-with-boards/manage-board-columns.md), [Een ad-hockaart aan een kaart toevoegen](../../agile/get-started-with-boards/add-card-to-board.md), en [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Klikken **[!UICONTROL All Boards]** om terug te keren naar het dashboard voor de raden.

   U kunt ook het vervolgkeuzemenu met de naam van het huidige board vinden en erop klikken om naar een ander bord te gaan.

   ![Lijst van borden](assets/boards-button-list-of-boards-350x188.png)

## Een bestaand bord bewerken

{{step1-to-boards}}

1. Selecteer op het dashboard het board dat u wilt openen.
1. Bewerk het bord naar wens. U kunt op de naam van het tekengebied klikken om de naam te wijzigen.

   Zie voor meer informatie [Leden toevoegen aan of verwijderen uit een board](../../agile/get-started-with-boards/add-members-to-board.md), [Bordkolommen beheren](../../agile/get-started-with-boards/manage-board-columns.md), en [Een kaart aan een kaart toevoegen](../../agile/get-started-with-boards/add-card-to-board.md).

1. Klikken **[!UICONTROL All Boards]** om terug te keren naar het dashboard voor de raden.

   U kunt ook het vervolgkeuzemenu met de naam van het huidige board vinden en erop klikken om naar een ander bord te gaan.
