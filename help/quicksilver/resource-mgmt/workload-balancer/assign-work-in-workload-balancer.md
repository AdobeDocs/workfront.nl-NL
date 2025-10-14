---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Overzicht van het toewijzen van werk in de werklastverdeler
description: Als middelmanager, kunt u de Balancer van de Werkbelasting van Adobe Workfront gebruiken om het werkpunten te bekijken die nog niet aan gebruikers zijn toegewezen evenals deze punten aan hen toe te wijzen.
author: Lisa
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 6db33763294bc9fa343bb010b318fbcceccfff4c
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 0%

---

# Overzicht van het toewijzen van werk in de werklastverdeler

{{preview-fast-release-general}}

<!-- Audited: 5/2025 -->

Als middelmanager, kunt u de Balancer van de Werkbelasting van Adobe Workfront gebruiken om het werkpunten te bekijken die nog niet aan gebruikers zijn toegewezen evenals deze punten aan hen toe te wijzen.

Voor algemene informatie over de Balancer van de Werklast, zie [&#x200B; Overzicht van de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

U kunt werkitems (taken en problemen) toewijzen aan gebruikers in andere gebieden van Workfront. Nochtans, door de Balancer van de Werklast te gebruiken kunt u de beschikbaarheid van gebruikers gemakkelijk begrijpen en duidelijk alle andere punten zien zij aan alvorens hen meer werk toe te wijzen worden toegewezen.

Raadpleeg de volgende artikelen voor informatie over het toewijzen van werkitems in andere gebieden van Workfront:

* [&#x200B; wijs taken &#x200B;](../../manage-work/tasks/assign-tasks/assign-tasks.md) toe
* [Problemen toewijzen](../../manage-work/issues/manage-issues/assign-issues.md)

## Beschikbaarheid van gebruikers in de werklastverhouding

U kunt werk toewijzen in Workload Balancer zodat dit overeenkomt met de beschikbare tijd van de gebruikers. Om ervoor te zorgen dat u de juiste hoeveelheid werk toewijst en de gebruiker niet te veel toewijst, moet het totale aantal geplande uren van de aan de gebruiker toegewezen werkitems overeenkomen met de dagelijkse of wekelijkse toewijzingen.

Het is belangrijk om te begrijpen hoe Workfront de beschikbare tijd voor een gebruiker berekent.

Workfront gebruikt de volgende informatie om de capaciteit van de gebruiker in de Workload Balancer te berekenen:

* De voorkeuren voor Bronbeheer. De beheerder van Workfront bepaalt hoe de beschikbare tijd voor het systeem door te selecteren wordt berekend om één van het volgende op het gebied van het Beheer van het Middel in Opstelling te gebruiken wordt berekend:

   * Het standaardschema van het Workfront-systeem en de FTE van de gebruiker.
   * Het schema van de gebruiker, zoals aangegeven in het gebied Gebruikersprofiel.

     Hiermee wordt de dagelijkse en wekelijkse beschikbaarheid van de gebruiker berekend. Alle planningsuitzonderingen op het geselecteerde schema worden weerspiegeld in de capaciteit van de gebruiker in de Werklastverdeler.

  Voor meer informatie, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

  Voor informatie over programma&#39;s, zie [&#x200B; een programma &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

* De time-out van de gebruiker. Dit geeft aan op welke dagen de gebruiker van plan is op te starten.

  Voor meer informatie, zie [&#x200B; persoonlijke tijd van &#x200B;](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md) vormen.

* De werktijd van de gebruiker. Dit wijst op het percentage van FTE tijd dat de gebruiker beschikbaar is om werkelijk project-verwant werk, zonder overheadkosten uit te voeren. Plaats de waarde van de Tijd van het Werk aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.


## Werk toewijzen in Workload Balancer

U kunt werkitems toewijzen die nog niet aan een gebruiker zijn toegewezen of items die aan gebruikers in de werklastbalans zijn toegewezen, opnieuw toewijzen.

U kunt werk in de Balancer van de Werkbelasting op de volgende manieren toewijzen:

* Eén item tegelijk door elk item handmatig toe te wijzen.

  U kunt Geavanceerde toewijzingen maken wanneer u items handmatig, één voor één toewijst.

  Voor meer informatie, zie [&#x200B; werk manueel toewijzen gebruikend de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* Eén item tegelijk, door het werkitem naar de gebruiker te slepen die het moet toewijzen.

  Voor meer informatie, zie [&#x200B; werk in de Balancer van de Werklast toewijzen door te slepen en te laten vallen &#x200B;](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* Meerdere items tegelijk, met de optie Meerdere toewijzingen. U kunt regels bepalen waardoor de punten aan veelvoudige gebruikers tegelijkertijd worden toegewezen.

  Voor meer informatie, zie [&#x200B; werk in bulk toewijzen gebruikend de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

Voor informatie over het unassigning van het werk, zie [&#x200B; werk in de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md) unassign.

## Toewijzingsgebieden in het werklastevenwicht

U kunt werk aan gebruikers toewijzen gebruikend de Balancer van de Werkbelasting in het gebied van het Middelen, op het project, of op het teamniveau. Voor meer informatie over waar de Balancer van de Werkbelasting in Workfront wordt gevestigd, zie [&#x200B; plaats van de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Er zijn twee gebieden in de Balancer van de Werkbelasting waar u het werkpunten kunt bekijken:

* **Niet toegewezen Werk**: De punten van vertoningen die niet aan gebruikers worden toegewezen.
* **Toegewezen Werk**: De punten van vertoningen die aan gebruikers worden toegewezen.

In de volgende tabel wordt beschreven welke items in elk gebied worden weergegeven op basis van hun toewijzingen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong> Type van taak </strong> </td> 
   <td colspan="2"><strong> Gebieden waarin de taken </strong> zichtbaar zijn </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>Niet toegewezen werk </td> 
   <td>Toegewezen werk </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;"> Niet toegewezen punt </span> </td> 
   <td><span> ✔ </span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00"> Rol </span> </td> 
   <td><span> ✔ </span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rol en team</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Gebruiker en team</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Gebruiker, Rol en Team</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Gebruiker en Rol</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00"> ✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42; wanneer een het werkpunt aan een gebruiker en een rol wordt toegewezen, toont het in het Niet toegewezen gebied van het Werk slechts wanneer de rol Primaire Toegewezen is. <span class="preview"> de taken van de Rol worden getoond onder het werkpunten in het Niet toegewezen gebied van het Werk wanneer **het plaatsen van de Taken van de Rol** wordt toegelaten.</span>

&#42;&#42; wanneer een het werkpunt aan een gebruiker en een andere entiteit wordt toegewezen, toont het in het Toegewezen gebied van het Werk slechts wanneer de gebruiker de Primaire Ontvanger is.

Voor meer informatie over de Niet toegewezen en Toegewezen gebieden van het Werk van de Balancer van de Werkbelasting, en de montages van de Balancer van de Werkbelasting, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers

Overweeg het volgende wanneer het toewijzen van veelvoudige middelen aan een het werkpunt:

* Gebruikers kunnen meer dan één taakrol aan hun profiel koppelen. Voor informatie over het associëren van gebruikers met baanrollen, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

* Taken of problemen worden doorgaans eerst toegewezen aan een of meer functies of aan een team. Wanneer de projecten klaar zijn om te beginnen, zouden zij ook aan gebruikers kunnen moeten worden toegewezen.\
  Als een taak of een kwestie aan één of veelvoudige rollen wordt toegewezen en u dan ook een gebruiker toewijst, beslist Adobe Workfront welke baanrol aan de extra gebruiker (als om het even welk) te associëren volgens de volgende regels:

   * Als er slechts één taakrol is toegewezen en deze overeenkomt met de primaire rol van de gebruiker, wordt de taak of kwestie alleen toegewezen aan de gebruiker die zijn primaire rol vervult.
   * Als er veelvoudige toegewezen rollen zijn en minstens één van de rollen de secundaire rollen van de gebruiker aanpast, dan wordt de taak of de kwestie toegewezen aan de gebruiker die één van hun Andere Rollen vervult — die Workfront willekeurig selecteert als er veelvoudige gelijken zijn — evenals om het even welke extra rollen die worden toegewezen.
   * Als er een of meer toegewezen taakrollen zijn en er geen overeenkomsten met de rollen van de gebruiker zijn, dan wordt de taak of kwestie toegewezen aan zowel de rol of de rollen als aan de gebruiker.

* Als een taak of een kwestie aan een team wordt toegewezen en u ook een gebruiker toewijst, blijft de taak of de kwestie toegewezen aan zowel het team als de gebruiker.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
