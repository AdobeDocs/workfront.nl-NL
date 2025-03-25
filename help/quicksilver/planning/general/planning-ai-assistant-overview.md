---
title: Adobe Workfront Planning AI Assistant - Overzicht
description: U kunt de AI-assistent gebruiken om records te genereren, bij te werken of te verwijderen die zijn gebaseerd op de context van de huidige pagina en de recordstructuur. De bevelen van de gebruiker en de uitvoering van AI van die bevelen werken samen om ervoor te zorgen dat de veranderingen door AI worden aangebracht nauwkeurig in uw milieu worden weerspiegeld.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant - overzicht

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


{{planning-important-intro}}

Met de AI-assistent kunt u records genereren, bijwerken of verwijderen op basis van de context en de recordstructuur van de huidige pagina.

De bevelen van de gebruiker en de uitvoering van AI van die bevelen werken samen om ervoor te zorgen dat de veranderingen door AI worden aangebracht nauwkeurig in uw milieu worden weerspiegeld.

## Overwegingen over de AI-assistent

* De AI-assistent moet zijn ingeschakeld voor uw organisatie voordat deze beschikbaar is voor gebruikers in uw bedrijf. Voor informatie, zie [ AI Hulpoverzicht ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Nadat Workfront de AI Assistant voor uw organisatie heeft ingeschakeld, is deze beschikbaar voor de Workfront-hoofdbeheerder. Voor informatie, zie [ basisinformatie voor uw systeem ](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

* De Workfront-beheerder moet de AI-assistent inschakelen voor alle andere gebruikers. Voor meer informatie, zie [ toelaten of AI Medewerker ](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) onbruikbaar maken.

* De AI Assistant werkt in de context van elke pagina. De aanvragen die u voor de AI-assistent indient, moeten verwijzen naar functionaliteit die beschikbaar is op de pagina die u hebt geopend.

* De acties die door de AI Medewerker in het Gebied van de Planning worden uitgevoerd zijn in de context van uw toestemmingen van de Planning van Workfront en uw toegangsniveau van Workfront. Raadpleeg de volgende artikelen voor meer informatie:

   * [Overzicht van het delen van machtigingen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Overzicht van licentietype bij gebruik van Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Wijzigingen die de AI-assistent namens de gebruiker aanbrengt, worden bijgehouden in het deelvenster Historie van de record.

* Met opdrachten kunt u handelingen ongedaan maken. U kunt bijvoorbeeld &quot;Laatste wijziging ongedaan maken&quot; typen om de wijziging ongedaan te maken.

* <span class="preview"> Wanneer u een object maakt, bijwerkt of verwijdert via AI Assistant, geeft AI Assistant de beoogde acties weer en wordt om bevestiging gevraagd. U kunt de acties vervolgens bevestigen of annuleren. </span>

## Momenteel beschikbare functionaliteit voor de AI-assistent

Momenteel is de AI Assistant beschikbaar in het planningsgebied van Workfront voor de volgende pagina&#39;s:

* Workspace-pagina
* Tekstpagina opnemen
* Pagina opnemen

Met de AI-assistent kunt u op dit moment de volgende handelingen uitvoeren:

* Zoeken naar records. U kunt zoeken op informatie in alle recordvelden.
* Records maken. Een id met een koppeling naar de nieuwe record wordt weergegeven nadat de record is gemaakt. U kunt opgeven welke velden u wilt bijwerken tijdens het maken, zoals datums of beschrijving.
* Maak records op basis van een document dat u uploadt. Workfront ondersteunt de volgende documentindelingen voor de AI Assistant:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT en de meeste afbeeldingsindelingen
* Velden bijwerken voor de records die u op het scherm ziet
* Records verwijderen
* Recten herstellen die u zojuist hebt verwijderd


## AI Assistant zoeken in Workfront-planning

U kunt de AI-assistent vinden op de volgende gebieden van de Workfront-planning:

* De hoofdnavigatiebalk, in de rechterbovenhoek van het scherm.
* Binnen het detailsgebied van een record, nadat u de record in de voorvertoning hebt geopend of nadat u de recordpagina hebt geopend.

## De AI-assistent openen in het planningsgebied

1. Login aan Workfront, dan klik het **pictogram van het Belangrijkste Menu ![ het belangrijkste menu van Dots ](assets/dots-main-menu.png) in de hoger-juiste hoek van het scherm, of het** Belangrijkste **pictogram ![ het belangrijkste menu van Lijnen ](assets/lines-main-menu.png) in de upper-left hoek, als beschikbaar.**

. Klik **Planning**. Het planningsgebied wordt geopend.

1. Klik a **werkruimtekaart**.

1. (Facultatief) klik a **verslagtype kaart**.

1. (Facultatief) klik a **verslag** om de 2} Details van het verslag **pagina te openen.**

1. Klik het **AI Hulppictogram** in de hoger-juiste hoek van het scherm in de globale navigatiebar of in de hoger-juiste hoek van de voorproef of de pagina van het verslag.

   ![ AI Hulp pictogram ](assets/ai-assistant-icon-highlighted.png)

1. Typ in de beschikbare ruimte opdrachten voor de AI-assistent en klik vervolgens op Enter wanneer u klaar bent.

   ![ AI Medewerker paneel met lege beveldoos ](assets/ai-assistant-panel-with-empty-command-box.png)

   U kunt bijvoorbeeld een van de volgende typen:

   * Maak een campagne met een startdatum van 4 juli en een einddatum van 30 juli
   * Het veld Beschrijving van de record in de zomercampagne bijwerken met de datum die moet worden bepaald
   * Laatste record verwijderen
   * De record herstellen

   Een visuele indicator toont terwijl de Medewerker AI bevelen verwerkt, die verwachtingen voor reactietijd plaatsen.

   Na ontvangst van een succesvolle reactie, volg de verstrekte verbindingen of merk de veranderingen op de linkerzijde op.



