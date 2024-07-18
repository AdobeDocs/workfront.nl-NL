---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Gekoppelde mappen worden niet ondersteund voor DOCU-object
description: Gekoppelde mappen worden niet ondersteund voor DOCU-object
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Het gebruik van de API om een gekoppelde map toe te voegen, wordt niet ondersteund

Het gebruik van de API om een gekoppelde map toe te voegen aan de mappenarray voor een Document (DOCU)-object, wordt niet ondersteund. Het verzoek is geslaagd, maar het document kan door sommige externe providers uit het systeem worden verwijderd. Dat komt omdat het externe systeem als laatste bron van waarheid zal worden gebruikt. Als het document daarom wordt verwijderd van de externe provider, wordt het document geacht niet meer te bestaan. Documenten die niet in de gekoppelde (externe) map zijn gevonden, kunnen automatisch uit [!DNL Workfront] worden verwijderd zonder dat ze kunnen worden hersteld.
