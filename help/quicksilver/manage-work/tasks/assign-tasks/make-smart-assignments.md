---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Slimme toewijzingen maken
description: U kunt slimme toewijzingen gebruiken om te bepalen wie de beste gebruiker het werk moet voltooien. De slimme taken zijn suggesties voor gebruikers, rollen, of teams die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst die op een algoritme worden gebaseerd dat het meest aangewezen middel voor de baan bepaalt. Zie Overzicht slimme toewijzingen voor informatie over slimme toewijzingen.
author: Lisa
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Slimme toewijzingen maken

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit beschikbaar slechts in het milieu van de Voorproef.</span>

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> This functionality will be removed from the Production environment for customers who enabled fast release with the 25.1 release in January 2025. For information about the 25.1 release, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md). -->

U kunt slimme toewijzingen gebruiken om te bepalen wie de beste gebruiker het werk moet voltooien.

De slimme taken zijn suggesties voor gebruikers, rollen, of teams die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst. Workfront baseert zijn suggesties op een algoritme dat de meest aangewezen bron voor de baan bepaalt.

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

Voor meer informatie over de criteria die in het bepalen van slimme taken worden gebruikt, zie [ Slim toewijzingsoverzicht ](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

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
   <td> <p>Nieuw: Standaard</p>
      of
      <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en problemen bewerken</p> <p>Toegang tot projecten weergeven of vergroten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger met de mogelijkheid om taken en uitgaven toe te wijzen</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Slimme toewijzingen maken

Slimme toewijzingen zijn beschikbaar op de meeste locaties waar u toewijzingen kunt maken in Workfront.

1. Ga naar de volgende gebieden de klik **Toewijzingen** of **toewijs dit aan** gebied:

   * Een taak- of uitgiftenlijst of rapport
   * Een taak- of uitgiftekoptekst
   * Het deelvenster Overzicht van taken of uitgaven
   * Een taak of probleem in het werklastevenwicht
     <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->

1. Plaats de cursor in het veld Toewijzingen en wacht twee seconden.

   <!--For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![](assets/smart-assignments-issue-header.png)-->

   De slimme toewijzingsvertoningen tonen in de volgende secties <!--, depending on which phase of the algorithm's calculation identified the assignments-->:

   <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
   * **Gebruikers en teams**, **de rollen van de Baan**, of <span class="preview">**de baanrollen van de kaart van het Tarief**</span>: <!--Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

   ![ Slim toewijzingsvoorbeeld in taaklijst ](assets/smart-assignments-task-list.png)

   Voor meer informatie, zie [ Slim toewijzingsoverzicht ](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Selecteer de bron in de lijst met aanbevelingen door op de naam ervan te klikken.

1. (Facultatief) klik **toewijzen aan me** om het het werkpunt aan zich toe te wijzen.

   >[!TIP]
   >
   >Als er geen suggesties zijn, wordt de lijst met suggesties niet geopend.

1. (Optioneel) Als u een van de aanbevolen gebruikers in de lijst met slimme toewijzingen niet wilt gebruiken, typt u de naam van de gewenste bron en selecteert u de naam wanneer deze in de lijst wordt weergegeven.
1. Klik **binnengaan** om de taak te maken.

   De geselecteerde gebruiker wordt toegewezen aan de taak of uitgave.
