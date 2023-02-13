---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Veelgestelde vragen over Adobe Workfront Fusion
description: In dit artikel worden veelgestelde vragen over [!DNL Adobe Workfront Fusion], met inbegrip van informatie over voorwerp algemeen gebruikt in de werkschema's van de Fusie
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '601'
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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Wat is een scenario?

### Antwoord

Een scenario definieert een reeks stappen die moet worden uitgevoerd door [!DNL Adobe Workfront Fusion]. Voor elk scenario, specificeert u de gegevensbron, hoe de gegevens moeten worden verwerkt, welke gegevens moeten worden gebruikt en wat moet worden genegeerd. [!DNL Workfront Fusion] kunt u zo complex van scenario&#39;s tot stand brengen aangezien u nodig hebt; zelfs de meest geavanceerde scenario &#39; s zijn mogelijk .

Zie voor meer informatie [Creeer een scenario van de praktijkintegratie in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Kan ik meer dan één module in een scenario gebruiken? Of gewoon een trigger en handeling?

### Antwoord

U kunt zoveel modules gebruiken als u in een scenario wilt. U kunt onafhankelijke routes tot stand brengen en specificeren welke gegevens door hen zouden moeten stromen. U kunt ook resultaten gebruiken die door afzonderlijke acties zijn geretourneerd en deze vervolgens doorgeven aan de volgende actie.

## Kan [!DNL Workfront Fusion] werken met bestanden?

### Antwoord

Ja. Gebruiken [!DNL Workfront Fusion], bestanden kunnen worden ontvangen, opgeslagen, getransformeerd, geconverteerd, gecodeerd enzovoort. Bovendien [!DNL Workfront Fusion] biedt een groot aantal ingebouwde functies die zijn ontworpen om gebruikers in staat te stellen effectief en creatief te werken met de gegevens in de bestanden.

Zie voor meer informatie [Bestanden toewijzen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Wat gebeurt er als ik laat [!DNL Workfront Fusion] een e-mail met meerdere bijlagen verwerken?

### Antwoord

Als u het [!UICONTROL Email] module [!UICONTROL Retrieve attachments], wordt elke gehechtheid verzonden individueel door de rest modules in het scenario. Soortgelijke modules zijn ook beschikbaar in andere apps die meerdere bestanden tegelijk ontvangen.

Zie voor meer informatie [[!UICONTROL Email] modules](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Bij sommige triggers kunnen scenario&#39;s direct worden uitgevoerd. Wat betekent &#39;onmiddellijk&#39;?

### Antwoord

De gemeenschappelijke scenario&#39;s worden in werking gesteld met intervallen volgens het programma u specificeert (bijvoorbeeld, elk uur, elke 5 minuten, eens per maand, en zo). Er zijn speciale triggers, ook wel &#39;instant triggers&#39; genoemd, die uw scenario direct kunnen starten nadat ze gegevens van een bepaalde service ontvangen. Directe triggers kunnen bijzonder nuttig zijn. We raden u aan om ze waar mogelijk te gebruiken. Ze helpen het aantal bewerkingen te verminderen. De ontvangen gegevens worden direct verwerkt zonder op de volgende geplande looppas te wachten. De [!DNL Google Sheets] module [!UICONTROL Watch Changes] start onmiddellijk een scenario nadat een cel is bijgewerkt.

## Wat zijn aggregators?

### Antwoord

An [!UICONTROL Aggregator] Hiermee voegt u gegevens samen in één verzameling. Een voorbeeld hiervan zijn bestanden die worden gecomprimeerd in een zip-archief en als e-mailbijlage worden verzonden.

Zie voor meer informatie [[!UICONTROL Aggregator] module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Wat is een operatie?

### Antwoord

Een verrichting is om het even welke die taak door een module wordt uitgevoerd. Een bewerking vindt bijvoorbeeld altijd plaats wanneer een trigger wordt uitgevoerd en telkens wanneer een handeling een taak uitvoert.

## Wat is gegevensoverdracht?

### Antwoord

De overdracht van gegevens verwijst naar de hoeveelheid gegevens die door uw scenario wordt overgebracht. Stel dat u een scenario hebt dat een 100 kB-afbeelding ophaalt uit FTP en de grootte tot 50 kB reduceert en beide afbeeldingen opslaat naar [!DNL Dropbox]. De hoeveelheid gegevens die in dit scenario wordt gebruikt, is 150 kB.

## Wat is een verbinding?

### Antwoord

Een verbinding is de verbinding tussen uw [!DNL Workfront Fusion] en de service van derden die u wilt gebruiken. De verbinding kan gemakkelijk worden tot stand gebracht wanneer het uitgeven van een scenario. Als u een verbinding wilt toevoegen, klikt u op de knop **[!UICONTROL Add]** in de module-instelling en volg de stapsgewijze instructies.

Zie voor meer informatie [Verbinding maken [!DNL Adobe Workfront Fusion] naar een app of service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
