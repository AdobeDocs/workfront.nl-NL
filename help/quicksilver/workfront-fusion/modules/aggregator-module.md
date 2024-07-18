---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Samenvoegmodule in Adobe Workfront Fusion
description: Een aggregatormodule is een type module dat is ontworpen om verschillende bundels gegevens samen te voegen tot één bundel.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# [!UICONTROL Aggregator] module in [!DNL Adobe Workfront Fusion]

Een aggregatormodule is een type module dat is ontworpen om verschillende bundels gegevens samen te voegen tot één bundel.

Voor meer informatie over moduletypes, zie [ Types van modules ](../../workfront-fusion/modules/module-types.md).

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

## [!UICONTROL Aggregator] module

Wanneer een module [!UICONTROL Aggregator] wordt uitgevoerd, doet deze het volgende:

* Accumuleert alle bundels het tijdens de verrichting van één enkele bronmodule ontvangt.
* Hiermee wordt één bundel uitgevoerd met een array die één item per geaccumuleerde bundel bevat. De inhoud van de items van de array is afhankelijk van de specifieke module [!UICONTROL Aggregator] en de instelling ervan.

In de volgende afbeelding ziet u een standaard instelling van de module [!UICONTROL Aggregator] :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>De module vanwaar de bundelaggregatie wordt gestart. De bronmodule is gewoonlijk een iterator of een onderzoeksmodule die een reeks bundels uitvoert. Wanneer u opstelling de bronmodule van de aggregator (en de opstelling van de aggregator sluit), wordt de route tussen de bronmodule en de samenvoegersmodule verpakt in een grijs gebied zodat u duidelijk het begin en het eind van de samenvoeging kunt zien. 
   </p> <p>Zie de module <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] in [!DNL Adobe Workfront Fusion]</a> voor meer informatie over iterators.</p> <p>Voor meer informatie over onderzoeksmodules zie onderzoeksmodules in <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref"> Types van modules </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>(Alleen van toepassing op de module [!UICONTROL Array aggregator] .) De doelstructuur waarin de gegevens moeten worden samengevoegd. De standaardoptie, [!UICONTROL Custom], laat u toe om punten te kiezen die in het 2} punt van de de outputbundel van A [!UICONTROL rray aggregator] {zouden moeten worden samengevoegd:<code>Array </code></p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Zodra u meer modules na de [!UICONTROL Array aggregator] module aansluit en aan de opstelling van de module terugkeert, zal het [!UICONTROL Target] structuurtype dropdown alle volgende modules en hun gebieden bevatten die van typeSerie van Inzamelingen zijn, zoals aangetoond in het [!UICONTROL Attachments] gebied van de [!DNL Slack] &gt; [!UICONTROL Create a Message] module:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>Selecteer de velden die u wilt opnemen in de uitvoer van de aggregatormodule.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>De uitvoer van de aggregator kan met behulp van het veld [!UICONTROL Group by] in verschillende groepen worden gesplitst. Het veld [!UICONTROL Group by] kan een formule bevatten die voor de invoerbundel van elke aggregator wordt geëvalueerd. De aggregator voert vervolgens één bundel uit per de waarde van elke afzonderlijke formule. Elke bundel bevat twee items:</p> 
    <ul> 
     <li><code>Key </code>bevat de specifieke waarde.</li> 
     <li><code>Array </code>bevat de samengevoegde gegevens van de bundels waarvoor de formule aan de <code>Key </code> waarde evalueerde.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwerking stoppen na een lege aggregatie</p> </td> 
   <td> <p>Standaard geeft de module [!UICONTROL Aggregator] het resultaat van de aggregatie door, zelfs als er geen bundels de module [!UICONTROL Aggregator] hebben bereikt (omdat ze bijvoorbeeld allemaal onderweg zijn uitgefilterd). Als de optie [!UICONTROL Stop processing after an empty aggregation] is ingeschakeld, produceert de module [!UICONTROL Aggregator] in dit geval geen uitvoerbundel en stopt de stroom.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Bundels die door modules tussen de bronmodule en de [!UICONTROL Aggregator] module worden geproduceerd worden niet uitgevoerd door de [!UICONTROL Aggregator] module, zodat zij niet toegankelijk door de modules in de stroom na [!UICONTROL Aggregator] zijn. Als u gegevens nodig hebt uit een bundel die is uitgevoerd door een module tussen de bronmodule en de module [!UICONTROL Aggregator] , moet u het opgegeven item opnemen in de instelling van de module [!UICONTROL Aggregator] (zoals in het veld [!UICONTROL Aggregated fields] in de installatie van de module [!UICONTROL Array aggregator] ).


>[!INFO]
>
>**Voorbeeld:** Het Geval van het Gebruik: het Zippen van alle e-mailgehechtheid en het uploaden van het PIT aan [!DNL Dropbox]
>
>In het onderstaande scenario wordt getoond hoe u:
>
>* Kijk naar een postvak voor binnenkomende e-mails: [!UICONTROL Email] > [!UICONTROL Watch emails] trigger voert een bundel uit met item `Attachments[]` . Dit is een array die alle bijlagen van de e-mail bevat.
>
>* Herhaal de bijlagen van de e-mail: [!UICONTROL Email] > [!UICONTROL Iterate attachments] iterator neemt de items één voor één uit de array `Attachments[]` en stuurt ze verder als afzonderlijke bundels.
>
>* Samenvoegen van de bundels die door de [!UICONTROL Email] > [!UICONTROL Iterate attachments] module worden uitgevoerd: [!UICONTROL Archive] > [!UICONTROL Create an archive aggregator] accumuleert alle bundels het ontvangt en output één enkele bundel die het dossier van het PIT bevat.
>
>* Upload het resulterende ZIP-bestand naar [!DNL Dropbox] : [!DNL Dropbox] > [!UICONTROL Upload a file] haalt het ZIP-bestand op uit de module [!UICONTROL Archive] > [!UICONTROL Create an archive] en uploadt het naar [!DNL Dropbox] .
>
>![](assets/dropbox-archive-350x87.png)
>
>Hieronder ziet u een voorbeeldinstelling van de aggregator [!UICONTROL Archive] > [!UICONTROL Create an archive] :
>
>![](assets/archive-create-an-archive-350x484.png)
