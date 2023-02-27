---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicaten die worden geretourneerd tijdens een grote gepagineerde zoekopdracht
description: Duplicaten die worden geretourneerd tijdens een grote gepagineerde zoekopdracht
author: Becky
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicaten die worden geretourneerd tijdens een grote gepagineerde zoekopdracht

## Probleem

Wanneer een grote gepagineerde zoekopdracht in de API voor een object wordt uitgevoerd, ontvangt de klant dubbele vermeldingen en ontbrekende records.

## Oplossing

Wanneer de orde niet formeel wordt bepaald, baseren wij op de orde van de rijen die door het gegevensbestand van het Oracle zijn teruggekeerd, dat geen deterministische opdracht garandeert. Twee opeenvolgende aanroepen met dezelfde query kunnen bijvoorbeeld rijen in een andere volgorde retourneren. Op dezelfde manier kunnen de rijen tijdens het pagineren willekeurig worden toegewezen aan verschillende &quot;pagina&#39;s&quot;, wat tot duplicaten leidt. De eenvoudigste oplossing kan het sorteren door identiteitskaart toevoegen:

```
&ID_Sort=asc
```

