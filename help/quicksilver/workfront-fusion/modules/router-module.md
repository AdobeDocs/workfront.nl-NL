---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Router module in Adobe Workfront Fusion
description: De module van de Router staat u toe om uw stroom in verscheidene routes te vertakken en de gegevens binnen elke route verschillend te verwerken. Zodra een module van de Router een bundel ontvangt, door:sturen het aan elke verbonden route in de orde de routes aan de module van de Router in bijlage waren.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# [!UICONTROL Router] module in [!DNL Adobe Workfront Fusion]

De [!UICONTROL Router] de module staat u toe om uw stroom in verscheidene routes te vertakken en de gegevens binnen elke route verschillend te verwerken. Eenmaal [!UICONTROL Router] de module ontvangt een bundel, door:sturen het aan elke verbonden route in de orde de routes in bijlage aan [!UICONTROL Router] module.

>[!NOTE]
>
>* Om de orde van de routes te verifiëren, kunt u klikken [!UICONTROL Auto-align] pictogram, dat de routes volgens de orde van boven naar onder zal rangschikken.
>
>  Als u de volgorde wilt wijzigen, verwijdert u de [!UICONTROL Router] en sluit de routes in de gewenste orde opnieuw aan.
>
>* Routes worden opeenvolgend verwerkt, niet parallel. Een bundel wordt niet verzonden naar de volgende route tot het volledig door de vorige route is verwerkt.
>




## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Een [!UICONTROL Router] module aan een scenario

A [!UICONTROL Router] kan op een van de volgende manieren aan een scenario worden toegevoegd:

* Als u verbinding wilt maken met de [!UICONTROL Router] module na een module, klik op het juiste handvat van de module, begin te typen **[!UICONTROL router]** als u er naar wilt zoeken, kiest u **[!UICONTROL Flow Control]** > **[!UICONTROL Router]** in de lijst met modules die worden weergegeven.

   ![](assets/connect-the-router-350x108.png)

* Als u de [!UICONTROL Router] de module tussen twee modules, klikt op het moersleutelpictogram onder de route die de twee modules verbindt (of klikt de route met de rechtermuisknop aan) en kiest **[!UICONTROL Add a router]** in het menu.

   ![](assets/insert-router-350x191.png)

* U kunt een [!UICONTROL Router] automatisch. Als u in de onderstaande afbeelding bijvoorbeeld de module in de rechterbenedenhoek wilt verbinden met de module in de linkerbovenhoek (die al is verbonden met de module in de rechterbovenhoek), sleept u de linkerhandgreep van de module rechtsonder en zet u deze neer op de module linksboven.

   ![](assets/insert-router-automatically-350x379.png)

## Filters

U kunt een filter op een route na plaatsen [!UICONTROL Router] -module voor het filteren van bundels zoals op elke andere route:

1. Klik één van de punten in de route.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. In de **[!UICONTROL Set up a filter]** doos die toont, voorwaarden toevoegt, dan klikt **[!UICONTROL OK]** om de filterinstelling op te slaan.

   ![](assets/set-up-a-filter-2-350x242.png)

Zie voor meer informatie [Een filter toevoegen aan een scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## De fallback-route

De filteropstelling op een route na [!UICONTROL Router] bevat een speciale optie: De terugvalroute:

![](assets/fallback-route-350x260.png)

Wanneer toegelaten, wordt deze route gebruikt in het geval wanneer een bundel niet van kan verdergaan [!UICONTROL Router] module via een andere route omdat de filters op de andere routes het uit filtreerden.

De terugvalroute wordt onderscheiden met een verschillend pijlteken binnen [!UICONTROL Router] module:

![](assets/arrow-sign-in-router-module-350x361.png)

## Indien/anders

Een typisch gebruiksgeval van de reserveroute moet de stroom met één route voortzetten als aan de voorwaarde wordt voldaan en met een andere route als het niet is, zoals in de volgende stappen:

1. Een [!UICONTROL Router] in uw scenario.
1. Verbind beide routes met [!UICONTROL Router] module.
1. Klik op de eerste route en specificeer een voorwaarde:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Klik op de tweede route en laat toe [!UICONTROL fallback route] optie:

   ![](assets/enable-fallback-route-option-350x238.png)
