---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Aan de slag met Resource Scheduling
description: Wanneer u de functie voor het plannen van bronnen in Adobe Workfront gebruikt, kunt u gemakkelijker taken en problemen toewijzen aan de juiste gebruikers.
author: Alina
feature: Resource Management
exl-id: 1858f6af-92e7-4d32-a401-40004eeb0cef
source-git-commit: f2297deed0640bbdad93cf2980e33afd7d1f23a0
workflow-type: tm+mt
source-wordcount: '2370'
ht-degree: 0%

---

# Aan de slag met Resource Scheduling

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(NOTE: LINKED TO THE PRODUCT FROM: ALL SCHEDULING TOOLS: GLOBAL, TEAM, PROJECT STAFFING *** LINKED TO LOTS OF ARTICLES, AS WELL!) </p>
<p>(NOTE: Alina: this article should be divided in multiple articles, but CAREFULLY because some sections are linked to the UI)</p>
</div>
-->

Wanneer u de functie voor het plannen van bronnen in Adobe Workfront gebruikt, kunt u gemakkelijker taken en problemen toewijzen aan de juiste gebruikers. U kunt bepalen welke gebruikers in staat zijn om de taak of kwestie te voltooien, rekening houdend zowel met de baanrol als met de beschikbaarheid van de gebruiker.

In de volgende secties vindt u meer informatie over het gebruik van de planningsgebieden in Workfront.

## Vereisten voor het gebruiken van de het plannen hulpmiddelen in Workfront

