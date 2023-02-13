---
title: Intaccingmodules
description: Intaccingmodules
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Intaccingmodules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die Intact gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr>
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Om de modules van de Intacct te gebruiken, moet u een rekening van het Intacct hebben.

## Connect Interface met Workfront Fusion

### Autorisatie [!DNL Workfront Fusion] om wijzigingen aan te brengen in Intact

Voor [!DNL Workfront Fusion] kan verbinding maken met [!DNL Intacct], moet u het autoriseren.

Navigeer in uw Intaccu-account naar de **[!UICONTROL Company]** tab.

1. Klikken **Bedrijfsinfo**.
1. Ga naar de **Beveiliging** tab.
1. Klikken [!UICONTROL Edit] in de rechterbovenhoek
1. Selecteer Webservices-machtigingen.
1. Klik op het plusteken
1. Ga AzuquaMPP als sender_id in.
1. (Optioneel) Voer een beschrijving in voor de verbinding

### Een verbinding instellen in [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

U kunt een verbinding maken met uw [!DNL Intacct] rechtstreeks vanuit een [!DNL Intacct] module.

1. Klik in een willekeurige Intactiemodule op **[!UICONTROL Add]** naast het veld Verbinding.
1. Voer uw Intactische gegevens in

   * Bedrijfs-id
   * Gebruikersnaam
   * Wachtwoord

1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## Interfacemodules en hun velden

Wanneer u [!DNL Intacct] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Daarnaast kunnen aanvullende Intactievelden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Search records]](#search-records)

### [!UICONTROL Make a custom API call] {#make-a-custom-api-call}

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Intacct] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Intacct] modules.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Verbinding</p> </td> 
   <td> <p>Voor instructies over het verbinden van uw rekening van de Intact met [!DNL Workfront Fusion] 2.0, zie <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Een verbinding instellen in Workfront Fusion</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Platte XML</td> 
   <td> <p>Neem alleen de XML in de hoofdtekst op. De aanvraag bevat automatisch verificatieheaders.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search records]

Deze zoekmodule haalt een lijst op met records die voldoen aan specifieke zoekcriteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Verbinding</p> </td> 
   <td> <p>Voor instructies over het verbinden van uw rekening van de Intact met [!DNL Workfront Fusion] 2.0, zie <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Een verbinding instellen in Workfront Fusion</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer het type record dat u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zoekcriteria</p> </td> 
   <td> 
    <ul> 
     <li> <p>Selecteer het veld waarin u wilt zoeken</p> </li> 
     <li> <p>Selecteer de operator die u voor de zoekopdracht wilt gebruiken</p> </li> 
     <li> <p>Voer de waarde in waarnaar u wilt zoeken</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resultaatset</td> 
   <td>Selecteer of u alle overeenkomende records of alleen de eerste overeenkomende record wilt retourneren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limiet</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorteren op</td> 
   <td>Selecteer het veld waarop u de resultaten wilt sorteren. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Volgorde</td> 
   <td>Selecteer of u oplopend of aflopend wilt sorteren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uitvoer</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoofdlettergevoeligheid</td> 
   <td>Schakel deze optie in om uw query hoofdlettergevoelig te maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query uitvoeren op particuliere entiteiten</td> 
   <td>Schakel deze optie in als u wilt dat de module kan zoeken in particuliere entiteiten.</td> 
  </tr> 
 </tbody> 
</table>
