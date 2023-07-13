---
product-area: templates
navigation-topic: templates-navigation-topic
title: Een projectsjabloon maken
description: U kunt sjablonen maken en verwijderen vanuit het gebied Sjablonen. Wanneer het bouwen van een nieuw malplaatje, kunt u de informatie voor alle taken en alle informatie voor uw toekomstige projectmontages ingaan. Deze informatie zal dan aan het project overbrengen, wanneer u het van het malplaatje creeert.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Een projectsjabloon maken

U kunt sjablonen maken en verwijderen vanuit het gebied Sjablonen. Wanneer het bouwen van een nieuw malplaatje, kunt u de informatie voor alle taken en alle informatie voor uw toekomstige projectmontages ingaan. Deze informatie zal dan aan het project overbrengen, wanneer u het van het malplaatje creeert.

>[!NOTE]
>
>Een malplaatje en zijn taken hebben geen daadwerkelijke data, maar eerder een aanwijzing van welke dag (van wanneer het toekomstige project zou kunnen beginnen) een taak zou kunnen beginnen en op welke dag de taak zou kunnen moeten voltooien. Wanneer het gebruiken van malplaatjes om de toekomstige projecten tot stand te brengen, zullen de projecten daadwerkelijke data ontvangen. Zie voor meer informatie [Een project maken](../create-projects/create-project.md).


U kunt op de volgende manieren een nieuwe sjabloon maken:

* Geheel nieuw, zoals beschreven in dit artikel.
* Van bestaande projecten, door een project als malplaatje te bewaren.

  Voor meer informatie over het creëren van malplaatjes van bestaande projecten, zie [Een project opslaan als een sjabloon](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Door deze uit een andere sjabloon te kopiëren.

  Voor meer informatie over het kopiëren van een bestaande sjabloon raadpleegt u [Een projectsjabloon kopiëren](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Als u een Workfront-beheerder bent, kunt u sjablonen maken door blauwdrukken te importeren. Zie voor meer informatie [Een blauwdruk configureren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Toegangsvereisten

U moet het volgende hebben:

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
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Systeembeheerder voor het importeren van sjablonen uit blauwdrukken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot sjablonen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U hebt standaard beheerdersmachtigingen voor de sjablonen die u maakt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een sjabloon maken

1. Van de **Hoofdmenu** ![](assets/main-menu-icon.png) klikken **Sjablonen**.

1. Klikken **Nieuwe sjabloon**.

   De sjabloon heeft geen naam.

   ![Nieuwe sjabloon](assets/create-template-nwe-2022-350x102.png)

1. Geef een naam voor de nieuwe sjabloon op in de sjabloonkoptekst en druk vervolgens op **Enter.**
1. Klik op de knop **Sjabloontaken** in het linkerdeelvenster.
1. Klikken **Sjabloontaken toevoegen starten**.

   of

   Klikken **Nieuwe sjabloontaak** om taken aan uw sjabloon toe te voegen.

   Het toevoegen van malplaatjetaken aan een malplaatje is identiek aan het toevoegen van taken aan een project.

   Voor meer informatie over het toevoegen van taken aan een project, zie [Taken maken in een project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >U kunt geen terugkerende taken aan een sjabloon toevoegen.

1. (Optioneel) Klik op de knop **Gantt-grafiek** pictogram in de hoger-juiste hoek van de Lijst van de Taak om een visuele vertegenwoordiging van de de taaklijst van het malplaatje te zien.

   >[!TIP]
   >
   >U kunt taken niet rechtstreeks vanuit dit Gantt-diagram bewerken.

1. Als u informatie wilt toevoegen aan uw nieuwe sjabloon, klikt u op de knop **Meer** menu ![](assets/more-icon.png)en klik vervolgens op **Bewerken**.

   Voor informatie over het bewerken van een sjabloon raadpleegt u [Projectsjablonen bewerken](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Klikken **Wijzigingen opslaan**.
1. (Optioneel) Zie de sectie als u aanvullende items aan de sjabloon wilt toevoegen [Extra items aan een sjabloon toevoegen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) in het artikel [Projectsjablonen bewerken](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Sjablooninstellingen bepaald door groepskoppeling

De koppeling van een projectsjabloon met een groep (of het ontbreken ervan) bepaalt hoe project-, taak- en uitgiftevoorkeuren bepaalde instellingen in de sjabloon bepalen. Zie de sectie voor meer informatie [De projectsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) in het artikel [De projectsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
