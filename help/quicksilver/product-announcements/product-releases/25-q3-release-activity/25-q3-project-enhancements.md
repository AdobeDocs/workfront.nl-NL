---
title: Verbeteringen van projecten in het derde kwartaal van 2025
description: Verbeteringen van projecten in het derde kwartaal van 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: b87b32d0396b0c277a5fc30d060c76a71192171b
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Verbeteringen van projecten in het derde kwartaal van 2025

Op deze pagina worden de projectverbeteringen beschreven die zijn aangebracht met de release van het derde kwartaal van 2025 voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving, zoals vermeld.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Derde Kwartaal 2025 versiecyclus, zie [ Derde Kwartaal 2025 releaseoverzicht ](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Het veld Bestaande werkelijke uren is vervangen door het veld Oudere werkelijke uren en het nieuwe veld Werkelijke uren is gemaakt

>[!NOTE]
>
> Voorbeeld en productie: 24 juni 2025 

Het bestaande veld Werkelijke uren is hernoemd naar Werkelijke uren verouderd. In dit veld wordt de tijd opgeslagen die is aangemeld voor projecten, taken en problemen in minuten. Het veld wordt in de Workfront-database opgeslagen als actualWorkRequired.

Wij hebben een nieuw ActualUren gebied toegevoegd dat de tijd opslaat die voor projecten, taken, en kwesties in uren, met decimale precisie wordt geregistreerd. Het veld wordt in de Workfront-database opgeslagen als actualWorkRequiredDouble.

Zowel de velden Werkuren als Werkelijke uren verouderd zijn zichtbaar in project-, taak- en probleemweergave en rapporten.

Het veld Werkelijke uren dat zichtbaar is in het project, de sectie Taken en de sectie Details van uitgaven vertegenwoordigt de verouderde werkelijke uren.


>[!IMPORTANT]
>
>Uren die vóór mei 2021 zijn geregistreerd, worden opgeslagen in het veld Oudere werkelijke uren.  
>&#x200B;>De waarde voor het gebied van Werkelijke Uren voor projecten, taken, en kwesties waar de uren vóór Mei 2021 werden geregistreerd is nul. 
>&#x200B;>De uren die na Mei 2021 worden geregistreerd worden opgeslagen op zowel het Ware gebied van Uren als het Echte gebied van Werkelijke Uren van de Oudheid.
>&#x200B;> Mogelijk moet u de rapporten bijwerken met de nieuwe velden.

Voor informatie, zie [ Ware Uren van de Mening ](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).


## Wijziging in de manier waarop Werkelijke uren worden opgeslagen in de database voor API-aanroepen

>[!NOTE]
>
>* Voorbeeld: met de volgende API-versie, gepland voor later in 2025
>* Snelle productie: met de volgende API-versie, gepland voor later in 2025
>* Productie voor alle klanten: met de volgende API-versie, gepland voor later in 2025

Deze update introduceert een verandering in de manier de Werkelijke Uren voor projecten, taken, en kwesties in het gegevensbestand worden opgeslagen. Vanaf deze update gebruiken de werkelijke uren een waardeveld van `actualWorkRequiredDouble` (met een waarde in uren).

Vóór deze update zijn de werkelijke uren opgeslagen met een waardeveld van `actualWorkRequired` (met een waarde in minuten). Deze update zorgt voor een nauwkeuriger telling van de werkelijke uren wanneer deze worden berekend met behulp van een API-aanroep.

Vanwege deze wijziging moet u mogelijk API-aanroepen bijwerken die naar het oorspronkelijke waardeveld verwijzen. Breng geen wijzigingen aan als u een waardeveld van `actualWorkRequiredExpression` gebruikt in de API-aanroepen.

Deze update verandert niet de berekeningen voor Ware Uren voor projecten, taken, en kwesties, in berekende kolommen van de douanegebieden.

## Bijwerken met de schuifregelaar Percentage voltooid in een taak- of uitgiftekop

>[!NOTE]
>
>* Voorbeeld: 27 mei 2025
>* Snelle productie: 27 mei 2025
>* Productie voor alle afnemers: 27 mei 2025

We hebben de manier bijgewerkt waarop de procentuele volledige schuifregelaar werkt voor taken en problemen.

De volgende functionaliteit is nu beschikbaar:

* Wanneer u de Volledige blauwe bubbel van Percentage in een taak of de kopbal van de kwestie schuift, zal de Percentage Voltooien van de taak of de kwestie nu bijwerken in vijf punttoename. Voordat deze update werd uitgevoerd, heeft u door het schuiven van de blauwe ballon Percentage de taken of problemen in stappen van één punt bijgewerkt.

* U kunt dubbelklikken op de blauwe ballon en deze handmatig bijwerken met een gewenst aantal zonder de schuifregelaar te gebruiken. Deze functionaliteit is niet gewijzigd.

Er zijn geen andere wijzigingen aangebracht in het bijwerken van het percentage Voltooide taken en problemen op andere gebieden van Workfront.

Voor informatie, zie [ Mening en werk Percent bij Voltooid voor taken ](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Meer transparantie bij het gebruik van AI Assistant voor projecten, taken en problemen

>[!NOTE]
>
>* Voorbeeld: 19 mei 2025
>* Snelle productie: 19 mei 2025
>* Productie voor alle afnemers: 19 mei 2025

Om duidelijker te maken hoe AI Assistant antwoorden zoekt op vragen over Workfront-projecten, -taken en -problemen, hebben we deze informatie toegevoegd aan het antwoord op de vraag. AI Assistant bevat nu de zoekgegevens in de uitvoer. U kunt deze informatie gebruiken als een manier om te controleren of AI Assistant de vraag die u stelde correct heeft geïdentificeerd en om de context van het antwoord te begrijpen.

Eerder was deze informatie niet beschikbaar in het antwoord van de AI Assistant.

Voor informatie over het gebruiken van AI Medewerker om informatie over de punten van Workfront te krijgen, zie [ Medewerker van het Gebruik AI om met projecten, taken, en kwesties ](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md) te werken.
