---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban Overzicht
description: Lees dit artikel om beter te begrijpen hoe het Kanban-bord werkt.
author: Courtney
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Kanban-overzicht

<!-- Audited: 01/2024 -->

In de volgende secties krijgt u meer inzicht in de werking van het [!UICONTROL Kanban] -board.

Voor een beschrijving van K [!UICONTROL anban] methodologie, zie [&#x200B; een team van de Gelijkheid &#x200B;](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md) creëren.

Als u in het migreren van een de teamraad van de Gibel [!UICONTROL Kanban] aan [!DNL Workfront] [!UICONTROL Boards] geinteresseerd bent, zie [&#x200B; Gelijke teamkaarten [!UICONTROL Kanban] aan  [!DNL Workfront]  boards &#x200B;](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md) migreren.

## [!UICONTROL Kanban] boardlayout en -functies

De [!UICONTROL Kanban] -board bestaat uit de volgende elementen:

**Achtergrondkolom**: Toont alle taken die momenteel op de backlog zijn. Deze kolom wordt niet standaard weergegeven. Voor meer informatie over de backlog, met inbegrip van hoe te om het op de [!UICONTROL Kanban] raad te tonen, zie [&#x200B; de Agile backlog &#x200B;](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) leiden.

**de Statussen van het Verhaal**: Wijst erop hoe een verhaal gebaseerd op welke statuskolom voortschrijdt het verhaal binnen is.

Voor meer informatie, zie [&#x200B; Update de status van verhalen op de [!UICONTROL Kanban] raad &#x200B;](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

De statussen van het verhaal kunnen voor het project worden aangepast door de mening van de Gelijkheid te wijzigen, zoals die in de sectie [[!UICONTROL Create or customize an Agile view]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [&#x200B; wordt beschreven creeer of geef meningen in  [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) uit.

>[!NOTE]
>
>Er worden standaard maximaal vijftig kaarten weergegeven op het Kanban-bord, maar u kunt op **[!UICONTROL Show More]** klikken om extra kaarten weer te geven.

## Relatie tussen subtaken en artikelen

Als een artikel subtaken bevat, kunt u geen informatie over het bovenliggende artikel zelf bijwerken (zoals punten/uren of procent voltooid). Bovendien kunt u het artikel niet over het [!UICONTROL Kanban] -board verplaatsen om de status ervan bij te werken. Alle wijzigingen die u aanbrengt in de subtaken van het artikel, worden weerspiegeld in het artikel. De punten of uren van het bovenliggende artikel worden bepaald door de gecombineerde artikelpunten of -uren voor alle subtaken.

Als een artikel bijvoorbeeld slechts één subtaak heeft die op 4 punten is gewaardeerd, heeft het artikel zelf ook 4 punten. Als u de subtaakpuntwaarde wijzigt in 3, wordt de puntwaarde van het bovenliggende artikel gewijzigd in 3. Als u een andere subtaak voor hetzelfde artikel maakt en de puntwaarde voor die subtaak instelt op 4, wordt de puntwaarde voor het artikel gewijzigd in 7 om de gecombineerde puntwaarde voor beide subtaken weer te geven.

Deze zelfde logica is op subtaken op het tweede niveau (subtaken van subtaken) van toepassing. Als een subtaak één of meerdere subtaken op het tweede niveau heeft, wordt de subtaak berekend gebaseerd op de subtaken op het tweede niveau.

## Ondersteunde functies

U kunt de volgende handelingen uitvoeren wanneer u het Kanban-bord gebruikt:

* [Een subtaak toevoegen aan een bestaand artikel op het [!UICONTROL Kanban] -bord](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Bestaande taken of problemen toevoegen aan de [!UICONTROL Kanban] -board](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Gebruikers toewijzen aan een artikel op het [!UICONTROL Kanban] -bord](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Artikelen en problemen toevoegen vanuit het [!UICONTROL Kanban] -bord](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Artikelen of problemen van het [!UICONTROL Kanban] -board verwijderen](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Artikelgegevens bewerken](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filteren op gebruiker op het [!UICONTROL Kanban] -board](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [De WIP-limiet (work in progress) op het [!UICONTROL Kanban] -board beheren](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Artikelen op het [!UICONTROL Kanban] -board opnieuw ordenen](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [De status van artikelen op het [!UICONTROL Kanban] -board bijwerken](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Vlaggen gebruiken op artikelen op het [!UICONTROL Kanban] -bord](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [De achterstand toevoegen aan de [!UICONTROL Kanban] -board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
