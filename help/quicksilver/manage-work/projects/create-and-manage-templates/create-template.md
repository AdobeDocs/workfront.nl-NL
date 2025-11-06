---
product-area: templates
navigation-topic: templates-navigation-topic
title: Een projectsjabloon maken
description: U kunt sjablonen maken en verwijderen vanuit het gebied Sjablonen. Wanneer u een nieuwe sjabloon maakt, kunt u de informatie voor alle taken en voor uw toekomstige projectinstellingen invoeren. Deze informatie zal dan aan om het even welk project overbrengen dat u van het malplaatje creeert.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Een projectsjabloon maken

<!-- Audited: 10/2025 -->

<div class="preview">

De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Dezelfde functies zijn ook beschikbaar in de productieomgeving voor alle klanten vanaf een week na de release Preview.

Voor meer informatie, zie [&#x200B; modernisering van de Interface &#x200B;](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

U kunt sjablonen maken en verwijderen vanuit het gebied Sjablonen. Wanneer u een nieuwe sjabloon maakt, kunt u de informatie voor alle taken en voor uw toekomstige projectinstellingen invoeren. Deze informatie zal dan aan om het even welk project overbrengen dat u van het malplaatje creeert.

>[!NOTE]
>
>Een malplaatje en zijn taken hebben geen daadwerkelijke data, maar eerder een aanwijzing van welke dag (van wanneer het toekomstige project zou kunnen beginnen) een taak zou kunnen beginnen en op welke dag de taak zou kunnen moeten voltooien. Wanneer het gebruiken van malplaatjes om de toekomstige projecten tot stand te brengen, zullen de projecten daadwerkelijke data ontvangen. Voor informatie, zie [&#x200B; een project &#x200B;](../create-projects/create-project.md) creëren.


U kunt op de volgende manieren een nieuwe sjabloon maken:

* Geheel nieuw, zoals beschreven in dit artikel.
* Van bestaande projecten, door een project als malplaatje te bewaren.

  Voor meer informatie over het creëren van malplaatjes van bestaande projecten, zie [&#x200B; sparen een project als malplaatje &#x200B;](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Door deze uit een andere sjabloon te kopiëren.

  Voor meer informatie over het kopiëren van een bestaand malplaatje, zie [&#x200B; een projectmalplaatje &#x200B;](../../../manage-work/projects/create-and-manage-templates/copy-template.md) kopiëren.

* Door blauwdrukken te importeren. U moet een Workfront-beheerder zijn om blauwdrukken te kunnen importeren. Voor informatie, zie [&#x200B; een blauwdruk &#x200B;](../../../administration-and-setup/blueprints/configure-template-package.md) vormen.

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
   <td> <p>Standard </p><p>Plan</p> <p>U moet systeembeheerder zijn om malplaatjes van Blauwdrukken in te voeren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot sjablonen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U hebt standaard beheerdersmachtigingen voor de sjablonen die u maakt</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Een sjabloon maken

{{step1-to-templates}}

1. Klik **Nieuw Malplaatje**.

   De sjabloon heeft geen naam.

   ![&#x200B; Nieuw malplaatje &#x200B;](assets/create-template-nwe-2022-350x102.png)

1. Specificeer een naam voor het nieuwe malplaatje in de malplaatjekopbal, dan druk **binnengaan.**
1. Klik de **sectie van de Taken van het Malplaatje** in het linkerpaneel.
1. Klik **Begin Toevoegend de Taken van het Malplaatje** om taken binnen toe te voegen

   of

   Klik **Nieuwe Taak van het Malplaatje** beginnen taken aan uw malplaatje in de **Nieuwe Taak van het Malplaatje** doos toe te voegen.

   ![&#x200B; Nieuwe doos van de Taak van het Malplaatje &#x200B;](assets/new-template-task-box.png)

   <span class="preview"> **creeer de Taak van het Malplaatje** doos opent in de nieuwe ervaring.</span>

1. <span class="preview"> (Voorwaardelijk) Gebruikend de nieuwe ervaring, werk informatie op de volgende gebieden in **tot de Taak van het Malplaatje** doos bij:</span>

   <div class="preview">

   * Naam sjabloontaak
   * Overzicht
   * Toewijzingen
   * Financiën
   * Aangepaste Forms
   * Documenten
   * Instellingen

   </div>

1. Klik **creeer malplaatjetaak**

   of

   <span class="preview"> klik **Schakelaar terug naar oude ervaring** bij de bodem van **creeer de Taak van het Malplaatje** doos.</span>
   <span class="preview"> de **Nieuwe Taak van het Malplaatje** opent in de oude ervaring.</span>

   >[!TIP]
   >
   >In Productie, opent de oude ervaring door gebrek.

1. De informatie van de update op de volgende gebieden in het **Nieuwe vakje van de Taak van het Malplaatje**:

   * Overzicht
   * Financiën
   * Instellingen
   * Toewijzingen
   * Aangepaste Forms
   * Document bijvoegen

     Het bijwerken van informatie voor een malplaatjetaak is gelijkaardig aan het uitgeven van taken over een project. Voor meer informatie, zie [&#x200B; taken &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven. <!--should this be relinked at preview/ prod release to say it's the same as Edit template tasks??-->

   >[!NOTE]
   >
   >U kunt geen terugkerende taken aan een sjabloon toevoegen.

1. Klik op een van de volgende opties:

   * **sparen de Taak van het Malplaatje** om de huidige malplaatjetaak te bewaren en het Nieuwe vakje van de Taak van het Malplaatje te sluiten.
   * **sparen de Taak van het Malplaatje &amp; Begin een andere** om de huidige malplaatjetaak te bewaren en een andere **Nieuwe doos van de Taak van het Malplaatje te openen** om een andere taak toe te voegen.
   * **annuleert** om de doos te sluiten zonder de malplaatjetaak op te slaan.
1. (Facultatief) na het toevoegen van de malplaatjetaken, in de sectie van de Taken van het Malplaatje, klik het **pictogram van de Gantt- grafiek in de hoger-juiste hoek van de Lijst van de Taak om een visuele vertegenwoordiging van de de taaklijst van het malplaatje te zien.**

   >[!TIP]
   >
   >U kunt taken niet rechtstreeks vanuit dit Gantt-diagram bewerken.

1. Om informatie aan uw nieuw malplaatje toe te voegen, klik **Meer** menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan de linkerzijde van de malplaatjenaam in de kopbal, dan klik **uitgeven**.

   Voor informatie over het uitgeven van een malplaatje, zie [&#x200B; projectmalplaatjes &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

   >[!NOTE]
   >
   >   De koppeling van een projectsjabloon met een groep (of het ontbreken van een groep) bepaalt hoe project-, taak- en uitgiftevoorkeuren bepaalde instellingen in de sjabloon bepalen.
   >
   >Voor meer informatie, zie de sectie &quot;hoe voorkeur op malplaatjes en malplaatjetaken&quot;in het artikel [&#x200B; van toepassing is creeer en wijzig het projectmalplaatjes van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

1. Klik **sparen**.
1. (Optioneel) Voeg de volgende items aan de sjabloon toe

   * Documenten
   * Risico&#39;s
   * Goedkeuringsprocessen
   * Factureringstarieven
   * Uitgaven
   * Wachtrij
   * Onderwerpgroepen en onderwerpen in de wachtrij

1. (Optioneel) Voeg de volgende items toe aan de taken in de sjabloon:

   * Documenten
   * Uitgaven
   * Goedkeuringen

   Voor informatie, zie de sectie &quot;meer punten aan een malplaatje&quot;in het artikel [&#x200B; toevoegen projectmalplaatjes &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeeft.




