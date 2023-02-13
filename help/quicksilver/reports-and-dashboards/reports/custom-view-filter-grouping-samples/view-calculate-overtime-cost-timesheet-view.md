---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: de kosten van overwerk berekenen in een tijdlijnweergave"'
description: Overuren worden niet standaard berekend in Adobe Workfront, maar u kunt wel een rapport met een tijdlijnrapport maken dat overwerk berekent.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Weergave: de kosten van overwerk berekenen in een tijdlijnweergave

Overuren worden niet standaard berekend in Adobe Workfront, maar u kunt wel een rapport met een tijdlijnrapport maken dat overwerk berekent.

Als de gebruiker in zijn profiel aan een kostenpercentage per uur is gekoppeld, kunt u ook de hoeveelheid kosten voor de overuren van die gebruiker berekenen.\
Raadpleeg het artikel voor informatie over het koppelen van gebruikers aan kosten per uur [Mijn instellingen configureren](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Het gebied van Overwerk dat u aan een mening van de Chronologie in een lijst of een rapport kunt toevoegen toont de informatie die op het gebied van Overuren van timesheet wordt gevonden. Deze informatie wordt manueel bijgewerkt door een gebruiker met toegang om timesheet te wijzigen. Raadpleeg het artikel voor meer informatie over het veld Overtime in een tijdspagina [De lay-out Timesheet begrijpen](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De kosten voor overwerk berekenen in een tijdlijnweergave

U voegt als volgt een berekende kolom Overuren toe aan een tijdlijnweergave:

1. Ga naar een lijst van chronologie, of creeer een Rapport van het Timesheet.

   Zie het artikel voor informatie over het maken van rapporten [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klikken **Weergave aanpassen** in een lijst van tijdbladen.

   of

   Selecteer **Kolommen (weergave)** in een rapport Timesheet.

1. Klikken **Kolom toevoegen**.
1. Klikken **Overschakelen naar tekstmodus**.
1. In de **Tonen in deze kolom** gebied, klikken **Klik om tekst te bewerken**.
1. Kopieer en plak de volgende code voor de tekstmodus in het dialoogvenster **Tekstmodus** in.
   <pre>displayname=Calculate Overtime Kosten<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueFormat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Deze berekening veronderstelt dat de gebruiker gewoonlijk een week van 40 uur werkt.

1. Klikken **Opslaan** geeft u de nieuwe weergave een naam en klikt u op **Weergave opslaan** in een lijst van tijdbladen.

   of

   Klikken **Opslaan + Sluiten** in een rapport Tijdschema.

1. (Optioneel en voorwaardelijk) als u een rapport Tijdschema samenstelt, geeft u een naam voor het rapport op en klikt u vervolgens op **Rapport opslaan**.

   De kosten van de overuren van elke gebruiker worden weergegeven in het dialoogvenster **Berekende overtime kosten** kolom.

   ![calculate_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
