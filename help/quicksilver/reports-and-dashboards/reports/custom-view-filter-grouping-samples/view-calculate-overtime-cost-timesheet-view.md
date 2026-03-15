---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Calculate Overtime Cost in a Timesheet View'
description: Overtime is not calculated by default in Adobe Workfront, but you can create a Timesheet report that calculates overtime.
author: Courtney
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# View: calculate overtime cost in a Timesheet View

<!--Audited: 11/2024-->

Overuren worden niet standaard berekend in Adobe Workfront, maar u kunt wel een rapport met een tijdlijnrapport maken dat overwerk berekent.

Als de gebruiker in zijn profiel aan een kostenpercentage per uur is gekoppeld, kunt u ook de hoeveelheid kosten voor de overuren van die gebruiker berekenen.\
For information about associating users with Cost per Hour rates, see the article [Configure My Settings](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>The Overtime field that you can add to a Timesheet view in a list or a report displays the information found in the Overtime field of the timesheet. This information is updated manually by a user with access to modify the timesheet. For more information about the Overtime field in a timesheet, see the article [Timesheet layout overview](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Calculate overtime cost in a Timesheet View

To add a calculated Overtime column to a timesheet view:

1. Ga naar een lijst met tijdbladen.

1. Klik het **drop-down menu van de Mening**, dan klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom**.
1. Click **Switch to Text Mode**, then click **Edit Text Mode**.
1. In the **Edit Text Mode** box, remove the text in the box, then copy and paste the following text mode code:

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >This calculation assumes that the user usually works a 40-hour week.

1. Click **Done**, then name the new view and click **Save View** in a list of timesheets.

   The cost of the overtime of each user is displayed in the **Calculated Overtime Cost** column.


