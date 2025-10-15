---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Overzicht van eigenaars en sponsors van projecten
description: U kunt een projecteigenaar en een projectsponsor voor een project aanwijzen.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Overzicht van eigenaars en sponsors van projecten

<!-- Audited: 1/2024 -->

U kunt een projecteigenaar en een projectsponsor voor een project aanwijzen.

De eigenaar van het project is de persoon die verantwoordelijk is voor de tijdige en budgettaire voltooiing van het project.

De projectsponsor is een belangrijke belanghebbende bij het project waarvoor middelen in het project zijn geïnvesteerd. De projectsponsor heeft doorgaans baat bij de voltooiing van het project.

Voor informatie over hoe te om de Eigenaar of Sponsor van het Project voor een project bij te werken, zie [&#x200B; de eigenaars en sponsors van het Project van de Update &#x200B;](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Projecteigenaars

U kunt de manager van een project aanwijzen door een Eigenaar van het Project op een project of een malplaatje te specificeren.

U kunt slechts één eigenaar van het Project voor een project definiëren.

Het veld Projecteigenaar kan het volgende gebruiken:

* U kunt slechts één gebruiker aanwijzen als de eigenaar van het project.
* U kunt de Eigenaars van het Project als urenfiatteur voor het project aanwijzen.
* U kunt de Eigenaar van het Project als generische fiatteur aanwijzen wanneer het bepalen van project, taak, of goedkeuringsprocessen. Voor informatie over goedkeuringen, zie [&#x200B; een goedkeuringsproces &#x200B;](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md) uitgeven.

  >[!IMPORTANT]
  >
  >Wanneer u een goedkeuring toewijst aan de Eigenaar van het Project en niemand als eigenaar van een project wordt aangewezen, wordt de goedkeuring opnieuw toegewezen aan de belangrijkste beheerder van Workfront zoals die in de sectie van de Info van de Klant in het gebied van de Opstelling wordt vermeld. Voor informatie, zie [&#x200B; basisinformatie voor uw systeem &#x200B;](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.
  >


* U kunt bepaalde berichten inschakelen die alleen aan de eigenaar van het project worden bezorgd.

  Voor meer informatie over e-mailberichten, zie de sectie [&#x200B; gebeurtenisberichten voor iedereen in het systeem &#x200B;](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) in het artikel [&#x200B; vormen gebeurtenisberichten voor iedereen in het systeem &#x200B;](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* U kunt het veld Projecteigenaar in een rapport of lijst weergeven.

  U kunt het veld Projecteigenaar ook weergeven in een weergave, groep of vraag.

  U kunt bijvoorbeeld de volgende expressie in de tekstmodus naar een filter kopiëren om projecten weer te geven die eigendom zijn van de aangemelde gebruiker:

  ```
  ownerID=$$USER.ID
  ```

Voor meer informatie over het creëren van rapporten, zie het artikel [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE: drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Projectsponsors

U kunt elke gebruiker in het systeem aanwijzen als projectsponsor. De projectsponsor is doorgaans een manager, uitvoerend of belanghebbende die moet weten wat er met het project gebeurt.

Houd rekening met het volgende wanneer u een projectsponsor toewijst:

* De projectsponsor krijgt geen extra toegang tot het project, maar wordt toegevoegd aan de e-mailmeldingen van het project. Voor informatie over berichten, zie het artikel [&#x200B; gebeurtenisberichten voor iedereen in het systeem &#x200B;](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) vormen.

* U kunt slechts één projectsponsor aanwijzen.
* U kunt de Projectsponsor aanwijzen als een generieke fiatteur wanneer het bepalen van project, taak, of goedkeuringsprocessen. Voor informatie over goedkeuringen, zie [&#x200B; een goedkeuringsproces &#x200B;](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md) uitgeven.

  >[!IMPORTANT]
  >
  >Wanneer u een goedkeuring toewijst aan de projectsponsor en niemand als sponsor van een project is aangewezen, wordt de goedkeuring opnieuw toegewezen aan de eigenaar van het project. Als niemand als eigenaar van het project wordt aangewezen, wordt de goedkeuring toegewezen aan de beheerder van Workfront.

* U kunt het veld Projectsponsor in een rapport of lijst weergeven.

  U kunt het veld Projectsponsor ook weergeven in een weergave, groep of vraag.

  U kunt bijvoorbeeld de volgende expressie in de tekstmodus naar een filter kopiëren om projecten weer te geven die worden gesponsord door de aangemelde gebruiker:

  ```
  sponsorID=$$USER.ID
  ```



  Voor meer informatie over het creëren van rapporten, zie het artikel [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
