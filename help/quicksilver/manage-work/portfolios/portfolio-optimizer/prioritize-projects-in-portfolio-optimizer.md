---
title: Prioriteit geven aan projecten in Portfolio Optimizer
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: U kunt prioriteiten stellen aan uw projecten in Portfolio Optimizer, om de orde te bepalen waarin zij zouden moeten worden voltooid.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: 714e6e09f1429f0382c36d17d3f2aca95edcfbc6
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Prioriteit geven aan projecten in de [!UICONTROL Portfolio Optimizer]

U kunt aan uw projecten in [!UICONTROL Portfolio Optimizer] voorrang geven, om de orde te bepalen waarin zij zouden moeten worden voltooid.

Houd rekening met het volgende wanneer u [!UICONTROL Portfolio Optimizer] gebruikt:

* De projecten boven aan de [!UICONTROL Portfolio Optimizer] worden belangrijker geacht dan de projecten onder aan de lijst. U moet de projecten voltooien in volgorde van prioriteit in de [!UICONTROL Portfolio Optimizer] om de Portfolio te optimaliseren.
* De prioriteit van projecten in [!UICONTROL Portfolio Optimizer] is niet gerelateerd aan het veld [!UICONTROL Priority] op het tabblad [!UICONTROL Project Details] van een project.

  Het veld [!UICONTROL Priority] op het tabblad [!UICONTROL Project Details] is een visuele markering die u handmatig opgeeft om te begrijpen hoe belangrijk een project moet zijn.

* De prioriteit van projecten in Portfolio Optimizer is zichtbaar in [!DNL Resource Planner], als het daar wordt toegelaten. In [!DNL Resource Planner] ontvangen projecten bronnen in de volgorde van hun [!UICONTROL Resource Planner] prioriteit, en niet die van de [!UICONTROL Portfolio Priority] .

  Voor informatie over het prioriteren van projecten in [!UICONTROL Resource Planner], zie het artikel [ projecten van Prioriteit in [!UICONTROL Resource Planner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* In het gebied **[!UICONTROL Project Prioritization]** van [!UICONTROL Portfolio Optimizer] worden projecten standaard in de volgorde [!UICONTROL Planned Start Dates] en [!UICONTROL Net Value] weergegeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Workfront Prime of hoger</p>
      <p>Workflow Prime of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!UICONTROL Portfolios] en [!UICONTROL Projects]</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor het portfolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang voor de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## De prioriteit van de projecten in de [!UICONTROL Portfolio Optimizer] wijzigen

{{step1-to-portfolios}}

1. (Optioneel) Selecteer het juiste filter in de vervolgkeuzelijst **[!UICONTROL Filter]** om de juiste lijst met portfolio&#39;s weer te geven.
1. Klik op de naam van een portfolio om het te openen.
1. Klik op **[!UICONTROL Portfolio Optimization]** in het linkerdeelvenster.
1. Wijzig in het gebied [!UICONTROL project optization] de prioriteit van uw projecten door de projecten in volgorde van prioriteit te slepen en vervolgens naar de gewenste weergavepositie te slepen.

   ![ Portfolio optimizer met projecten ](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Klik op **[!UICONTROL Set Priority]** in het gebied voor projectoptimalisatie wanneer u klaar bent met het herschikken van uw projecten. De projecten krijgen een nieuw nummer op basis van de nieuwe bestelling.

1. Klik op **[!UICONTROL Save]** om de nieuwe projectprioriteit op te slaan in [!UICONTROL Portfolio Optimizer] . De prioriteit wordt vermeld als een aantal in het aantal **#** kolom.

   >[!TIP]
   >
   >Dit verandert noodzakelijk niet de orde van de projecten in [!UICONTROL Portfolio Optimizer], omdat de lijst van projecten door een kolom buiten de **zou kunnen worden gesorteerd#** kolom. Klik op de kolomkop **#** om de lijst te rangschikken op projectprioriteit.

   U kunt de prioriteit van het project zien zoals deze wordt weergegeven in [!UICONTROL Portfolio Optimizer] in de functie Bronnen door de instelling **[!UICONTROL Display Portfolio Priorities]** in de functie Bronnen in te schakelen.

   Voor informatie over het prioriteren van projecten in [!UICONTROL Resource Planner], zie het artikel [ projecten van Prioriteit in [!UICONTROL Resource Planner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
