---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fout bij verwerken in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Fout bij verwerken in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ types van Fout ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/error-processing.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Soms kan een fout tijdens de uitvoering van een scenario voorkomen. Dit gebeurt gewoonlijk als een service niet beschikbaar is omdat er geen verbinding is met een service of als een validatie mislukt. In dit artikel worden de algemene fouten besproken die u kunt tegenkomen.

[!DNL Adobe Workfront Fusion] maakt onderscheid tussen verschillende basistypen fouten. Het zal verschillend afhankelijk van het type van fout reageren die voorkwam.

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

## Verbindingsfout

`ConnectionError`

De fout van de verbinding is één van de gemeenschappelijkste fouten gewoonlijk die door onbeschikbaarheid van de derdedienst om diverse redenen (overladend, onderhoud, stroomonderbreking, etc.) worden veroorzaakt. De standaardbehandeling van deze fout hangt van welke module het werd ontmoet op:

* Als de fout op de eerste module voorkomt, wordt de uitvoering van het scenario geëindigd met een waarschuwingsbericht. [!DNL Workfront Fusion] probeert vervolgens herhaaldelijk het scenario opnieuw uit te voeren met steeds langere tijdsintervallen (deze worden hieronder uitgelegd). Als alle pogingen mislukken, deactiveert [!DNL Workfront Fusion] het scenario.
* Als de verbindingsfout op een andere module dan eerste voorkomt, hangen de verdere stappen van [ het opslaan van onvolledige uitvoeringen ](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) optie in de scenario geavanceerde montages af:

   * Als deze optie is ingeschakeld, wordt de uitvoering van het scenario verplaatst naar de map [!UICONTROL Incomplete executions] waar [!DNL Workfront Fusion] herhaaldelijk probeert het scenario met toenemende tijdsintervallen opnieuw uit te voeren. Als alle pogingen mislukken, blijft de uitvoering in de map Onvolledige uitvoeringen staan, in afwachting van handmatige oplossing door de gebruiker.

     Voor meer informatie over onvolledige uitvoeringen, zie [ Mening en los onvolledige uitvoeringen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.
   * Als deze optie is uitgeschakeld, eindigt de uitvoering van het scenario met een fout gevolgd door een terugdraaifase. [!DNL Workfront Fusion] probeert vervolgens herhaaldelijk het scenario opnieuw uit te voeren met toenemende tijdsintervallen. Als alle pogingen mislukken, deactiveert [!DNL Workfront Fusion] het scenario.

### Tijdintervallen vergroten

Het algoritme van vermenigvuldigings stijgende tijdintervallen tussen pogingen wanneer een fout voorkomt is genoemd exponentiële backoff. De steeds langere tijdsintervallen worden als volgt ingesteld:

1. 10 minuten
1. 1 uur
1. 3 uur
1. 12 uur
1. 24 uur

De belangrijkste reden om de steeds langere tijdsintervallen in [!DNL Workfront Fusion] toe te passen, is om te voorkomen dat veelgebruikte scenario&#39;s bewerkingen verbruiken bij herhaaldelijk mislukken pogingen.

>[!INFO]
>
>**Voorbeeld:**
>
>Een scenario bevat de [!DNL Google Sheets] trigger [!UICONTROL Watch Rows] . [!DNL Google Sheets] is 30 minuten niet beschikbaar vanwege onderhoud wanneer [!DNL Workfront Fusion] het scenario start, zodat het geen nieuwe rijen kan ophalen. Het scenario stopt en probeert het over 10 minuten opnieuw. Omdat [!DNL Google Sheets] nog steeds niet beschikbaar is, kan [!DNL Workfront Fusion] nog steeds geen informatie over nieuwe rijen ophalen. De volgende looppas van het scenario is gepland in 1 uur. [!DNL Google Sheets] is op dit moment weer beschikbaar en het scenario wordt uitgevoerd.

## Gegevensfout

`DataError`

Er wordt een gegevensfout gegenereerd wanneer een item onjuist is toegewezen en de validatie die wordt uitgevoerd aan de [!DNL Workfront Fusion] zijde of aan de zijde van de service van derden die wordt gebruikt, niet doorstaat.

Als deze fout voorkomt, wordt het scenario, tot waar de module ontbrak, verplaatst naar de onvolledige uitvoeringsomslag waar u de kwestie kunt problemen oplossen. Het scenario stopt echter niet en blijft volgens het schema lopen. Als u de uitvoering van het scenario wilt stoppen wanneer er een gegevensfout optreedt, schakelt u de optie Opeenvolgende verwerking in het instellingenvenster Scenario in.

Als u de optie [!UICONTROL Allow storing incomplete executions] niet hebt ingeschakeld in de scenario-instellingen, wordt de uitvoering van het scenario beëindigd met de fout en wordt een terugdraaiactie uitgevoerd.

Voor meer informatie bij afbeelding, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Voor informatie over onvolledige uitvoeringen, zie [ Mening en los onvolledige uitvoeringen in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

Voor informatie over het scenario dat paneel plaatst, zie [ het paneel van scenario-montages in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Voor informatie over programma&#39;s, zie [ Plan een scenario in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Gegevensfout dupliceren

`DuplicateDataError`

Als [!DNL Workfront Fusion] probeert dezelfde bundel tweemaal in te voegen in een service die dubbele gegevens niet toestaat, wordt een dubbele gegevensfout gegenereerd. Als deze fout optreedt, gaat [!DNL Workfront Fusion] op dezelfde manier te werk als bij de gegevensfout.

## Fout: toegang tot token

`InvalidAccessTokenError`

Er treedt een fout met een toegangstoken op wanneer [!DNL Workfront Fusion] geen toegang heeft tot uw account die bij een service van derden is geregistreerd. Dit gebeurt gewoonlijk wanneer u toegangsrechten voor [!DNL Workfront Fusion] in het beheer van een bepaalde service intrekt, maar verwante scenario&#39;s blijven volgens schema lopen.

Als deze fout optreedt, wordt de uitvoering van een scenario onmiddellijk gestopt. De rest van het scenario dat van de module begint waar de fout voorkwam wordt verplaatst naar de onvolledige uitvoeringsomslag.

Voor informatie over onvolledige uitvoeringen, zie [ Mening en los onvolledige uitvoeringen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

## Fout tarieflimiet

`RateLimitError`

Als een door een bepaalde dienst vastgestelde grens wordt overschreden, wordt een fout van de tariefgrens geproduceerd. Als deze fout optreedt, gaat [!DNL Workfront Fusion] op dezelfde manier te werk als bij de verbindingsfout.

Voor meer informatie, zie [ Fout van de Verbinding ](#connection-error).

## Onvolledige gegevensfout

`IncompleteDataError`

Een onvolledige gegevensfout treedt alleen op bij triggers. Deze fout wordt gegenereerd als een trigger vereiste gegevens niet kan downloaden van een bepaalde service.

Als een scenario met `IncompleteDataError` eindigt, zal zijn verder gedrag van zijn het plaatsen van [!UICONTROL Max number of consecutive errors] afhangen.

Voor meer informatie, zie [ Aantal opeenvolgende fouten ](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in het artikel [ het paneel van scenario-montages in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Voorbeeld:**
>
>Voor een scenario is de [!DNL Workfront] trigger [!UICONTROL Watch Record] ingesteld op controleren voor documenten. Het scenario wordt uitgevoerd terwijl u een groot document uploadt, zoals een lange video. Aangezien [!UICONTROL Workfront Fusion] de video probeert te downloaden terwijl deze nog steeds naar Workfront wordt geüpload, wordt het scenario afgesloten met de instructie `IncompleteDataError` .

## Runtimefout

`RuntimeError`

Als er tijdens de uitvoering van het scenario een andere (niet hierboven vermelde) fout optreedt, wordt deze als een `RunTimeError` gerapporteerd.

Als een scenario met `RuntimeError` eindigt, zal zijn verder gedrag van zijn het plaatsen van [!UICONTROL Max number of consecutive errors] afhangen. Voor meer informatie, zie [ Aantal opeenvolgende fouten ](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in het artikel [ het paneel van scenario-montages in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Als een scenario begint met een onmiddellijke trigger, wordt de instelling van [!UICONTROL Max number of consecutive errors] genegeerd en wordt het scenario onmiddellijk gedeactiveerd zodra de eerste fout is opgetreden. Voor meer informatie, zie [ Onmiddellijke trekkers ](../../workfront-fusion/modules/module-types.md#instant) in het artikel [ Types van modules ](../../workfront-fusion/modules/module-types.md).

## Inconsistentiefout

`InconsistencyError`

Als er een hierboven beschreven fout optreedt tijdens de vastlegfase of terugdraaifase, wordt een scenario afgesloten met Inconsistentiefout. Voor meer informatie, zie [ uitvoering Scenario, cycli, en fasen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Als deze fout in een scenario verschijnt, wordt de uitvoering van het scenario onmiddellijk gestopt.

## Waarschuwing

Tijdens het uitvoeren van een scenario, kunt u een waarschuwing ontvangen die u over een probleem op de hoogte brengt. Dit belet echter niet dat het scenario met succes wordt voltooid.

Er kan bijvoorbeeld een waarschuwing verschijnen wanneer de maximaal toegestane bestandsgrootte wordt overschreden en de optie [!UICONTROL Enable data loss] is uitgeschakeld. Voor meer informatie, zie [ gegevensverlies ](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) toelaten in het artikel [ het paneel van de scenario-montages in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/scenario-settings-panel.md).
