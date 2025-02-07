---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Een groepstijdblad en de voorkeur voor uren vergrendelen of ontgrendelen
description: Als u een groepsbeheerder bent, kunt u een timesheet en een uurvoorkeur voor uw groep vormen en dan sluiten nadat een beheerder van Workfront het op het systeemniveau ontgrendelt.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Een groepsoverzicht en uurvoorkeur vergrendelen of ontgrendelen

Als u een groepsbeheerder bent, kunt u een timesheet en een uurvoorkeur voor uw groep vormen en dan sluiten nadat een beheerder van Workfront het op het systeemniveau ontgrendelt.

Als u een Adobe Workfront-voorkeur vergrendelt, zorgt u ervoor dat iedereen in uw groep en in de subgroepen dezelfde instelling gebruikt voor die voorkeur. Hoewel u een voorkeur kunt nog aanpassen die u sluit, kunnen de groepsbeheerders dit niet voor lagere subgroepen doen.

Omgekeerd, staat het ontgrendelen van een voorkeur op het groepsniveau subgroepbeheerders meer flexibiliteit toe om de manier te beheren hun groepen met die punten werken. Wanneer een voorkeur wordt ontgrendeld, kunnen groepsbeheerders deze opnieuw configureren voor deze subgroepen.

Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet vergrendelen of ontgrendelen.

Voor informatie over hoe een beheerder van Workfront een timesheet en een uurvoorkeur voor alle groepen in het systeem kan sluiten of ontgrendelen, zie [ timesheet en uurvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

Voor informatie over het vormen van een timesheet en een uurvoorkeur voor een groep, zie [ timesheet en uurvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md) vormen.

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een groepsoverzicht en uurvoorkeur vergrendelen of ontgrendelen

>[!TIP]
>
>Als u een Workfront-beheerder bent, kunt u de stappen 1 tot en met 4 omzeilen door naar Setup > Tijdblad en uren > Voorkeuren te gaan en vervolgens naar de naam van de groep te zoeken in het vak boven aan de pagina.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen**.
1. Klik op de naam van de groep waarin u tijdbladen en uren wilt vergrendelen of ontgrendelen.
1. In het linkerpaneel, klik **Tijdopnamen en de Voorkeur van Uren**.

1. Voer op de pagina die wordt weergegeven een van de volgende handelingen uit:

   * Als u beheerders van groepen onder uw groep een voorkeur voor hun groepen wilt kunnen vormen, ontgrendel het ![ knevel van de Ontgrendeling ](assets/unlock-toggle-button.png).
   * Als u alle groepen onder van u wilt gebruiken uw configuratie voor een voorkeur, zorg ervoor dat het gesloten ![ knevel van het Slot ](assets/lock-toggle-button.png) is (dit is het gebrek).

     >[!IMPORTANT]
     >
     >Het is belangrijk om met de beheerders en de gebruikers in groepen onder van u te communiceren om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het overgeërfd door hieronder om het even welke subgroepen. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders in lagere subgroups zouden kunnen hebben gemaakt.

1. Klik **sparen**.
