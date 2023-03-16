---
title: 23.2 Verbeteringen aan mobiele apparaten
description: 23.2 Verbeteringen aan mobiele apparaten
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 8a209bbe64b7b69b41cd9e4d2f603ff58491ba30
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 23.2 Verbeteringen aan mobiele apparaten

Deze pagina bevat een beschrijving van alle verbeteringen in de voorvertoningsomgeving die zijn aangebracht met de release 23.2. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving met de release 23.2.

Voor een lijst van alle veranderingen beschikbaar op dit punt in de 23.2 versiecyclus, zie [23.2 Overzicht van de release](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

<!--

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Second two articles will not be available in Main until I publish my branch.

## Add tasks and issues to Boards workstreams from lists and reports

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

-->

## Uren vastleggen op verbonden kaarten aan boord

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt nu uren aanmelden op verbonden kaarten, net als bij een taak of uitgave. U moet de correcte toestemmingen aan de taak of de kwestie hebben om de tijd te registreren.

De velden voor tijdregistratie worden standaard niet weergegeven op verbonden kaarten. U moet **Uren** in het Configure gebied onder Kaarten.

Zie voor meer informatie [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Weergave van velden op een kaart aanpassen

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.


Er is nu aanpassingsmogelijkheden beschikbaar om te bepalen welke velden op een kaart worden weergegeven, zowel in de volledige weergave wanneer de kaart is geopend als in de weergave voor gecondenseerde kaarten op het bord. Wanneer u een veld uitschakelt, wordt dit in geen van beide weergaven weergegeven. U kunt een veld ook inschakelen in de volledige weergave en verbergen in de versmalde weergave.

Zie voor meer informatie [Aanpassen welke velden worden weergegeven op een kaart](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Een standaardstatus definiëren voor kaarten die naar een bordkolom worden verplaatst

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt nu een standaardstatus instellen om toe te passen op kaarten die naar een specifieke kolom worden verplaatst door een aangepaste status en een systeemstatus te selecteren in het kolombeleid. Wanneer u een kaart naar de kolom verplaatst, probeert Workfront eerst de aangepaste status toe te passen (bijvoorbeeld Feedback wachten). Als de aangepaste status niet beschikbaar is voor die kaart, past Workfront de systeemstatus toe (bijvoorbeeld In wachtstand). Als de status van de verbonden taak of uitgave wordt gewijzigd in de aangepaste of systeemstatus die is ingesteld in het kolombeleid, wordt de kaart automatisch naar de kolom verplaatst.

Eerder werd u gevraagd een status te selecteren voor elke kaart die naar de kolom werd verplaatst, als er meerdere statussen beschikbaar waren.

Zie voor meer informatie [Kolommen beheren](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Verzamelingen die nu beschikbaar zijn in Adobe Workfront Boards

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt nu verzamelingen maken op het dashboard voor borden. Een verzameling is een groep raden van bestuur om samen te werken aan het werk. Nadat u de verzameling een naam hebt gegeven, kunt u tekengebieden aan de verzameling toevoegen met behulp van een set sjablonen met vooraf gedefinieerde instellingen, zoals kolomnamen. U kunt zelfstandige borden in een inzameling ook bewegen. Zodra een board in een inzameling is, kan het naar een andere inzameling worden verplaatst maar het kan geen standalone raad worden.

Het toevoegen van leden aan een verzameling werkt op dezelfde manier als het toevoegen van leden aan een board. Een persoon of team moet lid zijn in de verzameling voordat deze als leden aan een bestuur in de verzameling kunnen worden toegevoegd.

Zie voor meer informatie [Verzamelingen beheren](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3415609/){target=_blank}

## Schattingsveld op verbonden kaarten verwijst naar het veld Artikelpunten op Workfront-objecten

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

Het veld Schatting op verbonden kaarten in Workfront-boards verwijst nu naar het veld Artikelpunten voor het bijbehorende Workfront-object.

Het veld Nieuwe artikelpunten is een bewerkbaar, gratis formulierveld dat u kunt toevoegen aan een weergave in een lijst of rapport voor taken of problemen. Het is niet gebonden aan geplande uren of teamtaken.

Eerder was de schatting van de kaart een handmatig item en werd deze niet toegewezen aan een veld op een taak of uitgifte.

Het veld Schatting op zowel ad-hockaarten als op gekoppelde kaarten heeft bovendien geen tekenlimiet meer. Eerder was het maximumaantal tekens 99.

Zie voor meer informatie [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Kaart voorvertonen in innamekolom

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt nu op een aangesloten kaart in de innamekolom klikken om een alleen-weergaveversie van de inhoud te zien. U kunt de inhoud van de kaart pas bewerken als de kaart uit de innamekolom naar een andere kolom op het bord wordt verplaatst.
