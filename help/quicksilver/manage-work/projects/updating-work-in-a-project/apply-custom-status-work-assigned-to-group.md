---
product-area: projects
navigation-topic: update-work-in-a-project
title: Statussen toepassen op werk dat aan een groep is gekoppeld
description: Als een project met een groep wordt geassocieerd, kunt u zowel systeem-vlakke statussen evenals een douanestatus toepassen verbonden aan die groep aan het project, de taak of de kwesties op dat project.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Statussen toepassen op werk dat aan een groep is gekoppeld

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Als een project met een groep wordt geassocieerd, kunt u zowel systeem-vlakke statussen evenals een douanestatus toepassen verbonden aan die groep aan het project, of taken en kwesties op dat project. Voor informatie over groepsstatussen in Adobe Workfront, zie [ een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

>[!TIP]
>
>U kunt alleen projecten aan groepen koppelen. De kwesties en de taken erven de groep van het project zij tot behoren.

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

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Projectgroep en status bijwerken

Wanneer u de Groep voor een project bijwerkt, de opties beschikbaar voor de Status van taken, kwesties, of de projectverandering om de groep aan te passen.

1. Ga naar een project, of creeer een nieuw project, zoals die in [ wordt beschreven creeer een project ](../../../manage-work/projects/create-projects/create-project.md).
1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png), dan klik **uitgeven**.

1. In **geef de doos van het Project** uit die, dichtbij de bodem van de **sectie van het Overzicht** toont, selecteer de groep in het **Groep** drop-down menu.

1. In het **drop-down menu van de Status**, selecteer de douanestatus.

   >[!NOTE]
   >
   >Als u een verschillende groep in het **drop-down menu van de Groep** selecteert, veranderen de douanestatussen in het **3} menu van de Status {automatisch om met de nieuwe groep te correleren.**
   >
   >
   >![ drop-down Status die met douanestatus voor project wordt uitgebreid ](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. Selecteer de status van het project. De aangepaste status die u hebt gemaakt en toegepast op die groep, wordt weergegeven in de lijst.
