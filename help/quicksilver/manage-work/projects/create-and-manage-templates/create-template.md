---
product-area: templates
navigation-topic: templates-navigation-topic
title: Een projectsjabloon maken
description: U kunt sjablonen maken en verwijderen vanuit het gebied Sjablonen. Wanneer u een nieuwe sjabloon maakt, kunt u de informatie voor alle taken en voor uw toekomstige projectinstellingen invoeren. Deze informatie zal dan aan om het even welk project overbrengen dat u van het malplaatje creeert.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Een projectsjabloon maken

<!-- Audited: 1/2024 -->

U kunt sjablonen maken en verwijderen vanuit het gebied Sjablonen. Wanneer u een nieuwe sjabloon maakt, kunt u de informatie voor alle taken en voor uw toekomstige projectinstellingen invoeren. Deze informatie zal dan aan om het even welk project overbrengen dat u van het malplaatje creeert.

>[!NOTE]
>
>Een malplaatje en zijn taken hebben geen daadwerkelijke data, maar eerder een aanwijzing van welke dag (van wanneer het toekomstige project zou kunnen beginnen) een taak zou kunnen beginnen en op welke dag de taak zou kunnen moeten voltooien. Wanneer het gebruiken van malplaatjes om de toekomstige projecten tot stand te brengen, zullen de projecten daadwerkelijke data ontvangen. Voor informatie, zie [ een project ](../create-projects/create-project.md) creëren.


U kunt op de volgende manieren een nieuwe sjabloon maken:

* Geheel nieuw, zoals beschreven in dit artikel.
* Van bestaande projecten, door een project als malplaatje te bewaren.

  Voor meer informatie over het creëren van malplaatjes van bestaande projecten, zie [ sparen een project als malplaatje ](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Door deze uit een andere sjabloon te kopiëren.

  Voor meer informatie over het kopiëren van een bestaand malplaatje, zie [ een projectmalplaatje ](../../../manage-work/projects/create-and-manage-templates/copy-template.md) kopiëren.

* Door blauwdrukken te importeren. U moet een Workfront-beheerder zijn om blauwdrukken te kunnen importeren. Voor informatie, zie [ een blauwdruk ](../../../administration-and-setup/blueprints/configure-template-package.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

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
   <td> <p>Nieuw: Standaard </p><p>of </p><p>Huidig: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">U moet systeembeheerder zijn om malplaatjes van Blauwdrukken in te voeren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot sjablonen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U hebt standaard beheerdersmachtigingen voor de sjablonen die u maakt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een sjabloon maken

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Malplaatjes**.

1. Klik **Nieuw Malplaatje**.

   De sjabloon heeft geen naam.

   ![ Nieuw malplaatje ](assets/create-template-nwe-2022-350x102.png)

1. Specificeer een naam voor het nieuwe malplaatje in de malplaatjekopbal, dan druk **binnengaan.**
1. Klik de **sectie van de Taken van het Malplaatje** in het linkerpaneel.
1. Klik **Begin Toevoegend de Taken van het Malplaatje**.

   of

   Klik **Nieuwe Taak van het Malplaatje** beginnen taken aan uw malplaatje toe te voegen.

   Het toevoegen van malplaatjetaken aan een malplaatje is identiek aan het toevoegen van taken aan een project.

   Voor meer informatie over het toevoegen van taken aan een project, zie [ tot taken in een project ](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) leiden.

   >[!NOTE]
   >
   >U kunt geen terugkerende taken aan een sjabloon toevoegen.

1. (Facultatief) klik het **Gantt grafiekpictogram** in de hoger-juiste hoek van de Lijst van de Taak om een visuele vertegenwoordiging van de de taaklijst van het malplaatje te zien.

   >[!TIP]
   >
   >U kunt taken niet rechtstreeks vanuit dit Gantt-diagram bewerken.

1. Om informatie aan uw nieuw malplaatje toe te voegen, klik **Meer** menu ![ Meer pictogram ](assets/more-icon.png), dan klik **uitgeven**.

   Voor informatie over het uitgeven van een malplaatje, zie [ projectmalplaatjes ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

1. Klik **sparen Veranderingen**.
1. (Facultatief) als u extra punten aan het malplaatje wilt toevoegen, zie de sectie [ extra punten aan een malplaatje ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) in het artikel [ projectmalplaatjes ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

## Sjablooninstellingen bepaald door groepskoppeling

De koppeling van een projectsjabloon met een groep (of het ontbreken van een groep) bepaalt hoe project-, taak- en uitgiftevoorkeuren bepaalde instellingen in de sjabloon bepalen. Voor meer informatie, zie de sectie [ creeer en wijzig het projectmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) in het artikel [ creeer en wijzig het projectmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
