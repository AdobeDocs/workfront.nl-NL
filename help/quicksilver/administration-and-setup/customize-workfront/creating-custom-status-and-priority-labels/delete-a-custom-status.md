---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Een aangepaste status verwijderen
description: U kunt een aangepaste systeemstatus verwijderen als deze niet langer nuttig is voor uw organisatie.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
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
>  U kunt een rapport uitvoeren om de objecten te zoeken en de goedkeuringen in behandeling op te lossen en vervolgens opnieuw proberen om de status te verwijderen. Zie voor instructies [Objecten met een bepaalde status weergeven die in behandeling zijn](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Statussen die worden gebruikt in goedkeuringsprocessen die momenteel in afwachting zijn van goedkeuring voor ten minste één object in uw systeem.


Voor instructies over het verwijderen van een groepsstatus raadpleegt u [Een groepsstatus verwijderen](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een aangepaste systeemstatus verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Projectvoorkeuren** > **Statussen**.

1. Als u de status in het hele systeem wilt verwijderen (ook voor afzonderlijke groepen), klikt u met de muis op de status **Bewerken** zorgt ervoor dat **Vergrendelen voor alle groepen** is geselecteerd. Klikken **Opslaan**.

   of

   Als u de systeemstatus wilt verwijderen maar deze voor afzonderlijke groepen wilt behouden, klikt u met de muis op de status **Bewerken** zorgt ervoor dat **Vergrendelen voor alle groepen** is uitgeschakeld. Klikken **Opslaan**.

1. Houd de cursor boven de status die u wilt verwijderen en klik vervolgens op **Verwijderen**.
1. Klik in het bericht dat wordt weergegeven op **Status verwijderen**.
1. In de **Status verwijderen** die wordt weergegeven, selecteert u een status in het veld met het label **Stel alle projecten met deze status in op**.

   Projecten die de status gebruikten die u verwijdert, worden ingesteld op de status die u selecteert.

   Statussen zijn alleen beschikbaar in de vervolgkeuzelijst als ze overeenkomen met dezelfde status als de status die u verwijdert.

   Als u bijvoorbeeld een status verwijdert die gelijk is aan Huidig, kunnen alleen statussen worden geselecteerd die ook overeenkomen met Huidig.

1. Klikken **Status verwijderen**.
