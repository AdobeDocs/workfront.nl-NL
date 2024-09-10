---
title: Het aantal licenties weergeven dat is toegewezen en gebruikt in een groep
description: Als beheerder van Adobe Workfront, kunt u tellingen van de individuele types van vergunningen bekijken die momenteel in uw groep en zijn subgroups worden gebruikt. Dit is nuttig wanneer u moet beoordelen of om vergunningen opnieuw te verdelen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Het aantal licenties weergeven dat is toegewezen en gebruikt in een groep

Als beheerder van Adobe Workfront, kunt u tellingen van de individuele types van vergunningen bekijken die momenteel in uw groep en zijn subgroups worden gebruikt. Dit is nuttig wanneer u moet beoordelen of om vergunningen opnieuw te verdelen.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!IMPORTANT]
>
>De licentie van een gebruiker wordt alleen in een bepaalde groep geteld als de groep de thuisgroep van de gebruiker is.

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

## Het aantal licenties weergeven dat in een groep wordt gebruikt

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep.
1. Op de pagina die, in het kopbalgebied dichtbij de hoger-juiste hoek toont, bekijk de **Vergunningen in gebruik** gebied om het aantal **Plan** en **het werk** vergunningen te zien momenteel worden gebruikt.

   Als u een groep op hoofdniveau bekijkt en de beheerder van Workfront een maximumaantal van elk vergunningstype voor de groep bepaalde, worden deze aantallen ook getoond. In de onderstaande groep kunnen maximaal 10 gebruikers bijvoorbeeld een licentie voor een abonnement hebben en 15 gebruikers kunnen een werkvergunning hebben:

   ![](assets/licenses-used-allocated.png)

   Voor informatie over hoe een beheerder van Workfront een maximumaantal toegewezen vergunningen voor een groep bepaalt, zie de sectie [ de maximumvergunningstelling voor een Groep van het Huis ](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) in het artikel [ beheert beschikbare vergunningen in uw systeem ](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Als de groep die u bekijkt een subgroep is, kunt u alleen het aantal gebruikte licenties weergeven en niet het maximumaantal licenties dat voor de groep is toegewezen. Workfront-beheerders definiëren namelijk geen maximumaantal licenties voor een subgroep.
   >
   >![](assets/subgroup-used-licenses-only.png)
   >

1. Voor afzonderlijke tellingen van elk type van vergunning momenteel gebruikt in de groep (met inbegrip van Overzicht en Verzoek), klik het tekstgebied direct onder **Vergunningen in gebruik:**

   ![](assets/click-text-to-see-more.png)

   Het vak dat wordt weergegeven, bevat dezelfde informatie voor alle vier de Workfront-licentietypen: Overzicht, Werkplan, Revisie en Verzoek. Onder aan het vak ziet u het totale aantal licenties dat door leden van deze groep of een van de subgroepen wordt gebruikt:

   ![](assets/more-license-info.png)

   Voor Revisie- en Request-licenties wordt in de kolom Max altijd Onbeperkt weergegeven.
