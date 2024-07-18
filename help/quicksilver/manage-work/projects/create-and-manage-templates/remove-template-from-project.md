---
product-area: templates
navigation-topic: templates-navigation-topic
title: Sjabloongegevens uit een project verwijderen
description: U kunt een sjabloon niet uit een project verwijderen. U kunt informatie slechts manueel verwijderen die aan het project werd toegevoegd nadat een malplaatje aan het project in bijlage was. Voor informatie over het vastmaken van malplaatjes, zie een malplaatje aan een project vastmaken.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Sjabloongegevens uit een project verwijderen

U kunt een sjabloon niet uit een project verwijderen. U kunt informatie slechts manueel verwijderen die aan het project werd toegevoegd nadat een malplaatje aan het project in bijlage was. Voor informatie over het vastmaken van malplaatjes, zie [ een malplaatje aan een project ](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

## Toegangsvereisten

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
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot taken beheren </p> <p>Contribute of hoger toegang tot het project </p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

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
