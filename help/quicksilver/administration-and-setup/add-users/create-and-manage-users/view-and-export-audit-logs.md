---
title: Auditlogboeken weergeven en exporteren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: U kunt alle controlelogboeken in het systeem bekijken, of die die aan bepaalde het filtreren criteria voldoen. U kunt controlelogboeken ook exporteren. De logboeken van de controle maken een lijst gebruiker-veranderingen die in het systeem tijdens de afgelopen 90 dagen in werking worden gesteld.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Controleverslagen weergeven en exporteren

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

U kunt alle controlelogboeken in het systeem bekijken, of die die aan bepaalde het filtreren criteria voldoen. U kunt controlelogboeken ook exporteren.

De logboeken van de controle maken een lijst gebruiker-veranderingen die in het systeem tijdens de afgelopen 90 dagen in werking worden gesteld.

Voor informatie over alle types van controlelogboek en wat hen produceert, zie [ Logboeken van de Controle ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Controlelogboeken weergeven

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem > Logboeken van de Controle**.
1. In het **drop-down menu van het Type van Logboek**, selecteer het type van controlelogboek u wilt bekijken.

   **Alle Types van Logboek** wordt geselecteerd door gebrek.

   Voor een lijst van alle types van controlelogboek kunt u bekijken en de informatie zij omvatten, zie [ Logboeken van de Controle ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Optioneel) Stel de beschikbare filters in.

   >[!NOTE]
   >
   >De opties in het keuzemenu Type actie variëren afhankelijk van het geselecteerde controlelogboek.

   ![ Logboeken van de Controle ](assets/audit-logs.jpg)

1. Klik **toepassen**.
1. (Facultatief) klik **Duidelijke Filters** om veranderingen terug te stellen die aan de filters worden aangebracht.

## Controleverslagen exporteren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem > Logboeken van de Controle**.

1. In het **drop-down menu van het Type van Logboek**, selecteer een controlelogboek.

   **Alle Types van Logboek** wordt geselecteerd door gebrek.

1. Plaats om het even welke beschikbare filters, dan klik **toepassen**.

   >[!IMPORTANT]
   >
   >U kunt niet meer dan 50.000 logboeken tegelijkertijd uitvoeren. Workfront exporteert logbestanden op basis van de filters die u instelt, en niet op basis van het aantal logbestanden op de pagina. U kunt het totale aantal gefilterde logbestanden weergeven in de rechterbenedenhoek van de pagina.

1. Klik **Uitvoer**.
