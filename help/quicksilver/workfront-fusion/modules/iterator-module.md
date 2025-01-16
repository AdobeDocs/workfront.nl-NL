---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Iteratormodule in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL Iterator] module in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ de module van de Teller ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Een module [!UICONTROL Iterator] is een speciaal type module dat een array omzet in een reeks bundels. Elk arrayitem wordt als een afzonderlijke bundel uitgevoerd.

Voor meer informatie, zie [ Types van modules ](../../workfront-fusion/modules/module-types.md) en [ kaart een serie in de Fusie van Adobe Workfront ](../../workfront-fusion/mapping/map-an-array.md).

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
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet Adobe Workfront Fusion en Adobe Workfront aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterator] moduleconfiguratie

U stelt een [!UICONTROL Iterator] -module in op hetzelfde niveau als een andere module. Het veld [!UICONTROL Array] bevat de array die moet worden omgezet of gesplitst in afzonderlijke bundels.

![](assets/set-up-iterator-350x190.jpg)

Voor meer informatie, zie [ de montages van een module in de Fusie van Adobe Workfront ](../../workfront-fusion/modules/configure-a-modules-settings.md) vormen.

>[!INFO]
>
>**Voorbeelden:**
>
>* In het onderstaande scenario ziet u hoe u e-mails met bijlagen kunt ophalen en de bijlagen als afzonderlijke bestanden in een geselecteerde [!DNL Dropbox] -map kunt opslaan.
>
>   E-mails kunnen een array met bijlagen bevatten. Met de module [!UICONTROL Iterator] die na de eerste module wordt ingevoegd, kunt u elke bijlage afzonderlijk afhandelen. De module [!UICONTROL Iterator] splitst de array van bijlagen in afzonderlijke bundels. Elke bundel, met één bijlage, wordt vervolgens één voor één opgeslagen in een geselecteerde [!DNL Dropbox] -map. De instelling van de module [!UICONTROL Iterator] wordt hierboven weergegeven: het veld [!UICONTROL Array] moet de array `Attachments` bevatten.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Veel [!DNL Workfront Fusion] -apps bieden voor uw gemak gespecialiseerde [!UICONTROL Iterator] -modules met een vereenvoudigde installatie. De app [!UICONTROL Email] bevat bijvoorbeeld de speciale [!UICONTROL Iterator] module [!UICONTROL Email] > [!UICONTROL Iterate attachments] die dezelfde resultaten oplevert als de algemene module [!UICONTROL Iterator] .
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Problemen oplossen: het deelvenster Toewijzing geeft geen toewijzbare items weer onder de module [!UICONTROL Iterator]

Wanneer een module [!UICONTROL Iterator] geen informatie heeft over de structuur van de items van de array, worden in het deelvenster Toewijzing in de modules die volgen op de module [!UICONTROL Iterator] slechts twee items weergegeven onder de module [!UICONTROL Iterator] : `Total number of bundles` en `Bundle order position` :

![](assets/mapping-panel-doesnt-display-350x147.png)

Dit omdat elke module voor het verstrekken van informatie over punten verantwoordelijk is het output zodat deze punten behoorlijk in het toewijzingspaneel in de verdere modules kunnen worden getoond. In sommige gevallen kunnen meerdere modules deze informatie echter niet verschaffen, bijvoorbeeld modules [!UICONTROL JSON] > [!UICONTROL Parse JSON] of [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] met ontbrekende gegevensstructuur.

De oplossing moet het scenario manueel uitvoeren om de module over de punten te maken leren het output zodat kan het de informatie aan de volgende modules verstrekken.

Als u bijvoorbeeld een module [!UICONTROL JSON] > [!UICONTROL Parse JSON] zonder gegevensstructuur hebt, zoals hieronder:

![](assets/json-parse-json-350x285.png)

En als u er een [!UICONTROL Iterator] -module mee verbindt, kunt u de uitvoer van de module niet toewijzen aan het veld Array in het instellingenvenster van de [!UICONTROL Iterator] -module:

![](assets/connect-iterator-module-350x146.png)

Om dit op te lossen, begin manueel het scenario in de scenarioredacteur. U kunt de koppeling tussen de modules opheffen na de module [!UICONTROL JSON] > [!UICONTROL Parse JSON] om te voorkomen dat de stroom wordt voortgezet. U kunt ook met de rechtermuisknop op de module [!UICONTROL JSON] > [!UICONTROL Parse JSON] klikken en **[!UICONTROL Run this module only]** in het contextmenu kiezen om alleen de module [!UICONTROL JSON] > [!UICONTROL Parse JSON] uit te voeren.

Wanneer [!UICONTROL JSON] > [!UICONTROL Parse JSON] uitvoert, leert het over de punten die het output en verstrekt deze informatie aan alle verdere modules, met inbegrip van de module van de Teller uitvoert. In het deelvenster Toewijzing in de setup van de iterator worden vervolgens de items weergegeven:

![](assets/mapping-panel-displays-items-350x131.png)

Bovendien worden in het deelvenster voor toewijzingen in de modules die na de module [!UICONTROL Iterator] worden verbonden, de items weergegeven die zich in de items van de array bevinden:

![](assets/items-contained-in-array-350x156.png)

Als u niet sommige punten in het de afbeeldingspaneel van een module kunt zien, stel eens het scenario in werking zodat kunnen alle modules over de punten leren zij uitvoeren en deze informatie verstrekken aan de volgende modules.
