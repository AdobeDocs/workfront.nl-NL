---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling genereren in Adobe Workfront Fusion
description: In sommige gevallen kunt u de scenario-uitvoering die door Terugdraaiing of Vastleggingsfase wordt gevolgd forceren willen tegenhouden of de verwerking van een route ophouden en naar keuze het in de rij van Mening opslaan en onvolledige uitvoeringen in de Fusie van Adobe Workfront oplossen.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Foutafhandeling door genereren in [!DNL Adobe Workfront Fusion]

In sommige gevallen, kunt u de scenario-uitvoering die door [ wordt gevolgd het Terugdraaien ](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) of [ gedwongen willen tegenhouden ](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) fase of de verwerking van een route tegenhouden en naar keuze het in de rij van onvolledige uitvoeringen opslaan.

Momenteel kunnen de fout behandelende richtlijnen niet uit het werkingsgebied van een [ de managerroute van de Fout worden gebruikt ](../../workfront-fusion/errors/error-handling.md#error) en [!DNL Adobe Workfront Fusion] biedt geen module aan die u zou toelaten om (werpen) fouten gemakkelijk voorwaardelijk te produceren.

Voor informatie over onvolledige uitvoeringen, zie [ Mening en los onvolledige uitvoeringen in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

Voor informatie over fout behandelende richtlijnen, zie [ Richtlijnen voor fout behandeling in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <p>Of</p>
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

Zie [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md) voor informatie over [!DNL Adobe Workfront Fusion] -licenties

## Oplossing voor Throw

Als u een fout voorwaardelijk wilt genereren, kunt u een module zo configureren dat deze optioneel tijdens de bewerking mislukt. Één mogelijkheid moet [!UICONTROL JSON] gebruiken > [!UICONTROL Parse JSON] module (zie [ modules JSON ](../../workfront-fusion/apps-and-their-modules/json-modules.md)), die wordt gevormd om naar keuze een fout (BundleValidationError in dit geval) te werpen:

Vervolgens kunt u een van de foutafhandelingsinstructies aan de foutafhandelingsroute koppelen:

* Dwing de uitvoering van het scenario om de terugdraaifase te stoppen en uit te voeren: [!UICONTROL Rollback]
* Dwing de uitvoering van het scenario om de vastlegfase te stoppen en uit te voeren: [!UICONTROL Commit]
* Stop de verwerking van een route: [!UICONTROL Ignore]
* Stop de verwerking van een route en bewaar het in de rij van onvolledige uitvoeringenomslag: [!UICONTROL Break]

In het volgende voorbeeld wordt het gebruik van de instructie [!DNL Rollback] getoond:

![](assets/rollback-directive-350x175.png)
