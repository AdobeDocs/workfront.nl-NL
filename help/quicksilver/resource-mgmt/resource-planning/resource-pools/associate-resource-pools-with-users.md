---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen koppelen aan gebruikers
description: Brongroepen koppelen aan gebruikers
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Brongroepen koppelen aan gebruikers

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.

U moet een bronnenpool maken voordat u deze aan gebruikers kunt koppelen.

U kunt gebruikers aan middelpools associëren wanneer u uw middelpools creeert.

Als u bronnenpools maakt zonder deze te vullen met gebruikers, kunt u deze later koppelen aan gebruikers terwijl u nieuwe gebruikers bewerkt of maakt.

Voor informatie over bronnenpools raadpleegt u [Overzicht van bronnenpools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Voor informatie over het maken van bronnenpools raadpleegt u [Brongroepen maken](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot bronnenbeheer bewerken, inclusief toegang tot Brongroepen beheren</p> <p>Toegang tot projecten, sjablonen en gebruikers bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de projecten, sjablonen en gebruikers beheren waaraan u de bronnengroepen koppelt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Brongroepen koppelen aan één gebruiker

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Gebruikers**.
1. Schakel het vakje naast de naam van een gebruiker in de lijst in en klik op **Bewerken**.
1. Klikken **Bronplanning**.
1. Begin de naam van een middelpool te typen die u met de gebruiker in wilt associëren **Brongroepen** en selecteert u deze in de lijst wanneer deze wordt weergegeven.\
   U kunt meerdere bronnenpools aan één gebruiker koppelen.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Klikken **Wijzigingen opslaan**.

Voor meer informatie over het bewerken van gebruikers raadpleegt u [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Ga voor meer informatie over het maken van nieuwe gebruikers naar [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Brongroepen koppelen aan gebruikers in bulk

U kunt meerdere gebruikers bulksgewijs bewerken en dezelfde bronnenpools aan alle gebruikers tegelijk koppelen.

Brongroepen koppelen aan meerdere gebruikers in bulk:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Gebruikers**.
1. Selecteer meerdere gebruikers in de lijst en klik op **Bewerken**.
1. Klikken **Bronplanning**.
1. Begin de naam van een middelpool te typen die u met de gebruikers in wilt associëren **Brongroepen** en selecteert u deze in de lijst wanneer deze wordt weergegeven.\
   U kunt meerdere bronnenpools koppelen aan meerdere gebruikers.

   >[!NOTE]
   >
   >Alleen de bronnenpools die alle geselecteerde gebruikers gemeen hebben, worden in dit veld weergegeven. Als de geselecteerde gebruikers geen gedeelde bronnenpools hebben, is dit veld leeg. Als dit veld leeg is, overschrijven de hier opgegeven bronnenpools hun afzonderlijke bronnenpools.

1. Klikken **Wijzigingen opslaan**.

Voor meer informatie over hoe u gebruikers bulksgewijs kunt bewerken, raadpleegt u [Gebruikersprofielen bulksgewijs bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
