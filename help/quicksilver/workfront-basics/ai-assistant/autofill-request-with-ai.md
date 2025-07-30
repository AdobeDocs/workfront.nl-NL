---
title: Een aanvraag automatisch invullen met AI
content-type: reference
description: U kunt AI gebruiken om aanvraagvelden automatisch in te vullen.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: d890d467dfdade676a5c93f061a5cbeda53556b6
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Een aanvraag automatisch invullen met AI

>[!NOTE]
>
>Deze functionaliteit maakt momenteel deel uit van een gesloten bètaversie. Neem contact op met `sargism@adobe.com` als u deze functionaliteit wilt inschakelen.
>
>Uw organisatie moet voldoen aan de vereisten voor het gebruik van de Workfront AI Assistant om in aanmerking te komen voor de gesloten bètaversie. Voor details, zie [ Vereisten aan AI Medewerker ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

Met AI kunt u aanvraagvelden automatisch invullen. U kunt veldwaarden voorstellen op basis van eerdere aanvragen of deze parseren uit tekst zoals e-mails, die is geüpload naar documenten.

U kunt deze suggesties goedkeuren of verwerpen alvorens het verzoek in te dienen.

Met Automatisch vullen worden geen velden overschreven die u al hebt ingevuld.

Gebruikers ontvangen geen suggesties voor gegevens waartoe zij anders geen toegang hebben.

## Suggesties ophalen bij het invullen van het formulier

Als u het formulier automatisch invult, kunt u aangeven welke veldwaarden u wilt gebruiken. Als u waarden invoert in de aanvraagvelden, vergelijkt Workfront deze waarden met eerdere aanvragen. Als de ingevoerde waarde in eerdere verzoeken in een vergelijkbare context nauw samenvalt met andere veldwaarden, stelt Workfront deze waarden voor.

Als een kliniek bijvoorbeeld altijd dezelfde factureringscode gebruikt, suggereert Workfront dat factureringscode in het juiste veld wordt gebruikt wanneer de naam van de kliniek wordt ingevoerd.

Op eerdere verzoeken gebaseerde suggesties gebruiken:

1. Maak een aanvraag.

   Voor instructies, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

1. Velden invullen.

   Terwijl u velden invult, kunnen in andere velden suggesties worden weergegeven.

1. Voor elke gebiedssuggestie, keur **** goed of **verwerp** onder dat gebied.

   of

   Selecteer **goedkeuren allen** of **verwerping allen** bij de bovenkant van de pagina om alle suggesties goed te keuren of te verwerpen.

## Suggesties ophalen van een tekstprompt

Met Automatisch vullen kunt u veldwaarden voorstellen op basis van tekst, zoals e-mails. U plakt in een tekstblok en Workfront verwerkt de tekst om veldwaarden voor te stellen op basis van de tekst.

Als het e-mailbericht bijvoorbeeld &#39;Dit moet gebeuren op 1 juni&#39; bevat en het aanvraagformulier een veld voor de vervaldatum bevat, stelt Workfront voor de veldwaarde op 1 juni in te voeren.

Dit soort voorstellen controleert ook eerdere verzoeken om vergelijkbare contexten. Als de vraag bijvoorbeeld vermeldt dat de aanvraag voor een bepaalde client is, kan Workfront het factureringsadres voor die client automatisch zoeken en invoeren op basis van eerdere aanvragen.

U kunt tekst plakken die op het volledige formulier of op één sectie van het formulier moet worden toegepast.

Suggesties gebruiken op basis van een geplakte tekstprompt:

1. Maak een aanvraag.

   Voor instructies, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

1. Om de tekstherinnering op de volledige vorm toe te passen, klik het AI pictogram ![ AI pictogram ](assets/request-prompt-icon.png) onder de vormnaam.

   of

   Om de tekstherinnering voor één enkele sectie toe te passen, klik het AI pictogram ![ AI pictogram ](assets/request-prompt-icon.png) naast de sectienaam.

1. Plak de tekst in het snelle vak.
1. Klik **Vul de vorm**.

   Workfront genereert suggesties voor het formulier.
1. Voor elke gebiedssuggestie, keur **** goed of **verwerp** onder dat gebied.

   of

   Selecteer **goedkeuren allen** of **verwerping allen** bij de bovenkant van de pagina om alle suggesties goed te keuren of te verwerpen.

## Suggesties ophalen op basis van een document dat u uploadt

Automatisch vullen kan veldwaarden voorstellen op basis van een document dat u uploadt.

Dit soort voorstellen controleert ook eerdere verzoeken om vergelijkbare contexten. Als de vraag bijvoorbeeld vermeldt dat de aanvraag voor een bepaalde client is, kan Workfront het factureringsadres voor die client automatisch zoeken en invoeren op basis van eerdere aanvragen.

### Handleidingen voor het uploaden van documenten

#### Ondersteunde bestandstypen

De volgende bestandstypen worden ondersteund:

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### Ondersteunde bestandsgrootte

Elk bestand kan maximaal 100 MB groot zijn

#### Aantal bestanden

U kunt maximaal 50 bestanden (pagina&#39;s, dia&#39;s of bladen) uploaden.

>[!IMPORTANT]
>
>Documenten worden omgezet in een reeks afbeeldingen, die elk als een afzonderlijk bestand worden beschouwd.
>
>U kunt bijvoorbeeld één PowerPoint met 50 dia&#39;s of vijf Word-documenten uploaden die elk 10 pagina&#39;s bevatten.

#### Andere beste praktijken

Houd rekening met het volgende wanneer u een document uploadt voor automatisch invullen van aanvragen:

* Automatisch vullen is momenteel geoptimaliseerd voor het Latijnse alfabet.
* We raden u aan een tekstgrootte van 8 punten of groter te gebruiken.
* Automatisch vullen kan problemen opleveren met afbeeldingen in het document, zoals geroteerde of vervormde afbeeldingen, grafieken en het tellen of gebruiken van ruimtelijke redenen voor objecten in afbeeldingen.
* Zoals altijd adviseren wij controleresultaten voor nauwkeurigheid alvorens het verzoek voor te leggen.

### Een document uploaden om een aanvraag automatisch in te vullen

U kunt een document uploaden dat op het volledige formulier of op één sectie van het formulier moet worden toegepast.

1. Maak een aanvraag.

   Voor instructies, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

1. Om het document op de volledige vorm toe te passen, klik het AI pictogram ![ AI pictogram ](assets/request-prompt-icon.png) onder de vormnaam.

   of

   Om het document voor één enkele sectie toe te passen, klik het AI pictogram ![ AI pictogram ](assets/request-prompt-icon.png) naast de sectienaam.

1. Klik **uploadt dossiers**, dan selecteer het dossier van uw dossiermanager.

   of

   Sleep het document van uw dossiermanager aan **uploadt dossiers aan auto-vult verzoekvorm** doos.
1. Klik **Vul de vorm** van **Vul de sectie**.

   Workfront genereert suggesties voor het formulier.
1. Voor elke gebiedssuggestie, keur **** goed of **verwerp** onder dat gebied.

   of

   Selecteer **goedkeuren allen** of **verwerping allen** bij de bovenkant van de pagina om alle suggesties goed te keuren of te verwerpen.

## Problemen oplossen

Als u niet de verwachte suggesties krijgt, kan het toe te schrijven zijn aan één van het volgende:

* U moet ten minste één maand aanvraaggegevens in het systeem hebben voordat u veldwaarden van eerdere aanvragen kunt voorstellen.
* Een punt van verzoekgegevens moet meer dan 24 uren in het systeem geweest zijn alvorens het in een ander verzoek kan worden voorgesteld.
* Mogelijk hebt u de instructies voor het uploaden van documenten niet opgevolgd bij het uploaden van een document om suggesties van te trekken. Voor meer informatie, zie [ Document uploadt gidsen ](#document-upload-guardrails) in dit artikel.

