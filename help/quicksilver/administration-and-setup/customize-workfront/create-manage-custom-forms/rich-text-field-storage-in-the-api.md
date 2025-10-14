---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Opslag van rijke tekstvelden in de API
description: Als een object zoals een project, uitgave of taak RTF-opmaak bevat, wordt het opgeslagen en toegankelijk als parameterwaarde via de Workfront API.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Opslag van rijke tekstvelden in de API

Als een object zoals een project, uitgave of taak RTF-opmaak bevat, wordt het opgeslagen en toegankelijk als parameterwaarde via de Workfront API.

Het verzoeken van tekstinformatie van een projectvoorwerp dat rijke tekst bevat kan worden gedaan gebruikend het gebied **parameterValues**.

Een eenvoudige HTTP-aanvraag kan er bijvoorbeeld als volgt uitzien:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Als dit voorbeeldproject een aangepast formulier met 3 aangepaste velden bevatte: calc-veld, alineatekst en rich 1. Dan zou het bovengenoemde verzoek een reactie terugkeren die op het volgende lijkt, waar het gebied &quot;rijke 1&quot;een rijk gebied van de tekstparameter is en de tekstwaarde &quot;**Hello** *Wereld is!*&quot;:

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

Voor een meer diepgaande blik bij hoe de rijke tekstinformatie wordt opgeslagen en door Adobe Workfront API kan worden teruggewonnen, zie [&#x200B; Rijke tekstgebieden in Adobe Workfront API &#x200B;](../../../wf-api/general/rich-text-field-api.md).
