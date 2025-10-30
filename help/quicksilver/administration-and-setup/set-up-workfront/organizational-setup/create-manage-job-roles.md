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
source-git-commit: e5416fab4f4ad1f2c31edf962554ddd6a4c2f1e5
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 0%

---

# Taakrollen maken en beheren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Met versie 25.11, zal de Valuta van de Opheffing voor baanrollen in Productie worden verouderd. (De veroudering vindt plaats op 30 oktober in de voorvertoningsomgeving.) In plaats van een basisvaluta en overschrijvingsvaluta, zal er één valuta beschikbaar zijn voor functies, en de kosten en factureringstarieven zullen worden bepaald met behulp van die valuta.

Als [!DNL Adobe Workfront] beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen tot stand brengen die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn. Voor informatie over administratieve toegang in [!DNL Workfront], zie [&#x200B; gebruikers administratieve toegang van de Verlening tot bepaalde gebieden &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

     Voor informatie over het deactiveren van baanrollen, zie [&#x200B; werkrollen &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md) deactiveren.

   * **de Valuta van de Basis**: Dit is de Valuta van de Basis, zoals die in het gebied van de Opstelling door uw beheerder van Workfront wordt geplaatst. Voor informatie, zie [&#x200B; de wisselkoersen van de Opstelling &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     >[!TIP]
     >
     >U kunt de basisvaluta niet op het taakrolniveau bewerken. Dit veld is grijs en dient als herinnering voor wat de basisvaluta voor uw systeem is.

   * **Tarief van Kosten**: Dit is de kosten per uurtarief van de baanrol. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de koers in met de basisvaluta.

     Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.

     Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei 2025, wordt een einddatum van 30 april 2025 toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.

     >[!TIP]
     >
     >Wanneer het uitgeven van een bestaande baanrol, kunt u **Soort door begindatum** selecteren om de meest recente begindatum bij de bovenkant van de tarieflijst te zien.

   * **het Factureren Tarief**: Dit is het factureren per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de koers in met de basisvaluta.

     Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.

     Sommige datums worden automatisch toegevoegd. Als de eerste factureringsfrequentie bijvoorbeeld geen einddatum heeft en u een seconde toevoegt met een begindatum van 1 mei 2025, wordt een einddatum van 30 april 2025 toegevoegd aan de eerste factureringssnelheid zodat er geen hiaten bestaan.

     >[!TIP]
     >
     >Wanneer het uitgeven van een bestaande baanrol, kunt u **Soort door begindatum** selecteren om de meest recente begindatum bij de bovenkant van de tarieflijst te zien.

   * **treedt Valuta** met voeten: Selecteer een munt verbonden aan deze baanrol. Dit is de valuta die Workfront gebruikt voor het berekenen van de kosten en inkomsten die met deze functie samenhangen.

     Dit is verschillend dan de Valuta van de Basis die door uw beheerder van Workfront in het gebied van de Opstelling wordt opgesteld, en kan verschillend zijn dan de munt verbonden aan een project.

     >[!TIP]
     >
     >Alleen valuta&#39;s die beschikbaar zijn in het gebied Wisselkoersen in uw systeem zijn beschikbaar in dit veld. Als u slechts één valuta hebt ingesteld, wordt dit veld niet weergegeven.

     Voor informatie over vestiging de Valuta van de Basis in Workfront, zie [&#x200B; de wisselkoers van de Opstelling &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Voor informatie over het veranderen van de munt van een project, zie [&#x200B; de projectmunt &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md) veranderen.

   * **met voeten treedt het Tarief van de Kostprijs van de Valuta**: Dit is de kosten per uurtarief van de baanrol gebruikend de geselecteerde Valuta van de Overschrijving. Workfront gebruikt deze waarde om de geplande en de werkelijke kosten van taken en problemen in verband met de functie te berekenen.

     Voer de waarde in de bovenstaande valuta voor overschrijven in. Dit werkt ook het Tarief van Kosten voor deze baanrol bij wanneer het gebruiken van de Valuta van de Basis.

     Voor informatie over hoe Workfront kosten berekent, zie [&#x200B; Kosten van het Spoor &#x200B;](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Wanneer u een bestaande taakrol bijwerkt waaraan al een kostenpercentage is gekoppeld, berekent Workfront de wisselkoers bij overschrijven op basis van de omrekeningskoers in uw systeem. Als u de kostenvoet voor valuta overschrijven bijwerkt, wordt de kostenvoet van de taakrol ook automatisch bijgewerkt.

   * **met voeten treedt het FactureringsTarief van de Valuta**: Dit is het factureren per uurtarief van de baanrol gebruikend de geselecteerde Valuta van de Overschrijving. Workfront gebruikt deze waarde om de geplande en de daadwerkelijke opbrengst van taken en kwesties te berekenen verbonden aan de baanrol.

     Voer de waarde in de bovenstaande valuta voor overschrijven in. Dit werkt ook het Facturerings Tarief voor deze baanrol bij wanneer het gebruiken van de Valuta van de Basis.

     Voor informatie over hoe Workfront opbrengst berekent, zie [&#x200B; Overzicht van Facturering en Ontvangsten &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Wanneer u een bestaande taakrol bijwerkt waaraan al een factureringssnelheid is gekoppeld, berekent Workfront de wisselkoers bij overschrijven op basis van de conversiesnelheid in uw systeem. Als u de factureringssnelheid van valuta overschrijven bijwerkt, wordt de factureringssnelheid van de taakrol ook automatisch bijgewerkt.

<!--
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

>[!TIP]
>
>De rollen van de baan zijn een integraal deel van het beheren van middelen. Om de middelen planningshulpmiddelen te gebruiken, hebben de baanrollen een kosten en het facturerings tarief verbonden aan hen nodig. Voor informatie, zie [&#x200B; begonnen worden met het Beheer van het Middel &#x200B;](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Klik op **[!UICONTROL Create Job Role]**. De taakrol is nu beschikbaar om te worden toegewezen aan taken, uitgaven, goedkeuringen of u kunt lay-outsjablonen of andere objecten ermee delen. Voor informatie over al gebruik van baanrollen in [!DNL Workfront], zie [&#x200B; het overzicht van de rol van de Baan &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Voor informatie over het schrappen van een baanrol, zie [&#x200B; baanrollen van de Schrapping &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
