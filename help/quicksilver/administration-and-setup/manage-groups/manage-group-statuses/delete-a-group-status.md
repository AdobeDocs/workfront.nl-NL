---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Een groepsstatus verwijderen
description: Als groepsbeheerder, kunt u een status voor een groep schrappen die u beheert als het niet als vereiste of gesloten status op het systeemniveau, of voor een hogere groep in de hiërarchie wordt gevormd.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Een groepsstatus verwijderen

Als groepsbeheerder, kunt u een status voor een groep schrappen die u beheert als het niet als vereiste of gesloten status op het systeemniveau, of voor een hogere groep in de hiërarchie wordt gevormd.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!NOTE]
>
>U kunt het volgende niet verwijderen:
>
>* De ingebouwde statussen Planning, Huidig, en Volledig. U kunt hun namen bijwerken, hun kleuren bewerken en vergrendelen of ontgrendelen, maar ze kunnen niet worden verwijderd.
>* Statussen die zich in een toestand van goedkeuring bevinden voor ten minste één object dat aan de groep of een van de subgroepen ervan is gekoppeld.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> verlenen een gebruiker volledige administratieve toegang </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; als u moet weten welk plan of licentietype u hebt, contacteer uw beheerder van Workfront.

## Een groepsstatus verwijderen

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. In het linkerpaneel, klik **Groepen**.
1. Klik op de naam van de bovenste groep.
1. In het linkerpaneel klik **Statussen**.
1. In de lijst van statussen die toont, over de status bewegen u wilt schrappen, dan **Schrapping** klikken wanneer het aan uiterst rechts verschijnt.

   ![](assets/hover-click-delete.jpg)

1. In de doos die toont, selecteer een status om een vervangingsstatus voor voorwerpen (projecten, taken, kwesties, en goedkeuringsprocessen) aan te wijzen die de status gebruikten die u schrapt.

   Alleen statussen die overeenkomen met de status die u verwijdert, zijn beschikbaar. Als u bijvoorbeeld een status verwijdert die gelijk is aan Huidig, ziet u alleen statussen die gelijk zijn aan Huidig.

   De statussen die worden weergegeven, zijn ook afhankelijk van het feit of de status die u verwijdert, is ontgrendeld of vergrendeld:

   * **als het** ontgrendeld is: De niet-verborgen gesloten en ontgrendelde statussen zijn beschikbaar.

     Samen met de statussen die voor de subgroep zijn gemaakt, worden statussen opgenomen die van systeemniveau- en bovenste groepen zijn overgenomen.

   * **als het** gesloten is: Één van het volgende is waar:

      * Als er andere vergrendelde, niet-verborgen statussen zijn, zijn alleen deze beschikbaar.
      * Als er geen vergrendelde, niet-verborgen status is, is de standaard Workfront-status beschikbaar, zelfs als deze verborgen of ontgrendeld is.

        Voor informatie over de status standaard van Workfront, zie [ Toegang tot de lijst van de statussen van het systeemproject ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [ toegang tot de lijst van de statussen van de systeemtaak ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md), en de informatie over de 4 vereiste uitgevende status in [ toegang tot de lijst van de statussen van de systeemkwestie ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Klik **Status van de Schrapping**.

   Als de verwijderde status de standaardstatus voor dat type in de groep was, wordt de vervangende status gebruikt.

   Als de verwijderde status is ingesteld als de standaardprojectstatus in de projectvoorkeuren, wordt de voorkeur nu ingesteld op de vervangingsstatus.

## Wanneer een groep wordt verwijderd

Wanneer een groep wordt verwijderd en door een andere groep wordt vervangen, worden alle unieke statussen die de verwijderde groep had, toegevoegd aan de statussen van de vervangingsgroep. Voor meer informatie, zie {de statussen van 0} Douane in een groep die wordt bewogen of ](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md) geschrapt.[
