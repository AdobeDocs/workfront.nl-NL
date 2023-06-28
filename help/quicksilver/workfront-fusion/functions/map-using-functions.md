---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Items toewijzen met behulp van functies in [!DNL Adobe Workfront Fusion]
description: Wanneer u items toewijst, kunt u functies gebruiken om eenvoudige of complexe formules te maken.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Items toewijzen met behulp van functies in [!DNL Adobe Workfront Fusion]

Wanneer u items toewijst, kunt u functies gebruiken om eenvoudige of complexe formules te maken.

De functies die beschikbaar zijn in [!DNL Adobe Workfront Fusion] zijn gelijkaardig aan functies in Excel en in sommige programmeertalen. Ze evalueren algemene logica, wiskunde, tekst, datums en arrays. U kunt hiermee voorwaardelijke logica en transformaties van itemwaarden uitvoeren, zoals het omzetten van tekst in hoofdletters, het bijsnijden van tekst, het omzetten van een datum in een andere notatie en nog veel meer. Zie voor meer informatie [Informatie van de ene module toewijzen aan de andere in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
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

## Functies invoegen in velden

Als u op een veld klikt, [!UICONTROL mapping] wordt weergegeven. Het deelvenster Toewijzing bevat verschillende tabbladen:

![](assets/functions-toolbar-350x189.png)

De eerste tab ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (weergegeven bij het openen van het deelvenster) geeft de items weer die u vanuit andere modules kunt toewijzen.

De andere tabbladen bevatten de volgende typen functies:

* **Algemene functies** ![](assets/toolbar-icon-general-function.png) - Zie [Algemene functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) voor meer informatie .

* **Math-functies** ![](assets/toolbar-icon-math-functions.png) - Zie [Wiskundige functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) voor meer informatie .

* **Tekst- en binaire functies** ![](assets/toolbar-icon-text&binary-functions.png) - Zie [Tekenreeksfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) voor meer informatie .

* **Datum en tijd** ![](assets/toolbar-icon-date&time-functions.png) - Zie [Datum- en tijdfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) en de artikelen hieronder voor meer informatie .

   * [Tokens voor datum- en tijdnotaties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens voor datum- en tijdparsering bij [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Functies voor het werken met arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Zie [Arrayfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) voor meer informatie .

Een functie invoegen in een veld:

1. Klik op de naam van de functie.

   of

   Sleep de functie naar het veld.

>[!INFO]
>
>**Voorbeeld:** Sommige gegevenstypen verhinderen dat gebruikers meer dan een bepaald aantal tekens invoeren. U kunt de subtekenreeksfunctie gebruiken om een waarde te beperken tot een bepaald aantal tekens.
>
>In dit voorbeeld beperkt de subtekenreeksfunctie de projectnaam tot 50 tekens.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Nesten, functies

U kunt functies binnen elkaar nesten.

## Gebruiken [!DNL Google Sheets] functies

Indien [!DNL Workfront Fusion] heeft geen functie die u wilt gebruiken, maar deze is voorzien van [!DNL Google Sheets], kunt u het gebruiken door deze stappen te volgen:

1. In [!DNL Google Sheets], maakt u een nieuw leeg spreadsheet.
1. In [!DNL Workfront Fusion], open uw scenario.
1. Voeg de **[!DNL Google Sheets]** >**[!UICONTROL Update a cell]** aan het scenario.

   Voor instructies over het toevoegen van een module, zie [Voeg een module in een scenario toe](../../workfront-fusion/scenarios/create-a-scenario.md#add) in het artikel [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configureer de module:

   1. Kies het nieuwe werkblad in het dialoogvenster **[!UICONTROL Spreadsheet]** veld.
   1. Voeg uw formule in die de [!DNL Google Sheets] functie(s) in de **[!UICONTROL Value]** veld.

      U kunt de output van voorafgaande modules zoals gebruikelijk gebruiken.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Voeg de **[!UICONTROL Google Sheets]>[!UICONTROL Get a cell]** om het berekende resultaat te verkrijgen.
1. Vorm de module, gebruikend zelfde identiteitskaart van de Cel die u in stap 4 gebruikte.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
