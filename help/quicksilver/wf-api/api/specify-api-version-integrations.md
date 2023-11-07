---
content-type: api
navigation-topic: api-navigation-topic
title: Geef een API-versie op in uw integratie
description: Geef een API-versie op in uw integratie
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Een API-versie opgeven in uw integratie

Alle Adobe Workfront URI&#39;s moeten verwijzen naar een specifieke versie van de API na het gedeelte &quot;attask/api&quot; van de URI. In het volgende voorbeeld wordt versie 15.0 aangeroepen:

`attask/api/v15.0/<objectName>/<objectId>`

Zorg ervoor dat al uw integratieaanroepen momenteel ondersteunde Workfront API&#39;s bevatten.

## Release- en implementatieschema van Workfront API&#39;s

Nieuwe versies van de API worden regelmatig uitgebracht, meestal twee keer per jaar. Elke versie wordt ondersteund gedurende drie jaar na de releasedatum, met een extra jaar in een vervangen toestand waarin de versie beschikbaar maar niet ondersteund is.

Zie voor meer informatie over het schema voor het afbreken en afgekeuren van Workfront API&#39;s [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* De standaardversie van de API wordt ingesteld op de meest recente versie. Voor elke API-aanroep zonder de opgegeven versie wordt de standaardversie gebruikt. Elke keer dat Workfront een nieuwe versie van de API loslaat, wordt de standaardversie bijgewerkt naar de nieuwste versie. **Daarom moeten, nadat een nieuwe versie van de Workfront API is uitgebracht, alle API-aanroepen die de standaardversie gebruiken, worden gecontroleerd om ervoor te zorgen dat de functionaliteit nog steeds wordt ondersteund.**
>
>* Als uw organisatie momenteel de standaard-API gebruikt, heeft uw Workfront-beheerder een bericht van het Aankondigingscentrum ontvangen met verdere instructies betreffende de standaard-API.
>
>Ga voor de meest recente versie van de API naar [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).


## De API-versie bepalen die u gebruikt

U kunt de versie van de API bepalen die u gebruikt door de URI te controleren van een HTTP-aanvraag die naar de Workfront API wordt verzonden. In het volgende voorbeeld wordt een Workfront request-URI getoond die versie 15 van de API opgeeft:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Als een URI geen versie opgeeft, wordt de standaardversie van de API gebruikt, zoals in het volgende voorbeeld wordt getoond:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integraties die geen versie van de API in de URI opgeven, worden automatisch gerouteerd naar de standaardversie van de API.

## Integraties bijwerken voor gebruik van ondersteunde API-versies

Wanneer u Workfront-integratie maakt of onderhoudt, moet u een methode opnemen voor het dynamisch bijwerken van de API-versie en andere eigenschappen die kunnen worden gewijzigd (zoals de API-sleutel).

Om het bijwerken van integraties efficiënter te maken, zou u de volgende suggesties voor het registreren van integratiewaarden moeten overwegen:

* Waarden opslaan die in de toekomst worden gewijzigd in een eigenschappenbestand dat u bijwerkt
* Een webservice maken om eigenschappen in real-time te beheren
* Eigenschapwaarden opslaan in een gegevensopslagruimte die uw toepassing kan lezen

Door uw Workfront-integratie met dit in gedachten te ontwerpen, verlicht u de behoefte aan uitgebreide ontwikkelingswerkzaamheden wanneer deze waarden onvermijdelijk veranderen.
