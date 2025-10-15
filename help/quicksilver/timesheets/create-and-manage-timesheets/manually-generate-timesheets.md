---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdbladen handmatig genereren
description: Om veranderingen toe te laten die u aan de timesheet- profielen aanbracht om in huidige timesheets te weerspiegelen, moet u eerst bestaande timesheets schrappen en dan manueel nieuwe manueel produceren. U kunt tijdbladen handmatig genereren in het gedeelte Timesheets of in het gedeelte Diagnostics in Setup, zoals uitgelegd in dit artikel.
author: Lisa
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Tijdbladen handmatig genereren

Om veranderingen toe te laten die u aan de timesheet- profielen aanbracht om in huidige timesheets te weerspiegelen, moet u eerst bestaande timesheets schrappen en dan manueel nieuwe manueel produceren. U kunt tijdbladen handmatig genereren in het gedeelte Timesheets of in het gedeelte Diagnostics in Setup, zoals uitgelegd in dit artikel.

Voor instructies bij het schrappen van timesheets, zie [&#x200B; timesheets van de Schrapping in Adobe Workfront &#x200B;](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

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
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td><p>U moet een Workfront-beheerder zijn of, als u werkt aan timesheet-profielen voor een groep, u moet een groepsbeheerder (of Workfront-beheerder) zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen over manueel geproduceerde timesheets

Wanneer u handmatig tijdbladen genereert:

* Ze worden gegenereerd op basis van de tijdlijnprofielen die aan uw gebruikers zijn gekoppeld. De gebruikers die geen chronologieprofielen verbonden aan hen hebben ontvangen geen timesheets.
* Alleen de huidige tijdlijn en de volgende tijdlijn worden gegenereerd. Workfront genereert geen twee timesheets voor dezelfde periode. Als u reeds een timesheet voor het huidige tijdkader hebt, zal een andere niet produceren wanneer u het handproces gebruikt om timesheets te produceren.

## Genereer handmatig tijdbladen vanuit het gebied Timesheets &amp; Hours

U kunt systeem-niveau of groep-vlakke timesheets van het gebied van Timesheets &amp; van Uren in Opstelling manueel produceren.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. Als u timesheets in gebruik door het systeem produceert, klik **Chronologie &amp; Uren.**

   of

   Als u timesheets produceert die door een specifieke groep worden gebruikt, klik **Groepen**, dan klik de naam van de groep.

1. Klik **Profielen van de Chronologie**.
1. Klik het meer pictogram ![&#x200B; meer pictogram &#x200B;](assets/more-icon.png), dan **produceer Chronologie**.

1. Bij de bovenkant van de lijst van het timesheet profiel, klik het **Meer** pictogram ![&#x200B; pictogram &#x200B;](assets/more-icon.png) voor systeem-vlakke timesheet profielen, of **Meer**, voor groep timesheet profielen, dan klik **timesheets** produceren.

   Nieuwe tijdbladen worden gemaakt voor maximaal twee perioden voor gebruikers die aan tijdbladprofielen zijn gekoppeld.

## Tijdschema&#39;s op systeemniveau handmatig genereren vanuit het gebied Diagnostiek

U kunt handmatig tijdbladen op systeemniveau genereren in het gedeelte Diagnostiek in Setup.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. Breid **Systeem** uit, dan klik **Diagnostiek**.

1. Klik **Diagnostiek van het Gedrag**.
1. Klik **produceer Chronologie**.
