---
product-area: projects
navigation-topic: use-predecessors
title: Creeer de Verhoudingen van de Predecessor door Taken te bepalen
description: In Adobe Workfront kunt u op meerdere manieren voorgangersrelaties maken. Eén methode is het koppelen van taken.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Maak vorige relaties door taken in een keten te plaatsen

In Adobe Workfront kunt u op meerdere manieren voorgangersrelaties maken. Eén methode is het koppelen van taken.

Voor informatie over voorgangerstaken, zie [ Overzicht van taakvoorgangers ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Door taken in een keten op te nemen, kunt u het systeem toestaan om automatisch de voorgangersrelaties te maken voor geselecteerde taken, in plaats van handmatig zelf een relatie te maken voor elke taak. De verschillende types van voorgangersverhouding kunnen nog tussen taken worden gebruikt.

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## De taken van de ketting om voorgangersverhoudingen tot stand te brengen

1. Ga naar het project dat de taken bevat die u wilt ketenen.
1. Klik **Taken** in het linkerpaneel.
1. (Voorwaardelijk) Uitgezochte **Autosave** in de hoger-juiste hoek van de taaklijst, dan selecteer de taken die u wilt ketenen.

   ![ Autosave pictogram op benadrukte ](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Het is niet mogelijk taken in een takenlijst te voorzien wanneer u handmatig wijzigingen in taken opslaat of de planningsmodus van de tijdlijn gebruikt om taken op te slaan.

1. Klik de geselecteerde taken met de rechtermuisknop aan, dan klik **Keten**.
1. Selecteer een van de volgende afhankelijkheidstypen:

   * **beëindigen-Begin**
   * **beëindigen-Afwerking**
   * **begin-Begin**
   * **begin-Afwerking**

   Voor meer informatie over de types van voorgangsafhankelijkheid, zie [ Overzicht van de types van taakgebiedsdeel ](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Facultatief) klik **Unchain** als sommige taken eerder zijn geketend.

   >[!CAUTION]
   >
   >Alleen sequentiële voordecessors worden verwijderd met de optie voor het ongedaan maken van de keten bij taken voor bulkbewerking.

   De geselecteerde taken zijn nu gekoppeld aan eerdere relaties.
