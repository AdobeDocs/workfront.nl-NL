---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenario-uitvoeringsstroom in Adobe Workfront Fusion
description: In dit artikel wordt uitgelegd hoe een scenario wordt uitgevoerd en hoe de gegevens erin stromen. Hier wordt ook uitgelegd waar u informatie kunt vinden over uw verwerkte gegevens en hoe u deze kunt lezen.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Uitvoeringsstroom van scenario&#39;s in [!DNL Adobe Workfront Fusion]

In dit artikel wordt uitgelegd hoe een scenario wordt uitgevoerd en hoe de gegevens erin stromen. Hier wordt ook uitgelegd waar u informatie kunt vinden over uw verwerkte gegevens en hoe u deze kunt lezen.

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

## Uitvoerstroom van scenario

Nadat een scenario opstelling correct en geactiveerd is, voert het volgens zijn bepaald programma uit.

Terwijl het scenario begint, reageert de eerste module op een gebeurtenis waarvoor deze is ingesteld. Als het om het even welke bundels (gegevens) terugkeert, gaan zij tot de volgende module over en het scenario gaat verder, die de bundels door elke opeenvolgende module, één voor één overgaat.

Als de bundels correct door alle modules verwerken, is het scenario duidelijk als succes in het gebied van de scenario-details, zoals die in [Scenario-details in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Voor meer informatie bij vestiging een scenario, zie [Basisscenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Voor meer informatie bij het activeren van een scenario, zie [Een scenario activeren of deactiveren in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Voor meer informatie bij het plannen van een scenario, zie [Een scenario plannen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Voor meer informatie over modules, zie [Typen modules](../../workfront-fusion/modules/module-types.md).

### Voorbeeld: [!UICONTROL [!DNL Workfront Fusion] for Work Automation]

>[!INFO]
>
>**Voorbeeld:** In een scenario dat voor inkomende verzoeken binnen kijkt [!DNL Workfront] en zet ze vervolgens om in [!DNL Workfront] projecten zouden de gegevens als volgt stromen .
>
>De eerste stap van het scenario, die door de eerste module wordt uitgevoerd, moet op verzoeken letten. Elk verzoek dat binnen komt wordt beschouwd als één bundel. Als de module zonder enige bundels loopt te vinden, beëindigt het scenario na de eerste module.
>
>Als de eerste module een bundel terugkeert, gaat de bundel door de rest van het scenario. In dit voorbeeld, bestaat de rest van het scenario uit de tweede en laatste module, die het verzoek in een project omzet.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Voorbeeld: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]

>[!INFO]
>
>**Voorbeeld:** In een scenario waarin documenten worden gedownload van [!DNL Adobe Workfront] en verzendt deze naar een map in [!DNL Dropbox]De gegevens zouden als volgt stromen.
>
>De eerste stap van het scenario, die door de eerste module wordt uitgevoerd, is op bundels (documenten) te letten. In dit voorbeeld zoekt de module naar bundels in [!DNL Workfront]. Als het geen bundel terugkeert, eindigt het scenario na de eerste module.
>
>Als een bundel is teruggekeerd, gaat de bundel door de rest van het scenario. In dit voorbeeld bestaat de rest van het scenario uit de tweede en laatste module, die de bundel naar de [!DNL Dropbox] map.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Als de eerste module meerdere bundels retourneert, wordt de eerste bundel geüpload naar [!DNL Dropbox] voordat de tweede bundel is geüpload. Vervolgens uploadt de tweede bundel, vervolgens de derde, enzovoort.

## Informatie over verwerkte bundels

Voor elke module, gaat de bundel door een proces in vier stappen alvorens naar de volgende module te gaan of zijn definitieve bestemming te bereiken. Het proces in vier stappen is Initalization, Operation, Commit/Rollback en Finalization. Dit wordt genoemd transactieverwerking en het helpt om te verklaren hoe het gegeven in een module werd verwerkt.

Zodra een scenario looppas volledig is, toont elke module een pictogram dat het aantal uitgevoerde verrichtingen toont. U kunt op dit pictogram klikken om de gedetailleerde informatie over de verwerkte bundels in de hierboven beschreven indeling weer te geven. U kunt zien welke modules montages werden gebruikt en welke bundels door welke module werden teruggegeven.

![](assets/info-processed-bundles-350x396.png)

Een module ontving inputinformatie zoals:

* Omgezette afbeelding
* Geselecteerde map waarnaar de afbeelding moet worden geüpload
* Oorspronkelijke naam van de [!DNL Facebook] image

Na verwerking, keerde de module deze outputinformatie terug:

* Afbeeldings-id toegewezen door [!DNL Dropbox]
* Volledig pad waarin [!DNL Dropbox] [!DNL Workfront Fusion] Het bestand geüpload

De bovenstaande informatie wordt voor elke bundel afzonderlijk vastgelegd, zoals aangegeven in de vervolgkeuzelijsten [!UICONTROL Operation 1] en [!UICONTROL Operation 2] in de afbeelding.

Zie voor meer informatie over transactieverwerking [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Er is een fout opgetreden tijdens het uitvoeren van een scenario

Er kan een fout optreden tijdens het uitvoeren van het scenario. Als u bijvoorbeeld de opdracht [!DNL Dropbox] de omslag die u als doelomslag in de module het plaatsen hebt geplaatst, eindigt het scenario met een foutenmelding. Voor meer informatie over hoe te om fouten te behandelen, zie [Fout bij verwerken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
