---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatieven kopiëren in het deelvenster Scenario
description: U kunt initiatieven creëren door bestaande te kopiëren. U kunt initiatieven kopiëren op een plan dat u creeert of op een plan dat iemand met u deelt.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Initiatieven kopiëren in de [!DNL Scenario Planner]

<!--Audited: 07/2024-->

U kunt initiatieven creëren door bestaande te kopiëren. U kunt initiatieven kopiëren op een plan dat u creeert of op een plan dat iemand met u deelt.

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

## Initiatieven kopiëren

Houd rekening met het volgende wanneer u initiatieven kopieert:

* Door een initiatief te kopiëren wordt de kopie op hetzelfde plan geplaatst als het oorspronkelijke initiatief.
* Het kopiëren van een initiatief kopieert en voegt de volgende informatie van het oorspronkelijke initiatief toe aan het nieuwe initiatief:

   * [!UICONTROL Duration]
   * [!UICONTROL Job roles]
   * [!UICONTROL People] en [!UICONTROL Fixed Costs]
   * [!UICONTROL Planned Benefit]

* Het kopiëren van een initiatief kan de volgende informatie voor het plan wijzigen, als de informatie op het oorspronkelijke initiatief bestaat:

   * Vereiste hoeveelheid functies
   * [!UICONTROL Costs]
   * [!UICONTROL Plan Utilization]
   * Taakrolgebruik
   * [!UICONTROL Net Value]

* Het kopiëren van een initiatief dat is gemaakt door het importeren van een project of dat ten minste eenmaal naar een project is gepubliceerd, heeft de volgende gevolgen:

   * Het dupliceert niet het project dat aan het initiatief is gekoppeld.
   * Het verbindt niet het gekopieerde initiatief met het project.
   * De sectie [!DNL Scenario Planner] over het project wordt niet gewijzigd voor projecten die minstens één keer zijn gepubliceerd.

  Voor informatie over het publiceren van initiatieven aan projecten, zie [&#x200B; Update of creeer projecten door initiatieven in  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) te publiceren.

  Voor informatie over het creëren van initiatieven door projecten in te voeren, zie [&#x200B; projecten van de Invoer in plannen in  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Initiatieven kopiëren

{{step1-to-scenario-planner}}

Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek de initiatieven die u wilt kopiëren.
1. Selecteer het vakje links van het initiatief of de initiatieven die u wilt kopiëren, en klik dan **[!UICONTROL Copy]** van het menu dat bij de bodem van het plan verschijnt.

   ![&#x200B; initiatief van het Exemplaar &#x200B;](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] kopieert de initiatieven onmiddellijk en plaatst ze onder het laatst geselecteerde initiatief.

   De naam van het gekopieerde initiatief is *[!UICONTROL Copy of]`<Name of original initiative>`* .

   >[!NOTE]
   >
   >Afhankelijk van waar u de nieuwe initiatieven opneemt, kunnen de aantallen bestaande initiatieven veranderen.

1. De naam van het gekopieerde initiatief bijwerken.

   >[!TIP]
   >
   >We raden u aan de naam van het initiatief altijd bij te werken om verwarring te voorkomen als u de namen opnieuw wilt kopiëren.

1. (Optioneel) Werk de prioriteit van uw nieuwe initiatieven bij.

   Voor informatie over het prioriteren van initiatieven, zie [&#x200B; de initiatiefprioriteiten van de Update in  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klik op **[!UICONTROL Save Plan]** om de wijzigingen op te slaan.
