---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdbladen handmatig genereren
description: Om veranderingen toe te laten die u aan de timesheet- profielen aanbracht om in huidige timesheets te weerspiegelen, moet u eerst bestaande timesheets schrappen en dan manueel nieuwe manueel produceren. U kunt tijdbladen handmatig genereren in het gedeelte Timesheets of in het gedeelte Diagnostics in Setup, zoals uitgelegd in dit artikel.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Tijdbladen handmatig genereren

Om veranderingen toe te laten die u aan de timesheet- profielen aanbracht om in huidige timesheets te weerspiegelen, moet u eerst bestaande timesheets schrappen en dan manueel nieuwe manueel produceren. U kunt tijdbladen handmatig genereren in het gedeelte Timesheets of in het gedeelte Diagnostics in Setup, zoals uitgelegd in dit artikel.

Voor instructies bij het schrappen van timesheets, zie [ timesheets van de Schrapping in Adobe Workfront ](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een Workfront-beheerder zijn of, als u werkt aan timesheet-profielen voor een groep, u moet een groepsbeheerder (of Workfront-beheerder) zijn. Voor meer informatie, zie <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a>.</p> <p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

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
1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png), dan **produceer timesheets**.

   Nieuwe tijdbladen worden gemaakt voor maximaal twee perioden voor gebruikers die aan tijdbladprofielen zijn gekoppeld.

## Tijdschema&#39;s op systeemniveau handmatig genereren vanuit het gebied Diagnostiek

U kunt handmatig tijdbladen op systeemniveau genereren in het gedeelte Diagnostiek in Setup.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. Breid **Systeem** uit, dan klik **Diagnostiek**.

1. Klik **Diagnostiek van het Gedrag**. 
1. Klik **produceer Chronologie**.
