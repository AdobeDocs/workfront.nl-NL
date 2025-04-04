---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Taken deactiveren
description: Als  [!DNL Adobe Workfront]  beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen deactiveren die verouderd in uw systeem worden. Wanneer u een taakrol deactiveert in plaats van deze te verwijderen, kunt u alle historische gegevens bewaren die eraan zijn gekoppeld.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Taakrollen deactiveren

Als [!DNL Adobe Workfront] beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen deactiveren die verouderd in uw systeem worden. Wanneer u een taakrol deactiveert in plaats van deze te verwijderen, kunt u alle historische gegevens bewaren die eraan zijn gekoppeld.

U kunt taakrollen ook opnieuw activeren die eerder zijn gedeactiveerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>
   <p>Nieuw: [!UICONTROL Standard]</p>
   <p>of</p>
   <p>Huidige: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Administratieve toegang tot taakrollen</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het effect van het deactiveren van functies

Als u een taakrol deactiveert, wordt deze niet meer weergegeven in de volgende gebieden:

* Het [!UICONTROL Assignments] typeahead-veld (voor taken, sjabloontaken, problemen, goedkeuringen en routeringsregels)
* De velden [!UICONTROL Assignments] in lijsten en rapporten
* Gebruikersprofielen

  >[!NOTE]
  >
  >Wanneer u een nieuwe rol aan een gebruiker toevoegt, wordt een gedeactiveerde baanrol niet getoond. Maar deze wordt wel in de velden [!UICONTROL Primary Role] en [!UICONTROL Other Roles] weergegeven als de gebruiker aan de taakrol was gekoppeld voordat deze werd gedeactiveerd.

* Dialoogvenster [!UICONTROL Sharing] voor objecten, waaronder sjabloontoewijzing voor lay-out
* Typeahead-velden in aangepaste formulieren
* Het veld [!UICONTROL Pool Members] in [!UICONTROL Resource Pools]
* Het veld [!UICONTROL Job Role] van een [!UICONTROL Billing Rate] bewerkingsscherm wanneer een gebruiker de factureringssnelheden voor projecten overschrijft
* Het dialoogvenster [!UICONTROL Add assignment to Kanban board] in een project
* Het veld [!UICONTROL Job Role] van een abonnement of een initiatief wanneer iemand [!DNL Adobe Workfront Scenario Planner] gebruikt.

  [!DNL Scenario Planner] is alleen beschikbaar in de nieuwe [!DNL Adobe Workfront] -ervaring en vereist een extra licentie. Voor informatie over [!DNL Workfront Scenario Planner], zie [ het  [!DNL Scenario Planner]  overzicht ](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Gedetactiveerde rollen worden altijd weergegeven in filters in lijsten, rapporten en andere gereedschappen, zoals de [!UICONTROL Workload Balancer] .

## Overwegingen voordat u een taakrol deactiveert

Het is beter om baanrollen te deactiveren eerder dan te schrappen die verouderd worden zodat u alle historische informatie kunt houden verbonden aan rollen u in het verleden kunt hebben gebruikt.

>[!NOTE]
>
>Alle taken die voorafgaand aan deactivering aan de taakrol zijn toegewezen, blijven toegewezen.

We raden u aan het volgende te doen voordat u een ongebruikte taakrol deactiveert:

* Bouw rapporten voor om het even welke voorwerpen die aan de rol worden toegewezen u van plan bent om hen aan een actieve baanrol te deactiveren en opnieuw toe te wijzen. Voor informatie over de bouw van rapporten, zie [ een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren.

  >[!TIP]
  >
  >U kunt een rapport maken om te filteren op taken of problemen waaraan de gedeactiveerde rol is toegewezen. Gebruik het rapport vervolgens om openstaande taken of problemen opnieuw toe te wijzen aan een actieve rol.

* Neem een inventaris van alle goedkeuringsprocessen, huidige goedkeuringswegen, en verpletterende regels of andere voorwerpen die aan de baanrol worden toegewezen u van plan bent om hen aan een actieve rol te deactiveren en opnieuw toe te wijzen.

  >[!TIP]
  >
  >Wanneer het gebruiken van verzoekrijen, als u een baanrol deactiveert die als standaardtoegewezen ontvanger in een verpletterende regel wordt toegewezen, blijft de rol en de verzoeken nog worden verpletterd aan de gedeactiveerde rol. Wij adviseren het bijwerken verpletterend regels met actieve rollen alvorens u het team deactiveert.

  Voor informatie over het creëren van goedkeuringsprocessen en het verpletteren van regels, zie de volgende artikelen:

   * [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Verpletterende regels maken](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Een taakrol deactiveren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op &#x200B; **[!UICONTROL Job Roles].**
1. (Optioneel) Selecteer **[!UICONTROL Active]** in het vervolgkeuzemenu **[!UICONTROL Filter]** als u alleen actieve taakrollen wilt weergeven.
1. Klik op de naam van de taakrol die u wilt deactiveren.
1. Selecteer **[!UICONTROL No]** in de vervolgkeuzelijst **[!UICONTROL Is Active]** .

   ![ Deactivate baanrol ](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Klik op **[!UICONTROL Save Changes]**.

   De taakrol is gedeactiveerd en kan niet meer aan het werk worden toegewezen, gekoppeld aan lay-outsjablonen, enzovoort. Voor informatie over al gebruik van baanrollen in [!DNL Workfront], zie [ het overzicht van de rol van de Baan ](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
