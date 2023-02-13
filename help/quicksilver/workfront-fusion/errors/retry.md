---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling opnieuw uitvoeren in [!DNL Adobe Workfront Fusion]
description: In sommige gevallen is het nuttig om een falende module voor een paar keer opnieuw uit te voeren als er een kans is dat de reden voor de mislukking over tijd zou kunnen overgaan.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Foutafhandeling opnieuw uitvoeren in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Het probleem van de [!UICONTROL Retry] foutafhandelingsinstructie

[!UICONTROL Adobe Workfront Fusion] biedt momenteel geen [!UICONTROL Retry] foutafhandelingsinstructie, hoewel twee tijdelijke oplossingen kunnen worden gebruikt om de functionaliteit ervan na te bootsen. Zie voor meer informatie [Richtlijnen voor foutafhandeling in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Gebruik de [!UICONTROL Break] richtlijn

1. In het deelvenster met scenario-instellingen schakelt u de optie **[!UICONTROL Allow storing of Incomplete Executions]** optie.

   Zie voor meer informatie [Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Koppel een route van de foutenmanager aan de module, zoals die in wordt beschreven [Foutafhandeling in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. De koppeling [!UICONTROL Break] de richtlijn aan de route van de foutenmanager en vormt het.

   Zie voor meer informatie [Richtlijnen voor foutafhandeling in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Nadelen

* Het minimale interval voor opnieuw proberen is één minuut.
* Als de module meerdere bundels verwerkt en de verwerking van een bundel mislukt, wordt de gedeeltelijke uitvoering (alleen de bundel die de fout heeft veroorzaakt) verplaatst naar de onvolledige map voor uitvoeringen en wordt deze gepland voor nieuwe pogingen volgens de [!UICONTROL Break] compilerinstellingen. Nochtans, gaat de huidige uitvoering verder en de module blijft de verdere bundels verwerken. U kunt de optie &quot;[!UICONTROL Sequential processing]&quot; in de [!UICONTROL Scenario settings] om te voorkomen dat het scenario opnieuw wordt uitgevoerd totdat de uitvoering in de map Onvolledige uitvoeringen is opgelost.

Voor meer informatie over onvolledige uitvoeringen raadpleegt u [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Gebruik de [!UICONTROL Repeater] module

1. De **[!UICONTROL Repeater]** en stelt de [!UICONTROL Repeats] tot het maximumaantal pogingen.
1. Koppel de potentieel ontbrekende module aan de **[!UICONTROL Repeater]** module.
1. Koppel een route van de foutenmanager aan deze module (zie [Foutafhandeling in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. De koppeling **[!UICONTROL Tools]>[!UICONTROL Sleep]** module aan de route van de foutenmanager en reeks zijn **[!UICONTROL Delay]** tot het aantal seconden tussen de pogingen.

1. De koppeling **[!UICONTROL Ignore]** richtlijn na de **[!UICONTROL Tools]>[!UICONTROL Sleep]** module (zie [Richtlijnen voor foutafhandeling in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. De koppeling **[!UICONTROL Tools]>[!UICONTROL Set variable]** module na de potentieel falende module en vorm het om het resultaat van de module in een genoemde variabele op te slaan, bijvoorbeeld, `Result`.

1. De koppeling **[!UICONTROL Array aggregator]** module na de **[!UICONTROL Tools]>[!UICONTROL Set variable]** en kiest u **[!DNL Repeater]** in zijn Bronmodulegebied.

1. De koppeling **[!UICONTROL Tools]>[!UICONTROL Get variable]** aan de **[!UICONTROL Array aggregator]** en vormt het om de waarde van te verkrijgen `Result` variabele.

1. Voeg de **[!UICONTROL Tools]>[!UICONTROL Get variable]** tussen de **[!UICONTROL Repeater]** en de potentieel het ontbreken module en vormen het verkrijgen van de waarde van `Result` variabele.

1. Een filter invoegen tussen deze **[!UICONTROL Tools]>[!UICONTROL Get variable]** en de potentieel ontbrekende module om slechts verder te gaan als `Result` variabele bestaat niet.

>[!INFO]
>
>**Voorbeeld:** Hier volgt een voorbeeldscenario waarin [!UICONTROL HTTP] >[!UICONTROL Make a request] de module vertegenwoordigt de potentieel ontbrekende module:
>
>![](assets/http-make-request-350x116.png)
>
>Als het resultaat van de potentieel falende module te complex is om in een eenvoudige variabele worden opgeslagen, kunt u een gegevensopslag gebruiken om het resultaat op te slaan/terug te winnen. De gegevensopslag zou slechts één record bevatten. De sleutel van de record kan bijvoorbeeld `Result`.
>
>Voor meer informatie over gegevensopslag, zie [Gegevensopslag in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Terugspoelen

Deze oplossing lijkt misschien iets te complex en is ook wat betreft bewerkingen veeleisender.
