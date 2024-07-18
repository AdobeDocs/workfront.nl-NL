---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Een project beheren in de Google View
description: U kunt flexibele functionaliteit voor uw project gebruiken zonder de administratieve uitdagingen die agile praktijken typisch begeleiden (zoals het beheren van een teamachterstand of het creëren van herhalingen).
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 0%

---

# Een project beheren in de Google View

<!-- Audited: 2/2024 -->

U kunt flexibele functionaliteit voor uw project gebruiken zonder de administratieve uitdagingen die agile praktijken typisch begeleiden (zoals het beheren van een teamachterstand of het creëren van herhalingen).

Als u in een mobiel milieu wilt werken dat een teamachterstand gebruikt en u toestaat om herhalingen van taken op de achterstand tot stand te brengen, volg de instructies in [ Werk in een flexibel milieu ](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Huidig: Controleren of hoger</p> 
   <p>Nieuw: Medewerker of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot de volgende gebieden bewerken:</p> 
    <ul> 
     <li> <p>Projecten</p> </li> 
     <li> <p>Rapporten, dashboards, kalenders</p> </li> 
     <li> <p>Filters, weergaven, groepen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor het project</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agile-projecten begrijpen

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

* [ de functionaliteit van de Gelijkheid in een project ](#agile-functionality-in-a-project)
* [Verschillen bij gebruik van de functie Gelijk voor een project in plaats van voor een herhaling](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Functionaliteit in een project {#agile-functionality-in-a-project}

De volgende flexibele functionaliteit is beschikbaar wanneer u een project beheert in een flexibele weergave:

* Voltooiingsstatus\
  Voor meer gedetailleerde informatie over voltooiingsstatus, zie [ overzicht van de voltooiingsvoltooiingsstatus ](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Artikelbord\
  Voor meer gedetailleerde informatie over de verhaalraad, zie de [ sectie van het Bord van de Trommel ](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md).

Er zijn sommige verschillen wanneer het gebruiken van flexibele meningen op een project tegenover het werken in een zuivere agile milieu (met backlogs en herhalingen). Voor meer informatie, zie [ Verschillen wanneer het gebruiken van de Gelijke mening op een project tegenover op een herhaling ](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) in dit artikel.

### Verschillen bij gebruik van de functie Gelijk voor een project in plaats van voor een herhaling {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [ de Taken en subtasks volgen verschillende vertoningsregels in een projectGelijke mening en op de verhaalraad van een herhaling ](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [ de Achterlogboeken en de herhalingen worden niet gebruikt in de Gelijke mening ](#backlogs-and-iterations-are-not-used)
* [ de orde van de Taak wordt gehandhaafd in de Gelijke mening en kan niet worden herschikt ](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [ de Taken worden gemeten slechts in Geplande Uren op een projectlijst ](#tasks-are-measured-only-in-planned-hours)
* [ het Team van de Gelijkheid wordt niet gebruikt in een Gelijke mening ](#the-agile-team-is-not-used)
* [Elke gebruiker op het project kan het project in een verschillende mening van de Gelijkheid bekijken](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Taken en subtaken volgen verschillende weergaveregels in een projectwaaier en op de artikelboard van een herhaling {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Taken die geen bovenliggende taak of subtaak hebben, worden altijd als één artikelkaart weergegeven in de artikelboard van de weergave Gelijk.\
  Deze taken worden bijvoorbeeld als volgt weergegeven in de projectenlijstweergave:

  ![ de projectlijst van de Gelijkheid - taken zonder ouder of subtasks ](assets/agile-project-single-list-nwe.png)

  Deze taken worden als volgt weergegeven in de schakelweergave van het project:

  ![ Project schakelt mening - taken zonder ouder of subtasks ](assets/agile-project-singlecard-nwe.png)

* De bovenliggende taken die subtaken hebben, worden altijd weergegeven in de kolom **Artikelen** van de artikelboard van de Google-weergave. Subtaken worden weergegeven in de werkbalk van de bovenliggende taak.\
  Deze taken worden bijvoorbeeld als volgt weergegeven in de projectenlijstweergave:

  ![ het projectlijst van de Gelijkheid - taken met ouders en subtasks ](assets/agile-project-parent-list-nwe.png)\
  Deze taken worden als volgt weergegeven in de schakelweergave van het project:

  ![ het projectweergave van de Gelijkheid - taken met ouders en subtasks ](assets/agile-project-parent-nwe.png)

* Subtaken op het tweede niveau (subtaken van subtaken) worden weergegeven als een hangende grijze kaart van de directe bovenliggende taak.
* Subtaken op derde niveau (subtaken van subtaken van subtaken) worden nooit weergegeven in de weergave Gelijk.

#### Backlogs en herhalingen worden niet gebruikt in de weergave Geniet {#backlogs-and-iterations-are-not-used}

Wanneer het bekijken van een project in een veranderlijke mening, worden de volgende flexibele componenten niet gebruikt:

* **Achtergrond:** Geen achterstand wordt gebruikt omdat om het even welke taken in het project automatisch als verhalen worden getoond.
* **Herhalingen:** eerder dan het creëren van herhalingen om de data te bepalen wanneer het werk zal worden verwezenlijkt, worden de dagen momenteel aangewezen op de projectchronologie de werkdagen.

#### De taakvolgorde blijft behouden in de weergave Gelijk en kan niet opnieuw worden geordend {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

De volgorde waarin taken in een project worden weergegeven, blijft behouden wanneer u het project in een &#39;agile story board&#39; weergeeft.

U kunt taken in het project niet opnieuw rangschikken wanneer het bekijken van het project in een flexibele mening. Omdat het wijzigen van de taakorde andere taken kan beïnvloeden die gebiedsdelen zouden kunnen hebben, moet u het project in een standaardmening bekijken om taakorde te wijzigen.

#### De taken worden gemeten slechts in Geplande Uren op een projectlijst {#tasks-are-measured-only-in-planned-hours}

De taken op een project worden altijd gemeten in Geplande Uren.

In een herhaling kunnen taken (artikelen) in uren of punten worden gemeten.

#### Het gangbare team wordt niet gebruikt in een flexibele weergave {#the-agile-team-is-not-used}

Omdat de mobiele teams het werk op herhalingen voltooien die aan hen worden toegewezen, worden de mobiele teams niet gebruikt wanneer het bekijken van een project in een agile mening.

In plaats daarvan, worden om het even welke gebruikers op het project in feite het flexibele team voor dat project.

#### Elke gebruiker op het project kan het project in een verschillende mening van de Gelijkheid bekijken {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

In tegenstelling tot een mobiele herhaling kunnen gebruikers in een project de AGile-weergave voor zichzelf aanpassen, terwijl andere gebruikers een andere AGile-weergave gebruiken.

In een flexibele herhaling, wordt de informatie die op het agile verhaalbord (zoals statuskolommen beschikbaar) beschikbaar is bepaald op het teamniveau.

Voor informatie over hoe te om een gelijke mening aan te passen, zie [ een Gelijke mening ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [ creëren of uitgeven meningen in Adobe Workfront ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) aanpassen.

## Een project weergeven in de Google-weergave

1. Ga naar het project u in een flexibele mening, op of de taaklijst of de lijst van de kwestie wilt bekijken.
1. Klik het **pictogram van de 1} mening van de Raad ![ Raad ](assets/board-icon-for-agile-view.png).**

   De boardweergave van het project wordt standaard weergegeven.

   ![ Raad mening van project ](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Facultatief) klik **vormen** om opties voor de kolommen en de kaarten te plaatsen.

   Voor meer informatie, zie [ de kolommen van het Beheer ](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) en [ aanpassen welke gebieden op een kaart ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) worden getoond. Merk op dat u geen kolombeleid op de boardmening van een project kunt bepalen.

1. (Facultatief) klik **erfenis van het Gebruik {** om de erfenis te gebruiken behaagt mening in plaats van de bordmening.

1. (Optioneel - alleen weergave voor oudere bestanden) Als u een aangepaste, flexibele weergave hebt gemaakt of als een andere gebruiker een aangepaste, flexibele weergave heeft gemaakt en deze met u heeft gedeeld, kunt u deze weergeven in plaats van de standaardstapelweergave.

   Klik het **drop-down menu van de Mening**, dan klik de douane agile mening u wilt bekijken.

   De douane schakelt mening wordt gebruikt de volgende keer u het **Gelijke** pictogram klikt.

   Voor informatie over hoe te om een nieuwe gelijke mening tot stand te brengen, zie [ creëren en aanpassen de Gelijke meningen ](#create-and-customize-agile-views), hieronder.

   Het project wordt weergegeven in de aangepaste, flexibele weergave.

1. (Voorwaardelijk, alleen oudere, geordende weergave) Als taken in uw project andere statussen gebruiken dan &quot;Nieuw&quot;, &quot;Bezig&quot; of &quot;Voltooid&quot; (de standaardstatussen voor de Google-weergave), moet u de extra statussen toevoegen aan de geagile-weergave om taken in die statussen weer te geven.

   Als de taken zich in een status bevinden die niet wordt weergegeven op de &#39;agile story board&#39;, wordt de taak zelf niet weergegeven op de &#39;agile story board&#39; (de Percent Complete van deze taken draagt echter nog steeds bij aan de Percent Complete van alle bovenliggende taken en de Percent Complete van het algemene project).

   Om statussen aan de gelijke mening toe te voegen, of creeer een nieuwe gelijke mening of pas een bestaande gelijke mening aan, zoals die in [ wordt beschreven creëren en aanpassen Gelijke meningen ](#create-and-customize-agile-views), hieronder.

1. (Facultatief) om aan de lijstmening terug te keren, klik het **pictogram van de Lijst**.

## Eenvoudige weergaven maken en aanpassen {#create-and-customize-agile-views}

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

Net als bij standaardweergaven in Workfront kunt u bestaande flexibele weergaven aanpassen of nieuwe, flexibele weergaven maken. In tegenstelling tot standaardweergaven kunt u geen nieuwe, flexibele weergaven maken op basis van bestaande, flexibele weergaven.

Voor meer informatie over het creëren van en het aanpassen van veranderlijke meningen, zie [ creëren of aanpassen een Gelijke mening ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) sectie in het artikel [ creeert of geeft meningen in Adobe Workfront ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) uit.

## Een bestaande Google-weergave delen

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

U kunt een door u gemaakte apparaatweergave delen, net zoals u andere weergaven of filters of groepen deelt.

Voor meer informatie, zie [ een filter, mening, of groepering ](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md) delen.

## Een bestaande geanimeerde weergave verwijderen

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

U kunt een Google-weergave verwijderen op dezelfde manier als andere weergaven, filters of groepen worden verwijderd.

Voor meer informatie, zie [ filters, meningen, en groeperingen ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md) verwijderen.
