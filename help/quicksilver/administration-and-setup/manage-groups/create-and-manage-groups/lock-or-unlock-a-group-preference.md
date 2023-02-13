---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Een project, taak of uitgiftevoorkeur voor subgroepen vergrendelen of ontgrendelen
description: Als groepsbeheerder, kunt u een project, een taak, of een uitgiftevoorkeur vormen en dan sluiten als een beheerder van Workfront het op systeemniveau heeft ontgrendeld.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Een project, taak of uitgiftevoorkeur voor subgroepen vergrendelen of ontgrendelen

Als groepsbeheerder, kunt u een project, een taak, of een uitgiftevoorkeur vormen en dan sluiten als een beheerder van Workfront het op systeemniveau heeft ontgrendeld.

Door een project, taak of uitgiftevoorkeur te vergrendelen die u op het niveau hebt geconfigureerd, zorgt u ervoor dat iedereen in uw groep en in de subgroepen dezelfde instelling voor die voorkeur gebruikt. Hoewel u een voorkeur nog kunt aanpassen die u voor uw groep sluit, kunnen de groepsbeheerders niet het voor groepen aanpassen.

Omgekeerd, staat het ontgrendelen van een project, een taak, of een uitgiftevoorkeur groepsbeheerders meer flexibiliteit toe om de manier te beheren hun groepen met die punten werken. Wanneer een voorkeur wordt ontgrendeld, kunnen groepsbeheerders deze opnieuw configureren voor deze subgroepen.

Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet vergrendelen of ontgrendelen.

Voor informatie over hoe een Workfront-beheerder een voorkeur voor alle groepen in het systeem kan vergrendelen of ontgrendelen, raadpleegt u [Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## Een groepsproject, taak of uitgave vergrendelen of ontgrendelen, voorkeur

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen**.
1. Klik op de naam van de groep waar u een projectvoorkeur wilt vergrendelen of ontgrendelen.
1. Klik in het linkerdeelvenster op **Projectvoorkeuren** of **Voorkeuren voor taken en problemen**.

1. Voer op de pagina die wordt weergegeven een van de volgende handelingen uit voor een voorkeur die op systeemniveau is ontgrendeld of voor een groep boven uw groep:

   * Als u wilt dat beheerders van groepen onder uw groep een voorkeur voor hun groepen kunnen vormen, ontgrendel het ![](assets/unlock-toggle-button.png).
   * Als u wilt dat alle groepen onder de uwe uw configuratie voor een voorkeur gebruiken, zorg ervoor dat het gesloten is ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >Het is belangrijk om met de beheerders en de gebruikers in groepen onder van u te communiceren om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het overgeërfd door hieronder om het even welke subgroepen. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders in lagere subgroups zouden kunnen hebben gemaakt.

1. Klikken **Opslaan**.
