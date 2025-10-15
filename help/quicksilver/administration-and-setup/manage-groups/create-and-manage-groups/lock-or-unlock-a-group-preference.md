---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Een project-, taak- of Issue-voorkeur voor subgroepen vergrendelen of ontgrendelen
description: Als groepsbeheerder, kunt u een project, een taak, of een uitgiftevoorkeur vormen en dan sluiten als een beheerder van Workfront het op systeemniveau heeft ontgrendeld.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Een project, taak of uitgave van subgroepen vergrendelen of ontgrendelen

Als groepsbeheerder, kunt u een project, een taak, of een uitgiftevoorkeur vormen en dan sluiten als een beheerder van Workfront het op systeemniveau heeft ontgrendeld.

Door een project, taak of uitgiftevoorkeur te vergrendelen die u op het niveau hebt geconfigureerd, zorgt u ervoor dat iedereen in uw groep en in de subgroepen dezelfde instelling voor die voorkeur gebruikt. Hoewel u een voorkeur nog kunt aanpassen die u voor uw groep sluit, kunnen de groepsbeheerders niet het voor groepen aanpassen.

Omgekeerd, staat het ontgrendelen van een project, een taak, of een uitgiftevoorkeur groepsbeheerders meer flexibiliteit toe om de manier te beheren hun groepen met die punten werken. Wanneer een voorkeur wordt ontgrendeld, kunnen groepsbeheerders deze opnieuw configureren voor deze subgroepen.

Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet vergrendelen of ontgrendelen.

Voor informatie over hoe een beheerder van Workfront een voorkeur voor alle groepen in het systeem kan sluiten of ontgrendelen, zie [&#x200B; Vergrendelen of projectvoorkeur voor alle groepen in het systeem &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md) ontgrendelen.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Het configureren van een niet-vergrendelde voorkeur voor een groep heeft geen invloed op die voorkeur voor subgroepen onder de groep.
>
>  Wanneer echter een nieuwe subgroep wordt gemaakt, neemt deze de voorkeursinstellingen en de vergrendelde of ontgrendelde status over van de groep direct erboven.
>
>* Als u een groep verplaatst onder een groep met een vergrendelde voorkeur, neemt de verplaatste groep die voorkeur over en is deze vergrendeld voor de verplaatste groep.
>* Als u een groep verplaatst onder een groep waarvoor een niet-vergrendelde voorkeur geldt, heeft die voorkeur geen invloed op de verplaatste groep.
>
>  Als de voorkeur in de verplaatste groep op het tijdstip van de beweging wordt gesloten, blijft het gesloten, maar de groepbeheerder kan het nu ontgrendelen omdat het voor de oudergroep wordt ontgrendeld.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr>
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een groepsproject, taak of uitgave vergrendelen of ontgrendelen, voorkeur

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen**.
1. Klik op de naam van de groep waar u een projectvoorkeur wilt vergrendelen of ontgrendelen.
1. In het linkerpaneel, klik {de Voorkeur van het 0} Project **of** de Voorkeur van Taken &amp; van Kwesties **.**

1. Voer op de pagina die wordt weergegeven een van de volgende handelingen uit voor een voorkeur die op systeemniveau is ontgrendeld of voor een groep boven uw groep:

   * Als u beheerders van groepen onder uw groep een voorkeur voor hun groepen wilt kunnen vormen, ontgrendel het ![&#x200B; knevel van de Ontgrendeling &#x200B;](assets/unlock-toggle-button.png).
   * Als u alle groepen onder van u uw configuratie voor een voorkeur wilt gebruiken, zorg ervoor dat het gesloten ![&#x200B; knevel van het Slot &#x200B;](assets/lock-toggle-button.png) is.

     >[!IMPORTANT]
     >
     >Het is belangrijk om met de beheerders en de gebruikers in groepen onder van u te communiceren om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het overgeërfd door hieronder om het even welke subgroepen. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders in lagere subgroups zouden kunnen hebben gemaakt.

1. Klik **sparen**.
