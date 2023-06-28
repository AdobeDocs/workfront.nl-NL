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

# Foutafhandeling genereren in [!DNL Adobe Workfront Fusion]

In sommige gevallen wilt u mogelijk de uitvoering van het scenario, gevolgd door [Terugdraaien](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) of [Vastleggen](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) fase of om de verwerking van een route tegen te houden en naar keuze het in de rij van onvolledige uitvoeringen op te slaan.

De foutafhandelingsrichtlijnen kunnen momenteel niet buiten het bereik van een [Fouthandlerroute](../../workfront-fusion/errors/error-handling.md#error) en [!DNL Adobe Workfront Fusion] biedt geen module aan die u zou toelaten om (werpen) fouten gemakkelijk voorwaardelijk te produceren.

Voor informatie over onvolledige uitvoeringen raadpleegt u [Onvolledige uitvoeringen weergeven en oplossen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Voor informatie over foutafhandelingsrichtlijnen raadpleegt u [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Oplossing voor Throw

Om een fout voorwaardelijk te werpen, kunt u een module vormen om het naar keuze opzettelijk tijdens zijn verrichting te maken ontbreken. Eén mogelijkheid is om de [!UICONTROL JSON] > [!UICONTROL Parse JSON] module (zie [JSON-modules](../../workfront-fusion/apps-and-their-modules/json-modules.md)), geconfigureerd om optioneel een fout te genereren (in dit geval BundleValidationError):

Vervolgens kunt u een van de foutafhandelingsinstructies aan de foutafhandelingsroute koppelen:

* Dwing de scenario-uitvoering om de terugdraaifase te stoppen en uit te voeren: [!UICONTROL Rollback]
* Dwing de scenario uitvoering om te stoppen en uit te voeren begaan fase: [!UICONTROL Commit]
* Stop de verwerking van een route: [!UICONTROL Ignore]
* Stop de verwerking van een route en sla het in de rij van onvolledige uitvoeringenomslag op: [!UICONTROL Break]

In het volgende voorbeeld wordt het gebruik van het [!DNL Rollback] richtlijn :

![](assets/rollback-directive-350x175.png)
