---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Overzicht van de planningsgebieden
description: De volgende secties beschrijven waar u tot het het plannen gebied binnen Adobe Workfront kunt toegang hebben, evenals de functionaliteit beschikbaar in het het plannen gebied.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Overzicht van de planningsgebieden

>[!IMPORTANT]
>  
><span class="preview">De planningsfunctionaliteit die in dit artikel wordt beschreven, is vanaf de release 23.1 in januari 2023 vervangen en uit Adobe Workfront verwijderd.   </span>
>  
> <span class="preview"> Dit artikel wordt ook verwijderd kort na de release van 23.1, begin 2023. Op dit moment raden we u aan eventuele bladwijzers dienovereenkomstig bij te werken. </span>
> 
><span class="preview"> U kunt de werklastbalans nu gebruiken om werk voor uw bronnen te plannen. </span>
>  
> <span class="preview">Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie de sectie [De werklastbalans](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--  

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


De volgende secties beschrijven waar u tot het het plannen gebied binnen Adobe Workfront kunt toegang hebben, evenals de functionaliteit beschikbaar in het het plannen gebied.

## Workfront-gebieden waar u bronnen kunt plannen

In Workfront kunt u bronnen plannen in de volgende gebieden:

* **Voor om het even welke projecten waarvoor u de middelmanager bent** (van de **Planning** gebied) Het plannende gebied in Workfront laat middelmanagers toe om middeltaken over veelvoudige projecten te maken.

* **Voor een individueel project wanneer u een lid van het projectteam bent** (van de **Planning** gebied van een project):

   Het plannende gebied binnen een project laat leden van het projectteam toe om het werk van het project aan gebruikers op het projectteam toe te wijzen.

* **Voor een individueel team bent u lid van** (van de **Schema** sectie van het team) De plannende sectie in een team laat teamleden toe om werk toe te wijzen dat reeds aan het team van veelvoudige projecten aan individuele teamleden wordt toegewezen.

## Beschikbare functies in het planningsgebied

In het planningsgebied worden taken en problemen en de huidige bronnentoewijzingen weergegeven.\
![resource_Scheduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Gereedschappen voor filteren en wisselen](#filter-and-swap-tools)
* [Datumselectie](#date-selection)
* [Niet toegewezen gebied](#unassigned-area)
* [Gebruikers en rollen](#users-and-roles)
* [Tijdlijn plannen](#scheduling-timeline)

### Gereedschappen voor filteren en wisselen {#filter-and-swap-tools}

* **Filter:** Hiermee kunt u de inhoud filteren die op de tijdlijn van het plannen wordt weergegeven. Ga voor meer informatie over het gebruik van het gereedschap Filter naar [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Gereedschap Omwisselen:** (Beschikbaar slechts wanneer het plannen van middelen voor projecten van het Plannende lusje of het Doelen lusje) laat u toe om, gebruikers aan taken over veelvoudige projecten snel toe te wijzen ruilen of unassign. Zie voor meer informatie [Niet-toegewezen taken en problemen handmatig toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Datumselectie {#date-selection}

U kunt het datumbereik aanpassen waarvoor gegevens op de tijdlijn van de planning worden weergegeven. Standaard is het datumbereik 2 weken (14 opeenvolgende dagen, inclusief weekends) vanaf de huidige dag.

### Niet toegewezen gebied {#unassigned-area}

* [Wanneer het plannen van middelen als middelmanager (voor veelvoudige projecten in het Plannende gebied)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Wanneer het plannen van middelen als lid van het projectteam (van een project)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Wanneer het plannen van middelen als teamlid (van een team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Wanneer het plannen van middelen als middelmanager (voor veelvoudige projecten in het Plannende gebied) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

De **Niet toegewezen** worden alleen die taken en problemen weergegeven die aan alle volgende criteria voldoen:

* Niet toegewezen aan een gebruiker.
* Niet toegewezen aan een team.\
   Als de taak of de kwestie aan een team wordt toegewezen, wordt het nog getoond in **Niet toegewezen** gebied als de taak of de kwestie ook aan een rol naast de teamtaak wordt toegewezen.\
   Als taken of problemen aanvullende taakroltoewijzingen hebben die niet worden uitgevoerd door een gebruiker, worden deze ook weergegeven.\
   Een taak wordt bijvoorbeeld toegewezen aan drie taakrollen: Designer, Product Manager en Developer. U wijst deze taak toe aan gebruiker A die een Designer-taakrol heeft, en aan gebruiker B die een productmanager-taakrol heeft. In dit scenario is de taak nog steeds zichtbaar in het niet-toegewezen gebied op de tijdlijn van de planning, omdat de de baanrol van de Ontwikkelaar niet aan een gebruiker wordt toegewezen.

#### Wanneer het plannen van middelen als lid van het projectteam (van een project) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

De **Niet toegewezen** boven aan de tijdlijn worden taken en problemen weergegeven die aan de volgende criteria voldoen:

* Gekoppeld aan het project maar niet toegewezen aan om het even welke gebruikers op het projectteam.\
   De taken die met het project worden geassocieerd en aan een gebruiker op het projectteam worden toegewezen worden getoond in de rij van de gebruiker aan wie de taken worden toegewezen.
* Gekoppeld aan het project maar toegewezen aan een lid dat zich niet in het projectteam bevindt.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **Wanneer het plannen van middelen als teamlid (van een team)** {#when-scheduling-resources-as-a-team-member-from-a-team}

De **Niet toegewezen** boven aan de tijdlijn worden taken en problemen weergegeven die aan de volgende criteria voldoen:

* Toegewezen aan het team en aan geen andere gebruikers op het team.\
   De taken die zowel aan het team als aan een gebruiker op het team worden toegewezen worden getoond in de rij van de gebruiker aan wie de taken worden toegewezen.
* Toegewezen zowel aan het team als aan een gebruiker die geen lid van het team is.

### Gebruikers en rollen {#users-and-roles}

* [Wanneer het plannen van middelen als middelmanager (voor veelvoudige projecten in het Plannende gebied)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Wanneer het plannen van middelen als lid van het projectteam (van een project)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Wanneer het plannen van middelen als teamlid (van een team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Wanneer het plannen van middelen als middelmanager (voor veelvoudige projecten in het Plannende gebied) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Om het even welke gebruikers die verkiesbaar zijn om één van de niet toegewezen taken te worden toegewezen worden gevestigd onder **Niet toegewezen** gebied. De gebruikers zijn beschikbaar op de het plannen chronologie om een taak of kwestie in de volgende omstandigheden toe te wijzen:

* Door gebrek, worden de gebruikers getoond op de het plannen chronologie slechts wanneer zij een baanrol hebben die in het systeem wordt bepaald (of de primaire baanrol of een secundaire baanrol), en die baanrol past de baanrol aan die aan een taak of een kwestie wordt toegewezen die momenteel in wordt getoond **Niet toegewezen** op de tijdlijn van de planning. U kunt deze functionaliteit onbruikbaar maken zodat taken en kwesties worden toegewezen aan om het even welke gebruiker, ongeacht of die gebruiker een rol heeft die op hun gebruikersprofiel wordt bepaald die de roltaak van de taak of kwestie aanpast die aan hen wordt toegewezen. Zie voor meer informatie [Gebruikerstoewijzingen ongeacht rol en groepslidmaatschap in de planningsgebieden toestaan](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   Een gebruiker en de aan de gebruiker toegewezen taken kunnen meerdere keren op de tijdlijn van de planning verschijnen als de gebruiker meerdere taakrollen heeft toegewezen in het Workfront-systeem.\
   De gebruikers blijven op de het plannen chronologie nadat zij een taak of een kwestie worden toegewezen, zelfs als er geen resterende taken of kwesties zijn die een passende roltoewijzing hebben. Zo kunt u de benodigde wijzigingen aanbrengen nadat deze zijn toegewezen.\
   Als de taak niet aan een baanrol wordt toegewezen, worden alle gebruikers die aan de filtervereisten voldoen getoond. Zie voor meer informatie over het filter [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* Zij zijn aangewezen in het **Gebruikers** in het **Filter** tab.\
   Zie voor meer informatie over het filter [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   Wanneer het plannen van middelen voor een team (op het Werken aan lusje), wordt de teamtaak ook getoond.

Eventuele andere taken of problemen die aan deze gebruikers zijn toegewezen, worden ook op de tijdlijn weergegeven.

U kunt het niveau zien waarin gebruikers worden toegewezen op een bepaalde dag, zoals beschreven in [Gebruikerstoewijzingen beheren in de planningsgebieden](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Taken waarvoor u ten minste geen Contribute-machtigingen hebt, worden als een grijze balk weergegeven op de tijdlijn van de planning.

#### Wanneer het plannen van middelen als lid van het projectteam (van een project) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Elk lid van het team wordt altijd getoond op de het plannen chronologie, ongeacht de taken van de baanrol van de gebruikers en de roltaken van de taken in Unassigned gebied.

Als een gebruiker meerdere taakrollen heeft gedefinieerd in het systeem, wordt de gebruiker meerdere keren weergegeven op de tijdlijn van de planning wanneer aan een van de volgende criteria wordt voldaan:

* Er worden taken of problemen weergegeven in het dialoogvenster **Niet toegewezen** gebied dat aan de baanrollen wordt toegewezen die met de gebruiker worden geassocieerd.
* Er zijn taken of kwesties op het project die baanrollen hebben toegewezen, en die taken of kwesties worden toegewezen aan een gebruiker die die baanrol heeft die in het systeem wordt bepaald.

#### Wanneer het plannen van middelen als teamlid (van een team) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Elk lid van het team wordt altijd getoond op de het plannen chronologie, ongeacht de taken van de baanrol van de gebruikers en de roltaken van de taken in Unassigned gebied.

U kunt het niveau zien waarin gebruikers worden toegewezen op een bepaalde dag, zoals beschreven in [Gebruikerstoewijzingen beheren in de planningsgebieden](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Taken waarvoor u niet ten minste Contribute-machtigingen hebt om als een grijze balk op de tijdlijn van de planning weer te geven.

### Tijdlijn plannen {#scheduling-timeline}

* **Standaardinhoud:** Standaard alle taken die voldoen aan de vereisten die in de sectie zijn gedefinieerd [Voorwaarden voor taken en uitgaven](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) in de [Aan de slag met Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) artikel op alle projecten met de status van Huidig wordt getoond op de het plannen chronologie.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Om aan te passen wat op de het plannen chronologie wordt getoond, met inbegrip van het tonen van kwesties en projecten met een verschillende status, gebruik de filter, zoals die in [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Een maximum van 10 taken per dag wordt getoond voor een bepaalde gebruiker. U kunt de lijst uitvouwen om alle taken weer te geven die momenteel aan die gebruiker zijn toegewezen.

* **Bovenliggende taken:** Of bovenliggende taken op de tijdlijn worden weergegeven, is afhankelijk van verschillende instellingen. Voor meer informatie, zie de sectie &quot;vormen of de oudertaken op de het plannen chronologie&quot;worden getoond in [Instellingen configureren in de planningsgebieden](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artikel.

* **Kleurcodering:** Taken en problemen in de tijdlijn van de planning worden in kleur gecodeerd volgens het project waartoe ze behoren. U kunt de kleur die aan een specifiek project is gekoppeld, niet aanpassen.

   Wanneer het plannen van het werk voor teams (van het het Stafelen lusje), worden de kleuren gebruikt slechts als **Alle gebruikerstaken tonen** is ingeschakeld. Voor meer informatie, zie de sectie &quot;vormen of de oudertaken op de het plannen chronologie&quot;worden getoond in [Instellingen configureren in de planningsgebieden](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artikel.

* **Taakduur:** De duur van de taak wordt vertegenwoordigd op de chronologie voor elke taak (de taak overspant fysisch over het aantal dagen gelijk aan de duur). U kunt de taakduur niet vanaf de tijdlijn van de planning aanpassen.

* **Tijd uit:** De tijd van wordt vertegenwoordigd op de het plannen chronologie door een lichtgrijze indicator in de kolom op de dag waarvoor de tijd van voor een bepaalde gebruiker gepland is.\
   De tijd van wordt gevormd voor elke gebruiker die op de volgende informatie wordt gebaseerd:

   De persoonlijke kalender van de gebruiker. Voor meer informatie over de persoonlijke kalender, zie [Persoonlijke tijd in Adobe Workfront configureren](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   Het programma dat aan de gebruiker wordt toegewezen. Dit zou het standaardprogramma of een douaneschema kunnen zijn. Voor meer informatie over programma&#39;s, zie [Een schema maken](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Weekends:** Weekends worden op de tijdlijn van de planning weergegeven als lichtgrijze arcering op zaterdagen en zondag. De dagen van de week die als weekends op de het plannen chronologie worden geplaatst zijn niet configureerbaar. U kunt gebruikers plannen voor het werken in het weekend.
