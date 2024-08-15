---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Onvolledige uitvoeringen weergeven en oplossen in  [!DNL Adobe Workfront Fusion]
description: In de map [!UICONTROL Incomplete executions] worden scenario-uitvoeringen opgeslagen die niet zijn voltooid vanwege een fout. Elke opgeslagen onvolledige uitvoering kan handmatig of automatisch worden opgelost.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 53582d36ef2256f6073705ce3eabe8cd61c9b2cc
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]

In de map [!UICONTROL Incomplete executions] worden scenario-uitvoeringen opgeslagen die niet zijn voltooid vanwege een fout. Elke opgeslagen onvolledige uitvoering kan handmatig of automatisch worden opgelost.

>[!NOTE]
>
>Standaard is het opslaan van onvolledige uitvoeringen uitgeschakeld. Schakel de optie [!UICONTROL Allow storing incomplete executions] in de geavanceerde instellingen van het scenario in om deze optie in te schakelen.
>
>Voor meer informatie over scenario montages, zie [ het paneel van scenario montages in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## Onvolledige uitvoeringen weergeven

Als een module een fout tijdens zijn verrichting ontmoet, wordt een nieuwe onvolledige uitvoering toegevoegd aan de Onvolledige uitvoeringenomslag. Elke onvolledige uitvoering bevat de blauwdruk van het scenario en alle bundels die in de ontbroken module kunnen worden in kaart gebracht. De lijst met onvolledige uitvoeringen kan worden geopend door te klikken op de tab [!UICONTROL Incomplete Executions] op de pagina met de details van het scenario.

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

Voor meer informatie, zie [ Fouten resulterend in onvolledige uitvoeringen ](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>De huidige groottelimiet van de onopgeloste onvolledige uitvoeringenomslag per organisatie is 500 MB. Als uw organisatie deze limiet overschrijdt, kan de volgende fout optreden:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Voor meer informatie, zie [ gegevensverlies ](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) toelaten in [ het paneel van de scenario montages in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Onvolledige uitvoeringen oplossen

Wanneer een nieuwe onvolledige uitvoering wordt opgeslagen, kunt u deze als volgt oplossen:

1. Klik op de tab **[!UICONTROL Incomplete Executions]** .
1. Zoek de onvolledige uitvoering die u wilt oplossen en klik op **[!UICONTROL Detail]** .


   Als u het logboek van alle verrichtingen van de module wilt zien alvorens u probeert om de onvolledige uitvoering op te lossen, kunt u de onvolledige uitvoering van de [!UICONTROL History] omslag oplossen:

1. Klik op de tab **[!UICONTROL History]** .
1. Zoek het mislukte uitvoeringslogboek van het scenario en klik op **[!UICONTROL Details]** .
1. Open het logboek van de module waar alle verrichtingen van de module worden getoond.
1. Zoek de mislukte bewerking en klik op **[!UICONTROL Resolve]** :

   ![](assets/resolve-btn-350x188.png)

## Opties in verband met onvolledige uitvoeringen

De volgende opties in het deelvenster [!UICONTROL Scenario settings] bepalen of en hoe de onvolledige uitvoeringen worden opgeslagen:

* Toestaan dat onvolledige uitvoeringen worden opgeslagen
* Opeenvolgende verwerking
* Gegevensverlies inschakelen

Voor meer informatie over deze opties, zie [ het paneel van scenario montages in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Fouten die tot onvolledige uitvoering leiden

Er zijn verschillende soorten fouten die leiden tot het opslaan van onvolledige uitvoeringen. Deze kunnen het volgende omvatten:

* Validatiefouten die het gevolg zijn van onvolledige of onjuiste gegevens, voornamelijk als gevolg van een ontbrekend item dat wordt verwacht om alle gegevens in een module te kunnen verwerken.
* Fouten die optreden als gevolg van de onbeschikbaarheid van de eindbestemming als gevolg van een tijdelijke of langdurige verbindingsfout (bijvoorbeeld tijdens verbinding met e-mail of externe FTP-server).

Als een fout op de eerste module in het scenario voorkomt, houdt de uitvoering onmiddellijk tegen en geen onvolledige uitvoering wordt opgeslagen.

Als een fout op een andere module voorkomt en er geen foutenmanagerroute in bijlage is, komt één van het volgende voor:

* Als het fouttype `ConnectionError` , `RateLimitError` , `OutOfSpaceError` of `ModuleTimeoutError` is, wordt een onvolledige uitvoerrecord met automatisch opnieuw proberen opgeslagen.
* Als het fouttype `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError` of `MaxResultsExceededError` is, wordt een onvolledige uitvoerrecord opgeslagen zonder deze automatisch opnieuw te proberen.
* Als het fouttype iets anders is dan hierboven, mislukt de uitvoering.
