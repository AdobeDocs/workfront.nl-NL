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

Als u in een agile milieu wilt werken dat een teamachterstand gebruikt en u toestaat om herhalingen van taken op de backlog tot stand te brengen, volg de instructies in [Werken in een flexibele omgeving](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agile-projecten begrijpen

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

* [Functionaliteit in een project](#agile-functionality-in-a-project)
* [Verschillen bij gebruik van de functie Gelijk voor een project in plaats van voor een herhaling](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Functionaliteit in een project {#agile-functionality-in-a-project}

De volgende flexibele functionaliteit is beschikbaar wanneer u een project beheert in een flexibele weergave:

* Voltooiingsstatus\
  Zie voor meer informatie over de voltooiingsstatus [Overzicht van de voltooiingsstatus](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Artikelbord\
  Raadpleeg voor meer informatie over de artikelpagina de [Schuifbord](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) sectie.

Er zijn sommige verschillen wanneer het gebruiken van flexibele meningen op een project tegenover het werken in een zuivere agile milieu (met backlogs en herhalingen). Zie voor meer informatie [Verschillen bij gebruik van de functie Gelijk voor een project in plaats van voor een herhaling](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) in dit artikel.

### Verschillen bij gebruik van de functie Gelijk voor een project in plaats van voor een herhaling {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Taken en subtaken volgen verschillende weergaveregels in een projectwaaier en op de artikelboard van een herhaling](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Backlogs en herhalingen worden niet gebruikt in de weergave Geniet](#backlogs-and-iterations-are-not-used)
* [De taakvolgorde blijft behouden in de weergave Gelijk en kan niet opnieuw worden geordend](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [De taken worden gemeten slechts in Geplande Uren op een projectlijst](#tasks-are-measured-only-in-planned-hours)
* [Het gangbare team wordt niet gebruikt in een flexibele weergave](#the-agile-team-is-not-used)
* [Elke gebruiker op het project kan het project in een verschillende mening van de Gelijkheid bekijken](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Taken en subtaken volgen verschillende weergaveregels in een projectwaaier en op de artikelboard van een herhaling {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Taken die geen bovenliggende taak of subtaak hebben, worden altijd als één artikelkaart weergegeven in de artikelboard van de weergave Gelijk.\
  Deze taken worden bijvoorbeeld als volgt weergegeven in de projectenlijstweergave:

  ![Agile projectlijst - taken zonder ouder of subtaken](assets/agile-project-single-list-nwe.png)

  Deze taken worden als volgt weergegeven in de schakelweergave van het project:

  ![Projectweergave - taken zonder bovenliggende of subtaken](assets/agile-project-singlecard-nwe.png)

* De taken van de ouder die subtaken hebben worden altijd getoond in **Artikelen** in de artikellijst van de weergave Gelijk. Subtaken worden weergegeven in de werkbalk van de bovenliggende taak.\
  Deze taken worden bijvoorbeeld als volgt weergegeven in de projectenlijstweergave:

  ![Agile projectlijst - taken met ouders en subtaken](assets/agile-project-parent-list-nwe.png)\
  Deze taken worden als volgt weergegeven in de schakelweergave van het project:

  ![Een flexibele projectweergave - taken met ouders en subtaken](assets/agile-project-parent-nwe.png)

* Subtaken op het tweede niveau (subtaken van subtaken) worden weergegeven als een hangende grijze kaart van de directe bovenliggende taak.
* Subtaken op derde niveau (subtaken van subtaken van subtaken) worden nooit weergegeven in de weergave Gelijk.

#### Backlogs en herhalingen worden niet gebruikt in de weergave Geniet {#backlogs-and-iterations-are-not-used}

Wanneer het bekijken van een project in een veranderlijke mening, worden de volgende flexibele componenten niet gebruikt:

* **Backlog:** Geen achterstand wordt gebruikt omdat om het even welke taken in het project automatisch als verhalen worden getoond.
* **Herhalingen:** In plaats van herhalingen te maken om de datums te bepalen waarop het werk wordt uitgevoerd, worden de dagen die momenteel op de projecttijdlijn staan, de werkdagen.

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

Voor informatie over het aanpassen van een Tegelweergave raadpleegt u [Een eenvoudige weergave maken of aanpassen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Weergaven maken of bewerken in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Een project weergeven in de Google-weergave

1. Ga naar het project u in een flexibele mening, op of de taaklijst of de lijst van de kwestie wilt bekijken.
1. Klik op de knop **Boekhouding** pictogram ![Bordebord, pictogram](assets/board-icon-for-agile-view.png).

   De boardweergave van het project wordt standaard weergegeven.

   ![Weergave van het project door de raad](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Optioneel) Klik op **Configureren** om opties voor de kolommen en kaarten in te stellen.

   Zie voor meer informatie [Bordkolommen beheren](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) en [Aanpassen welke velden worden weergegeven op een kaart](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Merk op dat u geen kolombeleid op de boardmening van een project kunt bepalen.

1. (Optioneel) Klik op **Oudere pagina gebruiken** gebruiken in plaats van de weergave board.

1. (Optioneel - alleen weergave voor oudere bestanden) Als u een aangepaste, flexibele weergave hebt gemaakt of als een andere gebruiker een aangepaste, flexibele weergave heeft gemaakt en deze met u heeft gedeeld, kunt u deze weergeven in plaats van de standaardstapelweergave.

   Klik op de knop **Weergave** en klikt u op de aangepaste gerangschikte weergave die u wilt weergeven.

   De volgende keer dat u op de knop **Agile** pictogram.

   Voor informatie over het maken van een nieuwe, flexibele weergave raadpleegt u [Eenvoudige weergaven maken en aanpassen](#create-and-customize-agile-views), hieronder.

   Het project wordt weergegeven in de aangepaste, flexibele weergave.

1. (Voorwaardelijk, alleen oudere, geordende weergave) Als taken in uw project andere statussen gebruiken dan &quot;Nieuw&quot;, &quot;Bezig&quot; of &quot;Voltooid&quot; (de standaardstatussen voor de Google-weergave), moet u de extra statussen toevoegen aan de geagile-weergave om taken in die statussen weer te geven.

   Als de taken zich in een status bevinden die niet wordt weergegeven op de &#39;agile story board&#39;, wordt de taak zelf niet weergegeven op de &#39;agile story board&#39; (de Percent Complete van deze taken draagt echter nog steeds bij aan de Percent Complete van alle bovenliggende taken en de Percent Complete van het algemene project).

   Als u statussen wilt toevoegen aan de stapelweergave, maakt u een nieuwe, flexibele weergave of past u een bestaande, flexibele weergave aan, zoals beschreven in [Eenvoudige weergaven maken en aanpassen](#create-and-customize-agile-views), hieronder.

1. (Optioneel) Als u wilt terugkeren naar de lijstweergave, klikt u op de knop **Lijst** pictogram.

## Eenvoudige weergaven maken en aanpassen {#create-and-customize-agile-views}

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

Net als bij standaardweergaven in Workfront kunt u bestaande flexibele weergaven aanpassen of nieuwe, flexibele weergaven maken. In tegenstelling tot standaardweergaven kunt u geen nieuwe, flexibele weergaven maken op basis van bestaande, flexibele weergaven.

Voor meer informatie over het maken en aanpassen van flexibele weergaven raadpleegt u de [Een eenvoudige weergave maken of aanpassen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in het artikel [Weergaven maken of bewerken in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Een bestaande Google-weergave delen

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

U kunt een door u gemaakte apparaatweergave delen, net zoals u andere weergaven of filters of groepen deelt.

Zie voor meer informatie [Een filter, weergave of groep delen](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Een bestaande geanimeerde weergave verwijderen

>[!NOTE]
>
>Deze sectie is alleen van toepassing op de oudere Agile-weergave, niet op de weergave in de kaart van een project.

U kunt een Google-weergave verwijderen op dezelfde manier als andere weergaven, filters of groepen worden verwijderd.

Zie de klasse [Filters, weergaven en groepen verwijderen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
