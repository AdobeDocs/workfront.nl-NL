---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Stroomregeling in Adobe Workfront Fusion
description: Wanneer u een scenario creeert of uitgeeft, kunt u montages vormen om de manier te controleren de gegevens door het stromen.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Stroomregeling in Adobe Workfront Fusion

Wanneer u een scenario creeert of uitgeeft, kunt u montages vormen om de manier te controleren de gegevens door het stromen.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repeater

U kunt een [!UICONTROL Repeater] om een taak een bepaald aantal keren te herhalen. A [!UICONTROL Repeater] -module genereert bundels, een voor een.

U kunt bijvoorbeeld een [!UICONTROL Repeater] om vijf e-mails te verzenden met de onderwerpen &quot;Hello 1,&quot; &quot;Hello 2,&quot; enzovoort, door de **[!UICONTROL Email]>[!UICONTROL Send me an email]** aan de [!UICONTROL Repeater] module.

Als u een [!UICONTROL Repeater] module:

1. Klik op de knop [!UICONTROL Flow Control] pictogram ![](assets/flow-control-icon.gif) onder aan het scherm klikt u op **[!UICONTROL Repeater]** in het menu dat wordt weergegeven.
1. Klik op de knop [!UICONTROL Repeater] bundel, klik dan **[!UICONTROL Connect automatically]** in het vak dat wordt weergegeven.
1. In de [!UICONTROL Flow Control] vak dat wordt weergegeven, typt u het gewenste aantal herhalingen (uitvoerbundels) in het dialoogvenster **[!UICONTROL Repeats]** doos.

   In ons e-mailvoorbeeld typt u 5.

   ![](assets/repeater-2-350x207.png)

   De waarde van het item neemt in elke herhaling toe met de waarde die is opgegeven in het dialoogvenster **[!UICONTROL Step]** veld, dat u kunt bekijken door te selecteren **[!UICONTROL Show advanced settings]**. Dit getal is standaard 1.

1. Klikken **[!UICONTROL OK]** om de **[!UICONTROL Flow Control]** doos.

1. Klik op de app of servicemodule die is verbonden met de [!UICONTROL Repeater] module.
1. Typ in het vak dat wordt weergegeven de informatie die u wilt herhalen.

   In ons e-mailvoorbeeld typt u Hello in het dialoogvenster [!UICONTROL Subject] box, dan kaart `i` uit de repeatermodule.

   ![](assets/repeater-3-350x207.png)

| Item | Beschrijving |
|---|---|
| [!UICONTROL Initial value] | Ga of kaart het aantal in dat u de module wilt plaatsen zoals `i` in de eerste herhaling. De standaardwaarde is 1. |
| [!UICONTROL Repeats] | Ga of kaart het aantal tijden in dat u de module wilt herhalen. Dit getal moet groter dan of gelijk aan 0 zijn en kleiner dan of gelijk aan 10.000. |
| [!UICONTROL Step] | Dit is het aantal waardoor de module de waarde van verhoogt `i`. De standaardwaarde is 1. |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Het aantal herhalingen wordt niet bepaald door de waarde van `i`, zoals het in een lus in programmering zou zijn. In de module wordt het aantal keren herhaald dat in het dialoogvenster [!UICONTROL Repeats] veld. De waarde `i` veranderingen met elke herhaling van [!DNL repeater] en kan worden toegewezen aan latere modules. In het bovenstaande voorbeeld wordt de waarde van `i` in het bericht van Hello, resulterend in berichten die &quot;Hello 1,&quot;Hello 2,&quot;etc. lezen.

## [!UICONTROL Iterator]

An [!UICONTROL Iterator] is een speciaal type module dat een array omzet in een reeks bundels. Elk arrayitem wordt een aparte bundel in de [!UICONTROL Iterator] module uitvoer. Zie voor meer informatie [[!UICONTROL Iterator] module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Arrayaggregator

Een arrayaggregator is een speciaal type module waarmee u verschillende bundels kunt samenvoegen tot één bundel. Zie voor meer informatie [[!UICONTROL Aggregator] module in Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

De [!UICONTROL Router] de module staat u toe om uw stroom in verscheidene routes te vertakken en de gegevens binnen elke route verschillend te verwerken. Eenmaal [!UICONTROL Router] de module ontvangt een bundel, door:sturen het aan elke verbonden route in de orde de routes in bijlage aan [!UICONTROL Router] module. Zie voor meer informatie [Router module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
