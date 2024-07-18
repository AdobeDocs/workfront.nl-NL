---
title: 22.4 Beheerdersverbeteringen
description: 22.4 Beheerdersverbeteringen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 22.4 Beheerdersverbeteringen

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de versie 22.4 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de week van 3 oktober 2022.

Voor een lijst van alle veranderingen beschikbaar met de versie 22.4, zie [ overzicht van de Versie 22.4 ](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Onvergrendelde statussen gebruiken in een goedkeuringsproces

>[!NOTE]
>
>Deze functie werd voor het eerst geïntroduceerd in de voorvertoningsomgeving tijdens de releaseperiode van 22.3. Op 15 september 2022 wordt het product vrijgegeven aan Production.

Om u meer controle over de goedkeuringsprocessen en statussen in uw systeem te geven, hebben wij het mogelijk gemaakt om een goedkeuringsproces tot stand te brengen dat op een open systeemstatus wordt gebaseerd. Bovendien kunt u nu elke status ontgrendelen die al in een goedkeuringsproces wordt gebruikt. Eerder moest een systeemstatus die in een goedkeuringsproces werd gebruikt, worden gesloten. Dit maakte het beschikbaar voor alle groepen-zonder de mogelijkheid om het te verwijderen of anders te noemen-zodat konden de groepsbeheerders de lijst van statussen van hun groep niet stroomlijnen om hun specifieke behoeften te passen.

## Het pictogram Vervagen in het hoofdmenu wordt nu bestuurd via lay-outsjablonen

Systeembeheerders kunnen nu het pictogram Vervagen in het hoofdmenu toevoegen of verwijderen via de configuratie van de lay-outsjabloon. Hierdoor hebt u meer controle over wie door de catalogus Blauwdrukken kan bladeren.

Het pictogram Vervagen wordt weergegeven in het hoofdmenu wanneer:

* Er is geen lay-outsjabloon toegewezen aan de gebruiker

* De lay-outsjabloon van de gebruiker heeft de optie Vervagen in de lijst Actieve items

* De lay-outsjabloon van de gebruiker heeft de optie Vervagen in de lijst Beschikbare items. Het pictogram wordt niet weergegeven in het hoofdmenu.

Bestaande lay-outsjablonen bevatten automatisch het pictogram Vervagen en beheerders kunnen het pictogram verwijderen uit lay-outsjablonen om de zichtbaarheid van de catalogus Vervagen te beperken. De nieuwe lay-outmalplaatjes die na de versie 22.4 worden gecreeerd zullen het pictogram van Vervagen in de Actieve lijst van Punten omvatten.

Voor meer informatie, zie [ toegang tot Vervagen ](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md) vormen.

[ Bekijk een videodemonstratie van deze eigenschap ](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Aanpassing koptekst van probleem

Als Workfront- of groepsbeheerder kunt u nu de velden aanpassen die in de koptekst van een uitgave worden weergegeven wanneer u een lay-outsjabloon gebruikt.

Deze update bevat de volgende verbeteringen:

* Verwijder bestaande velden of wijzig de rangschikking van deze velden in de koptekst van de uitgave.

* Voeg nieuwe, niet-bewerkbare velden voor het overzicht van problemen toe. U kunt geen aangepaste velden of velden toevoegen die kunnen worden bewerkt. U kunt ook bewerkbare velden weergeven die zich momenteel in de uitgiftheader bevinden (bijvoorbeeld Status of Percentage voltooid).

* De uitgiftheader kan maximaal vijf velden bevatten.

* U kunt nu het veld &quot;Opgelost door&quot; toevoegen aan de uitgiftheader. Wanneer een oplossend voorwerp met de kwestie wordt geassocieerd, verandert het &quot;Opgeloste door&quot;gebied in &quot;Oplossend Kwestie,&quot;Oplossende Taak,&quot;of &quot;Oplossend Project,&quot;afhankelijk van het type van voorwerp dat met de kwestie wordt geassocieerd.

Vóór deze versie, slechts konden de project en taakkopballen worden aangepast.



Voor meer informatie, zie [ objecten kopballen aanpassen gebruikend een lay-outmalplaatje ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[ Bekijk een videodemonstratie van deze eigenschap ](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Aanpassing taakkoptekst

Als Workfront- of groepsbeheerder kunt u nu de velden aanpassen die in de koptekst van een taak worden weergegeven wanneer u een lay-outsjabloon gebruikt.

Deze update bevat de volgende verbeteringen:

* Verwijder bestaande velden of wijzig de volgorde van deze velden in de taakkoptekst.

* Voeg nieuwe, niet-bewerkbare gebieden van het Overzicht van de Taak toe. U kunt geen aangepaste velden of velden toevoegen die kunnen worden bewerkt. U kunt ook bewerkbare velden weergeven die zich momenteel in de taakkoptekst bevinden (bijvoorbeeld Status of Percentage voltooid).

* De taakkoptekst kan maximaal vijf velden bevatten.

Voorafgaand aan deze versie, konden slechts projectkopballen worden aangepast.

Voor meer informatie, zie [ objecten kopballen aanpassen gebruikend een Malplaatje van de Lay-out ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[ Bekijk een videodemonstratie van deze eigenschap.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Aanmelden met vroege functies voor de nieuwste functies in de raden van bestuur

We zijn erg blij om nieuwe functies voor raden van bestuur te openen, zodat u de functie voor vroege aanmelding kunt gebruiken. Dit optionele hulpmiddel is beschikbaar voor alle organisaties.

Alleen een Workfront-beheerder kan zich aanmelden bij de eerste functies. Wanneer de beheerder in aan vroege eigenschappen kiest, worden alle gebruikers in de organisatie verkozen binnen, en de extra eigenschappen worden toegelaten in uw productieWorkfront milieu.

Voor meer informatie, zie [ vroege eigenschapopt-in voor de Boards van Adobe Workfront ](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[ Bekijk een videodemonstratie van deze eigenschap.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## In de berekeningeditor van het aangepaste formulierveld worden foutgegevens weergegeven

>[!NOTE]
>
>Deze functie werd voor het eerst geïntroduceerd in de voorvertoningsomgeving tijdens de releaseperiode van 22.3. Met de release van 22.4 gaat het naar Production.

Het bewerken van berekeningen voor aangepaste velden is nu gemakkelijker omdat nuttige foutinformatie rechtstreeks in de berekening wordt vermeld. Tijdens het maken van een berekend veld in een aangepast formulier worden fouten roze gemarkeerd. Wanneer u de muisaanwijzer op het gemarkeerde gedeelte plaatst, wordt knopinfo weergegeven waarin het probleem wordt beschreven.

Voor meer informatie, zie [ berekende gegevens aan een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) toevoegen.

[ Bekijk een videodemonstratie van deze eigenschap.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migratie naar Adobe Unified Experience

OPMERKING: Deze migratie is uitgesteld tot Q1-Q2 van 2023. Alle betrokken klanten zullen op dat moment op de hoogte worden gesteld.

Als uw organisatie aan de Adobe Admin Console is geregistreerd, zal uw instantie van Workfront naar de Adobe Verenigde Ervaring met de 22.4 versie worden gemigreerd.

De Adobe Verenigde Ervaring omvat:

* Eén aanmelding voor alle Adobe-toepassingen via Adobe Experience Cloud

* Een &quot;bedrijfsswitch&quot; om te schakelen tussen Workfront-organisaties en -omgevingen

* Navigatie met opties voor Workfront-pagina&#39;s, Adobe Experience Cloud-voorkeuren en uw Workfront-profiel

Voor meer informatie, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[ Bekijk een videodemonstratie van deze eigenschap.](https://video.tv.adobe.com/v/3412388/){target=_blank}
