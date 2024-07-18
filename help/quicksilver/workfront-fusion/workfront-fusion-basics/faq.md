---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Veelgestelde vragen over Adobe Workfront Fusion
description: Dit artikel behandelt gemeenschappelijke vragen met betrekking tot  [!DNL Adobe Workfront Fusion], met inbegrip van informatie over voorwerp algemeen gebruikt in de werkschema's van de Fusie
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Veelgestelde vragen over Adobe Workfront Fusion

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

## Wat is een scenario?

### Antwoord

Een scenario definieert een reeks stappen die door [!DNL Adobe Workfront Fusion] moet worden uitgevoerd. Voor elk scenario, specificeert u de gegevensbron, hoe de gegevens moeten worden verwerkt, welke gegevens moeten worden gebruikt en wat moet worden genegeerd. Met [!DNL Workfront Fusion] kunt u zo complex mogelijke scenario&#39;s maken. Zelfs de meest geavanceerde scenario&#39;s zijn mogelijk.

Voor meer informatie, zie [ een scenario van de praktijkintegratie in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md) creëren.

## Kan ik meer dan één module in een scenario gebruiken? Of gewoon een trigger en handeling?

### Antwoord

U kunt zoveel modules gebruiken als u in een scenario wilt. U kunt onafhankelijke routes tot stand brengen en specificeren welke gegevens door hen zouden moeten stromen. U kunt ook resultaten gebruiken die door afzonderlijke acties zijn geretourneerd en deze vervolgens doorgeven aan de volgende actie.

## Kan [!DNL Workfront Fusion] werken met bestanden?

### Antwoord

Ja. Met [!DNL Workfront Fusion] kunnen bestanden worden ontvangen, opgeslagen, getransformeerd, geconverteerd, versleuteld, enzovoort. Bovendien biedt [!DNL Workfront Fusion] een groot aantal ingebouwde functies die zijn ontworpen om gebruikers in staat te stellen effectief en creatief te werken met de gegevens in de bestanden.

Voor meer informatie, zie [ Ongeveer toewijzingsdossiers in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Wat gebeurt er als ik [!DNL Workfront Fusion] een e-mailbericht met meerdere bijlagen laat verwerken?

### Antwoord

Als u de [!UICONTROL Email] module [!UICONTROL Retrieve attachments] gebruikt, wordt elke gehechtheid verzonden individueel door de rest modules in het scenario. Soortgelijke modules zijn ook beschikbaar in andere apps die meerdere bestanden tegelijk ontvangen.

Voor meer informatie, zie [[!UICONTROL Email] modules ](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Bij sommige triggers kunnen scenario&#39;s direct worden uitgevoerd. Wat betekent &#39;onmiddellijk&#39;?

### Antwoord

De gemeenschappelijke scenario&#39;s worden in werking gesteld met intervallen volgens het programma u specificeert (bijvoorbeeld, elk uur, elke 5 minuten, eens per maand, en zo). Er zijn speciale triggers, ook wel &#39;instant triggers&#39; genoemd, die uw scenario direct kunnen starten nadat ze gegevens van een bepaalde service ontvangen. Directe triggers kunnen bijzonder nuttig zijn. We raden u aan om ze waar mogelijk te gebruiken. Ze helpen het aantal bewerkingen te verminderen. De ontvangen gegevens worden direct verwerkt zonder op de volgende geplande looppas te wachten. Met de module [!DNL Google Sheets] [!UICONTROL Watch Changes] wordt bijvoorbeeld direct na het bijwerken van een cel een scenario gestart.

## Wat zijn aggregators?

### Antwoord

Met een [!UICONTROL Aggregator] worden gegevens samengevoegd in één verzameling. Een voorbeeld hiervan zijn bestanden die worden gecomprimeerd in een zip-archief en als e-mailbijlage worden verzonden.

Zie [[!UICONTROL Aggregator] module in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md) voor meer informatie.

## Wat is een operatie?

### Antwoord

Een verrichting is om het even welke die taak door een module wordt uitgevoerd. Een bewerking vindt bijvoorbeeld altijd plaats wanneer een trigger wordt uitgevoerd en telkens wanneer een handeling een taak uitvoert.

## Wat is gegevensoverdracht?

### Antwoord

De overdracht van gegevens verwijst naar de hoeveelheid gegevens die door uw scenario wordt overgebracht. Stel dat u een scenario hebt dat een 100 kB-afbeelding ophaalt van FTP en de grootte tot 50 kB reduceert en beide afbeeldingen opslaat naar [!DNL Dropbox] . De hoeveelheid gegevens die in dit scenario wordt gebruikt, is 250 kB.

## Wat is een verbinding?

### Antwoord

Een verbinding is de koppeling tussen uw [!DNL Workfront Fusion] -account en de service van derden die u wilt gebruiken. De verbinding kan gemakkelijk worden tot stand gebracht wanneer het uitgeven van een scenario. Als u een verbinding wilt toevoegen, klikt u op de knop **[!UICONTROL Add]** in de module-instelling en volgt u de stapsgewijze instructies.

Voor meer informatie, zie [ Overzicht van Verbindingen ](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
