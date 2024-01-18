---
title: 21.4 Projectverbeteringen
description: 21.4 Projectverbeteringen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# 21.4 Projectverbeteringen

Op deze pagina worden alle projectverbeteringen beschreven die zijn aangebracht met de release 21.4 voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving in de week van 4 oktober 2021.

Voor een lijst van alle veranderingen beschikbaar met versie 21.4, zie [21.4 Overzicht van de release](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Afbeeldingen opnemen in updates

Op het tabblad Updates van een object kunt u nu afbeeldingen toevoegen door op het pictogram Afbeelding op de werkbalk te klikken. U kunt ook een afbeelding naar het updategebied slepen. De Workfront-beheerder moet het toevoegen van afbeeldingen inschakelen voordat u het afbeeldingspictogram kunt zien.

U kunt afbeeldingen zowel in updates als in reacties toevoegen. Een afbeeldingsminiatuur in de update geeft aan dat ontvangers een voorvertoning van de afbeelding in de browser kunnen bekijken of deze kunnen downloaden, en uit e-mail- en in-app-meldingen blijkt dat de afbeeldingen aan de update zijn gekoppeld.

Eerder was de enige manier om een afbeelding te delen in Workfront dat u deze aan een object koppelde als een document. Afbeeldingen die zijn toegevoegd op het tabblad Updates, zijn alleen beschikbaar op dat tabblad en niet op het tabblad Documenten.

Zie voor meer informatie [Werk bijwerken](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Voordat Workfront-gebruikers afbeeldingen kunnen opnemen in updates, moet deze functie eerst worden ingeschakeld door de Adobe Workfront-beheerder, zoals beschreven in [Voorkeuren voor gebruikersupdates configureren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Bijgewerkt algoritme voor slimme toewijzingen

We hebben het algoritme verbeterd dat wordt gebruikt bij het maken van slimme toewijzingen. Met de nieuwe verbetering, bekijkt Workfront de 30 meest recente taken die door het programma geopende gebruiker worden gemaakt om suggesties te doen wanneer zij taken en kwesties toewijzen. De lijst met suggesties kan maximaal 50 gebruikers bevatten.

Voorafgaand aan deze verbetering, bezat Workfront de taken op de oudertaken en andere gebruikersattributen met betrekking tot die taken wanneer het adviseren van gebruikers.

Zie voor informatie over slimme toewijzingen [Overzicht van slimme toewijzingen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nieuwe ervaring bij het maken van een project op basis van een sjabloon

Om uw gebruik van Workfront in overeenstemming te brengen met de nieuwe ervaring van Workfront, hebben wij de interface voor het creëren van een project van malplaatje opnieuw ontworpen. De functionaliteit voor het maken van een project met een sjabloon is niet gewijzigd. Nochtans, omvatten sommige verbeteringen van deze onlangs opnieuw ontworpen interface het volgende:

* Sjabloongegevens voorvertonen voordat u deze koppelt
* Voeg malplaatjes aan een lijst van favorieten tijdens het proces van de projectverwezenlijking toe

Wij hebben de interface voor het creëren van het project bijgewerkt zowel wanneer u het van de Projecten evenals van het gebied van Malplaatjes creeert.

Ter informatie: [Een project maken met een sjabloon](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nieuwe ervaring bij het koppelen van sjablonen aan projecten

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

Om uw gebruik van Workfront in overeenstemming te brengen met de nieuwe ervaring van Workfront, hebben wij de interface voor het vastmaken van een malplaatje aan een project opnieuw ontworpen. De functionaliteit voor het koppelen van een sjabloon is niet gewijzigd. Nochtans, zijn er sommige verbeteringen van deze onlangs opnieuw ontworpen interface die het volgende omvatten:

* Sjabloongegevens voorvertonen voordat u deze koppelt
* Sjablonen toevoegen aan een lijst met favorieten tijdens het bijlageproces
* Alle opties voor het beheer van sjabloon- en projectinstellingen in één doorlopende pagina weergeven

Zie voor meer informatie [Een sjabloon aan een project koppelen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Verenigde duur en duureenheidwaarden voor taken

Voor een schonere en meer gestroomlijnde gebruikerservaring, hebben wij de waarde van het gebied van de Duur met de duureenheid van tijd samengevoegd. Voorafgaand aan deze verbetering, de eenheid van tijd die op een afzonderlijk drop-down gebied na het gebied van de Duur wordt getoond.

Naast de gebieden van de Duur in de de Details van de Taak, geeft Taken en Nieuwe Taakdozen uit, werken wij ook de volgende gebieden bij om deze ervaring aan te passen:

* Veld voor duur bij het maken van geavanceerde toewijzingen
* Het veld Vertraging niveaus bij het maken of bewerken van een taak
* Frequentieveld bij het maken van een terugkerende taak (binnenkort beschikbaar)
* Veld labelen bij het toevoegen van een voorganger (binnenkort beschikbaar)

Zie voor meer informatie [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Inline toevoegen van problemen in projecten uitschakelen

Om ervoor te zorgen dat de gebruikers nauwkeurige informatie verstrekken wanneer het toevoegen van kwesties aan projecten door een uitgifteformulier in te vullen, hebben wij een nieuw plaatsen geïntroduceerd die u toestaat om te beheren of zij kwesties aan een project of zijn taken kunnen inline toevoegen. Deze instelling is standaard ingeschakeld in het gebied Instellingen nieuwe uitgave van het vak Project bewerken. Als u deze optie uitschakelt, wordt de optie Meer problemen toevoegen in de sectie Problemen van een project grijs weergegeven zodat gebruikers geen problemen meer in de lijst kunnen toevoegen. De gebruikers kunnen nog kwesties aan de projecten toevoegen door de Nieuwe optie van de Uitgave in de sectie van Kwesties te gebruiken of een verzoekrij te gebruiken als voor het project wordt gevormd.

>[!NOTE]
>
>Deze instelling is alleen beschikbaar in de nieuwe Workfront-ervaring. Gebruikers die in Workfront klassiek werken, kunnen nog steeds inline problemen toevoegen aan een project of aan de taken ervan, zelfs als deze instelling voor het project is uitgeschakeld door een gebruiker die in de nieuwe Workfront-ervaring werkt.

Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

## Verbeterde weergave van aangepaste velden voor selectievakjes en keuzerondjes

Het weergeven en selecteren van opties voor selectievakjes en keuzerondjes in aangepaste formulieren is nu eenvoudiger geworden. Een aangepast veld met veel opties voor selectievakjes of keuzerondjes wordt nu in meerdere kolommen op de pagina weergegeven. Eerder werden ze in één kolom weergegeven. Hiervoor moesten gebruikers extra schuiven om het formulier in te vullen.

Dit hangt af van de positie van de velden in het aangepaste formulier. Als u een ander veld in dezelfde rij plaatst met het selectievakje of keuzerondje, hebben de opties mogelijk slechts voldoende horizontale ruimte om in één kolom weer te geven.

Zie voor informatie over het invullen van een aangepast formulier [Gegevens bewerken in aangepaste formuliervelden](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Zie de secties voor informatie over het maken van een selectievakje of keuzerondje in een aangepast formulier [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) en [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) in het artikel [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

