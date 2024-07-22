---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatieven verwijderen in het deelvenster Scenario
description: U kunt initiatieven op een plan schrappen dat u of op een plan creeerde dat iemand met u deelde. U kunt initiatieven die u hebt verwijderd, niet herstellen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Initiatieven verwijderen in de [!DNL Scenario Planner]

U kunt initiatieven op een plan schrappen dat u of op een plan creeerde dat iemand met u deelde. U kunt initiatieven die u hebt verwijderd, niet herstellen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Huidig: [!UICONTROL Business] of hoger</p>
   <p>Nieuw: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>Nieuw: Licht of hoger</p> 
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> 
   <p>Voor de huidige plannen van Workfront: </p>
   <p>U moet een extra licentie voor de [!DNL Adobe Workfront Scenario Planner] aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over toegang en toestemmingen voor [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Toegangsniveau </td> 
   <td> <p>[!UICONTROL Edit] toegang tot de [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie bij het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref"> de toegang van het Verzoek tot een plan in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Initiatieven verwijderen

Houd rekening met het volgende wanneer u initiatieven verwijdert:

* Als u een initiatief verwijdert, wordt het vereiste aantal functies en de aan het initiatief gekoppelde kosteninformatie uit het plan verwijderd.
* Als u een initiatief verwijdert dat is gemaakt door een project te importeren, wordt het project dat aan het initiatief is gekoppeld, niet verwijderd.
* Als u een initiatief verwijdert dat ten minste eenmaal voor een project is gepubliceerd, resulteert dat in het volgende:

   * Het initiatief wordt uit het scenario verwijderd, maar het gebied [!DNL Scenario Planner] blijft in de sectie [!UICONTROL Project Details] .
   * Als het initiatief dat u schrapt het enige gepubliceerde initiatief op het scenario is, wordt de indicator dat het plan is gepubliceerd ook geschrapt.

     Voor informatie over het publiceren van initiatieven aan projecten, zie [ Update of creeer projecten door initiatieven in  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) te publiceren.

     Voor informatie over het creëren van initiatieven door projecten in te voeren, zie [ projecten van de Invoer in plannen in  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

U kunt één initiatief tegelijk verwijderen of meerdere initiatieven bulksgewijs verwijderen.

* [ Schrap één initiatief ](#delete-one-initiative)
* [Initiatieven bulksgewijs verwijderen](#delete-initiatives-in-bulk)

### Eén initiatief verwijderen {#delete-one-initiative}

{{step1-to-scenario-planner}}

Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek het initiatief dat u wilt verwijderen.
1. Voer een van de volgende handelingen uit:

   * Klik op **[!UICONTROL More menu]** ![](assets/more-menu.png) rechts van de naam van het initiatief en klik vervolgens op **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]** .

   * Selecteer het vak links van het initiatief en klik op **[!UICONTROL Delete]** in het zwevende menu dat onder aan het abonnement wordt weergegeven en klik vervolgens op **[!UICONTROL Yes, delete it]** .

   Het initiatief en zijn functie en kosteninformatie worden uit het plan geschrapt.

1. Klik op **[!UICONTROL Save Plan]** om de wijzigingen op te slaan.

### Initiatieven bulksgewijs verwijderen {#delete-initiatives-in-bulk}

1. Klik op het pictogram **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) en klik vervolgens op [!UICONTROL Scenarios] .

   Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek het initiatief dat u wilt verwijderen.
1. Selecteer de vakjes links van de initiatieven die u wilt schrappen, dan klik **[!UICONTROL Delete]** van het menu dat bij de bodem van het plan verschijnt, dan klik **[!UICONTROL Yes, delete them]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   De initiatieven en hun functie en kosteninformatie worden uit het plan geschrapt.

1. Klik op **[!UICONTROL Save Plan]** om de wijzigingen op te slaan.
