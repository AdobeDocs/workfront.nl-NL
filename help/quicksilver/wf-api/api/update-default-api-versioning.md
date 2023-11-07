---
content-type: api
navigation-topic: api-navigation-topic
title: Integraties bijwerken die standaard-API-versies gebruiken
description: Integraties bijwerken die standaard-API-versies gebruiken
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Integraties bijwerken die standaard-API-versies gebruiken

We publiceren twee keer per jaar nieuwe versies van de Adobe Workfront API. Elke versie wordt ondersteund gedurende drie jaar na de release, met een extra jaar in een vervangen toestand waarin de versie beschikbaar maar niet ondersteund is.

Integraties die geen versie van de API in de URI opgeven, worden automatisch naar Standaard gerouteerd. Als u wilt dat uw API-aanroep een specifieke versie van de API gebruikt, moet u die versie opgeven in uw Workfront API-aanvragen.

>[!NOTE]
>
>Als uw organisatie momenteel de standaard-API gebruikt, heeft uw Workfront-beheerder een bericht van het Aankondigingscentrum ontvangen met verdere instructies betreffende de standaard-API.

Ga voor meer informatie over het opgeven van een versie in uw API-aanvragen naar [Geef een API-versie op in uw integratie](../../wf-api/api/specify-api-version-integrations.md).

## Overwegingen bij het gebruik van de standaard-API

Houd rekening met het volgende wanneer u werkt met de standaard-API van Workfront:

* De standaardversie van de API is de meest recente versie. Voor elke API-aanroep zonder de opgegeven versie wordt de standaardversie gebruikt. Elke keer dat Workfront een nieuwe versie van de API loslaat, wordt de standaardversie bijgewerkt naar de nieuwste versie. **Daarom moeten, nadat een nieuwe versie van de Workfront API is uitgebracht, alle API-aanroepen die de standaardversie gebruiken, worden gecontroleerd om ervoor te zorgen dat de functionaliteit nog steeds wordt ondersteund**.
* Als uw organisatie momenteel de eerder vervangen Standaard API gebruikt, heeft uw beheerder van Workfront een bericht van het Aankondigingscentrum met verdere instructies betreffende Standaard API ontvangen.

Ga voor de meest recente versie van de API naar [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

## Uw integratie bijwerken naar ondersteunde API-versies

Als uw Workfront API-aanvragen geen versie opgeven, gebruiken ze Standaard. We raden uw API-aanvragen aan om een ondersteunde versie van de API op te geven, bij voorkeur voor de meest recente ondersteunde API.

Met de volgende Workfront API-aanvraag wordt bijvoorbeeld geen API-versie opgegeven:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Wanneer deze aanvraag wordt ingediend, ontvangt u een reactie met JSON-gecodeerde tekst die gegevens van uw Workfront-instantie opgeeft. Omdat er geen API-versie is opgegeven in deze URI, gaat de aanroep naar Standaard.

Als u een standaard-API-aanvraag wilt omzetten in een versie-API-aanvraag, roept u gewoon een ondersteunde API-versie aan. De volgende URI vraagt bijvoorbeeld versie 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Wanneer u uw Workfront API-aanvragen bijwerkt, kunt u elke ondersteunde versie van onze API opgeven. Zie voor meer informatie over het verwijzen naar een specifieke API [Geef een API-versie op in uw integratie](../../wf-api/api/specify-api-version-integrations.md).

Als u het maximale ondersteuningsvenster wilt weergeven, roept u de nieuwste versie aan. U vindt een lijst met ondersteunde API&#39;s in [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

## Historie van de standaardversie van de API

De oorspronkelijke intentie van de standaard-API (Default) was om deze toe te wijzen aan de nieuwste versie van de Workfront-API. Hierdoor zouden klanten met basisintegraties die Default aanriepen, hun API-aanvragen nooit hoeven bij te werken.

In 2011 heeft Workfront versie 3.0 van de API uitgebracht. Het gebrek werd automatisch bewogen aan Versie 3.0, die vele klantenintegratie brak die te complex waren om Versie 3.0 te gebruiken zonder wordt bijgewerkt. Als gevolg hiervan heeft Workfront deze wijziging teruggedraaid en de standaardversie bij Versie 2 gelaten.

Sinds 2011 is de API-functionaliteit van Workfront aanzienlijk verbeterd. Daarom hebben we oudere versies van onze API vervangen. In 2017 hebben we in plaats van Default bij te werken het concept van een standaardversie volledig verwijderd. Dit was om onze klanten aan te moedigen om stabiele versies van onze APIs te gebruiken en hun integratie op een cyclus van, hoogstens, drie jaar te handhaven.

Workfront herstelt nu de standaard API-versie. De standaard-API wordt ingesteld op de meest recente versie van de Workfront API en wordt bijgewerkt naar de meest recente versie telkens wanneer een nieuwe versie wordt uitgebracht.

