---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatieven verwijderen in het deelvenster Scenario
description: U kunt initiatieven op een plan schrappen dat u of op een plan creeerde dat iemand met u deelde. U kunt initiatieven die u hebt verwijderd, niet herstellen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Initiatieven verwijderen in het dialoogvenster [!DNL Scenario Planner]

U kunt initiatieven op een plan schrappen dat u of op een plan creeerde dat iemand met u deelde. U kunt initiatieven die u hebt verwijderd, niet herstellen.

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
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven. </p> <p>Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de [!UICONTROL Scenario Planner]</a>. </p> </td> 
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

## Initiatieven verwijderen

Houd rekening met het volgende wanneer u initiatieven verwijdert:

* Als u een initiatief verwijdert, wordt het vereiste aantal functies en de aan het initiatief gekoppelde kosteninformatie uit het plan verwijderd.
* Als u een initiatief verwijdert dat is gemaakt door een project te importeren, wordt het project dat aan het initiatief is gekoppeld, niet verwijderd.
* Als u een initiatief verwijdert dat ten minste eenmaal voor een project is gepubliceerd, resulteert dat in het volgende:

   * Het initiatief wordt uit het scenario geschrapt, maar [!DNL Scenario Planner] het gebied blijft in [!UICONTROL Project Details] sectie.
   * Als het initiatief dat u schrapt het enige gepubliceerde initiatief op het scenario is, wordt de indicator dat het plan is gepubliceerd ook geschrapt.

      Voor informatie over het publiceren van initiatieven aan projecten, zie [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Voor informatie over het creëren van initiatieven door projecten in te voeren, zie [Projecten importeren naar plannen in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

U kunt één initiatief tegelijk verwijderen of meerdere initiatieven bulksgewijs verwijderen.

* [Eén initiatief verwijderen](#delete-one-initiative)
* [Initiatieven bulksgewijs verwijderen](#delete-initiatives-in-bulk)

### Eén initiatief verwijderen {#delete-one-initiative}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op [!UICONTROL Scenarios].

   Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek het initiatief dat u wilt verwijderen.
1. Voer een van de volgende handelingen uit:

   * Klik op de knop **[!UICONTROL More menu]** ![](assets/more-menu.png) rechts van de initiatiefnaam klikt u op **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   * Selecteer het vakje links van het initiatief en klik op **[!UICONTROL Delete]** in het zwevende menu dat onder aan het plan wordt weergegeven, klikt u op **[!UICONTROL Yes, delete it]**.

   Het initiatief en zijn functie en kosteninformatie worden uit het plan geschrapt.

1. Klikken **[!UICONTROL Save Plan]** om uw wijzigingen op te slaan.

### Initiatieven bulksgewijs verwijderen {#delete-initiatives-in-bulk}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op [!UICONTROL Scenarios].

   Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen en zoek het initiatief dat u wilt verwijderen.
1. Selecteer de vakjes links van de initiatieven die u wilt schrappen, dan klik **[!UICONTROL Delete]** in het menu dat onder aan het abonnement wordt weergegeven, klikt u op **[!UICONTROL Yes, delete them]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   De initiatieven en hun functie en kosteninformatie worden uit het plan geschrapt.

1. Klikken **[!UICONTROL Save Plan]** om uw wijzigingen op te slaan.
