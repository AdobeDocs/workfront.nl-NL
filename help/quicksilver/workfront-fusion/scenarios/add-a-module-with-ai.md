---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een module genereren met behulp van AI
description: U kunt een tekstherinnering ingaan om een module tot stand te brengen van HTTP die aan de herinnering wordt gevormd.
author: Becky
feature: Workfront Fusion
source-git-commit: 79b5baf5a9558e07b55fb810aa2d6c772faa51cf
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Een module genereren met behulp van AI

U kunt AI gebruiken om een tekstherinnering in te gaan die beschrijft wat u een module nodig hebt te doen. De fusie zal dan een module van HTTP produceren die met het correcte eindpunt van gewenste API zal verbinden.

Zoals met om het even wat die van AI wordt geproduceerd, adviseren wij dat u de geproduceerde module controleert en test om ervoor te zorgen dat het zoals bedoeld presteert.

## Momenteel ondersteunde AI-moduletoepassingen

De Fusion AI kan momenteel modules genereren die verbinding maken met de volgende toepassingen:

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

1. Voeg een module toe en selecteer **Genereren met AI** in de lijst met toepassingen.

   of

   Klik met de rechtermuisknop op een leeg gebied van de scenarioeditor en selecteer vervolgens **Genereren met AI**.
1. Typ een tekstprompt in het vak.

   Voor tips over aanwijzingen raadpleegt u [Tips voor het maken van tekstaanwijzingen](#tips-for-creating-text-prompts) in dit artikel.
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
>   Dit omvat de toepassing `Google Calendar` en de actie `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Dit omvat de toepassing `Spotify` en de actie `Retrieve popular songs`.

Houd rekening met het volgende wanneer u tekstaanwijzingen maakt:

* Omdat elke Fusion-module één actie uitvoert, moet uw tekstprompt één specifieke actie beschrijven.
* Gebruik directe, eenvoudige taal.
* Controleer en test de module. Als het niet zoals verwacht uitvoert, verfuw herinnering en probeer opnieuw.



