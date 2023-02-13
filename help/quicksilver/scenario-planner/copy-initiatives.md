---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatieven kopiëren in het deelvenster Scenario
description: U kunt initiatieven creëren door bestaande te kopiëren. U kunt initiatieven kopiëren op een plan dat u creeert of op een plan dat iemand met u deelt.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Initiatieven kopiëren in het dialoogvenster [!DNL Scenario Planner]

U kunt initiatieven creëren door bestaande te kopiëren. U kunt initiatieven kopiëren op een plan dat u creeert of op een plan dat iemand met u deelt.

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
   <td> <p>[!DNL Adobe Workfront]<b> licentie</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!DNL Scenario Planner]</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie over het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Toegang aanvragen tot een abonnement in de [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   * Het wijzigt de [!DNL Scenario Planner] voor projecten die ten minste eenmaal zijn gepubliceerd.

   Voor informatie over het publiceren van initiatieven aan projecten, zie [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   Voor informatie over het creëren van initiatieven door projecten in te voeren, zie [Projecten importeren naar plannen in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Initiatieven kopiëren

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op [!UICONTROL Scenarios].

   Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek de initiatieven die u wilt kopiëren.
1. Selecteer het vak links van het initiatief dat of de initiatieven die u wilt kopiëren en klik op **[!UICONTROL Copy]** in het menu dat onder aan het abonnement wordt weergegeven.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] kopieert de initiatieven onmiddellijk en plaatst ze onder het laatst geselecteerde initiatief .

   De naam van het gekopieerde initiatief is *[!UICONTROL Copy of]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Afhankelijk van waar u de nieuwe initiatieven opneemt, kunnen de aantallen bestaande initiatieven veranderen.

1. De naam van het gekopieerde initiatief bijwerken.

   >[!TIP]
   >
   >We raden u aan de naam van het initiatief altijd bij te werken om verwarring te voorkomen als u de namen opnieuw wilt kopiëren.

1. (Optioneel) Werk de prioriteit van uw nieuwe initiatieven bij.

   Voor informatie over het prioriteren van initiatieven, zie [Prioriteiten van initiatieven bijwerken in het [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klikken **[!UICONTROL Save Plan]** om uw wijzigingen op te slaan.
