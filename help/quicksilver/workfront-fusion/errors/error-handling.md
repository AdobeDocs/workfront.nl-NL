---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling in  [!DNL Adobe Workfront Fusion]
description: Wanneer de fouten tijdens de uitvoering van een scenario voorkomen, is het gewoonlijk omdat de dienst wegens een mislukking niet beschikbaar is, antwoordt de dienst met onverwachte gegevens, of de bevestiging van inputgegevens ontbreekt.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Foutafhandeling in [!DNL Adobe Workfront Fusion]

Wanneer de fouten tijdens de uitvoering van een scenario voorkomen, is het gewoonlijk omdat de dienst wegens een mislukking niet beschikbaar is, antwoordt de dienst met onverwachte gegevens, of de bevestiging van inputgegevens ontbreekt.

Als een module een fout tijdens de scenariouitvoering werpt en er geen fout behandelende route in bijlage aan de module is, voert de standaardfout behandelende logica uit, zoals die in [ wordt beschreven de verwerking van de Fout in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Door een route van de foutenmanager aan een module toe te voegen, kunt u de standaardfout behandelende logica met uw vervangen. [!DNL Adobe Workfront Fusion] biedt vijf verschillende instructies die aan het einde van de fouthandlerroutes kunnen worden ingevoegd.

Voor meer informatie, zie [ Richtlijnen voor fout behandeling in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Fouthandlerroute

Om een route van de foutenmanager aan een module toe te voegen:

1. Klik met de rechtermuisknop op de module en selecteer **[!UICONTROL Add error handler]** :

   ![](assets/error-handler-route.png)

   In de module ziet u een lijst met richtlijnen en de toepassingen die in uw scenario worden gebruikt.

1. Als de module die u een foutenmanager aan toevoegde de de laatste module in uw route is, selecteer één van de instructies.

   of

   Voeg één of meerdere modules aan de route van de foutenmanager toe.

   Als u meer modules aan de route toevoegt, wordt de [!UICONTROL Ignore] richtlijn toegepast door gebrek, en, in het geval van een fout, worden de verdere modules op die route verwerkt.


>[!INFO]
>
>In dit voorbeeld geldt dat als er een fout optreedt tijdens het uitvoeren van de module [!UICONTROL Create a folder] , de aanwijzing [!UICONTROL Ignore] automatisch wordt toegepast en het scenario naar de volgende module op de fouthandlerroute wordt verplaatst.
>
>Als er echter geen fout optreedt, wordt het scenario op de normale route naar de [!UICONTROL List all files in a folder module] verplaatst.
>
>![](assets/if-there-is-no-error-350x234.png)

Merk op dat een route van de foutenmanager uit transparante cirkels bestaat, terwijl een regelmatige route uit stevige cirkels bestaat.

## Instructies voor foutafhandeling

De richtlijnen worden hieronder kort toegelicht. Voor meer informatie, zie [ Richtlijnen voor fout behandeling in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Er zijn in totaal vijf richtlijnen die in de volgende categorieën kunnen worden ondergebracht, afhankelijk van de vraag of de uitvoering van een scenario al dan niet moet worden voortgezet.

De volgende richtlijnen zorgen ervoor dat de uitvoering van een scenario wordt voortgezet:

* **[!UICONTROL Resume]**: Hiermee kunt u een vervangende uitvoer voor de module opgeven met de fout. De status van de uitvoering van het scenario is gemarkeerd als geslaagd
* **[!UICONTROL Ignore]** : negeert de fout. De status van de uitvoering van het scenario is gemarkeerd als geslaagd
* **[!UICONTROL Break]**: slaat de invoer in de wachtrij van onvolledige uitvoeringen op. De status van de uitvoering van het scenario wordt gemarkeerd als waarschuwing. Voor meer informatie, zie [ Mening en los onvolledige uitvoeringen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

Als de uitvoering van een scenario moet stoppen wanneer een fout optreedt, gebruikt u een van de volgende instructies:

* **[!UICONTROL Rollback]**: stopt de uitvoering van het scenario onmiddellijk en markeert de status als fout
* **[!UICONTROL Commit]**: stopt de uitvoering van het scenario onmiddellijk en markeert de status als geslaagd

Zie voor meer informatie over foutafhandeling:

* [Richtlijnen voor foutafhandeling in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [ Geavanceerde fout behandeling in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)