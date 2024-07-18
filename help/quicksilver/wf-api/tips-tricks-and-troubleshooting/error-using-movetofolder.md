---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Handeling moveToFolder van document werkt niet
description: Als u de handeling Document moveToFolder gebruikt, wordt een fout van 422 geretourneerd.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Handeling moveToFolder van document werkt niet

## Probleem

Wanneer u de handeling `moveToFolder` van het object Document gebruikt, wordt een fout van 422 geretourneerd.

of

Als u deze actie gebruikt via de Adobe Authenticator-module in Workfront Fusion, wordt het document niet verplaatst, maar is er geen indicatie voor de fout. De fout is hetzelfde, maar de Adobe Authenticator-module geeft deze niet weer.

## Oplossing

Een mogelijke oorzaak van een fout van 422 voor deze actie is dat de actie probeert om een Document in één Gekoppelde Omslag in een andere Gekoppelde Omslag te bewegen.

Controleer of het document dat u wilt verplaatsen, zich nog niet in een gekoppelde map bevindt.
