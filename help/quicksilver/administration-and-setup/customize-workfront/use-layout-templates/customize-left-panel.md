---
title: Het linkerdeelvenster aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In een lay-outsjabloon kunt u aanpassen wat gebruikers in het linkerdeelvenstergebied in Adobe Workfront zien.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Het linkerdeelvenster aanpassen met een lay-outsjabloon

In een lay-outsjabloon kunt u aanpassen wat gebruikers in het linkerdeelvenstergebied in [!DNL Adobe Workfront] zien.

U kunt bijvoorbeeld bepalen welke van de volgende items gebruikers in het linkerdeelvenster zien wanneer ze een taak bekijken:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Wijzigingen die u aanbrengt in de volgorde en zichtbaarheid worden weerspiegeld in de mobiele app.

Voor informatie over het creëren van lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [ gebruikers aan een lay-outmalplaatje ](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> U hebt het toegangsniveau [!UICONTROL System Administrator] nodig om deze stappen op systeemniveau uit te voeren.<p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pas het linkerdeelvenster aan voor een gebied in [!DNL Workfront] :

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klik op de pijl-omlaag ![](assets/dropdown-arrow.png) onder **[!UICONTROL Customize what users see]** en klik vervolgens op het linkerdeelvenster dat u wilt aanpassen.

   >[!NOTE]
   >
   >Voor informatie over de [!UICONTROL Home] optie in deze drop-down lijst, zie [ aanpassen [!UICONTROL Home] en [!UICONTROL Summary] gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Voor informatie over de optie van Lijsten, zie [ Filters, Mening, en Groepen aanpassen gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Voer in de lijst **[!UICONTROL Left panel]** een van de volgende handelingen uit om te bepalen wat gebruikers in het linkerdeelvenster zien voor de optie ([!DNL Workfront] gebied of objecttype) die u hebt geselecteerd:

   * ![](assets/add-secondary-nav-item.png) items tonen of verbergen ![](assets/delete-secondary-nav-item.png) . Een item zonder ![](assets/add-secondary-nav-item.png) of ![](assets/delete-secondary-nav-item.png) kan niet worden verborgen.

   * Sleep items ![](assets/move-icon---dots.png) om de volgorde in het linkerdeelvenster te wijzigen.
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Optie</th> 
      <th>Wanneer gebruikers op het volgende klikken...</th> 
      <th>De linkerdeelvensteritems die u kiest, worden als volgt weergegeven:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>De naam van een project</td> 
      <td>[!UICONTROL Tasks], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Risks], [!UICONTROL Approvals], [!UICONTROL Baselines], [!UICONTROL Billing Rates], [!UICONTROL Billing Records], [!UICONTROL Expenses], [!UICONTROL Hours], [!UICONTROL Workload Balancer], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>De naam van een taak</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses] , [!UICONTROL Predecessors]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>De naam van een uitgave</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issue Details], [!UICONTROL Hours] , [!UICONTROL Approvals]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>De naam van een portfolio</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programs], [!UICONTROL Portfolio Details], [!UICONTROL Portfolio] [!UICONTROL Optimization], [!UICONTROL Documents] , [!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>De naam van een programma</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates] , [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>De naam van een projectsjabloon</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>De naam van een sjabloontaak</td> 
      <td>[!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Predecessors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Billing Record]</td> 
      <td>De naam van een factureringsrecord voor een project</td> 
      <td>[!UICONTROL Billing Record Details], [!UICONTROL Billable Hours], [!UICONTROL Billable Expenses] , [!UICONTROL Fixed Revenues]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>Projecten <img src="assets/projects-in-main-menu.png"> in de [!UICONTROL Main menu] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>De naam van een aanvraag</td> 
      <td>[!UICONTROL New Request], [!UICONTROL Submitted requests], [!UICONTROL All Requests] , [!UICONTROL Drafts]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>De naam van een dashboard</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]<p><b> NOTA </b>: Als u douanelusjes voor het [!UICONTROL Reports] gebied gebruikend een lay-outmalplaatje in [!DNL Adobe Workfront Classic] creeerde, tonen zij bij de bodem van deze lijst. Gebruikers kunnen ze onder aan het linkerdeelvenster weergeven in het [!UICONTROL Dashboards] -gebied.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>De naam van een scrum-team</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong> NOTA:</strong> het <strong>[!UICONTROL Current iteration]</strong> punt toont slechts in het linkerpaneel wanneer er minstens één taak of kwestie op de herhaling is.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>De naam van een Kanban-team</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Updates] , [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>De naam van een Watervalteam</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests] , [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>De naam van een herhaling</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >De laatste 3 items in de vervolgkeuzelijst **[!UICONTROL Customize what users see]** ( [!UICONTROL Lists] , [!UICONTROL Home and Summary] en [!UICONTROL Branding] ) zijn bedoeld voor het configureren van andere gebieden dan het linkerdeelvenster. Raadpleeg de volgende artikelen voor meer informatie over deze artikelen:
>   >   
* [ pas Filters, Weergaven, en Groepen aan gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [ pas [!UICONTROL Home] aan en [!UICONTROL Summary] gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [ Adobe van het Merk  [!DNL Workfront]  gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Optioneel) Als u een item uit het linkerdeelvenster wilt toevoegen dat is gekoppeld aan een van de dashboards van uw organisatie, klikt u op **[!UICONTROL Add custom section]** , typt u een **[!UICONTROL Custom section title]** voor het item en voegt u het dashboard toe.

   De dashboarditems worden onder in het linkerdeelvenster weergegeven. Gebruikers zien de titel van de sectie Aangepast die u typt naast het dashboarditem wanneer ze de muisaanwijzer op het linkerdeelvenster plaatsen.

   >[!NOTE]
   >
   Gebruikers kunnen aangepaste dashboarditems aan hun linkerdeelvenster toevoegen. Wanneer u aangepaste dashboarditems toevoegt aan een lay-outsjabloon, worden de items samengevoegd met de bijbehorende items zonder ze te overschrijven of opnieuw in te stellen. Dit geldt ook als u gebruikers toewijst aan een nieuwe lay-outsjabloon met aangepaste dashboarditems. Voor informatie over hoe de gebruikers het linkerpaneel kunnen aanpassen, zie [ douanetabellen of secties ](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) creëren.

   Voor informatie over dashboards, zie [ dashboards ](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Klik op **[!UICONTROL Save]** als u klaar bent met het aanpassen.

   >[!TIP]
   >
   U kunt op elk gewenst moment op [!UICONTROL Save] klikken om de voortgang op te slaan en de sjabloon later blijven wijzigen.
