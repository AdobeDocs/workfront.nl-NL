---
title: Auditlogboeken weergeven en exporteren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: U kunt alle controlelogboeken in het systeem bekijken, of die die aan bepaalde het filtreren criteria voldoen. U kunt controlelogboeken ook exporteren. De logboeken van de controle maken een lijst gebruiker-veranderingen die in het systeem tijdens de afgelopen 90 dagen in werking worden gesteld.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Controleverslagen weergeven en exporteren

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

U kunt alle controlelogboeken in het systeem bekijken, of die die aan bepaalde het filtreren criteria voldoen. U kunt controlelogboeken naar een Csv- dossier ook uitvoeren.

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
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td><p>Systeembeheerder</p></td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Controlelogboeken weergeven

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem > Logboeken van de Controle**.
1. In het **Type van Actie** drop-down, selecteer het type van controle u wilt bekijken.

   >[!NOTE]
   >
   >De opties in het keuzemenu Type actie variëren afhankelijk van het geselecteerde controlelogboek.

1. In het **drop-down menu van het Type van Logboek**, selecteer het type van controlelogboek u wilt bekijken.

   **Alle Types van Logboek** wordt geselecteerd door gebrek.

   Voor een lijst van alle types van controlelogboek kunt u bekijken en de informatie zij omvatten, zie [ Logboeken van de Controle ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Optioneel) Stel de beschikbare filters in voor de volgende velden:

   * **Gebruikers**: Type de naam van de gebruiker die een verandering aanbracht.
   * **van**: De datum van het begin van het tijdkader toen de verandering werd aangebracht.
   * **aan**: Einddatum van het tijdkader toen de verandering werd aangebracht.

   ![ Logboeken van de Controle ](assets/audit-logs.png)

1. Klik **toepassen**.
1. (Facultatief) klik **Duidelijk** om veranderingen terug te stellen die aan de filters worden aangebracht.

## Controleverslagen exporteren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Logboeken van de Controle**.

1. In het **drop-down menu van het Type van Logboek**, selecteer een controlelogboek.

   **Alle Types van Logboek** wordt geselecteerd door gebrek.

1. Plaats om het even welke beschikbare filters, dan klik **toepassen**.

   >[!IMPORTANT]
   >
   >U kunt niet meer dan 50.000 logboeken tegelijkertijd uitvoeren. Workfront exporteert logbestanden op basis van de filters die u instelt, en niet op basis van het aantal logbestanden op de pagina. U kunt het totale aantal gefilterde logbestanden weergeven in de rechterbenedenhoek van de pagina.

1. Klik **Uitvoer**.

   Het vak Bestand opslaan wordt geopend en u kunt het geëxporteerde bestand op uw computer opslaan.

   U kunt de controlelogboeken slechts in een formaat bewaren CSV.

   Sla het geëxporteerde bestand op. U kunt deze nu vinden op uw computer en delen met anderen.
