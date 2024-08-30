---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Aan de slag met bronnenbeheer
description: Met resourcebeheer kunt u uw systeem zodanig configureren dat het gebruik van uw bronnen nauwkeurig wordt voorspeld op basis van hun beschikbaarheid, zodat het werk dat moet worden uitgevoerd op tijd en op budget wordt voltooid.
author: Lisa
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 0%

---

# Aan de slag met Resource Management

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Met resourcebeheer kunt u uw systeem zodanig configureren dat het gebruik van uw bronnen nauwkeurig wordt voorspeld op basis van hun beschikbaarheid, zodat het werk dat moet worden uitgevoerd op tijd en op budget wordt voltooid.

## Overzicht van hulpbronnenbeheer in Adobe Workfront

Het Beheer van het middel verwijst naar alle activiteiten die door de beheerder van Adobe Workfront, de middelmanager, en de Eigenaar van het Project worden uitgevoerd om (de Planning van het Middel of van het Scenario) en programma (de Balancer van de Werkbelasting) de middelen van een organisatie te plannen en hen toe te wijzen aan het werk dat moet worden gedaan, rekening houdend met hun beschikbaarheid. Bovendien, verwijst het middelbeheer ook naar het bekijken van informatie over de geplande en daadwerkelijke middeltoewijzingen in een rapportmening (het rapport van het Gebruik).

Workfront beschikt over verschillende gereedschapssets die worden gebruikt voor het beheer van bronnen. Elk gereedschap heeft een afzonderlijk bereik. Op dit moment kunt u de volgende hulpprogramma&#39;s voor bronnenbeheer in Workfront gebruiken, afhankelijk van de fase van het bronnenbeheer waarin u zich bevindt:

