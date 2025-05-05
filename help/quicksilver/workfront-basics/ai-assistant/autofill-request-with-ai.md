---
title: Een aanvraag automatisch invullen met AI
content-type: reference
description: U kunt AI gebruiken om aanvraagvelden automatisch in te vullen.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Een aanvraag automatisch invullen met AI

Met AI kunt u aanvraagvelden automatisch invullen. U kunt veldwaarden voorstellen op basis van eerdere aanvragen of deze parseren op basis van tekst zoals e-mails.

U kunt deze verzendingen goedkeuren of afwijzen voordat u het verzoek indient.

Met Automatisch vullen worden geen velden overschreven die u al hebt ingevuld.

## Suggesties ophalen bij het invullen van het formulier

Als u het formulier automatisch invult, kunt u aangeven welke veldwaarden u wilt gebruiken. Als u waarden invoert in de aanvraagvelden, vergelijkt Workfront deze waarden met eerdere aanvragen. Als de ingevoerde waarde in eerdere verzoeken in een vergelijkbare context nauw samenvalt met andere veldwaarden, stelt Workfront deze waarden voor.

Als een kliniek bijvoorbeeld altijd dezelfde factureringscode gebruikt, suggereert Workfront dat factureringscode in het juiste veld wordt gebruikt wanneer de naam van de kliniek wordt ingevoerd.

Op eerdere verzoeken gebaseerde suggesties gebruiken:

1. Maak een aanvraag.

   Voor instructies, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

1. Velden invullen.

   Terwijl u velden invult, kunnen in andere velden suggesties worden weergegeven.

1. Voor elke gebiedssuggestie, keur **&#x200B;**&#x200B;goed of **verwerp** onder dat gebied.

   of

   Selecteer **goedkeuren allen** of **verwerping allen** bij de bovenkant van de pagina om alle suggesties goed te keuren of te verwerpen.

## Suggesties ophalen van een tekstprompt

Met Automatisch vullen kunt u veldwaarden voorstellen op basis van tekst, zoals e-mails. U plakt in een tekstblok en Workfront verwerkte de tekst om veldwaarden voor te stellen op basis van de tekst.

Als het e-mailbericht bijvoorbeeld &#39;Dit moet gebeuren op 1 juni&#39; bevat en het aanvraagformulier een veld voor de vervaldatum bevat, stelt Workfront voor de veldwaarde op 1 juni in te voeren.

Dit soort voorstellen controleert ook eerdere verzoeken om vergelijkbare contexten. Als de vraag bijvoorbeeld vermeldt dat de aanvraag voor een bepaalde client is, kan Workfront het factureringsadres voor die client automatisch zoeken en invoeren op basis van eerdere aanvragen.

U kunt tekst plakken die op het volledige formulier of op één sectie van het formulier moet worden toegepast.

Suggesties gebruiken op basis van een geplakte tekstprompt:

1. Maak een aanvraag.

   Voor instructies, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

1. Om de tekstherinnering op de volledige vorm toe te passen, klik **auto-vulling met AI** in de hoger-juiste hoek van het scherm.

   of

   Om de tekstherinnering voor één enkele sectie toe te passen, klik het AI pictogram ![ AI pictogram ](assets/request-prompt-icon.png) naast de sectienaam.

1. Plak de tekst in het snelle vak.
1. Klik **Vul de vorm**.

   Workfront genereert suggesties voor het formulier.
1. Voor elke gebiedssuggestie, keur **&#x200B;**&#x200B;goed of **verwerp** onder dat gebied.

   of

   Selecteer **goedkeuren allen** of **verwerping allen** bij de bovenkant van de pagina om alle suggesties goed te keuren of te verwerpen.

