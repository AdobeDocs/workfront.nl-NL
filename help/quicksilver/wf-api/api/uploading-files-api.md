---
content-type: api
navigation-topic: api-navigation-topic
title: Bestanden uploaden via de API
description: Bestanden uploaden via de API
author: John
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Bestanden uploaden via de API

U kunt bestanden uploaden met Workfront API&#39;s met API-gereedschappen, zoals Postman, of met eenvoudige cURL-opdrachten.

Zie de instructies voor het uploaden van documenten **Documenten uploaden** in Workfront [Gedrag na](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). U kunt dezelfde instructies ook gebruiken voor cURL-aanvragen.

**Houd u aan de volgende richtlijnen wanneer u API-gereedschappen gebruikt om bestanden te uploaden:**

* Gebruik de optie voor het gereedschap API om het bestand te uploaden. Dit is vaak een **Bestand kiezen** op het aanvraagscherm.

* Gebruik de HTTP-methode van de POST om een aanvraag in te dienen om het bestand te uploaden.

* Uw verzoek moet resulteren in een reactie die een waarde voor de handle bevat.

* Gebruik de handvatwaarde, het objecten type, en de waarde GUID voor objID in een nuttige lading JSON om een verdere vraag te maken. Dit is voor het maken van het object voor uw bestand, zoals in het volgende voorbeeld:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

U ontvangt een id voor het object in de reactie.

Raadpleeg de Help van het specifieke API-gereedschap dat u gebruikt voor meer informatie.
