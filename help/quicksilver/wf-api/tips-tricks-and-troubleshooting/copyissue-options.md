---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuratie van opties voor OPTASK copyIssue
description: Een verklaring van de geheelwaarden die door het copyIssue eindpunt worden verwacht.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 4%

---

# Configuratie van opties voor OPTASK copyIssue


Een van de eigenschappen voor een API-aanroep van copyIssue is een veld met de naam `options` . Dit veld verwacht een geheel getal.

Voer het overeenkomende gehele getal in als u een van de volgende opties wilt opnemen. Als u meerdere opties wilt opnemen, voert u de som van de overeenkomende gehele getallen in.

| option | waarde* |
|---|---|
| Toewijzingen wissen | 2 |
| Voortgang wissen | 4 |
| Documenten wissen | 128 |
| Updates wissen | 65536 |
| Rechten wissen | 524288 |
| Aangepaste gegevens wissen | 1048576 |

*Alle waarden zijn machten van 2.

Voorbeelden:

* Voer de `options` waarde `4` in om de voortgang te wissen wanneer u de uitgave kopieert.

* Als u zowel de voortgang als de documenten wilt wissen, voert u de `options` waarde `132` in.

  Voortgang wissen = 4

  Documenten wissen = 128

  4 + 128 = 132
