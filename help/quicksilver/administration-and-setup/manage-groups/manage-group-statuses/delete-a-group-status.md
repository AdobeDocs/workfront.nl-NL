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
source-wordcount: '572'
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
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## Een groepsstatus verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen**.
1. Klik op de naam van de bovenste groep.
1. Klik in het linkerdeelvenster op **Statussen**.
1. Houd de muisaanwijzer boven de status die u wilt verwijderen in de lijst met statussen die worden weergegeven en klik vervolgens op **Verwijderen** wanneer het helemaal rechts lijkt.

   ![](assets/hover-click-delete.jpg)

1. In de doos die toont, selecteer een status om een vervangingsstatus voor voorwerpen (projecten, taken, kwesties, en goedkeuringsprocessen) aan te wijzen die de status gebruikten die u schrapt.

   Alleen statussen die overeenkomen met de status die u verwijdert, zijn beschikbaar. Als u bijvoorbeeld een status verwijdert die gelijk is aan Huidig, ziet u alleen statussen die gelijk zijn aan Huidig.

   De statussen die worden weergegeven, zijn ook afhankelijk van het feit of de status die u verwijdert, is ontgrendeld of vergrendeld:

   * **Als het ontgrendeld is**: Niet-verborgen vergrendelde en ontgrendelde statussen zijn beschikbaar.

      Samen met de statussen die voor de subgroep zijn gemaakt, worden statussen opgenomen die van systeemniveau- en bovenste groepen zijn overgenomen.

   * **Als het vergrendeld is**: Een van de volgende uitspraken is waar:

      * Als er andere vergrendelde, niet-verborgen statussen zijn, zijn alleen deze beschikbaar.
      * Als er geen vergrendelde, niet-verborgen status is, is de standaard Workfront-status beschikbaar, zelfs als deze verborgen of ontgrendeld is.

         Voor informatie over de standaard Workfront-statussen raadpleegt u [Heb toegang tot de lijst van de statussen van het systeemproject](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [De lijst met taakstatussen van het systeem openen](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)en de informatie over de vier vereiste uitgiftestatussen in [Toegang krijgen tot de lijst met systeemuitgiftestatussen](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Klikken **Status verwijderen**.

   Als de verwijderde status de standaardstatus voor dat type in de groep was, wordt de vervangende status gebruikt.

   Als de verwijderde status is ingesteld als de standaardprojectstatus in de projectvoorkeuren, wordt de voorkeur nu ingesteld op de vervangingsstatus.

## Wanneer een groep wordt verwijderd

Wanneer een groep wordt verwijderd en door een andere groep wordt vervangen, worden alle unieke statussen die de verwijderde groep had, toegevoegd aan de statussen van de vervangingsgroep. Zie voor meer informatie [Aangepaste statussen in een groep die wordt verplaatst of verwijderd](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
