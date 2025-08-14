---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Portefeuilles verwijderen en deactiveren
description: Portfolio's zijn verzamelingen van projecten of programma's in Adobe Workfront. U kunt een portfolio verwijderen of deactiveren als u vindt dat dit niet relevant is voor uw systeem.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 8a4668a568fde2ca7ee26714caae3cd33efe4eda
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Portefeuilles verwijderen en deactiveren

<!--Audited: 2/2024-->

Portfolio&#39;s zijn verzamelingen van projecten of programma&#39;s in [!DNL Adobe Workfront] . U kunt een portfolio verwijderen of deactiveren als u vindt dat dit niet relevant is voor uw systeem.

Wij adviseren deactivering van een portefeuille die niet meer met toekomstige projecten moet worden geassocieerd in plaats van het te schrappen, om de historische informatie over de projecten te houden die momenteel met de portefeuille en zijn programma&#39;s worden geassocieerd.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

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
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL Edit] toegang tot projecten en portfolio's</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor het portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van het verwijderen en deactiveren van portfolio&#39;s

Houd rekening met het volgende wanneer u besluit of u portfolio&#39;s wilt verwijderen of deactiveren:

* Als u een portfolio verwijdert, worden de bijbehorende programma&#39;s verwijderd.

  >[!IMPORTANT]
  >
  >U hoeft geen machtigingen voor programma&#39;s te hebben om het portfolio te kunnen verwijderen.

* Als u een portfolio verwijdert, worden de bijbehorende projecten niet verwijderd.
* U kunt verwijderde portfolio&#39;s niet herstellen.
* Als u een portfolio deactiveert, weet u zeker dat de naam van het portfolio en de bijbehorende programma&#39;s niet meer aan projecten kunnen worden toegewezen wanneer u een project maakt.
* Als u een portfolio deactiveert die al aan een project is gekoppeld, wordt dit niet van het project verwijderd. Als u een gedeactiveerd portfolio uit een project verwijdert, moet u het opnieuw activeren voordat u het weer aan het project kunt koppelen.

## Een portfolio deactiveren

Wanneer u een portfolio deactiveert, hebt u nog steeds toegang tot dit portfolio vanuit het [!UICONTROL Portfolios] -gebied, maar het wordt niet meer weergegeven in de lijst met portfolio&#39;s wanneer gebruikers het willen toevoegen aan een project.

>[!NOTE]
>
>Afhankelijk van de configuratie van de lay-outsjabloon door de [!DNL Workfront] - of groepsbeheerder, wordt het [!UICONTROL Portfolios] -gebied mogelijk niet weergegeven in de [!UICONTROL Main Menu] . Voor meer informatie, zie [ het Belangrijkste Menu aanpassen gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Klik op **[!UICONTROL Portfolios]** .
1. Klik op de naam van het portfolio.
1. Klik **Meer** menu ![ Meer menu ](assets/more-icon.png) rechts van de portefeuillenaam, dan klik **[!UICONTROL Deactivate Portfolio]**.
Het portfolio wordt onmiddellijk gedeactiveerd.
1. (Facultatief) klik het **Meer** menu ![ Meer menu ](assets/more-icon.png) rechts van de portefeuillenaam, dan klik **[!UICONTROL Activate Portfolio]** om het te reactiveren.

## Een portfolio verwijderen

{{step1-to-portfolios}}

1. Voer een van de volgende handelingen uit:

   * Selecteer de portefeuille in de lijst, dan klik het **[!UICONTROL Delete]** pictogram ![ pictogram van de Schrapping ](assets/delete.png).
   * Klik de portefeuille om het te openen, dan klik **Meer** menu ![ ](assets/more-icon.png) aan het recht van de portefeuillenaam, dan **Schrapping Portfolio**.
1. Klik op **[!UICONTROL Yes, Delete It]** om te bevestigen.

   Het portfolio wordt verwijderd en kan niet worden hersteld.
