---
content-type: api
navigation-topic: api-navigation-topic
title: Vervalsing van API-intern
description: Vervalsing van API-intern
author: John
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Vervalsing van API-intern

API-Internal is een versie van de Adobe Workfront API die niet wordt ondersteund vanwege het ontwerp en het doel ervan. Hoewel het de meest recente updates van de Workfront API bevat, kan het zonder voorafgaande kennisgeving worden gewijzigd en moet het daarom met voorzichtigheid worden gebruikt bij de integratie van de productie. Workfront raadt ten zeerste aan alle API-interne integratie naar een versioned API bij te werken.

Ga voor meer informatie over ondersteunde versies van de Workfront API naar [API-versieschema en ondersteuningsschema](../../wf-api/api/api-version-support-schedule.md).

**API-toepassingen gebruiken die niet worden ondersteund**

Als voor uw integratie functies nodig zijn die niet beschikbaar zijn in een versioned API, raadt Workfront aan API-Unsupported te gebruiken. API-niet-ondersteund wordt niet ondersteund, vergelijkbaar met API-intern. API-Niet-ondersteund bevat ook de meest recente wijzigingen in de Workfront API en kan zonder voorafgaande kennisgeving worden gewijzigd. Workfront raadt u aan API-Unsupported te gebruiken in uw testomgeving waar u nieuwe functionaliteit kunt verkennen en ervoor kunt zorgen dat de API vrij is van fouten.

**De API-versie bepalen die u gebruikt**

U kunt de versie van API bepalen uw integraties door REST te gebruiken om URI te construeren die een vraag over HTTPS naar Workfront verzendt en dan een reactie JSON terugkeert.

In het volgende voorbeeld wordt een URI getoond die API-Internal aanroept:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

In het volgende voorbeeld ziet u URI die API-Unsupported aanroept:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

In het volgende voorbeeld ziet u een URI die versie 15.0 van de API aanroept:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
