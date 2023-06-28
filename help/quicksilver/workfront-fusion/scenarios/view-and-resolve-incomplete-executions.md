---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]
description: De [!UICONTROL Incomplete executions] de omslag slaat scenario-uitvoeringen op die niet met succes wegens een fout werden gebeëindigd. Elke opgeslagen onvolledige uitvoering kan handmatig of automatisch worden opgelost.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]

De [!UICONTROL Incomplete executions] de omslag slaat scenario-uitvoeringen op die niet met succes wegens een fout werden gebeëindigd. Elke opgeslagen onvolledige uitvoering kan handmatig of automatisch worden opgelost.

>[!NOTE]
>
>Standaard is het opslaan van onvolledige uitvoeringen uitgeschakeld. Om het toe te laten, laat toe [!UICONTROL Allow storing incomplete executions] in de scenario-geavanceerde instellingen.
>
>Voor meer informatie over scenario montages, zie [Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## Onvolledige uitvoeringen weergeven

Als een module een fout tijdens zijn verrichting ontmoet, wordt een nieuwe onvolledige uitvoering toegevoegd aan de Onvolledige uitvoeringenomslag. Elke onvolledige uitvoering bevat de blauwdruk van het scenario en alle bundels die in de ontbroken module kunnen worden in kaart gebracht. De lijst met onvolledige uitvoeringen kan worden geopend door op de knop [!UICONTROL Incomplete Executions] tabblad op de pagina met scenario-details:

![](assets/incomplete-executions-tab-350x102.png)

Zie voor meer informatie [Fouten die tot onvolledige uitvoering leiden](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>De huidige groottelimiet van de onopgeloste onvolledige uitvoeringenomslag per organisatie is 500 MB. Als uw organisatie deze limiet overschrijdt, kan de volgende fout optreden:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Zie voor meer informatie [Gegevensverlies inschakelen](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Onvolledige uitvoeringen oplossen

Wanneer een nieuwe onvolledige uitvoering wordt opgeslagen, kunt u deze als volgt oplossen:

1. Klik op de knop **[!UICONTROL Incomplete Executions]** tab.
1. Zoek de onvolledige uitvoering die u wilt oplossen en klik op **[!UICONTROL Detail]**.


   Als u het logboek van alle verrichtingen van de module wilt zien alvorens u probeert om de onvolledige uitvoering op te lossen, kunt u de onvolledige uitvoering van oplossen [!UICONTROL History] map:

1. Klik op de knop **[!UICONTROL History]** tab.
1. Zoek het mislukte uitvoeringslogboek van het scenario en klik **[!UICONTROL Details]**.
1. Open het logboek van de module waar alle verrichtingen van de module worden getoond.
1. Zoek de mislukte bewerking en klik op **[!UICONTROL Resolve]**:

   ![](assets/resolve-btn-350x188.png)

## Opties in verband met onvolledige uitvoeringen

De volgende opties in het dialoogvenster [!UICONTROL Scenario settings] bepaalt of en hoe de onvolledige uitvoeringen worden opgeslagen:

* Onvolledige uitvoeringen opslaan toestaan
* Opeenvolgende verwerking
* Gegevensverlies inschakelen

Voor meer informatie over deze opties raadpleegt u [Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Fouten die tot onvolledige uitvoering leiden

Er zijn verschillende soorten fouten die leiden tot het opslaan van onvolledige uitvoeringen. Deze kunnen omvatten:

* Validatiefouten die het gevolg zijn van onvolledige of onjuiste gegevens, voornamelijk als gevolg van een ontbrekend item dat wordt verwacht om alle gegevens in een module te kunnen verwerken.
* Fouten die optreden als gevolg van de onbeschikbaarheid van de eindbestemming als gevolg van een tijdelijke of langdurige verbindingsfout (bijvoorbeeld tijdens verbinding met e-mail of externe FTP-server).

Als een fout op de eerste module in het scenario voorkomt, houdt de uitvoering onmiddellijk tegen en geen onvolledige uitvoering wordt opgeslagen.

Als een fout op een andere module voorkomt en er geen foutenmanagerroute in bijlage is, komt één van het volgende voor:

* Als het fouttype `ConnectionError`, `RateLimitError`, `OutOfSpaceError` of `ModuleTimeoutError`, wordt een onvolledige uitvoeringsrecord met automatisch opnieuw proberen opgeslagen.
* Als het fouttype `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, of `MaxResultsExceededError`, wordt een onvolledige uitvoeringsrecord opgeslagen zonder dat het opnieuw wordt uitgevoerd.
* Als het fouttype iets anders is dan hierboven, mislukt de uitvoering.
