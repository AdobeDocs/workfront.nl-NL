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

Voor meer informatie over moduletypes, zie [Typen modules](../../workfront-fusion/modules/module-types.md).

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

## [!UICONTROL Aggregator] module

Wanneer een [!UICONTROL Aggregator] wordt als volgt uitgevoerd:

* Accumuleert alle bundels het tijdens de verrichting van één enkele bronmodule ontvangt.
* Hiermee wordt één bundel uitgevoerd met een array die één item per geaccumuleerde bundel bevat. De inhoud van de items van de array is afhankelijk van het specifieke [!UICONTROL Aggregator] en de instelling ervan.

In de volgende afbeelding ziet u een standaardinstelling voor het [!UICONTROL Aggregator] module:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>De module vanwaar de bundelaggregatie wordt gestart. De bronmodule is gewoonlijk een iterator of een onderzoeksmodule die een reeks bundels uitvoert. Wanneer u opstelling de bronmodule van de aggregator (en de opstelling van de aggregator sluit), wordt de route tussen de bronmodule en de samenvoegersmodule verpakt in een grijs gebied zodat u duidelijk het begin en het eind van de samenvoeging kunt zien. 
   </p> <p>Zie voor meer informatie over iterators <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] module in [!DNL Adobe Workfront Fusion]</a></p> <p>Voor meer informatie over onderzoeksmodules zie onderzoeksmodules in <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Typen modules</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>(Alleen van toepassing op de [!UICONTROL Array aggregator] module.) De doelstructuur waarin de gegevens moeten worden samengevoegd. De standaardoptie, [!UICONTROL Custom], kunt u items kiezen die moeten worden samengevoegd tot de A[!UICONTROL rray aggregator]Uitvoerbundel <code>Array </code>item:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Zodra u meer modules na verbindt [!UICONTROL Array aggregator] en terug naar de installatie van de module, [!UICONTROL Target] het structuurtype dropdown zal alle volgende modules en hun gebieden bevatten die van typeSerie van Inzamelingen zijn, zoals aangetoond in [!UICONTROL Attachments] van het [!DNL Slack] &gt;[!UICONTROL Create a Message] module:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>Selecteer de velden die u wilt opnemen in de uitvoer van de aggregatormodule.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>De uitvoer van de aggregator kan met behulp van de [!UICONTROL Group by] veld. De [!UICONTROL Group by] het veld kan een formule bevatten die voor de invoerbundel van elke aggregator wordt geëvalueerd. De aggregator voert vervolgens één bundel uit per de waarde van elke afzonderlijke formule. Elke bundel bevat twee items:</p> 
    <ul> 
     <li><code>Key </code>bevat de specifieke waarde.</li> 
     <li><code>Array </code>bevat de geaggregeerde gegevens van de bundels waarvoor de aan de <code>Key </code>waarde.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwerking stoppen na een lege aggregatie</p> </td> 
   <td> <p>Standaard worden de [!UICONTROL Aggregator] -module geeft het resultaat van de aggregatie weer, zelfs als geen bundels de [!UICONTROL Aggregator] (bijvoorbeeld omdat ze allemaal onderweg zijn uitgefilterd). Als de optie [!UICONTROL Stop processing after an empty aggregation] is ingeschakeld, wordt de [!UICONTROL Aggregator] -module in dit geval geen uitvoerbundel produceert en de stroom stopt.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Bundels die door modules tussen de bronmodule en [!UICONTROL Aggregator] wordt niet uitgevoerd door de [!UICONTROL Aggregator] -module, zodat ze niet toegankelijk zijn voor de modules in de flow na de [!UICONTROL Aggregator]. Als u om het even welke gegevens van een bundel nodig hebt die door een module tussen de bronmodule en wordt uitgevoerd [!UICONTROL Aggregator] moet u ervoor zorgen dat het opgegeven item wordt opgenomen in de [!UICONTROL Aggregator] de opstelling van de module (zoals in [!UICONTROL Aggregated fields] in de opstelling van het [!UICONTROL Array aggregator] module).


>[!INFO]
>
>**Voorbeeld:** Hoofdlettergebruik: Alle e-mailbijlagen bekijken en uploaden naar [!DNL Dropbox]
>
>In het onderstaande scenario wordt getoond hoe u:
>
>* Kijk naar een postbus voor binnenkomende e-mails: [!UICONTROL Email] >[!UICONTROL Watch emails] trigger zal een bundel met item uitvoeren `Attachments[]`, dit is een array die alle bijlagen van de e-mail bevat.
>
>* Bijlagen van de e-mail herhalen: [!UICONTROL Email] >[!UICONTROL Iterate attachments] de iterator neemt de punten van `Attachments[]` array een voor een en verzendt deze verder als afzonderlijke bundels.
>
>* De door de [!UICONTROL Email] >[!UICONTROL Iterate attachments] module: [!UICONTROL Archive] >[!UICONTROL Create an archive aggregator] worden alle ontvangen bundels geaccumuleerd en wordt één bundel uitgevoerd die het ZIP-bestand bevat.
>
>* Het resulterende ZIP-bestand uploaden naar [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Upload a file] verkrijgt het ZIP-bestand uit het [!UICONTROL Archive] > [!UICONTROL Create an archive] en uploadt naar [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Hieronder ziet u een voorbeeldinstelling voor het [!UICONTROL Archive] > [!UICONTROL Create an archive] aggregator:
>
>![](assets/archive-create-an-archive-350x484.png)
