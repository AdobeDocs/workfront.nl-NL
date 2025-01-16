---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Voeg een filter aan een scenario in  [!DNL Adobe]  de Fusie van Workfront toe
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Een filter toevoegen aan een scenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ voeg een filter aan een scenario ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-filter-to-a-scenario.html) toe
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

In sommige scenario&#39;s, moet u slechts met bundels werken die aan specifieke criteria voldoen. Met filters kunt u deze bundels selecteren.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

U kunt een filter tussen twee modules toevoegen en controleren of de bundels die van de voorafgaande modules worden ontvangen specifieke filtervoorwaarden vervullen:

* Als zij, de bundels overgaan tot de volgende module in het scenario.
* Als ze dat niet doen, wordt de verwerking voor de bundels beëindigd.

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
  <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

U moet beide modules aan een scenario toevoegen alvorens u een filter tussen hen kunt toevoegen.

## Voeg een filter tussen twee modules toe:

1. Klik op **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerdeelvenster en selecteer het scenario dat u wilt openen.
1. Klik in de rechterbovenhoek van het venster op **[!UICONTROL Edit]** .
1. Klik op de verbindingslijn tussen de modules.
1. Typ een **[!UICONTROL Label]** voor het filter in het vak dat wordt weergegeven.
1. Definieer een filter **[!UICONTROL Condition]** .

   U kunt een of twee operanden invoeren in de twee vakken. Als u operanden in beide vakken invoert, kunt u een operator selecteren in het vervolgkeuzemenu tussen de operanden om de relatie tussen de operanden op te geven.

   >[!TIP]
   >
   >In de operandgebieden, kunt u waarden op de zelfde manier ingaan aangezien u hen in kaart zou brengen, zoals die in [ wordt beschreven de informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Als u bijvoorbeeld wilt dat het filter bestanden zoekt in [!DNL Adobe Workfront] die eindigen met XML en deze doorgeeft aan [!DNL Dropbox] , typt u **[!UICONTROL File name]** in het eerste vak en.**[!UICONTROL xml]** in het tweede vak. In het vervolgkeuzemenu ertussen selecteert u **[!UICONTROL Ends with (case insensitive)]** . Dit filter wordt toegepast op binnenkomende bundels uit de eerste module (Workfront). Alleen bundels die XML-bestanden bevatten, worden doorgegeven aan de volgende module ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Klik op **[!DNL OK]**.

## Een filter kopiëren

Momenteel, omvat de scenario redacteur geen eigenschap voor het kopiëren van een filter.

>[!NOTE]
>
>Als u de modules aan weerszijden van het filter kopieert, wordt het filter ook gekopieerd.
>
>Voor meer informatie bij het kopiëren van modules, zie [ modules of scenario&#39;s van het Exemplaar in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Als u een filter wilt kopiëren zonder modules te kopiëren, kunt u [!DNL Google] Chrome gebruiken voor de volgende oplossing:

1. Installeer de extensie [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] .
1. Open het scenario in [!DNL Workfront Fusion] .
1. Klik op het Chrome-menu met drie punten en klik vervolgens op * *[!UICONTROL More tools*]* > **[!UICONTROL Developer tools]** .

1. Klik in het deelvenster [!UICONTROL Developer tools] dat wordt weergegeven op de menubalk boven in het scherm op de tab [!UICONTROL Workfront Fusion] .

   ![](assets/copy-a-filter-350x174.png)

1. Klik op het pictogram **[!UICONTROL Tools]** ![](assets/devtools-tools-icon.png) in de linkerzijbalk.

1. Klik op **[!UICONTROL Copy Filter]** en configureer het gereedschap **[!UICONTROL Copy Filter]** in het rechterdeelvenster:

   1. Stel de **[!UICONTROL Source Module]** in als de module rechts na het filter dat u wilt kopiëren.
   1. Stel de **[!UICONTROL Target Module]** in als de module vlak voor het filter dat u wilt kopiëren.

1. Klik op **[!UICONTROL Run]**.
