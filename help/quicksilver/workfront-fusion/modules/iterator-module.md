---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Iteratormodule in Adobe Workfront Fusion
description: Een iteratormodule is een speciaal type module dat een array omzet in een reeks bundels. Elk arrayitem wordt als een afzonderlijke bundel uitgevoerd.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# [!UICONTROL Iterator] module in [!DNL Adobe Workfront Fusion]

An [!UICONTROL Iterator] module is een speciaal type module dat een array omzet in een reeks bundels. Elk arrayitem wordt als een afzonderlijke bundel uitgevoerd.

Zie voor meer informatie [Typen modules](../../workfront-fusion/modules/module-types.md) en [Een array toewijzen in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>Uw organisatie moet Adobe Workfront Fusion en Adobe Workfront aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterator] moduleconfiguratie

U kunt een [!UICONTROL Iterator] dezelfde als u andere modules instelt. De [!UICONTROL Array] bevat de array die moet worden omgezet of gesplitst in afzonderlijke bundels.

![](assets/set-up-iterator-350x190.jpg)

Zie voor meer informatie [De instellingen van een module configureren in Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Voorbeelden:**
>
>* In het onderstaande scenario ziet u hoe u e-mails met bijlagen kunt ophalen en de bijlagen als afzonderlijke bestanden kunt opslaan in een geselecteerde [!DNL Dropbox] map.
   >
   >   E-mails kunnen een array met bijlagen bevatten. De [!UICONTROL Iterator] de module die na de eerste module wordt opgenomen zal u toelaten om elke gehechtheid afzonderlijk te behandelen. De [!UICONTROL Iterator] De array van bijlagen wordt in afzonderlijke bundels gesplitst. Elke bundel, met één bijlage, wordt dan bewaard één voor één in een geselecteerde [!DNL Dropbox] map. De [!UICONTROL Iterator] Hierboven ziet u de installatie van de module: de [!UICONTROL Array] moet het veld de `Attachments` array.
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* Voor uw gemak, velen [!DNL Workfront Fusion] apps bieden gespecialiseerde [!UICONTROL Iterator] modules met een vereenvoudigde installatie. De [!UICONTROL Email] app bevat de speciale [!UICONTROL Iterator] module [!UICONTROL Email] > [!UICONTROL Iterate attachments] dat dezelfde resultaten oplevert als in het algemeen [!UICONTROL Iterator] module.
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## Problemen oplossen: Toewijzingspaneel geeft geen toe te wijzen items weer onder [!UICONTROL Iterator] module

Wanneer een [!UICONTROL Iterator] -module heeft geen informatie over de structuur van de items van de array. Het deelvenster Toewijzing in de modules na het [!UICONTROL Iterator] in de module worden slechts 2 items onder de [!UICONTROL Iterator] module:`Total number of bundles` en `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Dit omdat elke module voor het verstrekken van informatie over punten verantwoordelijk is het output zodat deze punten behoorlijk in het toewijzingspaneel in de verdere modules kunnen worden getoond. Het is echter mogelijk dat verschillende modules deze informatie in sommige gevallen niet kunnen verstrekken; bijvoorbeeld: [!UICONTROL JSON] > [!UICONTROL Parse JSON] of [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] modules met ontbrekende gegevensstructuur.

De oplossing moet het scenario manueel uitvoeren om de module over de punten te maken leren het output zodat kan het de informatie aan de volgende modules verstrekken.

Als u bijvoorbeeld een [!UICONTROL JSON] > [!UICONTROL Parse JSON] zonder gegevensstructuur, zoals hieronder:

![](assets/json-parse-json-350x285.png)

En dan als u een [!UICONTROL Iterator] kunt u de uitvoer van de module niet toewijzen aan het veld Array in het instellingenvenster van het deelvenster [!UICONTROL Iterator] module:

![](assets/connect-iterator-module-350x146.png)

Om dit op te lossen, begin manueel het scenario in de scenarioredacteur. U kunt de modules na [!UICONTROL JSON] > [!UICONTROL Parse JSON] om te voorkomen dat de stroom verder gaat. U kunt ook met de rechtermuisknop op de knop [!UICONTROL JSON] > [!UICONTROL Parse JSON] en kiest u **[!UICONTROL Run this module only]** in het contextmenu alleen de opdracht [!UICONTROL JSON] > [!UICONTROL Parse JSON] module.

Wanneer de [!UICONTROL JSON] > [!UICONTROL Parse JSON] voert uit, leert het over de punten die het output en verstrekt deze informatie aan alle verdere modules, met inbegrip van de module van de Teller. In het deelvenster Toewijzing in de setup van de iterator worden vervolgens de items weergegeven:

![](assets/mapping-panel-displays-items-350x131.png)

Bovendien het kaartpaneel in de modules die na het [!UICONTROL Iterator] geeft de items in de items van de array weer:

![](assets/items-contained-in-array-350x156.png)

Als u niet sommige punten in het de afbeeldingspaneel van een module kunt zien, stel eens het scenario in werking zodat kunnen alle modules over de punten leren zij uitvoeren en deze informatie verstrekken aan de volgende modules.
