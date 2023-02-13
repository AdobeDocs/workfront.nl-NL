---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fout bij verwerken in [!DNL Adobe Workfront Fusion]
description: Soms kan een fout tijdens de uitvoering van een scenario voorkomen. Dit gebeurt gewoonlijk als een service niet beschikbaar is omdat er geen verbinding is met een service of als een validatie mislukt. In dit artikel worden de algemene fouten besproken die u kunt tegenkomen.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Fout bij verwerken in [!DNL Adobe Workfront Fusion]

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

## Verbindingsfout

`ConnectionError`

De fout van de verbinding is één van de gemeenschappelijkste fouten gewoonlijk die door onbeschikbaarheid van de derdedienst om diverse redenen (overladend, onderhoud, stroomonderbreking, etc.) worden veroorzaakt. De standaardbehandeling van deze fout hangt van welke module het werd ontmoet op:

* Als de fout op de eerste module voorkomt, wordt de uitvoering van het scenario geëindigd met een waarschuwingsbericht. [!DNL Workfront Fusion] herhaaldelijk wordt gepoogd het scenario met steeds langere tussenpozen opnieuw uit te voeren (deze worden hieronder uitgelegd). Als alle pogingen mislukken, [!DNL Workfront Fusion] Hiermee wordt het scenario gedeactiveerd.
* Als de verbindingsfout op een andere module dan de eerste voorkomt, hangen de verdere stappen van [Onvolledige uitvoeringen opslaan toestaan](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) optie in de scenario geavanceerde montages:

   * Als deze optie is ingeschakeld, wordt de uitvoering van het scenario verplaatst naar de [!UICONTROL Incomplete executions] map waar [!DNL Workfront Fusion] herhaaldelijk wordt gepoogd om het scenario met langere tijdsintervallen opnieuw uit te voeren. Als alle pogingen mislukken, blijft de uitvoering in de [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op handmatige oplossing door de gebruiker.
   * Als de optie is uitgeschakeld, eindigt de uitvoering van het scenario met een fout gevolgd door een terugdraaifase. [!DNL Workfront Fusion] probeert dan herhaaldelijk om het scenario met stijgende tijdintervallen opnieuw uit te voeren. Als alle pogingen mislukken, [!DNL Workfront Fusion] Hiermee wordt het scenario gedeactiveerd.

### Tijdintervallen vergroten

Het algoritme van vermenigvuldigings stijgende tijdintervallen tussen pogingen wanneer een fout voorkomt is genoemd exponentiële backoff. De steeds langere tijdsintervallen worden als volgt ingesteld:

1. 10 minuten
1. 1 uur
1. 3 uur
1. 12 uur
1. 24 uur

De belangrijkste reden waarom de steeds langere tijdsintervallen in [!DNL Workfront Fusion] moet voorkomen dat vaak uitgevoerde scenario&#39;s bewerkingen verbruiken bij herhaalde mislukte pogingen.

>[!INFO]
>
>**Voorbeeld:**
>
>Een scenario bevat de [!DNL Google Sheets] trigger [!UICONTROL Watch Rows]. [!DNL Google Sheets] is 30 minuten niet beschikbaar vanwege onderhoud wanneer [!DNL Workfront Fusion] start het scenario, zodat het geen nieuwe rijen kan terugwinnen. Het scenario stopt en probeert het over 10 minuten opnieuw. Aangezien de dienst binnen dit tijdkader niet beschikbaar blijft, [!DNL Workfront Fusion] kan nog steeds geen informatie ophalen over nieuwe rijen. De volgende looppas van het scenario is gepland in 1 uur. [!DNL Google Sheets] is opnieuw beschikbaar binnen deze tijd en de scenario looppas met succes.

## Gegevensfout

`DataError`

Er wordt een gegevensfout gegenereerd wanneer een item onjuist is toegewezen en de validatie die is uitgevoerd op het tabblad [!DNL Workfront Fusion] zij of aan de zijde van de dienst van derden die wordt gebruikt. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Als deze fout voorkomt, wordt het scenario, tot waar de module ontbrak, verplaatst naar de onvolledige uitvoeringsomslag waar u de kwestie kunt problemen oplossen. Het scenario stopt echter niet en blijft volgens het schema lopen. Als u de uitvoering van het scenario wilt stoppen wanneer er een gegevensfout optreedt, schakelt u de optie Opeenvolgende verwerking in het instellingenvenster Scenario in.

Als u de optie [!UICONTROL Allow storing incomplete executions] optie in de scenario montages, eindigt de uitvoering van het scenario met de fout en het terugschroeven van prijzen wordt uitgevoerd.

Voor informatie over onvolledige uitvoeringen raadpleegt u [Onvolledige uitvoeringen weergeven en oplossen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Voor informatie over het deelvenster met scenario-instellingen raadpleegt u [Het deelvenster met scenario-instellingen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Voor informatie over programma&#39;s, zie [Een scenario plannen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Gegevensfout dupliceren

`DuplicateDataError`

Indien [!DNL Workfront Fusion] probeert om de zelfde bundel tweemaal in de dienst op te nemen die dubbele gegevens niet toestaat, wordt een dubbele gegevensfout geproduceerd. Als deze fout optreedt, [!DNL Workfront Fusion] gaat op dezelfde manier te werk als bij de gegevensfout.

## Fout: toegang tot token

`InvalidAccessTokenError`

Er is een ongeldige fout in het toegangstoken opgetreden wanneer [!DNL Workfront Fusion] heeft geen toegang tot uw account dat bij een service van derden is geregistreerd. Dit gebeurt meestal wanneer u toegangsrechten intrekt voor [!DNL Workfront Fusion] bij het beheer van een bepaalde dienst, maar de bijbehorende scenario&#39;s blijven volgens schema lopen.

Als deze fout optreedt, wordt de uitvoering van een scenario onmiddellijk gestopt. De rest van het scenario dat van de module begint waar de fout voorkwam wordt verplaatst naar de onvolledige uitvoeringsomslag.

Voor informatie over onvolledige uitvoeringen raadpleegt u [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Fout tarieflimiet

`RateLimitError`

Als een door een bepaalde dienst vastgestelde grens wordt overschreden, wordt een fout van de tariefgrens geproduceerd. Als deze fout optreedt, [!DNL Workfront Fusion] gaat op dezelfde manier te werk als bij de verbindingsfout. Zie voor meer informatie [Verbindingsfout](#connection-error).

## Onvolledige gegevensfout

`IncompleteDataError`

Een onvolledige gegevensfout treedt alleen op bij triggers. Deze fout wordt gegenereerd als een trigger vereiste gegevens niet kan downloaden van een bepaalde service.

Als een scenario met eindigt `IncompleteDataError`zijn verdere gedrag zal afhangen van zijn instelling [!UICONTROL Max number of consecutive errors]. Zie voor meer informatie [Aantal opeenvolgende fouten](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in het artikel [Het deelvenster met scenario-instellingen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Voorbeeld:** Een scenario heeft de [!DNL Workfront] trigger [!UICONTROL Watch Record] instellen op controleren voor documenten. Het scenario wordt uitgevoerd terwijl u een groot document uploadt, zoals een lange video. Omdat [!UICONTROL Workfront Fusion] probeert de video te downloaden terwijl deze nog uploadt naar Workfront, wordt het scenario beëindigd met de `IncompleteDataError`.

## Runtimefout

`RuntimeError`

Als er tijdens de uitvoering van het scenario een andere (niet hierboven vermelde) fout optreedt, wordt deze als een `RunTimeError`.

Als een scenario met eindigt `RuntimeError`zijn verdere gedrag zal afhangen van zijn instelling [!UICONTROL Max number of consecutive errors]. Zie voor meer informatie [Aantal opeenvolgende fouten](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in het artikel [Het deelvenster met scenario-instellingen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Als een scenario met een onmiddellijke trekker begint, het plaatsen van [!UICONTROL Max number of consecutive errors] wordt genegeerd en het scenario onmiddellijk wordt gedeactiveerd zodra de eerste fout is opgetreden. Zie voor meer informatie [Instant triggers](../../workfront-fusion/modules/module-types.md#instant) in het artikel [Typen modules](../../workfront-fusion/modules/module-types.md).

## Inconsistentiefout

`InconsistencyError`

Als er een hierboven beschreven fout optreedt tijdens de vastlegfase of terugdraaifase, wordt een scenario afgesloten met Inconsistentiefout. Zie voor meer informatie [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Als deze fout in een scenario verschijnt, wordt de uitvoering van het scenario onmiddellijk gestopt.

## Waarschuwing

Tijdens het uitvoeren van een scenario, kunt u een waarschuwing ontvangen die u over een probleem op de hoogte brengt. Dit belet echter niet dat het scenario met succes wordt voltooid.

Er kan bijvoorbeeld een waarschuwing verschijnen wanneer de maximaal toegestane bestandsgrootte wordt overschreden en de instelling [!UICONTROL Enable data loss] is uitgeschakeld. Zie voor meer informatie [Gegevensverlies inschakelen](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in het artikel [Het deelvenster met scenario-instellingen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
