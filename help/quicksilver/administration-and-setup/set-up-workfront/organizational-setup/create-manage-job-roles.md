---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Taakrollen maken en beheren
description: Als  [!DNL Adobe Workfront]  beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen creëren die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: a30e505aa2061240f92642fda274be66e4947bce
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# Taakrollen maken en beheren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Met de versie 25.11 is de valuta van de Overschrijving voor baanrollen afgekeurd in Productie. (De veroudering vond plaats op 30 oktober in de voorvertoningsomgeving.) In plaats van een basisvaluta te hebben en valuta&#39;s te overschrijven, is er nu één valuta beschikbaar voor functies, en de kosten en factureringstarieven worden bepaald met behulp van die valuta.

Als [!DNL Adobe Workfront] beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen tot stand brengen die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn. Voor informatie over administratieve toegang in [!DNL Workfront], zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>De rollen van de baan zijn een integraal deel van het beheren van middelen. Om de middelen planningshulpmiddelen te gebruiken, hebben de baanrollen een kosten en het facturerings tarief verbonden aan hen nodig. Voor informatie, zie [ begonnen worden met het Beheer van het Middel ](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Administratieve toegang tot taakrollen</td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een taakrol maken

Een taakrol maken:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op &#x200B; **[!UICONTROL Job Roles].**
1. Klik op **[!UICONTROL New Job Role].**
1. Configureer de volgende velden:

   * **Naam**: Verwijs op een naam voor de baanrol. Dit is de naam die overal in Workfront wordt weergegeven waar het veld Functie wordt weergegeven.

     >[!TIP]
     >
     >De naam van een taakrol kan maximaal 255 tekens bevatten. Langere namen kunnen echter in bepaalde gebieden van Workfront worden afgebroken.

   * **Beschrijving**: Ga een beschrijving voor de rol in die erop wijst wat over het uniek is.
   * **is Actief**: Selecteer **ja** als u de rol actief en beschikbaar overal in Workfront wilt zijn om met gebruikers, het werkpunten, enz. worden geassocieerd. Selecteer **Nr** als u de rol wilt worden gedeactiveerd en niet beschikbaar aan gebruikers, het werkpunten, enz. toewijzen.

     Voor informatie over het deactiveren van baanrollen, zie [ werkrollen ](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md) deactiveren.

   * **Valuta**: De Valuta van de Basis wordt getoond door gebrek. De beheerder van Workfront voegt de Valuta van de Basis in het gebied van de Opstelling toe. U kunt de selectie wijzigen in een andere beschikbare valuta en u kunt de valuta wijzigen voor effectieve gedateerde tijdbereiken.

     >[!TIP]
     >
     >Alleen valuta&#39;s die beschikbaar zijn in het gebied Wisselkoersen in uw systeem zijn beschikbaar in dit veld. Als er maar één valuta is ingesteld, is alleen die valuta beschikbaar.

     Voor informatie over vestiging de Valuta van de Basis in Workfront, zie [ de wisselkoers van de Opstelling ](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Voor informatie over het veranderen van de munt van een project, zie [ de projectmunt ](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md) veranderen.

   * **Tarief van Kosten**: Dit is de kosten per uurtarief van de baanrol. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de koers in met de geselecteerde valuta.

     Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.

     Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei 2025, wordt een einddatum van 30 april 2025 toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.

     Voor informatie over hoe Workfront kosten berekent, zie [ Kosten van het Spoor ](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

   * **het Factureren Tarief**: Dit is het factureren per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de koers in met de geselecteerde valuta.

     Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.

     Sommige datums worden automatisch toegevoegd. Als de eerste factureringsfrequentie bijvoorbeeld geen einddatum heeft en u een seconde toevoegt met een begindatum van 1 mei 2025, wordt een einddatum van 30 april 2025 toegevoegd aan de eerste factureringssnelheid zodat er geen hiaten bestaan.

     Voor informatie over hoe Workfront opbrengst berekent, zie [ Overzicht van Facturering en Ontvangsten ](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

1. Klik op **[!UICONTROL Create Job Role]**. De taakrol is nu beschikbaar om te worden toegewezen aan taken, uitgaven, goedkeuringen of u kunt lay-outsjablonen of andere objecten ermee delen. Voor informatie over al gebruik van baanrollen in [!DNL Workfront], zie [ het overzicht van de rol van de Baan ](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Voor informatie over het schrappen van een baanrol, zie [ baanrollen van de Schrapping ](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->



