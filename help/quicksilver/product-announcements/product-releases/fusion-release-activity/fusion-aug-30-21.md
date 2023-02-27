---
title: Workfront Fusion release activity:&nbsp;Week van 30 augustus 2021
description: Workfront Fusion release activity:&nbsp;Week van 30 augustus 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Workfront Fusion release activity: Week van 30 augustus 2021

Op deze pagina worden alle verbeteringen beschreven die in Adobe Workfront Fusion in de week van 30 augustus 2021 zijn aangebracht.

Voor een lijst met alle recente wijzigingen raadpleegt u [Adobe Workfront Fusion-releaseactiviteit](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Voor een lijst met recente opgeloste problemen in Workfront Fusion raadpleegt u de [Workfront-onderhoudsupdates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) pagina en controleer op updates met het label Workfront Fusion Maintenance Update.

## Gebeurtenissen filteren die de module Workfront > Watch-gebeurtenissen activeren

1. Een aangepast filter instellen voor gebeurtenissen die de module Workfront > Watch-gebeurtenissen activeren

   Om het aantal onnodige scenario looppas te verminderen, hebben wij Workfront > de registratiemodule van het Controle bijgewerkt om gebeurtenis het filtreren toe te laten. U kunt nu een filter instellen wanneer u een webhaak maakt. Hierdoor kan het scenario alleen worden geactiveerd wanneer de gebeurtenis aan bepaalde criteria voldoet.

   Het gebeurtenisfilter biedt momenteel de volgende bewerkingen:

   * Gelijk: Trigger een scenario slechts wanneer een gebeurtenis de voorwaarden van de filter aanpast. U kunt bijvoorbeeld een filter instellen dat alleen een scenario activeert als de gebeurtenis in een bepaald project plaatsvindt.
   * Niet gelijk: Trigger een scenario slechts als een gebeurtenis niet de voorwaarden van de filter aanpast. U kunt bijvoorbeeld een filter maken dat alleen een scenario activeert als de uitgave waarin een gebeurtenis plaatsvindt, geen status Gesloten heeft.

   Eerder, zou de module van het Horloge verslagen alle verslagen terugwinnen. Gebruikers kunnen alleen filteren door later filters in het scenario in te stellen.

   Als u wilt profiteren van het filteren van gebeurtenissen, maakt u een nieuwe webhaak in de module voor controlegebeurtenissen. Het is momenteel niet mogelijk om bestaande websites te bewerken om deze functionaliteit in te bouwen. We raden u ten zeerste aan nieuwe webhooks te maken met behulp van gebeurtenisfilters voor bestaande scenario&#39;s.

1. Filter gebeurtenissen uit die door de huidige verbinding worden geactiveerd.

   We hebben het meest gangbare gebeurtenisfilter toegevoegd om uw websites gemakkelijker in te stellen voor de module Workfront > Watch-gebeurtenissen. Nu, heeft webhaak een optie om uit om het even welke veranderingen te filtreren die door modules worden aangebracht gebruikend de verbinding die voor de module van de Gebeurtenissen van het Controle wordt gespecificeerd. Met andere woorden, als dit filter is ingeschakeld, kunnen wijzigingen die door de Workfront-gebruiker zijn aangebracht in verband met die verbinding, het scenario niet activeren.

   Eerder was dit filter niet beschikbaar. Daarom was het gemakkelijker voor veranderingen die in de modules van Workfront worden aangebracht om scenario&#39;s teweeg te brengen die die modules bevatten, potentieel veroorzakend scenario&#39;s om zich in een oneindige lijn teweeg te brengen.

Zie voor meer informatie over gebeurtenisfilters in de module Workfront > Watch-gebeurtenissen [Adobe Workfront-modules](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

