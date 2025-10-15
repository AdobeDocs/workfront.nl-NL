---
product-area: projects;user-management
navigation-topic: manage-projects
title: Gebruikers verwijderen uit projecten
description: U kunt gebruikers uit een project verwijderen wanneer zij niet meer betrokken zijn bij de voltooiing van het werk aan het project.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Gebruikers uit projecten verwijderen

U kunt gebruikers uit een project verwijderen wanneer zij niet meer betrokken zijn bij de voltooiing van het werk aan het project. Het verwijderen van gebruikers uit projecten heeft implicaties op taak en probleemtaken, evenals op projectrollen. Verwijderde gebruikers houden op ontvangend berichten voorgenomen voor het Team van het Project. Voor meer informatie over berichten voor de projectteams, zie [&#x200B; de berichttypes van de Gebeurtenis &#x200B;](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

De gebruikers verbonden aan een project zijn vermeld in het gebied van Mensen van een project. Zij vertegenwoordigen het Team van het Project. Voor meer informatie over het Team van het Project, zie [&#x200B; Overzicht van het Team van het Project &#x200B;](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Hoe het verwijderen van een gebruiker bestaande taken, kwesties en projecten beïnvloedt

Wanneer een gebruiker uit een project wordt verwijderd, zouden om het even welke taken of kwesties die aan hen worden toegewezen kunnen worden beïnvloed, afhankelijk van of de taak of de kwestie werd voltooid toen de gebruiker werd verwijderd:

* **als het punt niet wordt voltooid wanneer de gebruiker wordt verwijderd:** het punt wordt opnieuw toegewezen aan een baanrol als een baanrol reeds werd toegewezen, of het wordt toegewezen aan de baanrol de gebruiker op het punt vervulde. Als het item of de gebruiker geen taakrol heeft toegewezen, moet u het item handmatig opnieuw toewijzen.
* **als het punt wordt voltooid wanneer de gebruiker wordt verwijderd:** De naam van de verwijderde gebruiker blijft op het punt.
* **als de verwijderde gebruiker ook de schepper van een project is:** het project wordt niet verwijderd uit hun **Projecten I op** lijst in het gebied van Projecten. Het project wordt verwijderd uit de lijsten voor alle andere gebruikers die voor dat project door het Ingegaan door gebied filtreren.
* **als de gebruiker de eigenaar of Sponsor van het project is:** de gebruiker blijft in hun rollen als sponsor of eigenaar van het project.

## Verwijder gebruikers uit een project en het Team van het Project

U kunt gebruikers uit een project verwijderen door hen uit het Team van het Project te verwijderen.

Wanneer de gebruikers rollen op een project vervullen, worden zij een deel van het Team van het Project.

Wanneer u gebruikers uit hun rollen op het project verwijdert, blijven zij deel van het projectteam.

Voor informatie over de rollen van gebruikers op een project, zie [&#x200B; het Team van het Project beheren &#x200B;](../planning-a-project/manage-project-team.md).

Om gebruikers uit het Team van het Project te verwijderen:

1. Ga naar het project waar u de gebruikers wilt verwijderen.

1. Klik **Mensen** in het linkerpaneel, dan selecteer de gebruikers u wilt verwijderen.

1. Klik **verwijderen** pictogram ![&#x200B; verwijderen punt &#x200B;](assets/remove-icon---x-in-circle.png) bij de bovenkant van de lijst van gebruikers.

1. Klik **ja, verwijder Geselecteerde Gebruikers** om verwijdering te bevestigen.

   De gebruikers worden verwijderd uit het projectteam en uit om het even welke onvolledige taken of kwesties die zij zouden kunnen worden toegewezen aan. Zij ontvangen niet meer berichten voorgenomen voor het Team van het Project.
