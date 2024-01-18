---
product-area: projects
navigation-topic: update-work-in-a-project
title: Datums vastleggen bijwerken voor taken en problemen
description: U kunt de datum van Vastleggen van een taak of een kwestie manueel bijwerken waaraan u wordt toegewezen. Zie Overzicht datum vastleggen voor meer informatie over Datums vastleggen in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Datums vastleggen bijwerken voor taken en problemen

U kunt de datum van Vastleggen van een taak of een kwestie manueel bijwerken waaraan u wordt toegewezen. Ga voor meer informatie over Datums vastleggen in Adobe Workfront naar [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Toegangsvereisten

<!--Audited: 01/2024-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
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

Voordat u begint, moet u worden toegewezen aan de taak of uitgave waarvoor u de datum van vastleggen moet bijwerken.

## Datums vastleggen bijwerken voor taken en problemen

Het bijwerken van de Vastlegdatum is identiek voor taken en kwesties.

1. Ga naar een taak of kwestie u als **Eigenaar**.

   Zie de sectie voor meer informatie over het achterhalen wie de Taakeigenaar voor een probleem of taak is [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) in het artikel [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Klikken **Taakdetails** of **Probleemdetails** in het linkerdeelvenster.
1. Klikken **Overzicht** om het uit te breiden.
1. Werk de **Vastlegdatum** veld.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klikken **Wijzigingen opslaan**.

   Het volgende gebeurt na het aanbrengen van deze wijziging: 

   * De datum van Vastleggen en de geplande datum van voltooiing van de taak of afgifte zijn niet langer dezelfde.

     In plaats daarvan worden de Datum vastleggen en de verwachte Voltooiingsdatum van de taak of uitgave hetzelfde.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Als u het gebied van de Updates van de erfenis gebruikt, wordt de Eigenaar van het Project op de hoogte gebracht dat u een nieuwe Datum van de Vastlegging voor de taak of de kwestie hebt voorgesteld en kan, op dit ogenblik, de Geplande Datum van de Voltooiing van de taak of de kwestie bijwerken om de Vastleggingsdatum aan te passen u stelde. Deze functionaliteit wordt niet ondersteund in de nieuwe opmerkingervaring. Zie voor meer informatie [De nieuwe ervaring met opmerkingen](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     Zie de sectie voor informatie over de meldingen en updates die door deze wijziging worden geactiveerd [Meldingen en updates die worden geactiveerd door het wijzigen van de Vastlegdatum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) in het artikel [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
