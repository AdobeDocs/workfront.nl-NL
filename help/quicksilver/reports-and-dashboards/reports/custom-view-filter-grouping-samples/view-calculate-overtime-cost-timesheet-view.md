---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de kosten van overwerk berekenen in een tijdlijnweergave'
description: Overuren worden niet standaard berekend in Adobe Workfront, maar u kunt wel een rapport met een tijdlijnrapport maken dat overwerk berekent.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Weergave: de kosten van overwerk berekenen in een tijdlijnweergave

Overuren worden niet standaard berekend in Adobe Workfront, maar u kunt wel een rapport met een tijdlijnrapport maken dat overwerk berekent.

Als de gebruiker in zijn profiel aan een kostenpercentage per uur is gekoppeld, kunt u ook de hoeveelheid kosten voor de overuren van die gebruiker berekenen.\
Voor informatie over het associëren van gebruikers met Kosten per de tarieven van het Uur, zie het artikel [ Mijn Montages ](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) vormen.

>[!NOTE]
>
>Het gebied van Overwerk dat u aan een mening van de Chronologie in een lijst of een rapport kunt toevoegen toont de informatie die op het gebied van Overuren van timesheet wordt gevonden. Deze informatie wordt manueel bijgewerkt door een gebruiker met toegang om timesheet te wijzigen. Voor meer informatie over het gebied van Overuren in een timesheet, zie het artikel [ overzicht van de lay-out van de Tijdopnemer ](../../../timesheets/timesheets/timesheet-layout.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De kosten voor overwerk berekenen in een tijdlijnweergave

U voegt als volgt een berekende kolom Overuren toe aan een tijdlijnweergave:

1. Ga naar een lijst van chronologie, of creeer een Rapport van het Timesheet.

   Voor informatie over het creëren van rapporten, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Klik **aanpassen Mening** in een lijst van timesheets.

   of

   Selecteer het **lusje van Kolommen (Mening)** in een rapport van de Chronologie.

1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. In **toon in dit kolom** gebied, klik **om tekst** uit te geven.
1. Kopieer en kleef de volgende code van de tekstwijze op het **de wijze van de Tekst** dialoogvakje.
   <pre>displayname=Calculated Overtime Kosten <br> linkedname=direct <br> namekey=totalHours <br> querysort=totalHours <br> textmode=true <br> valueexpression=IF ({totalHours}&gt;40, ({totalHours} - 40)* {user}.{costPerHour}, {totalHours} * {user}.{costPerHour}) <br> valueFormat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Deze berekening veronderstelt dat de gebruiker gewoonlijk een week van 40 uur werkt.

1. Klik **sparen**, dan noem de nieuwe mening en klik **sparen Mening** in een lijst van timesheets.

   of

   Klik **sparen + Sluiten** in een rapport van de Chronologie.

1. (Facultatief en voorwaardelijk) als u een rapport van de Chronologie bouwt, specificeer een naam voor het rapport, dan klik **sparen Rapport**.

   De kosten van overwerk van elke gebruiker worden getoond in de **Berekende Kostprijs van Overwerk** kolom.

   ![ calculate_overtime_cost_in_timesheet_report.png ](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
