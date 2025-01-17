---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een scenario-segment genereren met behulp van AI
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Een scenario-segment genereren met behulp van AI

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ produceer een scenario segment gebruikend AI ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-module-with-ai.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Omdat deze functie in Beta beschikbaar is, is deze alleen beschikbaar voor sommige Workfront-gebruikers.

U kunt AI gebruiken om een tekstherinnering in te gaan die beschrijft wat u een sectie van uw scenario nodig hebt te doen. De fusie zal dan modules produceren die die acties zullen uitvoeren, die u in uw scenario kunt gebruiken.

Zoals met om het even wat die van AI wordt geproduceerd, adviseren wij dat u de geproduceerde modules tweemaal controleert en test om ervoor te zorgen dat zij zoals bedoeld presteren.

## Momenteel ondersteunde AI-moduletoepassingen

De Fusion AI kan momenteel modules genereren die verbinding maken met de volgende toepassingen:

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobe Workfront Planning
* Adobe Analytics
* Adobe PDF Services
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Google-agenda
* Atlassian Jira
* GitLab
* Spotiseren
* Bitmap
* OpenAI
* Slack

## Modules genereren

1. Begin toevoegend een module en selecteer **met AI** van de lijst van toepassingen produceren.

   of

   Klik produceren met AI pictogram ![ produceert met AI ](assets/generate-with-ai-icon-beta.png) dichtbij de bodem van de pagina van de scenarioredacteur.

   Het deelvenster AI-assistent wordt geopend.
1. Typ een tekstprompt in het vak.

   Voor uiteinden op herinneringen, zie [ Uiteinden voor het creëren van tekstherinneringen ](#tips-for-creating-text-prompts) in dit artikel.

   AI Assistant genereert de module of set modules.
1. (Voorwaardelijk) Voeg indien nodig uw API-token voor de toepassing toe aan de modules.
1. Controleer de modules om ervoor te zorgen dat zij voor de aangewezen toepassing en de actie worden gevormd.
1. (Voorwaardelijk) als de geproduceerde scenario sectie niet in bijlage aan uw scenario is, sleep het in plaats.

Wij adviseren het testen van de modules om ervoor te zorgen dat zij zoals bedoeld presteren.

## Tips voor het maken van tekstaanwijzingen

Tekstopdrachten moeten minimaal de volgende informatie bevatten:

* De toepassing waarmee u verbinding maakt
* De handeling of handelingen die u wilt uitvoeren

>[!IMPORTANT]
>
>U kunt meer dan één module tegelijkertijd produceren, maar kunt slechts modules voor één toepassing tezelfdertijd produceren.

>[!INFO]
>
>**Voorbeelden**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Dit omvat de toepassing `Workfront Planning` en de handeling `delete records` . Deze herinnering leidt tot drie modules, voor elk verslag dat zal worden geschrapt.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Dit omvat de toepassing `Workfront Planning` en de handeling `change campaign summary` .
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Dit omvat de toepassing `Workfront Planning` en de handeling `get field details` .
>
>Het volgende voorbeeld is NOT correct:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Dit voorbeeld is onjuist omdat het meerdere toepassingen bevat

Houd rekening met het volgende wanneer u tekstaanwijzingen maakt:

* Gebruik directe, eenvoudige taal.
* Controleer en test de modules. Als het niet zoals verwacht uitvoert, verfuw herinnering en probeer opnieuw.
