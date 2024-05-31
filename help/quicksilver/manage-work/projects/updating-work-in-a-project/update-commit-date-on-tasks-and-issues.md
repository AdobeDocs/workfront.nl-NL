---
product-area: projects
navigation-topic: update-work-in-a-project
title: Datums vastleggen bijwerken voor taken en problemen
description: U kunt de datum van Vastleggen van een taak of een kwestie manueel bijwerken waaraan u wordt toegewezen. Zie Overzicht datum vastleggen voor meer informatie over Datums vastleggen in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---


# Datums vastleggen bijwerken voor taken en problemen

{{highlighted-preview}}

U kunt de datum van Vastleggen van een taak of een kwestie manueel bijwerken waaraan u wordt toegewezen. Ga voor meer informatie over Datums vastleggen in Adobe Workfront naar [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Toegangsvereisten

<!--Audited: 01/2024-->

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
   Voor de nieuwe vergunningen:
   <ul>
   <li><p>Standaard voor taken</p> </li>
   <li><p>Medewerker of hoger voor problemen</p></li>
   </ul>
   Voor huidige licenties:
<ul>
   <li><p>Werk of hoger voor taken</p></li> 
   <li><p>Aanvraag of hoger voor problemen</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en problemen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor de taak of uitgave</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voordat u de datum Vastleggen van een taak of uitgave kunt bewerken, moet u worden toegewezen aan de taak of uitgave waarvan u de datum voor vastleggen moet bijwerken.

## Datums vastleggen bijwerken voor taken en problemen


U kunt de Vastlegdatum van een taak of kwestie op de volgende gebieden van Workfront bijwerken:

* De sectie Details van een taak of kwestie
* <span class="preview">De taak- of uitgiftekop</span>

  <span class="preview">Uw Workfront of groepsbeheerder moet de datum Vastleggen toevoegen aan de taak- of uitgiftekoptekst van uw lay-outsjabloon om deze weer te geven vanaf de taak- of uitgiftepagina.
Zie voor meer informatie [Objectkoppen aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

Het bijwerken van de Vastlegdatum is identiek voor taken en kwesties.

>[!NOTE]
>
>U kunt uw systeem of groepsbeheerder vragen om het veld Datum vastleggen toe te voegen aan het deelvenster Overzicht, zodat u het in verschillende delen van Workfront gemakkelijker kunt bijwerken.
>
>Raadpleeg de volgende artikelen voor meer informatie:
>
>* [Overzicht van samenvattingen](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Home en overzicht aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Ga naar een taak of kwestie u als **Eigenaar**.

   Zie de sectie voor meer informatie over het achterhalen wie de Taakeigenaar voor een probleem of taak is [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) in het artikel [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">(Voorwaardelijk en optioneel) Als uw Workfront of groepsbeheerder de datum Vastleggen aan uw taak of uitgiftekop heeft toegevoegd, klikt u op de knop **Vastlegdatum** in de koptekst en selecteer vervolgens een datum in de kalender. Ga als volgt te werk als de datum vastleggen zich niet in de koptekst bevindt. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

1. Klikken **Taakdetails** of **Probleemdetails** in het linkerdeelvenster.
1. Klikken **Overzicht** om het uit te breiden.
1. Werk de **Vastlegdatum** veld.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klikken **Wijzigingen opslaan**.

   Het volgende gebeurt na het aanbrengen van deze wijziging:

   * De datum van Vastleggen en de geplande datum van voltooiing van de taak of afgifte zijn niet langer dezelfde.

     In plaats daarvan worden de Datum vastleggen en de verwachte Voltooiingsdatum van de taak of uitgave hetzelfde.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * De eigenaar van het project wordt in een Workfront-melding in de app op de hoogte gesteld van het feit dat u een nieuwe Vastlegdatum voor de taak of uitgave hebt voorgesteld.
   * De eigenaar van het project wordt in de sectie Updates op de hoogte gesteld van het feit dat u een nieuwe Vastlegdatum hebt voorgesteld en zij kunnen, op dit moment, de Geplande Voltooiingsdatum van de taak of kwestie bijwerken om de Vastleggingsdatum aan te passen u voorstelde.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Voor informatie over de berichten en updates die door deze verandering teweeggebracht worden, zie de sectie &quot;Meldingen en updates teweeggebracht door het veranderen van de Datum van het Vastleggen&quot;in het artikel [Overzicht van datum vastleggen](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->