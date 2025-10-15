---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Prioriteiten van het Initiatief in de Planner Scenario bijwerken
description: Prioriteit geven aan initiatieven is belangrijk omdat initiatieven uit het plan een baan krijgen en begrotingsmiddelen krijgen in de volgorde waarin ze in het plan zijn opgenomen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Prioriteiten voor initiatieven bijwerken in de [!DNL Scenario Planner]

Prioriteit geven aan initiatieven is belangrijk omdat initiatieven uit het plan een baan krijgen en begrotingsmiddelen krijgen in de volgorde waarin ze in het plan zijn opgenomen.

U kunt aan initiatieven op een plan voorrang geven dat u creeerde of op een plan dat iemand met u deelde.

Voor informatie over het creëren van plannen, zie [ plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

Voor informatie over het creëren van initiatieven, zie [ initiatieven in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) creëren en uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>OPMERKING</b></p>
<p>Neem contact op met uw Workfront-vertegenwoordiger als u een ander Workfront-pakket hebt.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie</p> </td> 
   <td> <p>[!UICONTROL Light] of hoger</p> 
   <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
    <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL Edit] toegang tot de [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over toegang tot de Planner van het Scenario, zie [ Toegang nodig om  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) te gebruiken.

Voor informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prioriteiten van initiatieven bijwerken

Als u de prioriteit van initiatieven wijzigt, wijzigt u de volgorde van de aanbiedingen in het abonnement.

We raden u aan om urgente initiatieven boven aan een plan te plaatsen en de meer dynamische initiatieven - die op elk moment en alleen als er middelen beschikbaar zijn - onder aan het plan te plaatsen.

>[!NOTE]
>
>[!DNL Workfront] wijst planmiddelen aan initiatieven in de orde toe zij op het plan worden vermeld.
>
>Bijvoorbeeld, als het plan 3 beschikbare ingenieurs en Initiatief 1 en Initiatief 2 heeft vereist elk 2 Ingenieurs om te voltooien en zij allebei voor het zelfde tijdkader gepland zijn, associeert Workfront 2 Ingenieurs met Initiatief 1 en één nog beschikbare Ingenieur met Initiatief 2. In dit geval blijkt uit initiatief 2 dat er sprake is van een conflict, omdat er één engineer ontbreekt. Soms is het wijzigen van de prioriteit van uw initiatieven de enige manier om conflicten in een plan te voorkomen.

Prioriteit initiatief bijwerken:

{{step1-to-scenario-planner}}

Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek vervolgens de initiatieven die u als prioriteit wilt instellen.
1. Klik op het vakje links van de naam van een of meer initiatieven en voer een van de volgende handelingen uit:

   * Klik op de handgreep links van een van de namen van de geselecteerde initiatieven en sleep deze omhoog of omlaag in de lijst om de prioriteit van het initiatief te wijzigen.

     Workfront geeft het aantal geselecteerde initiatieven weer.

     ![ Multi select initiatiefaantal ](assets/multi-select-initiative-number.png)

   * Klik op het vak **[!UICONTROL Prioritize]** onder aan het abonnement en kies een van de volgende opties:

      * **[!UICONTROL Top]**: hiermee plaatst u de geselecteerde initiatieven boven aan de lijst met initiatieven. De geselecteerde initiatieven staan bovenaan in het plan.
      * **[!UICONTROL Bottom]**: hiermee plaatst u de geselecteerde initiatieven onder aan de lijst met initiatieven. De geselecteerde initiatieven staan als laatste vermeld in het plan.
      * **[!UICONTROL Select a number]**: verplaatst de geselecteerde initiatieven na het initiatief dat u hier aangeeft.

        ![ Prioritize initiatieven ](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] plaatst de geselecteerde initiatieven onmiddellijk op de aangegeven locatie en het aantal van alle initiatieven wordt dienovereenkomstig bijgewerkt.

1. Klik op **[!UICONTROL Save Plan]** om de wijzigingen op te slaan.
