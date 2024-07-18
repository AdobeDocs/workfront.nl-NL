---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Valutanotatie ophalen voor een project wanneer de valuta null is
description: Valutanotatie ophalen voor een project wanneer de valuta null is
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Valutanotatie ophalen voor een project wanneer de valuta null is (niet toegewezen)

Het projectobject met het valutaveld kan worden opgehaald met de volgende aanvraag:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Dit retourneert de volgende responsinstantie:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Als de valuta niet is ingesteld voor het project, bevat deze reactie een valuta met de waarde `null` :

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Als u de valuta voor het project (zoals voor berekeningen) vereist, kunt u de standaardmunt voor de klant terugwinnen:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

De reactie omvat de valuta die de gebruiker als gebrek heeft geplaatst, die door om het even welke projecten voor die klant zou worden gebruikt die niet de muntreeks hebben:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
