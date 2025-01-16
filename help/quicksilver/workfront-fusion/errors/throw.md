---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling genereren in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Foutafhandeling door genereren in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ vorm `throw` foutenwerkaround ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

In sommige gevallen, kunt u de scenario-uitvoering die door [ wordt gevolgd van het Terugschroeven van prijzen ](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) of [ toewijzen ](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) fase of willen ophouden de verwerking van een route en naar keuze het opslaan in de rij van onvolledige uitvoeringen.

Momenteel kunnen de fout behandelende richtlijnen niet uit het werkingsgebied van een [ de managerroute van de Fout worden gebruikt ](../../workfront-fusion/errors/error-handling.md#error) en [!DNL Adobe Workfront Fusion] biedt geen module aan die u zou toelaten om (werpen) fouten gemakkelijk te produceren.

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

Zie [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md) voor informatie over [!DNL Adobe Workfront Fusion] -licenties

## Oplossing voor Throw

Om een fout voorwaardelijk te werpen, kunt u een module vormen om het naar keuze opzettelijk tijdens zijn verrichting te maken ontbreken. Één mogelijkheid moet [!UICONTROL JSON] gebruiken > [!UICONTROL Parse JSON] module (zie [ modules JSON ](../../workfront-fusion/apps-and-their-modules/json-modules.md)), die wordt gevormd om naar keuze een fout (BundleValidationError in dit geval) te werpen:

Vervolgens kunt u een van de foutafhandelingsinstructies aan de foutafhandelingsroute koppelen:

* Dwing de uitvoering van het scenario om de terugdraaifase te stoppen en uit te voeren: [!UICONTROL Rollback]
* Dwing de uitvoering van het scenario om de vastlegfase te stoppen en uit te voeren: [!UICONTROL Commit]
* Stop de verwerking van een route: [!UICONTROL Ignore]
* Stop de verwerking van een route en bewaar het in de rij van onvolledige uitvoeringenomslag: [!UICONTROL Break]

In het volgende voorbeeld wordt het gebruik van de instructie [!DNL Rollback] getoond:

![](assets/rollback-directive-350x175.png)
