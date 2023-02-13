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
source-wordcount: '451'
ht-degree: 0%

---

# Sjabloongegevens uit een project verwijderen

U kunt een sjabloon niet uit een project verwijderen. U kunt informatie slechts manueel verwijderen die aan het project werd toegevoegd nadat een malplaatje aan het project in bijlage was. Voor informatie over het bijvoegen van sjablonen raadpleegt u [Een sjabloon aan een project koppelen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

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
   <td> <p>Toegang tot taken bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot taken beheren </p> <p>Contribute of hoger toegang tot het project </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Opties voor het verwijderen van sjablooninformatie uit een project

Als u sjabloongegevens wilt verwijderen die aan het project zijn toegevoegd, kunt u een van de volgende handelingen uitvoeren:

* Verwijder handmatig informatie uit het project nadat de sjabloon is gekoppeld.

   Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

* Schrap de taken in het project die met het malplaatje werden toegevoegd.

   Zie voor meer informatie de [Taken verwijderen die met een sjabloon zijn gemaakt](#delete-tasks-created-from-a-template) in dit artikel.

* Verwijder de sjabloon uit Workfront. Als u de sjabloon uit Workfront verwijdert, worden de taken die aan de sjabloon zijn toegevoegd, niet verwijderd uit projecten.

   Zie voor meer informatie [Projectsjablonen verwijderen](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Taken verwijderen die met een sjabloon zijn gemaakt {#delete-tasks-created-from-a-template}

1. Ga naar de **Taken** van het project.
1. Voer een van de volgende handelingen uit:

   * Maak een filter voor de takenlijst om alleen taken weer te geven die met de volgende instructie zijn gemaakt op basis van een sjabloon:

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      Voor informatie over het maken van een filter raadpleegt u [Filters maken of bewerken in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      Wanneer u het filter toepast, worden alleen taken die aan een Sjabloontaak-id zijn gekoppeld, in de lijst weergegeven.

   * Maak een weergave voor de takenlijst om de **Sjabloontaak-id** of **Naam sjabloontaak** in een kolom.

      Wanneer u de mening toepast, werden de taken die informatie in identiteitskaart van de Taak van het Malplaatje of de naamkolom van de Taak van het Malplaatje bevatten gecreeerd gebruikend een malplaatje.

      Voor informatie over het maken van een weergave raadpleegt u [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Selecteer alle taken die in Stap 2 worden geïdentificeerd zoals die van een malplaatje worden gecreeerd, dan klik **Het pictogram Verwijderen****> Ja, verwijderen**. Zie voor meer informatie [Taken verwijderen](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
