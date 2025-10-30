---
content-type: api
navigation-topic: api-navigation-topic
title: Bestanden uploaden via de API
description: Bestanden uploaden via de API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: cf5a1ab848caae947829806e601662a31ce3a081
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Bestanden uploaden via de API

U kunt bestanden uploaden met Workfront API&#39;s met API-gereedschappen, zoals Postman, of met eenvoudige cURL-opdrachten.

Om documenten te uploaden, zie de instructies voor **Uploadend Documenten** in het Gedrag van het Post van Workfront [&#x200B; &#x200B;](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). U kunt dezelfde instructies ook gebruiken voor cURL-aanvragen.

**wanneer het gebruiken van API hulpmiddelen om dossiers te uploaden, volg deze richtlijnen:**

* Gebruik de optie voor het gereedschap API om het bestand te uploaden. Er is vaak a **verkies de knoop van het Dossier** op het verzoekscherm.

* Gebruik de HTTP-methode POST om een aanvraag in te dienen om het bestand te uploaden.

* Uw verzoek moet resulteren in een reactie die een waarde voor de handle bevat.

* Gebruik de handvatwaarde, het objecten type, en de waarde GUID voor objID in een nuttige lading JSON om een verdere vraag te maken. Dit is voor het maken van het object voor uw bestand, zoals in het volgende voorbeeld:

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

U ontvangt een id voor het object in de reactie.

Raadpleeg de Help van het specifieke API-gereedschap dat u gebruikt voor meer informatie.
