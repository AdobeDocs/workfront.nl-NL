---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling opnieuw proberen in  [!DNL Adobe Workfront Fusion]
description: In sommige gevallen is het nuttig om een falende module voor een paar keer opnieuw uit te voeren als er een kans is dat de reden voor de mislukking over tijd zou kunnen overgaan.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Foutafhandeling opnieuw proberen in [!DNL Adobe Workfront Fusion]

In sommige gevallen is het nuttig om een falende module opnieuw uit te voeren als er een kans is dat de reden voor de mislukking over tijd zou kunnen overgaan.

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

## Problemen met de aanwijzing voor foutafhandeling van [!UICONTROL Retry]

[!UICONTROL Adobe Workfront Fusion] biedt momenteel geen aanwijzing voor foutafhandeling van [!UICONTROL Retry] , hoewel twee tijdelijke oplossingen kunnen worden gebruikt om de functionaliteit ervan te simuleren. Voor meer informatie, zie [ Richtlijnen voor fout behandeling in de Fusie van Adobe Workfront ](../../workfront-fusion/errors/directives-for-error-handling.md).

### De instructie [!UICONTROL Break] gebruiken

1. Schakel de optie **[!UICONTROL Allow storing of Incomplete Executions]** in het deelvenster met scenario-instellingen in.

   Voor meer informatie, zie [ het paneel van scenario montages in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Koppel een route van de foutenmanager aan de module, zoals die in [ de behandeling van de Fout in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md) wordt beschreven.
1. Koppel de instructie [!UICONTROL Break] aan de fouthandlerroute en configureer deze.

   Zie [ Richtlijnen voor foutafhandeling in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md) voor meer informatie.

   ![](assets/break-directive-350x241.png)

#### Nadelen

* Het minimale interval voor opnieuw proberen is één minuut.
* Als de module meerdere bundels verwerkt en de verwerking van een bundel mislukt, wordt de gedeeltelijke uitvoering (alleen de bundel die de fout heeft veroorzaakt) verplaatst naar de onvolledige map voor uitvoeringen en wordt deze gepland voor nieuwe pogingen volgens de instellingen van de instructie [!UICONTROL Break] . Nochtans, gaat de huidige uitvoering verder en de module blijft de verdere bundels verwerken. U kunt de optie &quot;[!UICONTROL Sequential processing]&quot; in [!UICONTROL Scenario settings] inschakelen om te voorkomen dat het scenario opnieuw wordt uitgevoerd totdat de uitvoering die in de map Onvolledige uitvoeringen is opgeslagen, is voltooid.

  Voor meer informatie over onvolledige uitvoeringen, zie [ Mening en los onvolledige uitvoeringen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

### De module [!UICONTROL Repeater] gebruiken

1. Gebruik de module **[!UICONTROL Repeater]** en stel het veld **[!UICONTROL Repeats]** ervan in op het maximumaantal pogingen.
1. Koppel de module die mogelijk mislukt aan de module **[!UICONTROL Repeater]** .
1. Verbind een route van de foutenmanager aan deze module (zie [ Fout behandeling in  [!DNL Adobe Workfront Fusio] n ](../../workfront-fusion/errors/error-handling.md)).
1. Koppel de module **[!UICONTROL Tools]>[!UICONTROL Sleep]** aan de fouthandlerroute en stel het veld **[!UICONTROL Delay]** ervan in op het aantal seconden tussen de pogingen.

1. Verbind de **[!UICONTROL Ignore]** richtlijn na de **[!UICONTROL Tools]>[!UICONTROL Sleep]** module (zie [ Richtlijnen voor foutenbehandeling in de Fusie van Adobe Workfront ](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Koppel de module **[!UICONTROL Tools]>[!UICONTROL Set variable]** na de module die mogelijk mislukt en configureer deze om het resultaat van de module op te slaan in een variabele met de naam `Result` .

1. Koppel de module **[!UICONTROL Array aggregator]** na **[!UICONTROL Tools]>[!UICONTROL Set variable]** en kies de module **[!DNL Repeater]** in het veld Source Module.

1. Koppel de module **[!UICONTROL Tools]>[!UICONTROL Get variable]** aan de module **[!UICONTROL Array aggregator]** en configureer deze om de waarde van de variabele `Result` te verkrijgen.

1. Voeg de module **[!UICONTROL Tools]>[!UICONTROL Get variable]** tussen de module **[!UICONTROL Repeater]** en de module die mogelijk niet werkt in en configureer deze om de waarde van de variabele `Result` te verkrijgen.

1. Voeg een filter in tussen deze module **[!UICONTROL Tools]>[!UICONTROL Get variable]** en de module die mogelijk niet werkt, alleen als de variabele `Result` niet bestaat.

>[!INFO]
>
>**Voorbeeld:** hier is een steekproefscenario waar de [!UICONTROL HTTP] > [!UICONTROL Make a request] module de potentieel ontbrekende module vertegenwoordigt:
>
>![](assets/http-make-request-350x116.png)
>
>Als het resultaat van de potentieel falende module te complex is om in een eenvoudige variabele worden opgeslagen, kunt u een gegevensopslag gebruiken om het resultaat op te slaan/terug te winnen. De gegevensopslag zou slechts één record bevatten. De sleutel van de record kan bijvoorbeeld `Result` zijn.
>
>Voor meer informatie over gegevensopslag, zie [ Opslag van Gegevens in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Terugspoelen

Deze tijdelijke oplossing lijkt misschien iets te complex en is ook wat betreft bewerkingen veeleisender.
