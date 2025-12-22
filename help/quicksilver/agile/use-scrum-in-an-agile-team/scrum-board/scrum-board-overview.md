---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Overzicht van de scrollstructuur
description: Het scorebord voor het rasterverhaal wordt weergegeven samen met de voltooiingsstatus en het uitvouwdiagram.
author: Jenny
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# [!UICONTROL Scrum] Overzicht van het board

<!-- Audited: 5/2025 -->

Het [!UICONTROL Scrum] Google-artikelbord wordt samen met de voltooiingsstatus en het uitvouwdiagram weergegeven. Deze componenten van het Geavanceerd systeem zijn beschikbaar in de volgende situaties in [!UICONTROL Adobe Workfront]:

* Op mobiele iteraties. Voor meer details over het gebruiken van de het verhaalraad van de Stijl, burndown grafiek, en voltooiingsstatus in een zuiver milieu van de Stijl (met backlogs en een herhaling), zie [ Werk in een milieu van de Stijl ](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Wanneer u een project weergeeft in een Google-weergave. Voor informatie over hoe u hefboomwerking de het verhaalraad van de Gelijkheid, burndown grafiek, en voltooiingsstatus binnen een bestaand project kunt, zie [ een project in de Gelijke Mening ](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md) leiden.

![ de iteratie van de Gelijkheid ](assets/agile-iteration-with-callouts.png)

## Layout en functies van het artikelbord

![ het verhaalbord van de Gelijkheid ](assets/agile-storyboard-callouts.png)

De whiteboard bestaat uit de volgende elementen:

* **Kolom van het Verhaal van de Ouder**: In tegenstelling tot de andere kolommen op de verhaalraad, is de [!UICONTROL Parent Story] kolom geen taakstatus, maar bestaat eerder om het even welke verhalen te huisvesten die subtaken in de herhaling of het project bevatten. Alleen bovenliggende artikelen die ten minste één subtaak op de artikelkaart hebben, kunnen in deze kolom voorkomen. De bovenliggende artikelen gaan niet van status naar status over het hele artikel.

  In een herhaling wordt deze kolom alleen op het artikelbord weergegeven wanneer een of meer artikelen op het artikelbord ten minste één subtaak bevatten die aan de volgende vereisten voldoet:

   * Toegewezen aan het zelfde team van gal zoals de oudertaak.
   * Behoort tot de herhaling.

     In een project, lijkt deze kolom wanneer een taak minstens één subtaak heeft.

     ![ de kolom van het het verhaal van de ouder ](assets/agile-parentstory-swimlane.png)

* **Statussen van de Taak**: Wijs op hoe een verhaal door de herhaling of het project vordert dat op welke statuskolom wordt gebaseerd het verhaal binnen is.

  De statussen van de taak kunnen voor het project worden aangepast door de mening van de Gelijkheid te wijzigen.

* **Waaier Lane**: Wanneer een ouderverhaal en zijn subtaken op de verhaalraad verschijnen, wordt een zwemweg gecreeerd specifiek voor het verhaal en zijn subtasks. Dit biedt een visueel onderscheid om beter te kunnen zien hoe de subtaken van een artikel zich over de hele whitepaper ontwikkelen.

  In een herhaling worden zwempaden alleen op het artikelbord weergegeven wanneer een artikel op het artikelbord ten minste één subtaak bevat die aan de volgende vereisten voldoet:

   * Toegewezen aan het zelfde team van gal zoals de oudertaak.
   * Behoort tot de herhaling.

  In een project, verschijnen de zwemwegen wanneer een taak minstens één subtaak of één oudertaak heeft.

* **Individuele Verhalen**: De individuele verhalen en de kwesties worden getoond onder om het even welke zwemwegen op de verhaalraad. Dit geeft een visueel onderscheid ten opzichte van de verhalen die deel uitmaken van een zwembaan.

## Relatie tussen subtaken en artikelen

Als een artikel subtaken bevat, kunt u geen informatie over het bovenliggende artikel zelf bijwerken (zoals punten/uren of procent voltooid). Bovendien kunt u het artikel niet over de artikelkaart verplaatsen om de status bij te werken. Alle wijzigingen die u aanbrengt in de subtaken van het artikel, worden weerspiegeld in het artikel. De gecombineerde artikelpunten of -uren voor alle subtaken bepalen de punten of uren van het bovenliggende artikel.

Als een artikel bijvoorbeeld slechts één subtaak heeft die op 4 punten wordt gewaardeerd, heeft het artikel zelf ook vier punten. Als u de waarde voor het subtaakpunt wijzigt in 3, wordt de puntwaarde van het bovenliggende artikel gewijzigd in 3. Als u een andere subtaak voor hetzelfde artikel maakt en de puntwaarde voor die subtaak instelt op 4, wordt de puntwaarde voor het artikel gewijzigd in 7 om de gecombineerde puntwaarde voor beide subtaken weer te geven.

Deze zelfde logica is op subtaken op het tweede niveau (subtaken van subtaken) van toepassing. Als subtask één of meerdere subtasks op het tweede niveau heeft, wordt subtask berekend gebaseerd op de subtaken op het tweede niveau.

## Relatie tussen de Artikelraad en de Achtergrond

De iteratieachterstand geeft alleen artikelen of subtaken weer waar u een schatting kunt instellen. Als een ouderverhaal subtaken heeft die op de verhaalraad worden getoond (omdat zij aan het zelfde team van gal worden toegewezen en tot de herhaling behoren), wordt de oudertaak niet getoond op de backlog. In deze situatie worden alleen de subtaken weergegeven op de achtergrond, terwijl de subtaken en het bovenliggende artikel worden weergegeven op de artikellijst.

Bijvoorbeeld, veronderstel dat Artikel A Subtask 1 en Subtask 2 bevat (en beide subtaken worden toegewezen aan het zelfde team van gal). In deze situatie wordt artikel A weergegeven op de whiteboard in een zwempad met Subtask 1 en Subtask 2. Nochtans, slechts worden Subtask 1 en Subtask 2 getoond in de backlog.

Deze zelfde logica is op subtaken op het tweede niveau (subtaken van subtaken) van toepassing. Als een subtask één of meerdere subtasks op het tweede niveau heeft die aan het zelfde team van gal worden toegewezen en tot de herhaling behoren, slechts wordt de subtask van het tweede niveau getoond in de backlog.

Voor meer informatie over de backlog, zie [ leiden de Agile backlog ](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
