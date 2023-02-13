---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuratie van opties voor OPTASK copyIssue
description: Een verklaring van de geheelwaarden die door het copyIssue eindpunt worden verwacht.
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---

# Configuratie van opties voor OPTASK copyIssue


Een van de eigenschappen van een API-aanroep van copyIssue is een veld met de naam `options`. Dit veld verwacht een geheel getal.

Voer het overeenkomende gehele getal in als u een van de volgende opties wilt opnemen. Als u meerdere opties wilt opnemen, voert u de som van de overeenkomende gehele getallen in.

| option | waarde* |
|---|---|
| Toewijzingen wissen | 2 |
| Voortgang wissen | 4 |
| Documenten wissen | 128 |
| Updates wissen | 65536 |
| Machtigingen wissen | 524288 |
| Aangepaste gegevens wissen | 1048576 |

*Alle waarden zijn machten van 2.

Voorbeelden:

* Als u de voortgang wilt wissen wanneer u het probleem kopieert, voert u een `options` waarde van `4`.

* Als u zowel de voortgang als de documenten wilt wissen, voert u een `options` waarde van `132`.

   Voortgang wissen = 4

   Documenten wissen = 128

   4 + 128 = 132
