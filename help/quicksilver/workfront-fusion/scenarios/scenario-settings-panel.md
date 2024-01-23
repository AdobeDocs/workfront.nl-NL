---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Het deelvenster met scenario-instellingen in Adobe Workfront Fusion
description: In dit artikel worden de instellingen beschreven die beschikbaar zijn in het dialoogvenster [!UICONTROL scenario settings] in uw [!DNL Adobe Workfront Fusion] scenario's.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 4d9832d0870c3fccf847c3932ad4f985a62b9672
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 0%

---

# Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]

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
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## De scenario-instellingen openen

1. Open de scenario-editor, zoals wordt uitgelegd in [De scenario-editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Klik op het tandwielpictogram links onder op de pagina.

   ![](assets/scenario-settings-350x221.png)

   In de [!UICONTROL Scenario settings] die toont, kunt u diverse geavanceerde montages voor het scenario vormen.

## [!UICONTROL Allow storing incomplete executions]

Deze optie bepaalt hoe [!DNL Adobe Workfront Fusion] gaat verder als er een fout optreedt tijdens de uitvoering van een scenario. Als deze optie is ingeschakeld, wordt het scenario gepauzeerd en verplaatst naar [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Dit geeft u de mogelijkheid om de kwestie te bevestigen en verder uit te voeren van waar het scenario werd tegengehouden. Als deze optie is uitgeschakeld, stopt de uitvoering van het scenario en wordt een terugdraaifase gestart.

## [!UICONTROL Sequential processing]

Deze optie bepaalt hoe [!DNL Workfront Fusion] gaat te werk als een fout voorkomt en de uitvoering van een scenario wordt verplaatst naar [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Als de [!UICONTROL Sequential processing] is ingeschakeld, stopt Workfront Fusion met het verwerken van de taakreeks totdat alle onvolledige uitvoeringen zijn opgelost. Als de [!UICONTROL Sequential processing] deze optie is uitgeschakeld, blijft het scenario volgens zijn planning lopen, samen met herhaalde pogingen om de onvolledige executies opnieuw uit te voeren.

>[!NOTE]
>
>De opeenvolgende verwerking kan een vertraging in de uitvoering van een scenario veroorzaken. Als er onvolledige uitvoeringen nog in de rij zijn wanneer een onmiddellijk scenario trekkers of een gepland scenario om wordt geplaatst uit te voeren, zal dat scenario na alle uitvoeringen uitvoeren alvorens het in de rij volledig is.
>
>Als het gebruiksgeval voor uw scenario&#39;s geen opeenvolgende verwerking vereist, adviseren wij onbruikbaar makend de opeenvolgende verwerkingsoptie.

Voor meer informatie bij het plannen, zie [Een scenario plannen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Gegevens zijn vertrouwelijk

Zodra een scenario is uitgevoerd, kunt u door gebrek vertoningsinformatie tonen over welke gegevens door modules in het scenario werden verwerkt. Als u deze gegevens niet wilt opslaan, schakelt u het [!UICONTROL Data is confidential] -optie.

Zie voor meer informatie over het weergeven van informatie [Uitvoeringsstroom scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Als u deze optie inschakelt, kan het moeilijk zijn fouten op te lossen die tijdens de uitvoering van een scenario kunnen optreden.

## Gegevensverlies inschakelen

Deze optie heeft te maken met het inschakelen van gegevensverlies als [!DNL Workfront Fusion] kan een bundel niet opslaan in de wachtrij van [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (bijvoorbeeld vanwege een gebrek aan vrije ruimte). Als deze optie is ingeschakeld, gaan de gegevens verloren om onderbrekingen in de uitvoering van het algemene scenario te voorkomen. Dit is nuttig voor scenario&#39;s waar de hoogste prioriteit is ononderbroken uitvoering en de inkomende onjuiste gegevens niet zo belangrijk zijn.

Buiten dat, wanneer het uitvoeren van een scenario, kan een module soms een dossier ontmoeten dat groter is dan de maximaal toegestane grootte. In dit geval: [!DNL Workfront Fusion] de opbrengsten overeenkomstig de vaststelling van de [!UICONTROL Enable data loss] en er wordt een waarschuwingsbericht weergegeven.

Zie voor meer informatie over de maximale bestandsgrootte [Bestanden toewijzen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Zie voor meer informatie over waarschuwingen [Fout bij verwerken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Auto commit]

De [!UICONTROL Auto commit] de montages zijn op transacties van toepassing en bepalen de manier om een scenario te verwerken. Als Auto begaan optie is, begint de commit fase op elke module onmiddellijk na de voltooiing van de verrichtingsfase. Als de optie Automatisch vastleggen is uitgeschakeld, wordt pas een bewerking uitgevoerd als alle modules worden uitgevoerd (dit is de standaardmodus).

Zie voor meer informatie over transacties [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximumaantal cycli

Het plaatsen van meer cycli kan nuttig zijn wanneer u verbindingsonderbreking aan een derdedienst wilt verhinderen en ervoor zorgen dat alle verslagen binnen de één scenario looppas worden verwerkt.

* Als het scenario met een opiniepeilingtrigger begint, bepaalt het plaatsen het maximum aantal cycli die tijdens de uitvoering van het scenario worden toegestaan.

  Zie voor meer informatie over opiniepeilingtriggers [Opiniepeilingtriggers](../../workfront-fusion/modules/module-types.md#polling) in [Typen modules](../../workfront-fusion/modules/module-types.md).

* Als het scenario met een onmiddellijke trekker begint, wordt het plaatsen genegeerd en alle hangende gebeurtenissen worden verwerkt tijdens één enkele scenariouitvoering, één gebeurtenis per één cyclus.

  Zie voor meer informatie over instant triggers [Instant triggers](../../workfront-fusion/modules/module-types.md#instant) in [Typen modules](../../workfront-fusion/modules/module-types.md).

* Als het scenario niet met een trekker (instant/polling) begint, wordt het gespecificeerde maximumaantal cycli altijd uitgevoerd.

>[!INFO]
>
>**Voorbeelden:**  [!DNL Workfront] > [!UICONTROL Watch record] zoekt naar nieuwe problemen die binnenkomen, en [!DNL Workfront] >[!UICONTROL Convert object] converteert het nieuwe verzoek in een project en wijst het het aangewezen malplaatje toe.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL more cycles] het plaatsen wordt toegepast slechts wanneer u de uitvoering van het scenario plant. Wanneer u de opdracht [!UICONTROL Run once] , wordt rekening gehouden met de cyclusinstellingen.
>
>### Max. aantal cycli is ingesteld op 1 (standaardwaarde)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>De [!UICONTROL Maximum number of returned files] in de [!UICONTROL Dropbox] >[!UICONTROL Watch files] module is ingesteld op `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Indien 100 verzoeken worden ingediend bij [!DNL Workfront]en de [!UICONTROL Limit] het veld is ingesteld op 10 en 90 bestanden worden niet verwerkt nadat één scenario is uitgevoerd. De volgende 10 dossiers worden verwerkt in de volgende geplande scenario uitvoering.
>
>### Max. aantal cycli is ingesteld op 10
>
>De [!UICONTROL Maximum number of returned files] in de [!UICONTROL Dropbox] >[!UICONTROL Watch files] module is ingesteld op `10`.
>
>Als 100 bestanden worden toegevoegd aan de map Dropbox en de map [!UICONTROL Maximum number of returned files] Deze optie is ingesteld op 10, vervolgens worden 10 bestanden verwerkt tijdens de eerste cyclus, de volgende 10 bestanden in de tweede cyclus, de volgende 10 bestanden in de derde cyclus enzovoort, totdat alle bestanden zijn verwerkt.
>
>Alle bestanden worden verwerkt binnen 1 scenario-uitvoering.
>
>U kunt de reeds in werking gestelde cycli in de details van het Scenario zien:
>
>![](assets/scenario-detail-350x207.png)
>
>Zie voor meer informatie over deze pagina [Scenario-details in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Aantal opeenvolgende fouten

Definieert het maximumaantal opeenvolgende uitvoeringspogingen voordat de uitvoering van een scenario wordt gedeactiveerd (exclusief [!UICONTROL DataError], [!UICONTROL DuplicateDataError] en [!UICONTROL ConnectionError]).

Zie voor meer informatie over fouten [Fout bij verwerken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Als een scenario met een onmiddellijke trekker begint, wordt het plaatsen genegeerd en het scenario wordt onmiddellijk gedeactiveerd zodra de eerste fout is voorgekomen.
