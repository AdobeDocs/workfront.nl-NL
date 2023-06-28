---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een filter toevoegen aan een scenario in [!DNL Adobe] Workfront Fusion
description: In sommige scenario's, moet u slechts met bundels werken die aan specifieke criteria voldoen. Met filters kunt u deze bundels selecteren.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Een filter toevoegen aan een scenario in [!DNL Adobe Workfront Fusion]

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

U moet beide modules aan een scenario toevoegen alvorens u een filter tussen hen kunt toevoegen.

## Voeg een filter tussen twee modules toe:

1. Klikken **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerpaneel, dan selecteer het scenario om het te openen.
1. Klik in de rechterbovenhoek van het venster op **[!UICONTROL Edit]**.
1. Klik op de verbindingslijn tussen de modules.
1. Typ in het vak dat wordt weergegeven een **[!UICONTROL Label]** voor het filter.
1. Een filter definiëren **[!UICONTROL Condition]**.

   U kunt een of twee operanden invoeren in de twee vakken. Als u operanden in beide vakken invoert, kunt u een operator selecteren in het vervolgkeuzemenu tussen de operanden om de relatie tussen de operanden op te geven.

   >[!TIP]
   >
   >In de operandvelden kunt u waarden invoeren op dezelfde manier als u deze toewijst, zoals wordt beschreven in [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Als u bijvoorbeeld wilt dat het filter bestanden zoekt in [!DNL Adobe Workfront] eindigen met XML en doorgeven aan [!DNL Dropbox], voert u in **[!UICONTROL File name]** in het eerste vak en .**[!UICONTROL xml]** in het tweede vak. In het vervolgkeuzemenu ertussen selecteert u **[!UICONTROL Ends with (case insensitive)]**. Dit filter wordt toegepast op binnenkomende bundels uit de eerste module (Workfront). Alleen pakketten met XML-bestanden worden doorgegeven aan de volgende module ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Klik op **[!DNL OK]**.

## Een filter kopiëren

Momenteel, omvat de scenario redacteur geen eigenschap voor het kopiëren van een filter.

>[!NOTE]
>
>Als u de modules aan weerszijden van het filter kopieert, wordt het filter ook gekopieerd.
>
>Voor meer informatie over het kopiëren van modules, zie [Modules of scenario&#39;s kopiëren in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Als u een filter wilt kopiëren zonder modules te kopiëren, kunt u [!DNL Google] Chroom voor de volgende tijdelijke oplossing:

1. Installeer de [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] extensie.
1. In [!DNL Workfront Fusion], opent u het scenario.
1. Klik op het menu Chrome met drie punten en klik op **[!UICONTROL More tools*]* > **[!UICONTROL Developer tools]**.

1. In de [!UICONTROL Developer tools] in het deelvenster dat wordt weergegeven, op de menubalk aan de bovenkant, klikt u op de knop [!UICONTROL Workfront Fusion] tab.

   ![](assets/copy-a-filter-350x174.png)

1. Klik op de knop **[!UICONTROL Tools]** pictogram ![](assets/devtools-tools-icon.png) in de linkerzijbalk.

1. Klikken **[!UICONTROL Copy Filter]** en configureer vervolgens de **[!UICONTROL Copy Filter]** in het rechterzijpaneel:

   1. Stel de **[!UICONTROL Source Module]** als de module rechts na het filter dat u wilt kopiëren.
   1. Stel de **[!UICONTROL Target Module]** als de module vlak voor het filter dat u wilt kopiëren.

1. Klik op **[!UICONTROL Run]**.
