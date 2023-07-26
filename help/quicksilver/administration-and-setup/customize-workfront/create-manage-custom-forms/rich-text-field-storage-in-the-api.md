---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Opslag van rijke tekstvelden in de API
description: Als een object zoals een project, uitgave of taak RTF-opmaak bevat, wordt het opgeslagen en toegankelijk als parameterwaarde via de Workfront API.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Opslag van rijke tekstvelden in de API

Als een object zoals een project, uitgave of taak RTF-opmaak bevat, wordt het opgeslagen en toegankelijk als parameterwaarde via de Workfront API.

Het aanvragen van tekstinformatie van een projectvoorwerp dat rijke tekst bevat kan het gebruiken van het gebied doen **parameterValues**.

Een eenvoudige HTTP-aanvraag kan er bijvoorbeeld als volgt uitzien:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Als dit voorbeeldproject een aangepast formulier met 3 aangepaste velden bevatte: calc-veld, alineatekst en rich 1. Vervolgens retourneert het bovenstaande verzoek een reactie die lijkt op het volgende, waarbij het veld &quot;rich 1&quot; een RTF-parameterveld is en de tekstwaarde &quot;**Hallo** *Wereld!*&quot;:

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Zie voor meer informatie over hoe uitgebreide tekstgegevens worden opgeslagen en kunnen worden opgehaald via de Adobe Workfront API voor meer informatie [Rijke tekstvelden in de Adobe Workfront API](../../../wf-api/general/rich-text-field-api.md).