* Om te plannen hoe de middelen op een hoger niveau worden toegewezen, alvorens het daadwerkelijke werk aan projecten begint, gebruik de volgende hulpmiddelen:

   * **de Planner van het Middel**: U kunt de Planner van het Middel in de eerste fase van middelbeheer gebruiken aan de tijd van het begrotingsproject voor uw middelen volgens hun geplande beschikbaarheid. Tijdens de planning van middelenfase, kunt u gebruikers in middelpools organiseren en veelvoudige middelpools aan een project toewijzen.

     Voor meer informatie over de Planning van het Middel, zie [ Planning van het Middel: artikelindex ](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **de Planner van het Scenario**: Dit is een hoger-vlakke planning van middelen die u toestaat om hen over veelvoudige initiatieven te beheren die over een één, drie, of vijf jaar plan kunnen overspannen en veelvoudige projecten omvatten. U kunt het beste scenario gebruiken om het beste uit hun beschikbaarheid en uw budget te halen.

     De Scenario Planner vereist naast de Workfront-licentie een aparte licentie. Voor informatie over de Planner van het Scenario van Workfront, zie [ het overzicht van de Planner van het Scenario ](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Als u middelen wilt plannen of toewijzen aan daadwerkelijk werk (taken en uitgaven), gebruikt u het volgende gereedschap:

   * **de Balancer van de Werkbelasting**: Dit behoort tot een laag-vlakke stadium van middelbeheer, waar u uw middelen aan het daadwerkelijke werk (taken en kwesties) kunt toewijzen die zij moeten voltooien, gebaseerd op de hoeveelheid uren nodig om hen en hun beschikbaarheid te voltooien. Met behulp van Workload Balancer kunt u gebruikers toewijzen aan daadwerkelijk werk dat momenteel niet is toegewezen aan of is toegewezen aan taakrollen.

     Voor informatie over de Balancer van Workfront, zie [ de Balancer van de Werklast: artikelindex ](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Gebruik het volgende gereedschap om de begrote, geplande en feitelijke toewijzingen voor meerdere projecten te analyseren:

   * **het Rapport van het Gebruik**: Gebruik dit rapport om het gebruik van middelen voor projecten te bekijken. U kunt begrote, geplande, en daadwerkelijke toewijzingen voor uw projecten en hun effect op de kosten en de opbrengst van de projecten vergelijken.

     Voor informatie over het Rapport van het Gebruik, zie [ informatie van het het middelgebruik van de Mening ](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## De componenten van het proces van het Beheer van het Middel

>[!NOTE]
>
>Resourcebeheer is nooit een stagnerend proces in Workfront. Aangezien de programma&#39;s van uw projecten, de beschikbaarheid van uw gebruikers, of hun rollen veranderen, moet u voortdurend de informatie over uw middelen, hun taken, en hun toewijzingen aan projecten, taken, en kwesties aanpassen.

Het beheer van bronnen in Workfront omvat de volgende fasen:

* **Configuratie**: Als systeembeheerder, middelmanager, of de Eigenaar van het Project moet u bepaalde gebieden en voorwerpen in uw instantie van Workfront vormen alvorens uw middelen te beheren. Voor meer informatie over de eerste vereisten noodzakelijk beginnen middelen in Workfront te beheren, zie de [ Vereisten voor nauwkeurige middelbeheer ](#prerequisites-for-accurate-resource-management) sectie in dit artikel.\
  Naast het hebben van projecten met het werkpunten, moet u de volgende punten in Workfront vormen:

   * Gebruikers\
     Voor meer informatie over het creëren van gebruikers, zie het artikel [ gebruikers ](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

   * Taken rollen\
     Voor meer informatie over het creëren van baanrollen, zie het artikel [ creëren en baanrollen beheren ](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Planningen\
     Voor meer informatie over het creëren van programma&#39;s, zie het artikel [ een programma ](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

   * Projectvoorkeuren

     >[!TIP]
     >
     >Slechts kan een systeem of groepsbeheerder de Voorkeur van het Project voor uw systeem of voor uw groep wijzigen.

     Voor meer informatie over het bepalen van de Voorkeur van het Project, zie het artikel [ systeem-brede projectvoorkeur ](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

   * Brongroepen

     Voor meer informatie over het creëren van middelpools, zie [ middelpools ](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md) creëren.

   * Voorkeuren voor beheer van bronnen

     Als systeem, moet u beslissen hoe Workfront gebruikersbeschikbaarheid op systeemniveau berekent, of gebruikend het programma van de gebruiker of het Standaard Programma van uw systeem.

     Voor meer informatie, zie [ de voorkeur van het Beheer van het Middel ](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

* **toewijzing van het Middel**: Als middelmanager, of een Eigenaar van het Project, kunt u toewijzing van middelen voor uw projecten bepalen evenals werk toewijzen. Voor deze stap, kunt u de schatting van de toewijzing van uw middelen beheren gebruikend de Planner van het Middel of de Planner van het Scenario, en het daadwerkelijke werk aan gebruikers in de Balancer van de Werkbelasting toewijzen.

  Raadpleeg de volgende secties voor meer informatie over het plannen en toewijzen van resources:

   * [Bronnen plannen: artikelindex](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront Scenario Planner](../../scenario-planner/scenario-planning.md)
   * [De werklastbalans: artikelindex](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analyse**: Als middelmanager, de Eigenaar van het Project, of personenmanager, herzie het Rapport van het Gebruik om te begrijpen hoe de begrote en geplande toewijzingen van uw middelen met daadwerkelijke degenen vergelijken. Gegevens controleren op uren, kosten of inkomsten. Voor informatie over het rapport van het Gebruik, zie [ informatie van het het middelgebruik van de Mening ](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Toegang die nodig is om bronnen te bekijken en te beheren met de tools voor resourcebeheer in Workfront

De volgende gebruikers hebben toegang tot de hulpmiddelen van het Beheer van het Middel in Workfront:

U moet een van de volgende gebruikers zijn en over de volgende toegang en machtigingen beschikken om toegang te krijgen tot hulpmiddelen voor bronnenbeheer:

* De systeembeheerder.
* Een gebruiker met een Standard- of Plan-licentie.

  Een gebruiker met een werkvergunning kan de Balancer van de Werklast van een project gebruiken en taken en toewijzingen beheren.

  Naast een werkvergunning of een hogere vergunning (of een Vergunning Standaard), moet u het volgende hebben om specifieke hulpmiddelen van het middelbeheer te gebruiken:

   * Toegang tot bronnenbeheer bewerken (niet nodig voor het uitvoeren van toewijzingen in Workload Balancer)
   * Toegang tot financiële gegevens bewerken om kosteninformatie weer te geven in de functie voor middelenplanner
   * Toegang tot financiële gegevens bekijken om informatie over kosten en opbrengsten weer te geven in het gebruiksrapport (alleen gebruikers met een licentie voor een abonnement)

* Contribute of hogere toestemmingen die de Taken van het Merk op de projecten omvatten u middelen voor wilt beheren.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Voor informatie over de toegang nodig aan begrotingsmiddelen, zie de artikel [ Toegang nodig aan begrotingsmiddelen ](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Voor informatie over de toegang nodig om middelen in de Balancer van de Werklast te beheren, zie [ Toegang nodig om middelen in de Balancer van de Werklast te beheren ](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Vereisten voor een accuraat beheer van bronnen  {#prerequisites-for-accurate-resource-management}

U moet aan een reeks vereisten voldoen voordat u de hulpmiddelen voor resourcebeheer in Workfront efficiënt kunt gebruiken.

Raadpleeg de volgende bronnen voor informatie over de vereisten voor elk hulpprogramma voor resourcebeheer in Workfront:

* De sectie [ Vereisten voor het werken in de Planner van het Middel ](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) in het artikel [ overzicht van de Planner van het Middel ](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
* De sectie [ Beste praktijken voor het gebruiken van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) in het artikel [ Overzicht van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [ toegang nodig aan begrotingsmiddelen in Adobe Workfront ](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [ toegang nodig om middelen in de Balancer van de Werklast te beheren ](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
