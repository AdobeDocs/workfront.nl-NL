---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Prioriteiten van initiatieven bijwerken in het scenario Scenario Planner
description: Prioriteit geven aan initiatieven is belangrijk omdat initiatieven uit het plan een baan krijgen en begrotingsmiddelen krijgen in de volgorde waarin ze in het plan zijn opgenomen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Prioriteiten van initiatieven bijwerken in het [!DNL Scenario Planner]

Prioriteit geven aan initiatieven is belangrijk omdat initiatieven uit het plan een baan krijgen en begrotingsmiddelen krijgen in de volgorde waarin ze in het plan zijn opgenomen.

U kunt aan initiatieven op een plan voorrang geven dat u creeerde of op een plan dat iemand met u deelde.

Voor informatie over het maken van plannen raadpleegt u [Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Voor informatie over het maken van initiatieven raadpleegt u [Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Toegangsvereisten

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] of hoger</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licentie*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!DNL Scenario Planner]</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie over het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Toegang aanvragen tot een abonnement in de [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prioriteiten van initiatieven bijwerken

Als u de prioriteit van initiatieven wijzigt, wijzigt u de volgorde van de aanbiedingen in het abonnement.

We raden u aan om urgente initiatieven boven aan een plan te plaatsen en de meer dynamische initiatieven - die op elk moment en alleen als er middelen beschikbaar zijn - onder aan het plan te plaatsen.

>[!NOTE]
>
>[!DNL Workfront] wijst planningsmiddelen aan initiatieven toe in de orde zij op het plan worden vermeld.
>
>Bijvoorbeeld, als het plan 3 beschikbare ingenieurs en Initiatief 1 en Initiatief 2 heeft vereist elk 2 Ingenieurs om te voltooien en zij allebei voor het zelfde tijdkader gepland zijn, associeert Workfront 2 Ingenieurs met Initiatief 1 en één nog beschikbare Ingenieur met Initiatief 2. In dit geval blijkt uit initiatief 2 dat er sprake is van een conflict, omdat er één engineer ontbreekt. Soms is het wijzigen van de prioriteit van uw initiatieven de enige manier om conflicten in een plan te voorkomen.

Prioriteit initiatief bijwerken:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op [!UICONTROL Scenarios].

   Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek vervolgens de initiatieven die u als prioriteit wilt instellen.
1. Klik op het vakje links van de naam van een of meer initiatieven en voer een van de volgende handelingen uit:

   * Klik op de handgreep links van een van de namen van de geselecteerde initiatieven en sleep deze omhoog of omlaag in de lijst om de prioriteit van het initiatief te wijzigen.

      Workfront geeft het aantal geselecteerde initiatieven weer.

      ![](assets/multi-select-initiative-number.png)

   * Klik op de knop **[!UICONTROL Prioritize]** onder aan het abonnement kiest u een van de volgende opties:

      * **[!UICONTROL Top]**: Hiermee plaatst u de geselecteerde initiatieven boven aan de lijst met initiatieven. De geselecteerde initiatieven staan bovenaan in het plan.
      * **[!UICONTROL Bottom]**: Hiermee plaatst u de geselecteerde initiatieven onder aan de lijst met initiatieven. De geselecteerde initiatieven staan als laatste vermeld in het plan.
      * **[!UICONTROL Select a number]**: Hiermee verplaatst u de geselecteerde initiatieven na het initiatief dat u hier aangeeft.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] plaatst de geselecteerde initiatieven onmiddellijk op de aangegeven plaatsen en het aantal initiatieven wordt dienovereenkomstig aangepast.


1. Klikken **[!UICONTROL Save Plan]** om uw wijzigingen op te slaan.
