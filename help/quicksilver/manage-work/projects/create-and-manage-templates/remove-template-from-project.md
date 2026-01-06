---
product-area: templates
navigation-topic: templates-navigation-topic
title: Sjabloongegevens uit een project verwijderen
description: U kunt een sjabloon niet uit een project verwijderen. U kunt informatie slechts manueel verwijderen die aan het project werd toegevoegd nadat een malplaatje aan het project in bijlage was. Voor informatie over het vastmaken van malplaatjes, zie een malplaatje aan een project vastmaken.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Sjabloongegevens uit een project verwijderen

U kunt een sjabloon niet uit een project verwijderen. U kunt informatie slechts manueel verwijderen die aan het project werd toegevoegd nadat een malplaatje aan het project in bijlage was. Voor informatie over het vastmaken van malplaatjes, zie [ een malplaatje aan een project ](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

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
   <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot taken beheren </p> <p>Contribute of hoger toegang tot het project</p>  </td> 
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Opties voor het verwijderen van sjablooninformatie uit een project

Als u sjabloongegevens wilt verwijderen die aan het project zijn toegevoegd, kunt u een van de volgende handelingen uitvoeren:

* Verwijder handmatig informatie uit het project nadat de sjabloon is gekoppeld.

  Voor informatie, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

* Schrap de taken in het project die met het malplaatje werden toegevoegd.

  Voor informatie, zie de [ taken van de Schrapping die van een malplaatje ](#delete-tasks-created-from-a-template) sectie in dit artikel worden gecreeerd.

* Verwijder de sjabloon uit Workfront. Als u de sjabloon uit Workfront verwijdert, worden de taken die aan de sjabloon zijn toegevoegd, niet verwijderd uit projecten.

  Voor informatie, zie [ projectmalplaatjes van de Schrapping ](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Taken verwijderen die met een sjabloon zijn gemaakt {#delete-tasks-created-from-a-template}

1. Ga naar de **sectie van Taken** van het project.
1. Voer een van de volgende handelingen uit:

   * Maak een filter voor de takenlijst om alleen taken weer te geven die met de volgende instructie zijn gemaakt op basis van een sjabloon:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Voor informatie over het creëren van een filter, zie [ filters in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.

     Wanneer u het filter toepast, worden alleen taken die aan een Sjabloontaak-id zijn gekoppeld, in de lijst weergegeven.

   * Creeer een mening voor de taaklijst om **identiteitskaart van de Taak van het Malplaatje** of **de gebieden van de Naam van de Taak van het Malplaatje** in een kolom te tonen.

     Wanneer u de mening toepast, werden de taken die informatie in identiteitskaart van de Taak van het Malplaatje of de naamkolom van de Taak van het Malplaatje bevatten gecreeerd gebruikend een malplaatje.

     Voor informatie over het creëren van een mening, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Selecteer alle taken die in Stap 2 worden geïdentificeerd zoals die van een malplaatje worden gecreeerd, dan klik **het pictogram van de Schrapping****> ja, schrap het**. Voor meer informatie, zie [ de taken van de Schrapping ](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
