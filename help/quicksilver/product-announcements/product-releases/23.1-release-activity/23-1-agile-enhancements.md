---
title: 23.1 Verbeteringen aan mobiele apparaten
description: 23.1 Verbeteringen aan mobiele apparaten
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1 Verbeteringen aan mobiele apparaten

Op deze pagina worden alle verbeteringen beschreven die in de versie 23.1 van Agile zijn aangebracht voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving in de week van 16 januari 2023.

Voor een lijst met alle wijzigingen die beschikbaar zijn in de versie 23.1 raadpleegt u [23.1 Overzicht van de release](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Scrumplanning voor Workfront Boards

De nieuwe functies voor de planning van scrum in Adobe Workfront Boards bieden flexibele opties voor het beheer van uw flexibele processen. Met de volgende gereedschappen kunt u:

* Trackwerk in herhalingen of sprints
* De snelheid van het gebruik om teamverplichtingen te begeleiden
* Spoorbelasting en voltooiingssnelheid

De planningsfuncties voor de scrum zullen na de release van 23.1 een &#39;snelle follow&#39; zijn.

## Vervaldatums op kaarten die zijn toegewezen aan de geplande voltooiingsdatum op Workfront-objecten

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

Vervaldatums op verbonden kaarten in Workfront Boards zijn nu gekoppeld aan de geplande voltooiingsdatum op het bijbehorende Workfront-object. Als u de vervaldatum op een kaart bijwerkt, wordt de geplande voltooiingsdatum bijgewerkt op de taak of de uitgave. Als de geplande datum van voltooiing wordt gewijzigd, verandert ook de vervaldatum op de kaart. Eerder was de vervaldatum van de kaart een handmatige invoer en was deze niet toegewezen aan een datum op een taak of uitgifte.

Datumtoewijzing is ook van toepassing op verbonden controlelijstitems die worden gesynchroniseerd met subtaken.

De vervaldatum op zowel de aangesloten kaarten als de ad hoc kaarten omvat nu ook een tijdveld.

Zie voor meer informatie [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Controlelijstitems en Workfront-subtaken zijn nu gekoppeld

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

Wanneer u een aangesloten kaart aan een raad voor een taak van Workfront toevoegt, worden om het even welke subtaken ingevoerd als checklist punten op de kaart. Wanneer u een controlelijstitem maakt op een aangesloten kaart, wordt ook een subtaak toegevoegd aan de Workfront-taak. De controlelijstitems voor problemen zijn niet verbonden met Workfront-objecten.

Eerder waren items en subtaken in de controlelijst niet gekoppeld. Als u een subtaak in het bord wilt opnemen, kunt u deze importeren als een aparte, aangesloten kaart of handmatig een item uit de controlelijst aan een kaart toevoegen.

Zie voor meer informatie [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) en [Controlelijstitems op kaarten beheren](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Kaartteller aan boord van kolommen

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

Een nieuwe configuratie-instelling is beschikbaar om een kaartteller voor alle kolommen op een board in te schakelen. Als u de grens van het KLOOFJE op een kolom gebruikt, wordt een afzonderlijke kaartteller niet toegevoegd.

Zie voor meer informatie [Bordkolommen beheren](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Zoeken en sorteren op het dashboard voor tekengebieden

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt het dashboard van de boards nu sorteren op bordnaam of datum, en naar een specifieke raad in de lijst zoeken.

Zie voor meer informatie [Het dashboard voor tekengebieden gebruiken](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Statusweergave op kaart

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

Als aan een kaart op een kaart de status is toegewezen, wordt de status nu weergegeven op de kaart zodat u de kaart niet hoeft te openen om de status te zien. Deze verbetering geldt zowel voor ad-hockaarten als voor kaarten met een verbinding.

Zie voor meer informatie [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) en [Een ad-hockaart aan een kaart toevoegen](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![status op kaart](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Koppelbare kaarten zijn nu beschikbaar op borden

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt nu een koppeling naar een specifieke kaart naar een andere gebruiker van een kaart verzenden. De persoon moet toegang hebben tot het bord voordat hij of zij de koppeling kan openen.

Wanneer u een kaart op een bord opent, ziet de browser URL er als volgt uit:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

U kunt de volledige URL kopiëren en naar iemand anders verzenden. Ze zullen rechtstreeks naar de open kaart gaan wanneer ze de link openen.

Eerder waren er koppelingen beschikbaar naar borden, maar niet naar specifieke kaarten.

Voor informatie over kaarten raadpleegt u [Een ad-hockaart aan een kaart toevoegen](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) en [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filteren op verbinding aan boord

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

De lijst met filters op een bord bevat nu de optie om via verbinding te filteren. Hierin ziet u alle aangesloten kaarten voor een bepaald project. U kunt ook filteren op kaarten die niet zijn aangesloten.

Zie voor meer informatie [Filteren en zoeken in een board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Kaarten archiveren van een bord volgens een schema

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt een kaart zodanig configureren dat kaarten volgens een schema worden gearchiveerd of &#39;van de kaart vallen&#39;. Er zijn opties beschikbaar om kaarten in een bepaalde kolom in te stellen voor archivering in een bepaald aantal dagen of weken. U kunt bijvoorbeeld het wegvallen definiëren, zodat kaarten in een kolom Voltooien worden gearchiveerd nadat ze gedurende twee weken in de kolom staan.

Als u de kaarten weer wilt weergeven nadat ze van het bord zijn gevallen, kunt u het bordfilter instellen op het weergeven van gearchiveerde kaarten.

Zie voor meer informatie [Afvalfunctie van kaart configureren](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Een videodemonstratie van deze functie weergeven](https://video.tv.adobe.com/v/3412323/){target=_blank}
