---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Prioriteiten van initiatieven bijwerken in het scenario Scenario Planner
description: Prioriteit geven aan initiatieven is belangrijk omdat initiatieven uit het plan een baan krijgen en begrotingsmiddelen krijgen in de volgorde waarin ze in het plan zijn opgenomen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Prioriteiten voor initiatieven bijwerken in de [!DNL Scenario Planner]

Prioriteit geven aan initiatieven is belangrijk omdat initiatieven uit het plan een baan krijgen en begrotingsmiddelen krijgen in de volgorde waarin ze in het plan zijn opgenomen.

U kunt aan initiatieven op een plan voorrang geven dat u creeerde of op een plan dat iemand met u deelde.

Voor informatie over het creëren van plannen, zie [&#x200B; plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

Voor informatie over het creëren van initiatieven, zie [&#x200B; initiatieven in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) creëren en uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nieuw: Ultimate </p></li>
   <p>De Scenario Planner is niet beschikbaar voor de nieuwe Workfront Select- of Workfront Prime-plannen. </p>
   <li><p>Huidig: [!UICONTROL Business] of hoger</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>Nieuw: Licht of hoger</p> 
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>Voor de nieuwe plannen van Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Voor de huidige plannen van Workfront: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>Voor meer informatie, zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
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

*For informatie, zie [&#x200B; vereisten van de Toegang tot de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

     ![&#x200B; Multi select initiatiefaantal &#x200B;](assets/multi-select-initiative-number.png)

   * Klik op het vak **[!UICONTROL Prioritize]** onder aan het abonnement en kies een van de volgende opties:

      * **[!UICONTROL Top]**: hiermee plaatst u de geselecteerde initiatieven boven aan de lijst met initiatieven. De geselecteerde initiatieven staan bovenaan in het plan.
      * **[!UICONTROL Bottom]**: hiermee plaatst u de geselecteerde initiatieven onder aan de lijst met initiatieven. De geselecteerde initiatieven staan als laatste vermeld in het plan.
      * **[!UICONTROL Select a number]**: verplaatst de geselecteerde initiatieven na het initiatief dat u hier aangeeft.

        ![&#x200B; Prioritize initiatieven &#x200B;](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] plaatst de geselecteerde initiatieven onmiddellijk op de aangegeven locatie en het aantal van alle initiatieven wordt dienovereenkomstig bijgewerkt.

1. Klik op **[!UICONTROL Save Plan]** om de wijzigingen op te slaan.
