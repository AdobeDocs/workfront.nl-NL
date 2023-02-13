---
content-type: api
navigation-topic: api-navigation-topic
title: Geef een API-versie op in uw integratie
description: Geef een API-versie op in uw integratie
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Geef een API-versie op in uw integratie

Alle Adobe Workfront URI&#39;s moeten naar een specifieke versie van de API verwijzen na het gedeelte &quot;attask/api&quot; van de URI. In het volgende voorbeeld wordt versie 7.0 aangeroepen:
`attask/api/v7.0/<objectName>/<objectId>` Zorg ervoor dat al uw integratieaanroepen momenteel ondersteunde Workfront API&#39;s bevatten.

## Release- en implementatieschema van Workfront API&#39;s

Nieuwe versies van de API worden elke zes tot acht maanden op tweejaarlijkse basis uitgebracht. Elke versie wordt ondersteund gedurende drie jaar na de releasedatum, met een extra jaar in een vervangen toestand waarin de versie beschikbaar maar niet ondersteund is.

Zie voor meer informatie over het schema voor het afbreken en afbreken van de release van Workfront API&#39;s [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

Workfront heeft de standaardversie van de API vanaf juli 2017 vervangen. Dit betekent dat Workfront niet langer een specifieke versie van de API aanwijst als de standaardversie. Alle toekomstige API-URI&#39;s moeten een versie van de API opgeven om geldig te zijn.

>[!IMPORTANT]
>
> Integraties die de standaard API-versie gebruiken, moeten worden bijgewerkt om uiterlijk 1 juli 2018 een specifieke ondersteunde API-versie aan te roepen.

## De API-versie bepalen die u gebruikt

U kunt de versie van de API bepalen die u gebruikt door de URI te controleren van een HTTP-aanvraag die naar de Workfront API wordt verzonden. In het volgende voorbeeld wordt een Workfront request-URI getoond die versie 7 van de API opgeeft:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Als een URI geen versie opgeeft, wordt de standaardversie van de API gebruikt, zoals in het volgende voorbeeld wordt getoond:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integraties die geen versie van de API in de URI opgeven, worden automatisch gerouteerd naar de standaardversie van de API en werken niet meer na 1 juli 2018.

## Integraties bijwerken voor gebruik van ondersteunde API-versies

Wanneer u Workfront-integratie maakt of onderhoudt, moet u een methode opnemen voor het dynamisch bijwerken van de API-versie en andere eigenschappen die kunnen worden gewijzigd (zoals de API-sleutel).

Om het bijwerken van integraties efficiënter te maken, zou u de volgende suggesties voor het registreren van integratiewaarden moeten overwegen:

* Waarden opslaan die in de toekomst worden gewijzigd in een eigenschappenbestand dat u bijwerkt
* Een webservice maken om eigenschappen in real-time te beheren
* Eigenschapwaarden opslaan in een gegevensopslagruimte die uw toepassing kan lezen

Door uw Workfront-integratie met dit in gedachten te ontwerpen, verlicht u de behoefte aan uitgebreide ontwikkelingswerkzaamheden wanneer deze waarden onvermijdelijk veranderen.
