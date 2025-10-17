---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Een aangepaste status verwijderen
description: U kunt een aangepaste systeemstatus verwijderen als deze niet langer nuttig is voor uw organisatie.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Een aangepaste status verwijderen

U kunt een aangepaste systeemstatus verwijderen als deze niet langer nuttig is voor uw organisatie.

Of de status vergrendeld of ontgrendeld is, bepaalt of de status voor alle groepen in het systeem wordt verwijderd:

* Wanneer u een systeemstatus verwijdert die momenteel is vergrendeld, wordt de status verwijderd voor alle groepen in het systeem, ongeacht of de naam van de groep is gewijzigd.
* Wanneer u daarentegen een systeemstatus verwijdert die momenteel is ontgrendeld, blijft de status van alle groepen in het systeem behouden.


>[!NOTE]
>
>U kunt het volgende niet verwijderen:
>
>* Een vergrendelde of ontgrendelde systeemstatus die wordt gebruikt in een systeemgoedkeuringsproces dat momenteel in afwachting is van goedkeuring voor ten minste één object in uw systeem.
>
>  U kunt echter een ontgrendelde systeemstatus verwijderen die wordt gebruikt in een goedkeuringsproces op basis van één gebruik of op groepsniveau dat momenteel in afwachting is van goedkeuring.
>
>  U kunt een rapport uitvoeren om de objecten te zoeken en de goedkeuringen in behandeling op te lossen en vervolgens opnieuw proberen om de status te verwijderen. Voor instructies, zie [ de voorwerpen van de Lijst met een hangende goedkeuringsprocessen gebruikend een bepaalde status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Statussen die worden gebruikt in goedkeuringsprocessen die momenteel in afwachting zijn van goedkeuring voor ten minste één object in uw systeem.

Voor instructies bij het schrappen van een groepsstatus, zie [ een groepsstatus schrappen ](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aangepaste systeemstatus verwijderen

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Voorkeur van het Project** > **Statussen**.

1. Om de status over het volledige systeem (met inbegrip van individuele groepen), muis over de status te schrappen, geeft de klik **** uit, dan zorgt ervoor dat **Slot voor alle groepen** wordt geselecteerd. Klik **sparen**.

   of

   Om de systeemstatus te schrappen maar het voor individuele groepen, muis over de status te behouden, **uitgeeft**, dan zorg ervoor dat **Slot voor alle groepen** niet geselecteerd is. Klik **sparen**.

1. Beweeg over de status u wilt schrappen, dan **Schrapping** klikken.
1. In het bericht dat verschijnt, klik **Status van de Schrapping**.
1. In de **doos van de Status van de Schrapping** die toont, selecteer een status op het gebied geëtiketteerd **plaats momenteel alle projecten met deze status aan**.

   Projecten die de status gebruikten die u verwijdert, worden ingesteld op de status die u selecteert.

   Statussen zijn alleen beschikbaar in de vervolgkeuzelijst als ze overeenkomen met dezelfde status als de status die u verwijdert.

   Als u bijvoorbeeld een status verwijdert die gelijk is aan Huidig, kunnen alleen statussen worden geselecteerd die ook overeenkomen met Huidig.

1. Klik **Status van de Schrapping**.
