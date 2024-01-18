---
title: 22.1 Verbeteringen voor beheerders
description: 22.1 Verbeteringen voor beheerders
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 22.1 Verbeteringen voor beheerders

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de versie 22.1 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

de week van 17 januari 2022.

Zie voor een lijst met alle wijzigingen die beschikbaar zijn in de versie 22.1 [22.1 Overzicht van de release](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Documentdownloads zijn aangemeld in het gebied Updates

Om uw gebruikers te helpen het downloaden van documenten volgen die zij in Workfront opslaan, registreert het systeem nu een ingang in het gebied van Updates voor een document wanneer iemand het downloadt.

>[!NOTE]
>
>We raden u aan deze functie te testen in Voorvertoning op een nieuw geüpload document.

Ga voor meer informatie over hoe Workfront automatische updates van objecten registreert [Door het systeem bijgehouden updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Toegang verlenen aan teams die gebruikmaken van toegangsniveaus

Een nieuwe sectie in het gebied van de Niveaus van de Toegang geeft u meer korrelige controles voor het beheren van de toegang van uw gebruikers tot teams. Nu kunt u bepalen wie teams kan maken, bewerken en weergeven.

Dit verandert niets de bestaande toegang van uw gebruikers tot teams.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Groepstoewijzing nu beschikbaar in blauwdrukken

Sommige blauwdrukken bevatten nu groepen die u kunt aanpassen voordat u de blauwdruk installeert. U kunt een groep in de blauwdruk toewijzen aan een bestaande groep in uw Workfront-instantie of zo nodig een nieuwe groep maken.

Zie voor meer informatie [Een blauwdruk configureren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Updates opmaken in het gebied Aangepaste Forms

Het aangepaste Forms-gebied heeft een nieuw uiterlijk dat het up-to-date brengt met vele andere gebieden in de nieuwe Workfront-ervaring.

Voor informatie over het maken van een aangepast formulier raadpleegt u [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Veel verbeteringen voor het maken van berekende aangepaste velden

Het maken van berekende aangepaste velden is nu veel eenvoudiger met deze toevoegingen in de nieuwe Rekeningeditor:

* U kunt over om het even welke uitdrukking in uw berekening bewegen om informatie over het, met inbegrip van een beschrijving, een voorbeeld van hoe het kan worden gebruikt, en een verbinding aan meer informatie in een hulpartikel te tonen.
* Elke expressie die u toevoegt, heeft een kleurcode, afhankelijk van het type. Hierdoor is het gemakkelijker om uw expressies te vinden en het type ervan direct te herkennen.
* Met regelnummers kunt u functies in een lange berekening identificeren en ernaar verwijzen.
* Wanneer u een expressie of veldnaam begint te typen, wordt een lijst met beschikbare items weergegeven, zodat u de gewenste optie kunt kiezen. En wanneer u een haakje openen typt, wordt het haakje sluiten automatisch toegevoegd.
* U kunt het resultaat van de berekening voorvertonen met een bestaand object zonder de berekeningseditor te verlaten.

In de aanpasbare tekst Instructies voor een berekend aangepast veld kunt u ook de formule van het veld weergeven of verbergen. Dit is handig als u denkt dat de gebruikers die het aangepaste formulier invullen, deze informatie niet nodig hebben.

Zie voor meer informatie over het maken van een berekend aangepast veld [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## De informatie van het controlelogboek van de mening over statussen en bedrijven

Nu kunt u incidenten met statussen en bedrijven gemakkelijker oplossen door informatie over hen in het gebied van de Logboeken van de Controle in Opstelling te bekijken.

Bijvoorbeeld:

* U kunt erachter komen wie de naam van de status heeft gewijzigd, wie de status heeft vergrendeld of verborgen en wanneer ze dat hebben gedaan.
* U kunt erachter komen wie sommige leden of baanrollen van een bedrijf heeft verwijderd, en wanneer zij dit deden.

Voor informatie over het bekijken van de informatie van het controlelogboek, zie [Controleverslagen weergeven en exporteren](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blauwdrukbedrijven in kaart brengen en andere verbeteringen

De volgende verbeteringen voor blauwdrukken zijn nu beschikbaar:

* Sommige blauwdrukken bevatten nu bedrijven die u kunt aanpassen voordat u de blauwdruk installeert. U kunt een bedrijf in de blauwdruk aan een bestaand bedrijf in uw instantie van Workfront in kaart brengen, of een nieuw bedrijf tot stand brengen indien nodig.
* Er is nu een nieuw blauwdruktype beschikbaar, de Organizational Structure. Sommige blauwdrukken bevatten elementen van meerdere typen (bijvoorbeeld Projectsjabloon en Organisatiestructuur). U kunt filteren op het type blauwdruk op de cataloguspagina.
* De secties &quot;Voorkeuren installeren&quot; en &quot;Sjablooneigendom&quot; op de configuratiepagina zijn voor de eenvoud gecombineerd tot &quot;Sjabloonvoorkeuren&quot;.

Zie voor meer informatie [Een blauwdruk configureren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Beheer bedrijfslidmaatschappen gemakkelijker

In het gebied van Bedrijven, maakt een bijgewerkte toolbar het gemakkelijk om bestaande gebruikers van Workfront aan een bedrijf toe te voegen en bedrijfsleden te verwijderen.

Eerder waren deze acties alleen beschikbaar in het vak Bedrijf bewerken.

De bijgewerkte werkbalk bevat ook alle acties die beschikbaar waren op de vorige werkbalk, zoals het bewerken van de gebruikersprofielgegevens van leden en het deactiveren van deze gegevens in het systeem.

Zie voor meer informatie [Ondernemingslidmaatschappen beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Expressies en velden selecteren in het nieuwe berekende veldvenster

We maken het nog steeds gemakkelijker om een berekend veld te maken in een aangepaste vorm. Wanneer u nu op Maximaliseren klikt om de nieuwe berekeningseditor te openen, kunt u de gewenste expressies en velden zoeken en selecteren.

Zie voor meer informatie [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## De groepen kunnen hun eigen timesheet en uurvoorkeur vormen

>[!NOTE]
>
>Deze functie was aanvankelijk alleen beschikbaar als onderdeel van een gefaseerde implementatie voor klanten met Cluster 4 als onderdeel van de release 21.4. Deze functie is beschikbaar voor alle resterende clusters in Production op 8 november 2021.

In een grote organisatie, zouden sommige groepen timesheet en uurvoorkeur onafhankelijk kunnen moeten vormen om hun unieke werkschema&#39;s te passen, eerder dan het erven van de voorkeur die door een beheerder op het systeemniveau wordt gevormd. Nu kunnen de beheerders van Workfront een timesheet en een uurvoorkeur voor alle groepen in het systeem ontgrendelen zodat zij het op hun kunnen vormen.

Deze mogelijkheid is onlangs ook toegevoegd voor projectvoorkeuren en voor voorkeuren voor taken en uitgaven.

Voor informatie over hoe een beheerder van Workfront een timesheet en een uurvoorkeur ontgrendelt, zie de sectie [Tijdschema en uurvoorkeuren voor groepen ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) in het artikel [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Voor informatie over hoe een groepsbeheerder ontgrendelde taken en voorkeuren voor de afgifte van een groep configureert, raadpleegt u [Voorkeuren voor tijdschriften en uren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Meerdere meldingen selecteren die u wilt ontgrendelen of opnieuw vergrendelen voor groepen

Het is nu sneller en eenvoudiger om e-mailberichten voor groepen te ontgrendelen of opnieuw te vergrendelen. Nu kunt u meerdere meldingen selecteren, uw selecties controleren om te controleren of deze correct zijn en vervolgens op de nieuwe knop Ontgrendelen of Vergrendelen op de werkbalk klikken.

Eerder moest u meldingen een voor een ontgrendelen en opnieuw vergrendelen. Workfront heeft momenteel 95 meldingen, dus het duurde even voordat u dit voor al deze of vele ervan moest doen.

Zie voor meer informatie [Configuratie van gebeurtenismeldingen voor alle groepen ontgrendelen of vergrendelen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Voor groepsbeheerders: eenvoudiger om een vervangingsgroep te selecteren wanneer u een groep verwijdert

Wanneer u een groep verwijdert, kunt u met twee verbeteringen in het vak Groep verwijderen de vervangingsgroep selecteren die u wilt behouden voor de gebruikers, werkitems en subgroepen van de verwijderde groep:

* U kunt de naam van de groep typen om deze snel te vinden. Eerder was er alleen een vervolgkeuzelijst die u niet kon typen. Dit was problematisch voor organisaties met vele groepen omdat u door de lijst moest scrollen om de groep te vinden u wilde. Bovendien had de vervolgkeuzelijst een itemlimiet, zodat het mogelijk was dat de gewenste groep niet werd weergegeven.
* U kunt het nieuwe infopictogram gebruiken om ervoor te zorgen u de vervangingsgroep selecteert u wilt. Als u de muisaanwijzer op het pictogram plaatst, wordt knopinfo met informatie over de groep weergegeven, zoals de hiërarchie van de bovenliggende groepen en de namen van de beheerders.

Zie voor meer informatie [Een groep verwijderen](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Groter gebied voor het maken van berekende velden

Het is nu gemakkelijker om complexe berekende velden te maken in een aangepast formulier. Klik op de nieuwe knop Maximaliseren om een groot bewerkvenster te openen waarin u uw berekening kunt samenstellen. Als u klaar bent, klikt u op Minimaliseren om verder te gaan met het bewerken van uw aangepaste formulier.

Zie voor meer informatie [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Aangepaste formulieren toevoegen aan groepen

Aangepaste formulieren worden nu ondersteund voor het Group-object. Hierdoor wordt het voor groepen in uw organisatie gemakkelijker om informatie vast te leggen en te delen die aan hun specifieke behoeften en workflows voldoet. Gebruikers kunnen het volgende doen voor een groep, net als voor andere Workfront-objecten:

* Een aangepast formulier maken
* Een aangepast formulier bijvoegen
* Aangepaste formuliergegevens opslaan
* Een aangepast formulier verwijderen
* Aangepaste gegevens bewerken uit lijsten en, in de nieuwe Workfront-ervaring, uit de pagina Groep

Voor informatie over aangepaste formulieren raadpleegt u [Aangepaste formulieren](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## OAuth2-apps maken om toepassingen te integreren met Workfront

Nu kunt u Workfront integreren met andere toepassingen waarvoor Workfront geen ingebouwde integratie biedt. Door een OAuth2-app te maken voor de toepassing waarmee u wilt integreren, kunt u die toepassing toegang geven tot Workfront, terwijl u weet dat uw gegevens worden beveiligd door het veilige, industriestandaard OAuth2-verificatieprotocol.

Eerder kon u alleen integreren met andere toepassingen via ingebouwde integratie, Workfront Fusion of de Workfront API.

Zie voor meer informatie [OAuth2-toepassingen maken voor Workfront-integratie](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Verbeteringen in interfacetekst in het gebied Ondernemingen

In het gebied van Bedrijven in Opstelling, maken de nieuwe bevestigingsberichten en de lichte formuleringsveranderingen het gemakkelijker om het lidmaatschap van het bedrijf te beheren. De sectienaam &quot;Personen&quot; in het linkerdeelvenster is bijvoorbeeld &quot;Bedrijfsleden&quot;.

Voor informatie over het beheren van bedrijflidmaatschappen, zie [Ondernemingslidmaatschappen beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
