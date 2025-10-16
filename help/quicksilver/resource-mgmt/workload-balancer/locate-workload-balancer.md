---
product-area: resource-management
keywords: werken,team,personeel,bronnen
navigation-topic: the-workload-balancer
title: De werklastbalans zoeken
description: De taakverdeler is beschikbaar voor veelvoudige projecten op het gebied van Middelen, voor een team, voor een project, en voor een gebruiker.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: e1580f7b9065fce7bb31ab0c7edb00fd2856e1df
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# De werklastbalans zoeken

U kunt de taakverdeler gebruiken om middelen voor het werk te plannen of hun beschikbaarheid en huidige toewijzingen te herzien.

U hebt op de volgende manieren toegang tot de taakverdelingsfunctie:

* Van verschillende vooraf door Adobe Workfront gedefinieerde gebieden
* Door het als dashboard aan het linkerpaneel toe te voegen

In dit artikel worden de gebieden beschreven waar u toegang kunt krijgen tot Workload Balancer.

>[!NOTE]
>
>Ongeacht de methode u gebruikt om tot de Balancer van de Werkbelasting toegang te hebben, het navigeren van het, en het beheren van middelen is identiek.
>
>Raadpleeg de volgende artikelen voor informatie over de werklastbalans en hoe u deze kunt gebruiken voor het beheren en plannen van uw bronnen voor werk:
>
>* [ Overzicht van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [ navigeer de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [ Overzicht van het toewijzen van het werk in de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [ beheer gebruikerstoewijzingen in de Balancer van de Werklast ](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan, wanneer het gebruiken van de Balancer van de Werkbelasting in het gebied van Middelen; het werk, wanneer het gebruiken van de Balancer van de Werkbelasting van een team of een project</p>
       <p><span class="preview">Opmerking: alle gebruikers hebben zonder licentievereisten toegang tot de taakverdelingsfunctie in hun eigen gebruikersprofielen.</span></p></td>
  </tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot het volgende weergeven of vergroten:</p> 
    <ul> 
     <li>Bronbeheer</li> 
     <li>Projecten</li> 
     <li>Taken</li> 
     <li>Problemen</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>Toestemmingen van de mening of hoger aan de projecten, de taken, en de kwesties</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Toegang tot werklastbalans in vooraf gedefinieerde gebieden

In de volgende secties ziet u waar u toegang kunt krijgen tot Workload Balancer in Workfront.

### Heb toegang tot de Balancer van de Werkbelasting voor veelvoudige projecten in het gebied van de Middelen

{{step1-to-resourcing}}

1. Klik **de Balancer van de Werkbelasting** in het linkerpaneel.

   ![ de Balancer van de Werkbelasting ](assets/nwe-balancer-global.png)

   In Workload Balancer wordt standaard het volgende weergegeven op basis van informatie in het gebied Bronnen:

   * **Niet toegewezen Werk**: Geen unassigned het werkpunten.
   * **Toegewezen Werk**: Alle actieve gebruikers in het systeem.

     We raden u aan filters te gebruiken wanneer u gebruikers weergeeft in het gebied Toegewezen werk. Voor meer informatie, zie [ informatie van de Filter in de Balancer van de Werklast ](../workload-balancer/filter-information-workload-balancer.md).

### Toegang tot de werklastbalans voor een team

Voor meer informatie over teams in Workfront, zie [ Overzicht van Teams ](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/teams-overview.md).

{{step1-to-team}}

De pagina van uw Home Team wordt weergegeven.

1. Klik **de Balancer van de Werkbelasting** in het linkerpaneel.

   ![ de Balancer van de Werkbelasting voor team ](assets/nwe-balancer-team-350x172.png)

   De werklastbalans van een team geeft standaard de volgende informatie weer:

   * **Niet toegewezen Werk**: Punten die aan het team worden toegewezen en niet aan gebruikers worden toegewezen.
   * **Toegewezen Werk**: Alle leden van het team met al hun taken.

     >[!TIP]
     >
     >De leden van het team zouden aan het werk ook kunnen worden toegewezen dat aan het team of aan het werk wordt toegewezen aan andere teams of rollen.

### Heb toegang tot de Balancer van de Werkbelasting voor een project

{{step1-to-projects}}

1. Klik op de naam van een project om de projectpagina te openen.
1. Klik **de Balancer van de Werkbelasting** in het linkerpaneel.

   De werklastbalans voor de projectweergave.

   ![ de Balancer van de Werklast voor Project ](assets/nwe-balancer-project-350x152.png)

   De taakverdeler van een project toont het volgende door informatie, door gebrek:

   * **Niet toegewezen Werk**: Punten van het project die aan baanrollen of teams worden toegewezen en niet aan gebruikers worden toegewezen.
   * **Toegewezen Werk**: Gebruikers die aan punten op het project worden toegewezen.

     >[!TIP]
     >
     >U kunt alle gebruikers in het systeem in plaats van slechts degenen op het project (in het Toegewezen gebied van het Werk) tonen door de Toon alle gebruikersoptie toe te laten. Voor informatie, zie [ de Balancer van de Werkbelasting ](../workload-balancer/navigate-the-workload-balancer.md) navigeren.

### Toegang tot werklastbalans voor een gebruiker

Alle gebruikers hebben toegang tot de werklastbalans op hun eigen profielen. Werklastverdelingsgegevens voor een gebruiker zijn alleen-lezen. U kunt geen werk toewijzen, werk ongedaan maken of toewijzingen op gebruikersniveau aanpassen.

Alle weergave-instellingen zijn beschikbaar voor Workload Balancer voor een gebruiker. Voor meer informatie, zie [ de Balancer van de Werkbelasting ](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

{{step1-click-profile-pic}}

1. Klik **de Balancer van de Werkbelasting** in het linkerpaneel.

   De werklastbalans voor de gebruiker wordt weergegeven.

   ![ Balancer van de Werkbelasting voor een gebruiker ](assets/workload-balancer-user.png)

   De werklastbalans van een gebruiker geeft standaard het volgende weer op basis van informatie:

   * **Toegewezen Werk**: De taken en de kwesties die aan de specifieke gebruiker worden toegewezen.

## De werklastbalans als dashboard aan het linkerdeelvenster toevoegen

U kunt de werklastbalans als een dashboard toevoegen aan het linkerdeelvenster met objecten die kunnen worden aangepast.

De meeste aanpassingen die u al op Workload Balancer hebt toegepast, blijven behouden wanneer u deze aan het linkerdeelvenster toevoegt.

1. Ga naar een van de volgende gebieden om de werklastbalans te openen:

   * Het gebied met hulpbronnen
   * Een team
   * Een project

1. Verkrijg een shareable verbinding en kopieer het aan uw klembord zoals die in [ wordt beschreven Deel de Balancer van de Werkbelasting met een verbinding ](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Creeer een dashboard met een externe pagina zoals die in [ wordt beschreven bed een externe Web-pagina in een dashboard ](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) in. Gebruik de deelbare koppeling die u in Stap 2 hebt verkregen voor de externe pagina.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Voeg een dashboard aan het linkernavigatievenster van een voorwerp toe, zoals die in [ wordt beschreven voeg een dashboard in het linkerpaneel van een voorwerp of gebied van Workfront ](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) toe om het dashboard op het douanetabblad te plaatsen.

   Wanneer u de werklastbalans opent vanuit het dashboard, kunt u deze weergeven alsof u deze rechtstreeks benadert vanuit een van de oorspronkelijke gebieden die in Stap 1 zijn vermeld.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Facultatief) deel het dashboard in een Malplaatje van de Lay-out zoals die in [ wordt beschreven Pas het linkerpaneel aan gebruikend een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->
