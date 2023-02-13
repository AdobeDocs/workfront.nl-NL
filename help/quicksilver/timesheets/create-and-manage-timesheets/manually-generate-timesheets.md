---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tijdbladen handmatig genereren
description: Om veranderingen toe te laten die u aan de timesheet- profielen aanbracht om in huidige timesheets te weerspiegelen, moet u eerst bestaande timesheets schrappen en dan manueel nieuwe manueel produceren. U kunt tijdbladen handmatig genereren in het gedeelte Timesheets of in het gedeelte Diagnostics in Setup, zoals uitgelegd in dit artikel.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Tijdbladen handmatig genereren

Om veranderingen toe te laten die u aan de timesheet- profielen aanbracht om in huidige timesheets te weerspiegelen, moet u eerst bestaande timesheets schrappen en dan manueel nieuwe manueel produceren. U kunt tijdbladen handmatig genereren in het gedeelte Timesheets of in het gedeelte Diagnostics in Setup, zoals uitgelegd in dit artikel.

Voor instructies over het schrappen van timesheets, zie [Tijdschema&#39;s in Adobe Workfront verwijderen](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

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
   <td> <p>U moet een Workfront-beheerder zijn of, als u werkt aan timesheet-profielen voor een groep, u moet een groepsbeheerder (of Workfront-beheerder) zijn. Zie voor meer informatie <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a>.</p> <p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen over manueel geproduceerde timesheets

Wanneer u handmatig tijdbladen genereert:

* Ze worden gegenereerd op basis van de tijdlijnprofielen die aan uw gebruikers zijn gekoppeld. De gebruikers die geen chronologieprofielen verbonden aan hen hebben ontvangen geen timesheets. 
* Alleen de huidige tijdlijn en de volgende tijdlijn worden gegenereerd. Workfront genereert geen twee timesheets voor dezelfde periode. Als u reeds een timesheet voor een specifiek tijdkader hebt, zal een andere niet produceren wanneer u het handproces gebruikt om timesheets te produceren.

## Genereer handmatig tijdbladen vanuit het gebied Timesheets &amp; Hours

U kunt systeem-niveau of groep-vlakke timesheets van het gebied van Timesheets &amp; van Uren in Opstelling manueel produceren.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Als u timesheets in gebruik door het systeem produceert, klik **Timesheets en uren.**

   of

   Als u timesheets genereert die door een specifieke groep worden gebruikt, klikt u op **Groepen** en klikt u op de naam van de groep.

1. Klikken **Tijdbladprofielen**.
1. Klikken **Meer** vervolgens **Timesheets genereren**.

   Nieuwe tijdbladen worden gemaakt voor maximaal twee perioden voor gebruikers die aan tijdbladprofielen zijn gekoppeld.

## Tijdschema&#39;s op systeemniveau handmatig genereren vanuit het gebied Diagnostiek

U kunt handmatig tijdbladen op systeemniveau genereren in het gedeelte Diagnostiek in Setup.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Uitbreiden **Systeem** en klik vervolgens op **Diagnostiek**.

1. Klikken **Diagnostiek uitvoeren**. 
1. Klikken **Timesheets genereren**.
