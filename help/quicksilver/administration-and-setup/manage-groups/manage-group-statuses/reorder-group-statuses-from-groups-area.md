---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Groepsstatussen opnieuw ordenen
description: Als groepsbeheerder, kunt u de orde van project, taak veranderen, en status voor een groep uitgeven u beheert.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
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
>* U kunt vergrendelde statussen opnieuw ordenen. Voor informatie over vergrendelde statussen raadpleegt u [Een groepsstatus maken of bewerken](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## Toegangsvereisten

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
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

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

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** en klikt u op de naam van de groep.
1. Klik in het linkerdeelvenster op **Statussen**.
1. Klik boven de lijst Statussen die wordt weergegeven op de knop **Projecten** of **Taken** tab.

1. Sleep de statussen naar de gewenste volgorde.

   De nieuwe statusvolgorde wordt automatisch opgeslagen.

1. Om de nieuwe statusorde te testen, ga naar een taak of een project verbonden aan de groep, klik de status in de hoger-juiste hoek, en zorg ervoor de statussen die vertoning in de orde zijn die u vormde.

## Statussen opnieuw ordenen voor problemen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** en klikt u op de naam van de groep.
1. Klik in het linkerdeelvenster op **Statussen**.
1. Klik op de knop **Problemen** tab.
1. (Optioneel) Selecteer een type uitgave (**Foutrapport**, **Volgorde wijzigen**, **Probleem**, of **Verzoek**).

   >[!NOTE]
   >
   >* U kunt de volgorde van statussen voor de Master lijst niet aanpassen.
   >* Wij adviseren dat u orde van statussen voor elke kwestie de zelfde manier typt. Voor meer informatie over emissietypen raadpleegt u [Aanvraagtypen configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Sleep de statussen naar de gewenste volgorde.

   De nieuwe statusvolgorde wordt automatisch opgeslagen.

1. Om de nieuwe statusorde te testen, ga naar een kwestie verbonden aan de groep, klik de status in de hoger-juiste hoek, en zorg ervoor de statussen die vertoning in de orde zijn die u vormde.
