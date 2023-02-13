---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling in [!DNL Adobe Workfront Fusion]
description: Wanneer de fouten tijdens de uitvoering van een scenario voorkomen, is het gewoonlijk omdat de dienst wegens een mislukking niet beschikbaar is, antwoordt de dienst met onverwachte gegevens, of de bevestiging van inputgegevens ontbreekt.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# Foutafhandeling in [!DNL Adobe Workfront Fusion]

Wanneer de fouten tijdens de uitvoering van een scenario voorkomen, is het gewoonlijk omdat de dienst wegens een mislukking niet beschikbaar is, antwoordt de dienst met onverwachte gegevens, of de bevestiging van inputgegevens ontbreekt.

>[!NOTE]
>
>Als een module een fout tijdens de scenariouitvoering werpt en er geen fout behandelende route aan de module in bijlage is, wordt een standaardfout behandelende logica uitgevoerd zoals die in wordt beschreven [Fout bij verwerken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Door een route van de foutenmanager aan een module toe te voegen, kunt u de standaardfout behandelende logica met uw vervangen. [!DNL Adobe Workfront Fusion] biedt 5 verschillende richtlijnen aan, om het even welke die aan het eind van uw foutenmanager routes kunnen worden opgenomen. Zie voor meer informatie [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Fouthandlerroute

Om een route van de foutenmanager aan een module toe te voegen, (wij zullen het Module X roepen), klik de module met de rechtermuisknop aan en selecteer **[!UICONTROL Add error handler]**:

![](assets/error-handler-route.png)

De module bevat een lijst met richtlijnen en de toepassingen die in uw scenario worden gebruikt. Als Module X de laatste module in uw route is, moet u één van de instructies kiezen. Of u kunt verdergaan om één of meerdere modules aan uw route toe te voegen. In dit geval worden de [!UICONTROL Ignore] de richtlijn wordt door gebrek toegepast op Module X en, in het geval van een fout, worden de verdere modules op die route verwerkt.

![](assets/directives-350x426.png)

Zoals u hieronder kunt zien, als er een fout optreedt bij het uitvoeren van de opdracht [!UICONTROL Create a folder] de [!UICONTROL Ignore] De richtlijn zal automatisch worden toegepast en het scenario zal zich naar de volgende module op de route van de foutenmanager bewegen als de filter &quot;de Fout van Gegevens&quot;één of meerdere bundels terugkeert.

Als er echter geen fout optreedt, wordt het scenario verplaatst naar de [!UICONTROL List all files in a folder module] op de gewone route.

![](assets/if-there-is-no-error-350x234.png)

Om een fouthandlerroute te onderscheiden van een reguliere route, bestaat de eerste route ook uit transparante cirkels, zoals hierboven getoond.

## Instructies voor foutafhandeling

De richtlijnen worden hieronder kort toegelicht. Zie voor meer informatie [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Er zijn in totaal vijf richtlijnen die in de volgende categorieën kunnen worden onderverdeeld op basis van de vraag of de uitvoering van een scenario al dan niet moet worden voortgezet:

De volgende richtlijnen zorgen ervoor dat de uitvoering van een scenario wordt voortgezet:

* **[!UICONTROL Resume]** staat u toe om een substituut output voor de module met de fout te specificeren en de status van de scenariouitvoering duidelijk als succes is
* **[!UICONTROL Ignore]** negeert eenvoudig de fout en de status van de scenariouitvoering wordt duidelijk als succes
* **[!UICONTROL Break]** slaat de input aan de rij van onvolledige uitvoeringen op en de status van de scenario uitvoering is duidelijk als waarschuwing. Zie voor meer informatie [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Anderzijds, als een scenario uitvoering zou moeten worden tegengehouden, moet u één van de volgende richtlijnen gebruiken:

* **[!UICONTROL Rollback]** Hiermee wordt de uitvoering van het scenario onmiddellijk gestopt en wordt de status als fout gemarkeerd
* **[!UICONTROL Commit]** stopt onmiddellijk de uitvoering van het scenario en markeert de status ervan als geslaagd

## Aanvullende bronnen

* [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Geavanceerde foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (inclusief de instelling van het hierboven genoemde Dropbox-scenario)
