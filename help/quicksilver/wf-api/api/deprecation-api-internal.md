---
content-type: api
navigation-topic: api-navigation-topic
title: Vervalsing van API-intern
description: Vervalsing van API-intern
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Vervalsing van API-intern

API-Internal is een versie van de Adobe Workfront API die niet wordt ondersteund vanwege het ontwerp en het doel ervan. Hoewel het de meest recente updates van de Workfront API bevat, kan het zonder voorafgaande kennisgeving worden gewijzigd en moet het daarom met voorzichtigheid worden gebruikt bij de integratie van de productie. Workfront raadt ten zeerste aan alle API-interne integratie naar een versioned API bij te werken.

Meer over gesteunde versies van Workfront API leren, zie [ API versioning en steunprogramma ](../../wf-api/api/api-version-support-schedule.md).

**Gebruikend API-niet gesteund**

Als voor uw integratie functies nodig zijn die niet beschikbaar zijn in een versioned API, raadt Workfront aan API-Unsupported te gebruiken. API-niet-ondersteund wordt niet ondersteund, vergelijkbaar met API-intern. API-Niet-ondersteund bevat ook de meest recente wijzigingen in de Workfront API en kan zonder voorafgaande kennisgeving worden gewijzigd. Workfront raadt u aan API-Unsupported te gebruiken in uw testomgeving waar u nieuwe functionaliteit kunt verkennen en ervoor kunt zorgen dat de API vrij is van fouten.

**Bepalend de API Versie u** gebruikt

U kunt de versie van API bepalen uw integraties door REST te gebruiken om URI te construeren die een vraag over HTTPS naar Workfront verzendt en dan een reactie JSON terugkeert.

In het volgende voorbeeld wordt een URI getoond die API-Internal aanroept:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

In het volgende voorbeeld ziet u URI die API-Unsupported aanroept:

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>API-Niet-ondersteunde aanroepen laten de sectie `/api` van de URL weg.

In het volgende voorbeeld ziet u een URI die versie 15.0 van de API aanroept:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
