---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een module genereren met behulp van AI
description: U kunt een tekstherinnering ingaan om een module tot stand te brengen van HTTP die aan de herinnering wordt gevormd.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Een module genereren met behulp van AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Omdat deze functie nog in de beginfase van de ontwikkeling is, is deze alleen beschikbaar voor interne Workfront-gebruikers.

U kunt AI gebruiken om een tekstherinnering in te gaan die beschrijft wat u een module nodig hebt te doen. De fusie zal dan een module van HTTP produceren die met het correcte eindpunt van gewenste API zal verbinden.

Zoals met om het even wat die van AI wordt geproduceerd, adviseren wij dat u de geproduceerde module controleert en test om ervoor te zorgen dat het zoals bedoeld presteert.

## Momenteel ondersteunde AI-moduletoepassingen

De Fusion AI kan momenteel modules genereren die verbinding maken met de volgende toepassingen:

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobe Maestro
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

## Een module genereren

1. Voeg een module toe en selecteer **produceren met AI** van de lijst van toepassingen.

   of

   Klik met de rechtermuisknop op een leeg gebied van de scenario-editor en selecteer vervolgens **Genereren met AI** .
1. Typ een tekstprompt in het vak.

   Voor uiteinden op herinneringen, zie [ Uiteinden voor het creëren van tekstherinneringen ](#tips-for-creating-text-prompts) in dit artikel.
1. Voeg uw API-token voor de toepassing toe aan de module.
1. Controleer de module om ervoor te zorgen dat het voor de aangewezen toepassing en de actie lijkt te worden gevormd.
1. (Voorwaardelijk) als de module niet in bijlage aan uw scenario is, sleep het in plaats.

Wij adviseren testend de module om ervoor te zorgen dat de geproduceerde module zoals bedoeld presteert.

## Tips voor het maken van tekstaanwijzingen

Tekstopdrachten moeten minimaal de volgende informatie bevatten:

* De toepassing waarmee u verbinding maakt
* De handeling die u wilt uitvoeren

>[!INFO]
>
>**Voorbeelden**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Dit omvat de toepassing `Google Calendar` en de handeling `Retrieve a list of my calendars` .
>
>* `Retrieve popular songs from Spotify`
>
>   Dit omvat de toepassing `Spotify` en de handeling `Retrieve popular songs` .

Houd rekening met het volgende wanneer u tekstaanwijzingen maakt:

* Omdat elke Fusion-module één actie uitvoert, moet uw tekstprompt één specifieke actie beschrijven.
* Gebruik directe, eenvoudige taal.
* Controleer en test de module. Als het niet zoals verwacht uitvoert, verfuw herinnering en probeer opnieuw.
