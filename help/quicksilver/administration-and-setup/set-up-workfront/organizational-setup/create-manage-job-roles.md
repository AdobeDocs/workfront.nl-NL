---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Taakrollen maken en beheren
description: Als [!DNL Adobe Workfront] beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen creëren die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: e7ce6f0b02a1ecde3daaeb9ab678caaae112ac23
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---

# Taakrollen maken en beheren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen creëren die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn. Voor informatie over administratieve toegang in [!DNL Workfront], zie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>Huidige: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot functies</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een taakrol maken

Een taakrol maken:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op &#x200B; **[!UICONTROL Job Roles].**
1. Klikken **[!UICONTROL New Job Role].**
1. Configureer het volgende:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Geef een naam op voor de taakrol. Dit is de naam die overal wordt weergegeven in [!DNL Workfront] waarbij [!UICONTROL Job Role] wordt weergegeven. </p> <p>Tip: de naam van een taakrol kan maximaal 255 tekens bevatten. Langere namen kunnen echter worden afgebroken in bepaalde gebieden van [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Voer een beschrijving in voor de rol die aangeeft wat er uniek aan is. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Selecteren <b>[!UICONTROL Yes]</b> als u wilt dat de rol actief is en overal beschikbaar is in [!DNL Workfront] die aan gebruikers, werkpunten, enz. moeten worden geassocieerd. </p> </li> 
        <li> <p>Selecteren <b>[!UICONTROL No]</b>, als u wilt dat de rol wordt gedeactiveerd en niet beschikbaar is om toe te wijzen aan gebruikers, werkitems, enz. </p> </li> 
       </ul> <p><span>Voor informatie over het deactiveren van functies raadpleegt u</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Taakrollen deactiveren</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>Dit is het [!UICONTROL Base Currency], zoals ingesteld in de [!UICONTROL Setup] door uw Workfront-beheerder. Zie voor meer informatie</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wisselkoersen instellen</a> .</p> <p>Tip: <span>U kunt de [!UICONTROL Base Currency] op het taakrolniveau. Dit veld is grijs en dient als herinnering voor wat de basisvaluta voor uw systeem is.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Dit is het kostenpercentage per uur van de functie. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de snelheid in met de [!UICONTROL Base Currency].</p> 
      <p>Voor kosteneffectieve datums klikt u op <strong>[!UICONTROL Add Rate]</strong>. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs een [!UICONTROL Start Date] en [!UICONTROL End Date] indien nodig. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.</p> <p>Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei 2023, wordt een einddatum van 30 april 2023 toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.</p> <p>Tip: wanneer u een bestaande taakrol bewerkt, kunt u <strong>Sorteren op begindatum</strong> om de meest recente begindatum boven aan de tarieflijst te zien.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>Dit is het facturerings per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de snelheid in met de [!UICONTROL Base Currency].</p> <p>Voor effectieve factureringssnelheden klikt u op <strong>[!UICONTROL Add Rate]</strong>. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs een [!UICONTROL Start Date] en [!UICONTROL End Date] indien nodig. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.</p> <p>Sommige datums worden automatisch toegevoegd. Als de eerste factureringsfrequentie bijvoorbeeld geen einddatum heeft en u een seconde toevoegt met een begindatum van 1 mei 2023, wordt een einddatum van 30 april 2023 toegevoegd aan de eerste factureringssnelheid zodat er geen hiaten bestaan.</p> <p>Tip: wanneer u een bestaande taakrol bewerkt, kunt u <strong>Sorteren op begindatum</strong> om de meest recente begindatum boven aan de tarieflijst te zien.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Selecteer een valuta die aan deze taakrol is gekoppeld. Dit is de valuta die [!DNL Workfront] gebruik voor het berekenen van de kosten en opbrengsten die met deze functie samenhangen. </p> 
        <p><span>Dit is anders dan de [!UICONTROL Base Currency] door uw [!DNL Workfront] beheerder in de [!UICONTROL Setup] en kan verschillen van de valuta die aan een project is gekoppeld.</span> </p> 
        <p>Tip: alleen valuta's beschikbaar in de [!UICONTROL Exchange Rates] in uw systeem beschikbaar zijn in dit veld. Als u slechts één valuta hebt ingesteld, wordt dit veld niet weergegeven.</p> 
       <p><span>Voor informatie over het instellen van de [!UICONTROL Base Currency] in [!DNL Workfront], zie</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wisselkoersen instellen</a>.</p> <p><span>Voor informatie over het wijzigen van de valuta van een project raadpleegt u</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">De projectvaluta wijzigen</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>Dit is het kostenpercentage per uur van de functie die wordt gebruikt voor de geselecteerde [!UICONTROL Override Currency]. [!DNL Workfront] gebruikt deze waarde om de geplande en de werkelijke kosten van taken en kwesties te berekenen die verband houden met de functie. </p> 
        <p><span>Voer de snelheid in het dialoogvenster [!UICONTROL Override Currency] hierboven gespecificeerd. Dit werkt ook het Kostentarief voor deze baanrol bij wanneer het gebruiken van [!UICONTROL Base Currency].</span> </p> 
        <p>Voor informatie over hoe [!DNL Workfront] berekent kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>.</p> 
       <p>Tip: wanneer u een bestaande rol bijwerkt waaraan al een kostenpercentage is gekoppeld, [!DNL Workfront] berekent de [!UICONTROL Override Currency] op basis van de conversiesnelheid in uw systeem. Als u de [!UICONTROL Override Currency Cost Rate], wordt het kostenpercentage van de functie ook automatisch bijgewerkt.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>Dit is het facturerings per uurtarief van de baanrol gebruikend geselecteerde [!UICONTROL Override Currency]. [!DNL Workfront] gebruikt deze waarde om de geplande en de daadwerkelijke opbrengst van taken en kwesties te berekenen verbonden aan de baanrol. </p>
        <p><span>Voer de snelheid in het dialoogvenster [!UICONTROL Override Currency] hierboven gespecificeerd. Dit werkt ook het Facturerings Rate voor deze baanrol bij wanneer het gebruiken van [!UICONTROL Base Currency].</span> </p>
        <p>Voor informatie over hoe [!DNL Workfront] berekent inkomsten, zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overzicht van facturering en inkomsten</a>.</p>
        <p>Tip: wanneer u een bestaande taakrol bijwerkt waaraan al een factureringspercentage is gekoppeld [!DNL Workfront] berekent de wisselkoers bij overschrijven op basis van de conversiekoers in uw systeem. Als u de factureringssnelheid voor valuta overschrijven bijwerkt, wordt de factureringssnelheid van de taakrol ook automatisch bijgewerkt. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >De rollen van de baan zijn een integraal deel van het beheren van middelen. Om de middelen planningshulpmiddelen te gebruiken, hebben de baanrollen een kosten en het facturerings tarief verbonden aan hen nodig. Zie voor meer informatie [Aan de slag met Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Klik op **[!UICONTROL Create Job Role]**. De taakrol is nu beschikbaar om te worden toegewezen aan taken, uitgaven, goedkeuringen of u kunt lay-outsjablonen of andere objecten ermee delen. Voor informatie over alle toepassingen van functies in [!DNL Workfront], zie [Overzicht van de taakrol](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Zie voor informatie over het verwijderen van een taakrol [Taakrollen verwijderen](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
