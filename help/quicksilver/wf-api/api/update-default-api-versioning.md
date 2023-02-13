---
content-type: api
navigation-topic: api-navigation-topic
title: Integraties bijwerken die standaard-API-versies gebruiken
description: Integraties bijwerken die standaard-API-versies gebruiken
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Integraties bijwerken die standaard-API-versies gebruiken

We publiceren twee keer per jaar nieuwe versies van de Adobe Workfront API. Elke versie wordt ondersteund gedurende drie jaar na de release, met een extra jaar in een vervangen toestand waarin de versie beschikbaar maar niet ondersteund is.

Integraties die geen versie van de API in de URI opgeven, worden automatisch gerouteerd naar Standaard, hetgeen is vervangen. Uw Workfront-integratie is alleen geldig als u een ondersteunde API-versie opgeeft in uw Workfront API-aanvragen.

Ga voor meer informatie over het opgeven van een versie in uw API-aanvragen naar [Geef een API-versie op in uw integratie](../../wf-api/api/specify-api-version-integrations.md).

## De standaardversie van de API begrijpen

De oorspronkelijke intentie van de standaard-API (Default) was om deze toe te wijzen aan de nieuwste versie van de Workfront-API. Hierdoor zouden klanten met basisintegraties die Default aanriepen, hun API-aanvragen nooit hoeven bij te werken.

In 2011 heeft Workfront versie 3.0 van de API uitgebracht. Het gebrek werd automatisch bewogen aan Versie 3.0, die vele klantenintegratie brak die te complex waren om Versie 3.0 te gebruiken zonder wordt bijgewerkt. Als gevolg hiervan heeft Workfront deze wijziging teruggedraaid en de standaardversie bij Versie 2 gelaten.

Helaas is dit onderwerp nooit opnieuw besproken. Nu we de API-functionaliteit aanzienlijk willen uitbreiden, zijn we gedwongen oudere versies van onze API, inclusief Default, af te stoten. In plaats van Default bij te werken, wat ongetwijfeld meer integraties zou doorbreken, verwijderen we het concept van een standaardversie volledig. Dit is om onze klanten aan te moedigen om stabiele versies van onze APIs te gebruiken en hun integratie op een cyclus van, hoogstens, drie jaar te handhaven.

## Standaardwaarde wordt verwijderd

Om de Workfront API te verbeteren, zijn we bezig met het verwijderen van oudere API-versies die ons supportvenster van drie jaar hebben overschreden. Één van deze versies is Versie 2, waaraan Standaard in kaart wordt gebracht. Deze versie is in 2010 uitgebracht en veel van de logica die op dat moment in de toepassing Attask/Workfront wordt ondersteund, bestaat niet meer of is ingrijpend gewijzigd.

We hebben Default in juli 2017 vervangen en we wijzen niet langer een specifieke versie van de API aan als de standaardversie. In plaats daarvan moeten alle Workfront API-aanvragen een specifieke API-versie opgeven.

>[!IMPORTANT]
>
> Tegen 1 juli 2018 moeten al uw Workfront-integraties die gebruikmaken van Standaard zijn bijgewerkt om een specifieke ondersteunde API-versie aan te roepen. Na die datum zullen alle Workfront API-aanvragen die worden gebruikt door integraties die geen versie opgeven, mislukken.

Ga voor meer informatie over de Workfront-afgekeurde camera naar [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

## Uw integratie bijwerken naar ondersteunde API-versies

Als uw Workfront API-aanvragen geen versie opgeven, gebruiken ze Standaard. U moet uw API-aanvragen bijwerken om een ondersteunde versie van de API op te geven, bij voorkeur de meest recente ondersteunde API.

Met de volgende Workfront API-aanvraag wordt bijvoorbeeld geen API-versie opgegeven:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Wanneer deze aanvraag wordt ingediend, ontvangt u een reactie met JSON-gecodeerde tekst die gegevens van uw Workfront-instantie opgeeft. Omdat er geen API-versie is opgegeven in deze URI, gaat de aanroep naar Standaard.

Als u een standaard-API-aanvraag wilt omzetten in een versie-API-aanvraag, roept u gewoon een ondersteunde API-versie aan. Met de volgende URI wordt bijvoorbeeld versie 9 aangevraagd:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Wanneer u uw Workfront API-aanvragen bijwerkt, kunt u elke ondersteunde versie van onze API opgeven. Zie voor meer informatie over het verwijzen naar een specifieke API [Geef een API-versie op in uw integratie](../../wf-api/api/specify-api-version-integrations.md).

Als u het maximale ondersteuningsvenster wilt weergeven, roept u de nieuwste versie aan (versie 9). U vindt een lijst met ondersteunde API&#39;s in [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

Het is absoluut noodzakelijk dat u de integraties bijwerkt u die Standaard gebruiken. Als u momenteel integraties hebt die geen versie specificeren, zou u bericht van uw verkoper van Workfront, de manager van het klantensucces, of steunvertegenwoordiger, of een bericht van het aankondigingscentrum kunnen ontvangen.

Zorg er zo snel mogelijk voor dat uw integratie wordt bijgewerkt om een ondersteunde versie van onze API aan te roepen.
