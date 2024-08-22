---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Groepstatussen opnieuw ordenen
description: Als groepsbeheerder, kunt u de orde van project, taak veranderen, en status voor een groep uitgeven u beheert.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Groepsstatussen opnieuw ordenen

Als groepsbeheerder, kunt u de orde van project, taak veranderen, en status voor een groep uitgeven u beheert.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!NOTE]
>
>* Een Workfront-beheerder kan de statussen opnieuw ordenen op systeemniveau. Dit heeft geen invloed op de volgorde van statussen in groepen.
>
>  Nochtans, erven de statussen binnen een pas gecreëerde top-level groep de orde van de systeem-vlakke statussen. (Een nieuwe subgroep erft de volgorde van de statussen in de groep één niveau omhoog.)
>
>* U kunt vergrendelde statussen opnieuw ordenen. Voor informatie over gesloten statussen, zie [ tot stand brengen of een groepsstatus ](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) uitgeven.
>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement* </td> 
   <td>Alle</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> verlenen een gebruiker volledige administratieve toegang </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; als u moet weten welk plan of licentietype u hebt, contacteer uw beheerder van Workfront.

+++

## Standaardvolgorde van statussen

Statussen worden standaard in de volgende volgorde weergegeven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Project</th> 
   <th width="33.33%">Taak</th> 
   <th width="33.33%">Probleem</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>Huidig</p> 
     <p>Dead</p> 
     <p> In de wachtstand </p> 
     <p> Planning </p> 
     <p> Voltooid </p> 
     <p> Gevraagd </p> 
     <p> Goedgekeurd </p> 
     <p> Geweigerd </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>Nieuw</p> 
     <p>In uitvoering</p> 
     <p>Voltooid</p> 
   </td> 
   <td> 
     <p>Nieuw</p> 
     <p>In uitvoering</p> 
     <p>Opnieuw geopend</p> 
     <p>Nog geen feedback</p> 
     <p>In de wachtstand</p> 
     <p>Kan niet dupliceren</p> 
     <p>Gesloten</p> 
     <p>Opgelost</p> 
     <p>Geverifieerd voltooid</p> 
     <p>Geen oplossing</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Statussen opnieuw ordenen voor taken en projecten in een groep die u beheert

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen**, dan klik de naam van de groep.
1. In het linkerpaneel, klik **Statussen**.
1. Boven de lijst van Statussen die toont, klik de **Projecten** of **Taken** tabel.

1. Sleep de statussen naar de gewenste volgorde.

   De nieuwe statusvolgorde wordt automatisch opgeslagen.

1. Om de nieuwe statusorde te testen, ga naar een taak of een project verbonden aan de groep, klik de status in de hoger-juiste hoek, en zorg ervoor de statussen die vertoning in de orde zijn die u vormde.

## Statussen opnieuw ordenen voor problemen

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen**, dan klik de naam van de groep.
1. In het linkerpaneel, klik **Statussen**.
1. Klik de **Kwesties** tabel.
1. (Facultatief) selecteer een type van kwestie (**Bug Rapport**, **de Orde van de Verandering**, **Uitgave**, of **Verzoek**).

   >[!NOTE]
   >
   >* U kunt de volgorde van statussen voor de hoofdlijst niet aanpassen.
   >* Wij adviseren dat u orde van statussen voor elke kwestie de zelfde manier typt. Voor meer informatie over kwesties types, zie [ aanvraagtypes ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md) vormen.

1. Sleep de statussen naar de gewenste volgorde.

   De nieuwe statusvolgorde wordt automatisch opgeslagen.

1. Om de nieuwe statusorde te testen, ga naar een kwestie verbonden aan de groep, klik de status in de hoger-juiste hoek, en zorg ervoor de statussen die vertoning in de orde zijn die u vormde.
