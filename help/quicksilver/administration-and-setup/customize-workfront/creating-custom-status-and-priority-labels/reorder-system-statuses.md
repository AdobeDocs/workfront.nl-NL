---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Statussen op systeemniveau en groepen opnieuw ordenen
description: Als beheerder van Workfront, kunt u de orde van project, taak veranderen, en status voor iedereen in het systeem of voor één enkele groep uitgeven.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Statussen op systeemniveau en groepen opnieuw ordenen

Als beheerder van Workfront, kunt u de orde van project, taak veranderen, en status voor iedereen in het systeem of voor één enkele groep uitgeven.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Het opnieuw ordenen van de statussen op systeemniveau heeft geen invloed op de volgorde van statussen binnen groepen.
>
>  Nochtans, erven de statussen binnen een pas gecreëerde top-level groep de orde van de systeem-vlakke statussen. (Een nieuwe subgroep erft de volgorde van de statussen in de groep één niveau omhoog.)
>
>* U kunt vergrendelde statussen opnieuw ordenen. Voor informatie over vergrendelde statussen raadpleegt u [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* De beheerders van de groep kunnen statussen ook herschikken die in hun groepen worden gebruikt. Zie voor meer informatie [Groepsstatussen opnieuw ordenen](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
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
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een Workfront-beheerder zijn. Voor informatie over Workfront-beheerders raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
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
    <ul> 
     <li>Huidig</li> 
     <li>Dead</li> 
     <li> In de wachtstand </li> 
     <li> Planning </li> 
     <li> Voltooid </li> 
     <li> Gevraagd </li> 
     <li> Goedgekeurd </li> 
     <li> Geweigerd </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nieuw</li> 
     <li>In uitvoering</li> 
     <li>Voltooid</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nieuw</li> 
     <li>In uitvoering</li> 
     <li>Opnieuw geopend</li> 
     <li>Nog geen feedback</li> 
     <li>In de wachtstand</li> 
     <li>Kan niet dupliceren</li> 
     <li>Gesloten</li> 
     <li>Opgelost</li> 
     <li>Geverifieerd voltooid</li> 
     <li>Geen oplossing</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Statussen opnieuw ordenen voor taken en projecten in het gehele systeem of voor een groep

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Projectvoorkeuren > Statussen**.
1. (Voorwaardelijk) als u statussen voor een groep opnieuw rangschikt, begin de naam van de groep in het vakje in de hoger-juiste hoek te typen, dan klik de naam wanneer het verschijnt.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Klik boven de lijst Statussen die wordt weergegeven op de knop **Projecten** of **Taken** tab.

1. Sleep de statussen naar de gewenste volgorde.

   De nieuwe statusvolgorde wordt automatisch opgeslagen.

1. Om de nieuwe statusorde te testen, ga naar een taak of een project, klik de status in de hoger-juiste hoek, en zorg ervoor de statussen die vertoning in de orde zijn die u vormde.

## Statussen opnieuw ordenen voor problemen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Projectvoorkeuren > Statussen.**
1. (Voorwaardelijk) als u statussen voor een groep opnieuw rangschikt, begin de naam van de groep in het vakje in de hoger-juiste hoek te typen, dan klik de naam wanneer het verschijnt.

   ![](assets/issue-statuses-group-name.png)

1. Klik op de knop **Problemen** tab.
1. (Optioneel) Selecteer een type uitgave (**Foutrapport**, **Volgorde wijzigen**, **Probleem**, of **Verzoek**).

   >[!NOTE]
   >
   >* U kunt de volgorde van statussen voor de Master lijst niet aanpassen.
   >* Wij adviseren dat u orde van statussen voor elke kwestie de zelfde manier typt. Voor meer informatie over emissietypen raadpleegt u [Aanvraagtypen configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Sleep de statussen naar de gewenste volgorde.

   De nieuwe statusvolgorde wordt automatisch opgeslagen.

1. Om de nieuwe statusorde te testen, ga naar een kwestie, klik de status in de hoger-juiste hoek, en zorg ervoor de statussen die vertoning in de orde zijn die u vormde.
