---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Het deelvenster met scenario-instellingen in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 0%

---

# Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ vorm scenario montages ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/configure-scenario-settings.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

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

## De scenario-instellingen openen

1. Open de scenario redacteur, zoals die in [ wordt verklaard de scenarioredacteur in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Klik op het tandwielpictogram links onder op de pagina.

   ![](assets/scenario-settings-350x221.png)

   In het deelvenster [!UICONTROL Scenario settings] dat wordt weergegeven, kunt u verschillende geavanceerde instellingen voor het scenario configureren.

## [!UICONTROL Allow storing incomplete executions]

Deze optie bepaalt hoe [!DNL Adobe Workfront Fusion] te werk gaat als er een fout optreedt tijdens de uitvoering van een scenario. Met deze toegelaten optie, wordt het scenario gepauzeerd en verplaatst naar [ Mening en lost onvolledige uitvoeringen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op. Dit geeft u de mogelijkheid om de kwestie te bevestigen en verder uit te voeren van waar het scenario werd tegengehouden. Als deze optie is uitgeschakeld, stopt de uitvoering van het scenario en wordt een terugdraaifase gestart.

## [!UICONTROL Sequential processing]

Deze optie dwingt alle executies om in orde te gebeuren, en is hoofdzakelijk relevant voor Webhooks en voor Onvolledige Uitvoeringen.

Wanneer de opeenvolgende verwerking wordt toegelaten, zijn de parallelle uitvoeringen van het scenario gehandicapt.

### Instant Webhooks

Als een webhaaktrigger is geconfigureerd als `instant` en &#39;Opeenvolgende verwerking&#39; is ingeschakeld, worden alle instant webhaakpayloads in de wachtrij geplaatst en verwerkt in de volgorde waarin ze aankomen. Dit kan handig zijn wanneer gebeurtenissen van externe systemen in een exacte volgorde worden verwerkt.

>[!NOTE]
>
>Er zullen automatische verwerkingstermijnen zijn aangezien elke lading wordt verwerkt alvorens volgende is begonnen.

### Onvolledige uitvoeringen

Als &quot;Onvolledige Uitvoeringen&quot;ook wordt toegelaten, als een fout tijdens de uitvoering van een scenario voorkomt, wordt het scenario gepauzeerd. Een van de volgende gebeurtenissen vindt dan plaats:

* Als de Opeenvolgende verwerkingsoptie **** wordt toegelaten, houdt de Fusie van Workfront op verwerkend de reeds bestaande opeenvolging tot alle onvolledige uitvoeringen worden opgelost.
* Als de Opeenvolgende verwerkingsoptie **** gehandicapt is, blijft het scenario volgens zijn programma lopen, vergezeld van herhaalde pogingen om de onvolledige uitvoeringen opnieuw uit te voeren.

Voor meer informatie over onvolledige uitvoeringen, zie [ Mening en los onvolledige uitvoeringen in de Fusie van Adobe Workfront ](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>De opeenvolgende verwerking kan een vertraging in de uitvoering van een scenario veroorzaken. Als er onvolledige uitvoeringen nog in de rij zijn wanneer een onmiddellijk scenario trekkers of een gepland scenario om wordt geplaatst uit te voeren, zal dat scenario na alle uitvoeringen uitvoeren alvorens het in de rij volledig is.
>
>Als het gebruiksgeval voor uw scenario&#39;s geen opeenvolgende verwerking vereist, adviseren wij onbruikbaar makend de opeenvolgende verwerkingsoptie.

Voor meer informatie bij het plannen, zie [ Plan een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Gegevens zijn vertrouwelijk

Zodra een scenario is uitgevoerd, kunt u door gebrek vertoningsinformatie tonen over welke gegevens door modules in het scenario werden verwerkt. Schakel de optie [!UICONTROL Data is confidential] in als u niet wilt dat deze gegevens worden opgeslagen.

Voor meer informatie over het tonen van informatie, zie [ de uitvoeringsstroom van het Scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Als u deze optie inschakelt, kan het moeilijk zijn fouten op te lossen die tijdens de uitvoering van een scenario kunnen optreden.

## Gegevensverlies inschakelen

Deze optie moet met het toelaten van gegevensverlies doen als [!DNL Workfront Fusion] er niet in slaagt om een bundel aan de rij van [ Mening te bewaren en onvolledige uitvoeringen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op te lossen (bijvoorbeeld, wegens een gebrek aan vrije ruimte). Als deze optie is ingeschakeld, gaan de gegevens verloren om onderbrekingen in de uitvoering van het algemene scenario te voorkomen. Dit is nuttig voor scenario&#39;s waar de hoogste prioriteit is ononderbroken uitvoering en de inkomende onjuiste gegevens niet zo belangrijk zijn.

Buiten dat, wanneer het uitvoeren van een scenario, kan een module soms een dossier ontmoeten dat groter is dan de maximaal toegestane grootte. In dit geval gaat [!DNL Workfront Fusion] verder volgens de instelling van de optie [!UICONTROL Enable data loss] en wordt een waarschuwingsbericht weergegeven.

Voor meer informatie over maximumdossiergrootte, zie [ Ongeveer toewijzingsdossiers in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Voor meer informatie over waarschuwingen, zie [ de verwerking van de Fout in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Auto commit]

De instellingen [!UICONTROL Auto commit] zijn van toepassing op transacties en definiëren de manier waarop een scenario moet worden verwerkt. Als Auto begaan optie is, begint de commit fase op elke module onmiddellijk na de voltooiing van de verrichtingsfase. Als de optie Automatisch vastleggen is uitgeschakeld, wordt pas een bewerking uitgevoerd als alle modules worden uitgevoerd (dit is de standaardmodus).

Voor meer informatie over transacties, zie [ uitvoering Scenario, cycli, en fasen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximumaantal cycli

Het plaatsen van meer cycli kan nuttig zijn wanneer u verbindingsonderbreking aan een derdedienst wilt verhinderen en ervoor zorgen dat alle verslagen binnen de één scenario looppas worden verwerkt.

* Als het scenario met een opiniepeilingtrigger begint, bepaalt het plaatsen het maximum aantal cycli die tijdens de uitvoering van het scenario worden toegestaan.

  Voor meer informatie over opiniepeilingstrekkers, zie [ Opiniepeilende trekkers ](../../workfront-fusion/modules/module-types.md#polling) in [ Types van modules ](../../workfront-fusion/modules/module-types.md).

* Als het scenario met een onmiddellijke trekker begint, wordt het plaatsen genegeerd en alle hangende gebeurtenissen worden verwerkt tijdens één enkele scenariouitvoering, één gebeurtenis per één cyclus.

  Voor meer informatie over onmiddellijke trekkers, zie [ Onmiddellijke trekkers ](../../workfront-fusion/modules/module-types.md#instant) in [ Types van modules ](../../workfront-fusion/modules/module-types.md).

* Als het scenario niet met een trekker (instant/polling) begint, wordt het gespecificeerde maximumaantal cycli altijd uitgevoerd.

>[!INFO]
>
>**Voorbeelden:** [!DNL Workfront] > [!UICONTROL Watch record] horloges voor nieuwe kwesties die binnen komen, en [!DNL Workfront] > [!UICONTROL Convert object] zet het nieuwe verzoek in een project om en wijst het het aangewezen malplaatje toe.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>Een instelling [!UICONTROL more cycles] wordt alleen toegepast wanneer u de uitvoering van het scenario plant. Wanneer u de knop [!UICONTROL Run once] gebruikt, wordt rekening gehouden met de cyclusinstellingen.
>
>### Max. aantal cycli is ingesteld op 1 (standaardwaarde)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>[!UICONTROL Maximum number of returned files] in de [!UICONTROL Workfront] > [!UICONTROL Watch records] module wordt geplaatst aan `10`.
>Als 100 aanvragen worden verzonden naar [!DNL Workfront] en het veld [!UICONTROL Limit] is ingesteld op 10, worden 90 bestanden niet verwerkt nadat één scenario is uitgevoerd. De volgende 10 dossiers worden verwerkt in de volgende geplande scenario uitvoering.
>
>### Max. aantal cycli is ingesteld op 10
>
>[!UICONTROL Maximum number of returned files] in de [!UICONTROL Dropbox] > [!UICONTROL Watch files] module wordt geplaatst aan `10`.
>
>Als 100 bestanden worden toegevoegd aan de map Dropbox en de optie [!UICONTROL Maximum number of returned files] is ingesteld op 10, worden 10 bestanden verwerkt tijdens de eerste cyclus, de volgende 10 bestanden in de tweede cyclus, de volgende 10 bestanden in de derde cyclus enzovoort, totdat alle bestanden zijn verwerkt.
>
>Alle bestanden worden verwerkt binnen 1 scenario-uitvoering.
>
>U kunt de reeds in werking gestelde cycli in de details van het Scenario zien:
>
>![](assets/scenario-detail-350x207.png)
>
>Voor meer informatie over deze pagina, zie [ details van het Scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Aantal opeenvolgende fouten

Definieert het maximum aantal opeenvolgende uitvoeringspogingen voordat de uitvoering van een scenario wordt gedeactiveerd (exclusief [!UICONTROL DataError] , [!UICONTROL DuplicateDataError] en [!UICONTROL ConnectionError] ).

Voor meer informatie over fouten, zie [ de verwerking van de Fout in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Als een scenario met een onmiddellijke trekker begint, wordt het plaatsen genegeerd en het scenario wordt onmiddellijk gedeactiveerd zodra de eerste fout is voorgekomen.