>[!IMPORTANT]
>
>De voorwaarden die in dit artikel worden beschreven, gelden alleen voor de planningsgebieden van Workfront. Voor informatie over beste praktijken voor het gebruiken van de Balancer van de Werkbelasting, zie [Overzicht van de werklastbalans](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Als u de functionaliteit voor het plannen van bronnen in Workfront met succes wilt gebruiken, moet u er eerst voor zorgen dat u, uw projecten en uw taken en problemen aan de volgende voorwaarden voldoen:

* [Voorwaarden voor gebruikers](#user-prerequisites)
* [Voorwaarden voor projecten](#project-prerequisites)
* [Voorwaarden voor taken en uitgaven](#task-and-issue-prerequisites)

### Voorwaarden voor gebruikers {#user-prerequisites}

U kunt de middelen gebruiken die hulpmiddelen plannen beschikbaar bij of het Plannende lusje, van het het Vallen lusje, of van het Werken aan lusje wanneer elk van de volgende voorwaarden worden voldaan:

**Bij het plannen van middelen als middelmanager (van het Plannende lusje):**

* U wordt aangewezen als Manager van het Middel voor de projecten waarvoor u middelen wilt beheren.

   Voor meer informatie over het aanwijzen van middelmanagers voor een project, zie het artikel [Bronbeheerders aanwijzen voor een project of sjabloon](../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md).

* U bent een gebruiker met een licentie voor abonnementen.

Door gebrek, worden de gebruikers getoond op de het plannen chronologie slechts wanneer zij een baanrol hebben die in het systeem wordt bepaald (of de primaire baanrol of een secundaire baanrol), en die baanrol past de baanrol aan die aan een taak of een kwestie wordt toegewezen die momenteel in wordt getoond **Niet toegewezen** op de tijdlijn van de planning. U kunt deze functionaliteit onbruikbaar maken zodat taken en kwesties worden toegewezen aan om het even welke gebruiker, ongeacht of die gebruiker een rol heeft die op hun gebruikersprofiel wordt bepaald die de roltaak van de taak of kwestie aanpast die aan hen wordt toegewezen. Zie het artikel voor meer informatie [Gebruikerstoewijzingen ongeacht rol en groepslidmaatschap in de planningsgebieden toestaan](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).

Door gebrek, kunnen de taken slechts aan gebruikers worden gemaakt die een rol hebben die op hun gebruikersprofiel wordt bepaald dat de roltaak van de taak of de kwestie aanpast die aan hen wordt toegewezen.

**Wanneer het plannen van middelen als lid van het projectteam (van het het Personelen lusje in een project):**

* U hebt machtigingen om het project weer te geven, bij te dragen of te beheren
* U hebt een abonnement of werkvergunning

<!--
<note type="note">  If Workfront has not removed the Use New Scheduling Area option from your Scheduling settings, users must have a Plan license and Manage permissions to the project to view the Scheduling timeline. For more information about the removal of the Use New Scheduling Area option, see the article
<a href="../../product-announcements/announcements/announcement-archive/replace-flash-tools.md" class="MCXref xref">Replacement of Flash-based tools in Adobe Workfront</a>.
</note>
-->

**Wanneer het plannen van middelen als teamlid (van het Werken aan lusje):**

* U bent lid van het team\
   Alle leden van het team worden weergegeven op de geplande tijdlijn. Taken en kwesties die aan het team worden toegewezen en niet aan een gebruiker worden toegewezen worden getoond in het Unassigned gebied. De taak en de kwesties die aan het team en aan een gebruiker op het team worden toegewezen worden getoond in de rij van de gebruiker aan wie zij worden toegewezen.

### Voorwaarden voor projecten {#project-prerequisites}

De projectvereisten die in deze sectie worden beschreven zijn slechts van toepassing wanneer het plannen van middelen als middelmanager van de het plannen chronologie.

De projecten u beheert moeten in één van de volgende statussen (of een status zijn die met één van deze statussen) vergelijkt opdat de het werkpunten van die projecten op de het plannen chronologie worden getoond: Planning, Huidige of Goedgekeurd. Door gebrek, slechts worden de projecten in de Huidige status getoond.

Raadpleeg het artikel voor meer informatie over de status van projecten [Een status maken of bewerken](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! I assume this doesn't apply when using the Staffing tab on a single project? The project can be in whatever status?]) </p>
-->

### Voorwaarden voor taken en uitgaven {#task-and-issue-prerequisites}

Om het meest effectief te zijn wanneer het gebruiken van de middelen het plannen hulpmiddelen in Workfront, zorg ervoor dat de taken en de kwesties in uw systeem de volgende gedefinieerde criteria hebben:

* Duur
* Geplande begindatums
* Geplande uren\
   Geplande uren zijn vereist om de gebruikerstoewijzingen te wijzigen, zoals beschreven in het artikel [Gebruikerstoewijzingen beheren in de planningsgebieden](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

   >[!NOTE]
   >
   >Het Geplande gebied van Uren in het Middel dat kaart plant toont eigenlijk de som alle workPerDay waarden, niet de Geplande Uren op de taak. De waarden workPerDay worden berekend door de Geplande waarde van Uren door de Duur van de Taak te delen. Voor Duur niet-nul, passen de waarden gewoonlijk de Geplande Uren van de taak aan, hoewel sommige kleine discrepanties toe te schrijven aan het rond maken konden gebeuren. Wanneer een Duur 0 dagen is, worden de geplande uren 0 uur weergegeven.

* Roltoewijzingen

## Informatie weergeven in de planningsgebieden

* [Informatie zoeken en weergeven in de planningsgebieden](#locate-and-view-information-in-the-scheduling-areas)
* [Brontoewijzingen en details weergeven](#view-resource-assignments-and-details)
* [Taken en problemen in de planningsgebieden minimaliseren](#minimize-tasks-and-issues-on-the-scheduling-areas)
* [Het datumbereik van de planningsgebieden aanpassen](#adjust-the-date-range-of-the-scheduling-areas)

### Informatie zoeken en weergeven in de planningsgebieden {#locate-and-view-information-in-the-scheduling-areas}

Afhankelijk van waar u middelen wilt plannen, kunt u tot de Plannende chronologie in de volgende gebieden van Workfront toegang hebben:

* Voor veelvoudige projecten, in het Plannende gebied
* Voor een project in de Plannende sectie
* Voor een team, in de sectie van het Programma

1. Ga naar de het plannen chronologie voor veelvoudige projecten, voor een individueel project, of voor een team:

   * **Voor meerdere projecten**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
   * **Voor een afzonderlijk project**: Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.
   * **Voor een team**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Teams**, selecteert u een team en klikt u op **Werklastverdeling** in het linkerdeelvenster selecteert u vervolgens **Planning** in het keuzemenu linksboven.

1. (Optioneel) Klik op de knop **Volledig scherm** in de rechterbovenhoek van de tijdlijn van de planning.\
   ![planning_fullscreen_enter.png](assets/scheduling-fullscreen-enter.png)\
   De plantijdlijn wordt weergegeven in de modus Volledig scherm. Wanneer de tijdlijn van de planning in de modus Volledig scherm wordt weergegeven, neemt de tijdlijn van de planning het volledige scherm in beslag. alle andere informatie is verborgen (met inbegrip van om het even welk team of projectinformatie, de Globale Bar van de Navigatie, en browser informatie).

1. (Optioneel) Voer een van de volgende twee handelingen uit om de modus Volledig scherm af te sluiten:

   * Klik op de knop **Volledig scherm** pictogram.
   * Druk op Esc.

### Brontoewijzingen en details weergeven {#view-resource-assignments-and-details}

U kunt de huidige brontoewijzingen en andere details over individuele taken en kwesties op de geplande chronologie bekijken.

1. Ga naar de het plannen chronologie voor veelvoudige projecten, voor een individueel project, of voor een team:

   * **Voor meerdere projecten**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
   * **Voor een afzonderlijk project**: Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.
   * **Voor een team**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Teams**, selecteert u een team en klikt u op **Werklastverdeling** in het linkerdeelvenster selecteert u vervolgens **Planning** in het keuzemenu linksboven.

1. (Optioneel) Als u wilt aanpassen welke inhoud op de tijdlijn van de planning wordt weergegeven, maakt u een filter, zoals beschreven in [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
1. Vouw een taak of kwestie uit om de volgende informatie te bekijken:

   * **Project:** De naam en de verbinding met het project waar de taak verblijft.

   * **Datums:** Het begin op en Verwacht op data verbonden aan de taak.

   * **Geplande uren:** Het aantal geplande uren dat aan de taak is gekoppeld.\
      Geplande uren worden alleen weergegeven als de taak is toegewezen aan een gebruiker- of taakrol.

   * **Voorgangspictogram:** Alle voordecessors die aan de taak zijn gekoppeld. Het voorgangspictogram wordt alleen weergegeven als er voorgangers aan de taak zijn gekoppeld. Het voorgangerpictogram is groen wanneer de voorganger is voltooid en de taak klaar is om te worden bewerkt.

   * **Toewijzingen:** Om het even welke gebruiker of baanroltaken verbonden aan de taak. Taken worden tussen haakjes weergegeven naast de gebruikerstoewijzing.\
      Teamtoewijzingen worden niet weergegeven.\
      Als u Contribute toegang hebt tot de taak of uitgave, kunt u de uren wijzigen waarvoor gebruikers op elke dag binnen de taak of de uitgifteduur worden toegewezen. Raadpleeg het artikel voor meer informatie over het wijzigen van gebruikerstoewijzingen [Gebruikerstoewijzingen beheren in de planningsgebieden](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

### Taken en problemen in de planningsgebieden minimaliseren {#minimize-tasks-and-issues-on-the-scheduling-areas}

Door taken en problemen te minimaliseren, kunt u gebruikerstoewijzingen voor een groot aantal gebruikers op één scherm bekijken.\
Alle taken en problemen in de tijdlijn van de planning worden standaard geminimaliseerd.

Wanneer taken en problemen worden geminimaliseerd, kunt u:

* Taakduur weergeven
* Projectkleur weergeven
* Taken vanuit het niet-toegewezen gebied toewijzen aan gebruikers op de tijdlijn van de planning

Wanneer taken en problemen worden geminimaliseerd, kunt u niet:

* Taaknamen weergeven
* Taken slepen die al aan een gebruiker zijn toegewezen en opnieuw toewijzen
* Taken uitvouwen om details weer te geven

Als u de instelling Totalen tonen voor Daily Planned Hours inschakelt, kunt u alleen:

* Bekijk het totaal van de geplande uren per dag voor elke gebruiker.

Wanneer u taken en problemen minimaliseert zoals beschreven in deze sectie, worden die veranderingen getoond slechts voor u. Taken en problemen blijven geminimaliseerd totdat u ze uitbreidt of totdat u de browsersessie beëindigt. (Als u de pagina vernieuwt, worden geminimaliseerde taken en uitgaven niet teruggezet naar een uitgevouwen status.)

Op de plannende chronologie, kunt u taken en kwesties minimaliseren die voor individuele gebruikers, voor baanrollen, of voor alle gebruikers worden getoond.

* [Taken en problemen voor individuele gebruikers minimaliseren](#minimize-tasks-and-issues-for-individual-users)
* [Taken en problemen voor een taakrol minimaliseren](#minimize-tasks-and-issues-for-a-job-role)
* [Taken en problemen voor alle gebruikers minimaliseren](#minimize-tasks-and-issues-for-all-users)

#### Taken en problemen voor individuele gebruikers minimaliseren {#minimize-tasks-and-issues-for-individual-users}

1. Klik op het invoegpunt naast de gebruiker op de tijdlijn voor de planning waarvan u de taken en problemen wilt minimaliseren.\
   ![plannen_minimize_gebruiker.png](assets/scheduling-minimize-user-350x137.png)\
   De manier waarop taken worden uitgevoerd en de uitgave wordt weergegeven, is afhankelijk van de volgende instellingen:

   * Als u de optie **Totalen tonen voor daggeplante uren** de volgende voorwaarden zijn van toepassing:

      * Alleen geplande uren voor weergave door de gebruiker
      * Taken en problemen zijn verborgen
   * Als u de optie **Totalen tonen voor daggeplante uren** taken en problemen voor de gebruiker worden geminimaliseerd.\
      ![RS_user_collapse__1_.png](assets/rs-user-collapsed--1--350x152.png)


#### Taken en problemen voor een taakrol minimaliseren {#minimize-tasks-and-issues-for-a-job-role}

U kunt taken en problemen minimaliseren voor alle gebruikers die aan een specifieke taakrol zijn gekoppeld.

1. Klik op het invoegpunt naast de taakrol in de tijdlijn voor het plannen met de gebruikers wier taken en problemen u wilt minimaliseren.\
   ![plannen_minimize_groep.png](assets/scheduling-minimize-group-350x137.png)\
   De taken en de kwesties voor alle gebruikers verbonden aan die rol worden geminimaliseerd als u onbruikbaar maakt **Totalen tonen voor daggeplante uren** instellen.\
   Taken en problemen zijn verborgen en alleen de geplande uren voor de gebruikers worden weergegeven als u deze instelling inschakelt.\
   ![RS_rol_samengevouwen__1_.png](assets/rs-role-collapsed--1--350x125.png)

#### Taken en problemen voor alle gebruikers minimaliseren {#minimize-tasks-and-issues-for-all-users}

1. Klikken **Alles samenvouwen** boven aan het gebied Gebruikers en rollen.\
   ![vindescheduling_samenvouwen.png](assets/resourcescheduling-collapseall-350x261.png)\
   of\
   Klik op het invoegpunt naast een gebruiker- of taakrol op de tijdlijn van de planning terwijl u Shift ingedrukt houdt.\
   ![](assets/scheduling-minimize-user-350x137.png)\
   Taken en problemen voor alle gebruikers en rollen worden geminimaliseerd als u de **Totalen tonen voor daggeplante uren** en taken en problemen worden verborgen als u deze inschakelt.\
   Als de **Totalen tonen voor daggeplante uren** is alleen ingeschakeld voor de Geplande uren die door de gebruikers worden weergegeven. Taken en problemen blijven geminimaliseerd voor het niet-toegewezen gebied.\
   ![RS_all_collapse__1_.png](assets/rs-all-collapsed---1--350x102.png)

### Het datumbereik van de planningsgebieden aanpassen {#adjust-the-date-range-of-the-scheduling-areas}

Standaard worden 14 opeenvolgende dagen (inclusief weekends) weergegeven op de tijdlijn van de planning, te beginnen met de huidige dag.

Gebruik een van de volgende opties om het datumbereik te wijzigen waarvoor gegevens worden weergegeven op de tijdlijn van de planning:

* **Opties datumbereik:** Klik op het huidige datumbereik en selecteer het aantal weken dat u wilt weergeven op de tijdlijn. U kunt Dag (enige dag), 1 week (7 dagen), 2 weken (14 dagen), 3 weken (21 dagen), 4 weken (28 dagen) of 6 weken (42 dagen) tonen.\
   Houd rekening met het volgende wanneer u het datumbereik van de tijdlijn van de planning aanpast:

   * De opties voor het datumbereik die u selecteert, blijven behouden wanneer u de tijdlijn voor de planning weer bezoekt.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! Not sure if this is going to apply to all 3 scheduling areas...]) </p>   
     -->

   * Wanneer u de planningtijdlijn in de Dagweergave bekijkt, worden gebruikerstoewijzingen niet weergegeven.\
      ![resource_daterange_zoom.png](assets/resource-daterange-zoom-350x227.png)

* **Kalender:** Klik op het huidige datumbereik en klik vervolgens op de dag voor of na de huidige dag. De tijd tussen de huidige dag en de geselecteerde dag is het nieuwe bereik.\
   ![resource_daterange.png](assets/resource-daterange-350x227.png)

* **Vandaag:** Klik op deze optie om de huidige dag weer te geven. De huidige dag wordt dan getoond uiterst links van de datumwaaier.\
   Klik op de pijl naar links en naar rechts om eerdere of toekomstige datums weer te geven.

   >[!NOTE]
   >
   >Het tijdkader dat u selecteert, blijft behouden wanneer u de pagina vernieuwt.

   ![resource_daterange_today.png](assets/resource-daterange-today-350x227.png)

* **Slepen en neerzetten van het datumbereik:** Sleep het datumbereik boven aan de tijdlijn van de planning.\
   ![resourcescheduling_daterange.png](assets/resourcescheduling-daterange-350x141.png)

## Instellingen configureren in de planningsgebieden

Bepaalde informatie wordt standaard weergegeven in de planningtijdlijn. U kunt uw montages ook vormen om extra informatie te tonen.

Raadpleeg de volgende artikelen voor informatie over het configureren van instellingen in de planningtijdlijn:

[Instellingen configureren in de planningsgebieden](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md)

[Gebruikerstoewijzingen ongeacht rol en groepslidmaatschap in de planningsgebieden toestaan](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

[Automatisch niet-toegewezen taken en problemen toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/automatically-assign-items-scheduling-areas.md)

## Gegevens filteren in de planningsgebieden

U kunt definiëren wat op de tijdlijn van de planning wordt weergegeven door een filter te maken.

Zie het artikel voor meer informatie [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

## Gebruikerstoewijzingen en toewijzingen wijzigen

* [Gebruikerstoewijzingen wijzigen](#modify-user-assignments)
* [Toewijzingen van gebruikers wijzigen](#modify-user-allocations)

### Gebruikerstoewijzingen wijzigen {#modify-user-assignments}

U kunt gebruikerstoewijzingen van het Plannende lusje (wanneer het plannen van middelen voor projecten) of wijzigen door het ruilmiddel te gebruiken of door taken en kwesties direct van de het plannen chronologie te wijzigen. U kunt gebruikerstaken van het Werken aan lusje (wanneer het plannen van middelen voor teams) wijzigen door taken en kwesties direct van de het plannen chronologie te wijzigen.

Zie het artikel voor meer informatie [Niet-toegewezen taken en problemen handmatig toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Toewijzingen van gebruikers wijzigen {#modify-user-allocations}

U kunt bepalen hoe de geplande uren voor een taak of kwestie aan gebruikers worden toegewezen. Geplande uren kunnen als volgt worden verdeeld:

* Onder gebruikers die aan de taak of de kwestie worden toegewezen.
* Over de duur van de taak of kwestie.

Zie het artikel voor meer informatie [Gebruikerstoewijzingen beheren in de planningsgebieden](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
