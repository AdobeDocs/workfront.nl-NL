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
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Taakrollen maken en beheren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

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
1. Configureer het volgende:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Geef een naam op voor de taakrol. Dit is de naam die overal wordt weergegeven in [!DNL Workfront] waar het veld [!UICONTROL Job Role] wordt weergegeven. </p> <p>Tip: de naam van een taakrol kan maximaal 255 tekens bevatten. Langere namen kunnen echter worden afgebroken in bepaalde gebieden van [!DNL Workfront] . </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Voer een beschrijving in voor de rol die aangeeft wat er uniek aan is. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Selecteer <b>[!UICONTROL Yes]</b> als u wilt dat de rol actief is en overal beschikbaar is in [!DNL Workfront] , en dat deze wordt gekoppeld aan gebruikers, werkitems enzovoort. </p> </li> 
        <li> <p>Selecteer <b>[!UICONTROL No]</b> als u wilt dat de rol wordt gedeactiveerd en niet beschikbaar is om toe te wijzen aan gebruikers, werkitems, enz. </p> </li> 
       </ul> <p><span> voor informatie over het deactiveren van baanrollen, zie </span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref"> baanrollen </a> deactiveren. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span> dit is [!UICONTROL Base Currency], zoals die in het [!UICONTROL Setup] gebied door uw beheerder van Workfront wordt geplaatst. Voor informatie, zie </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref"> de wisselkoersen van de Opstelling </a>.</p> <p>Tip: <span> u kunt [!UICONTROL Base Currency] niet op het niveau van de baanrol uitgeven. Dit gebied wordt gedimd en dient als herinnering voor wat de basismunt voor uw systeem is.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Dit is het kostenpercentage per uur van de functie. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de snelheid in met de [!UICONTROL Base Currency] .</p> 
      <p>Klik op <strong>[!UICONTROL Add Rate]</strong> voor kosteneffectieve datumtarieven. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs een [!UICONTROL Start Date] en [!UICONTROL End Date] toe. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.</p> <p>Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei 2023, wordt een einddatum van 30 april 2023 toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.</p> <p>Tip: Wanneer het uitgeven van een bestaande baanrol, kunt u <strong> Soort door begindatum </strong> selecteren om de meest recente begindatum bij de bovenkant van de tarieflijst te zien.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>Dit is het facturerings per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de snelheid in met de [!UICONTROL Base Currency] .</p> <p>Klik op <strong>[!UICONTROL Add Rate]</strong> voor effectieve factureringssnelheden. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs een [!UICONTROL Start Date] en [!UICONTROL End Date] toe. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.</p> <p>Sommige datums worden automatisch toegevoegd. Als de eerste factureringsfrequentie bijvoorbeeld geen einddatum heeft en u een seconde toevoegt met een begindatum van 1 mei 2023, wordt een einddatum van 30 april 2023 toegevoegd aan de eerste factureringssnelheid zodat er geen hiaten bestaan.</p> <p>Tip: Wanneer het uitgeven van een bestaande baanrol, kunt u <strong> Soort door begindatum </strong> selecteren om de meest recente begindatum bij de bovenkant van de tarieflijst te zien.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Selecteer een valuta die aan deze taakrol is gekoppeld. Dit is de valuta die [!DNL Workfront] gebruikt voor het berekenen van kosten en opbrengsten die aan deze taakrol zijn gekoppeld. </p> 
        <p><span> dit is verschillend dan [!UICONTROL Base Currency] opstelling door uw [!DNL Workfront] beheerder in het [!UICONTROL Setup] gebied, en kan verschillend zijn dan de munt verbonden aan een project.</span> </p> 
        <p>Tip: in dit veld zijn alleen valuta's beschikbaar in het gebied [!UICONTROL Exchange Rates] in uw systeem. Als u slechts één valuta hebt ingesteld, wordt dit veld niet weergegeven.</p> 
       <p><span> voor informatie over vestiging [!UICONTROL Base Currency] in [!DNL Workfront], zie </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref"> de wisselkoersen van de Opstelling </a>.</p> <p><span> voor informatie over het veranderen van de munt van een project, zie </span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref"> de projectmunt </a> veranderen.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>Dit is de kosten per uur voor de rol van de taak die wordt uitgevoerd met de geselecteerde [!UICONTROL Override Currency] . [!DNL Workfront] gebruikt deze waarde om de geplande en werkelijke kosten van taken en problemen te berekenen die aan de rol van de taak zijn gekoppeld. </p> 
        <p><span> ga het tarief in [!UICONTROL Override Currency] hierboven gespecificeerd in. Dit werkt ook het Tarief van Kosten voor deze baanrol bij wanneer het gebruiken van [!UICONTROL Base Currency].</span> </p> 
        <p>Voor informatie over hoe [!DNL Workfront] kosten berekent, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> de kosten van het Spoor </a>.</p> 
       <p>Tip: bij het bijwerken van een bestaande taakrol waaraan al een kostenpercentage is gekoppeld, berekent [!DNL Workfront] de [!UICONTROL Override Currency] -snelheid op basis van de conversiesnelheid in uw systeem. Als u [!UICONTROL Override Currency Cost Rate] bijwerkt, wordt de kostenpercentage van de taakrol ook automatisch bijgewerkt.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>Dit is de facturering per uur van de taakrol die de geselecteerde [!UICONTROL Override Currency] gebruikt. [!DNL Workfront] gebruikt deze waarde om de geplande en de daadwerkelijke opbrengst van taken en kwesties te berekenen verbonden aan de baanrol. </p>
        <p><span> ga het tarief in [!UICONTROL Override Currency] hierboven gespecificeerd in. Dit werkt ook het Facturerings Rate voor deze baanrol bij wanneer het gebruiken van [!UICONTROL Base Currency].</span> </p>
        <p>Voor informatie over hoe [!DNL Workfront] opbrengst berekent, zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>.</p>
        <p>Tip: bij het bijwerken van een bestaande taakrol waaraan al een factureringssnelheid is gekoppeld, berekent [!DNL Workfront] de overschrijvingswisselkoers op basis van de conversiesnelheid in uw systeem. Als u de factureringssnelheid voor valuta overschrijven bijwerkt, wordt de factureringssnelheid van de taakrol ook automatisch bijgewerkt. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

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
