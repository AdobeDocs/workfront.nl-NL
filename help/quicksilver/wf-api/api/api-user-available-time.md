---
content-type: api
navigation-topic: wf-api
title: Gebruikers beschikbare tijd-API ophalen
description: Gebruikers beschikbare tijd-API ophalen
author: John
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: aea37c1d200dfadf9ccbb7b36145eb04d5ab4b6d
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---

# Gebruikers beschikbare tijd-API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

Het gebruikers beschikbare tijdeindpunt wint gegevens over de beschikbare tijd van de gebruiker terug. Hierdoor kunnen gegevens worden samengevoegd op basis van gebruikerskenmerken en tijdsintervallen.

## Voorbeeld van aanvraag

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parameters aanvragen

* **userIDs**: array van tekenreeksen. Vereist. Voorbeeld: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. tekenreeks. Vereist. Voorbeeld:  `"2022-07-10T00:00:00"`.

* **toDate**: datetime. tekenreeks. Vereist. Voorbeeld `"2022-07-20T23:59:59"`.

## Voorbeeld van reactie:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Responsparameters

* **AVL**: Werkelijke beschikbare uren. Array met getallen.
* **PAVL**: Zuiver beschikbare uren voor het plannen die niet niet het niet-werkdagen of gebruikerstijd weg omvatten. Tekenreeks.
