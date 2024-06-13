---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Handeling moveToFolder van document werkt niet
description: Als u de handeling Document moveToFolder gebruikt, wordt een fout van 422 geretourneerd.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# Handeling moveToFolder van document werkt niet

## Probleem

Wanneer u de objecten Document gebruikt `moveToFolder` handeling, er wordt een fout van 422 geretourneerd.

of

Als u deze actie gebruikt via de Adobe Authenticator-module in Workfront Fusion, wordt het document niet verplaatst, maar is er geen indicatie voor de fout. De fout is hetzelfde, maar de Adobe Authenticator-module geeft deze niet weer.

## Oplossing

Een mogelijke oorzaak van een fout van 422 voor deze actie is dat de actie probeert om een Document in één Gekoppelde Omslag in een andere Gekoppelde Omslag te bewegen.

Controleer of het document dat u wilt verplaatsen, zich nog niet in een gekoppelde map bevindt.
