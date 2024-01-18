---
title: 21.4 Verbeteringen voor beheerders
description: 21.4 Verbeteringen voor beheerders
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 21.4 Verbeteringen voor beheerders

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de versie 21.4 voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving in de week van 4 oktober 2021.

Voor een lijst van alle veranderingen beschikbaar met versie 21.4, zie [21.4 Overzicht van de release](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Voor beheerders: zie welke groepen aan een goedkeuringsproces worden geassocieerd

Om u te helpen te weten komen welke groepen met de goedkeuringsprocessen in uw systeem worden geassocieerd, hebben wij een kolom van de Naam van de Groep aan de Standaardmening op de pagina van Goedkeuringen in Opstelling toegevoegd. Nu kunt u deze gegevens weergeven zonder dat u een aangepaste weergave hoeft te maken.

Voor informatie over goedkeuringsprocessen raadpleegt u [Overzicht van goedkeuringsproces](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Voor informatie over het beheren van groepsgoedkeuringsprocessen raadpleegt u [Goedkeuringsprocessen op groepsniveau](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Nieuw voor beheerders: de groepen kunnen hun eigen timesheet en uurvoorkeur vormen

>[!NOTE]
>
>Aanvankelijk, in Productie, zal deze functionaliteit als deel van een gefaseerde uitrol slechts voor klanten op Cluster 4 beschikbaar zijn. Deze notitie wordt bijgewerkt wanneer de functionaliteit beschikbaar wordt voor andere clusters.

In een grote organisatie, zouden sommige groepen timesheet en uurvoorkeur onafhankelijk kunnen moeten vormen om hun unieke werkschema&#39;s te passen, eerder dan het erven van de voorkeur die door een beheerder op het systeemniveau wordt gevormd. Nu kunnen de beheerders van Workfront een timesheet en een uurvoorkeur voor alle groepen in het systeem ontgrendelen zodat zij het op hun kunnen vormen.

Deze mogelijkheid is onlangs ook toegevoegd voor projectvoorkeuren en voor voorkeuren voor taken en uitgaven.

Voor informatie over hoe een beheerder van Workfront een timesheet en een uurvoorkeur ontgrendelt, zie de sectie [Tijdschema en uurvoorkeuren voor groepen ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) in het artikel [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Voor informatie over hoe een groepsbeheerder ontgrendelde taken en voorkeuren voor de afgifte van een groep configureert, raadpleegt u [Voorkeuren voor tijdschriften en uren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Nieuw voor Workfront-beheerders: lay-outsjablonen configureren voor gebruikers met automatische provisioning in de nieuwe Workfront-ervaring

Nu kunt u lay-outmalplaatjes in de nieuwe ervaring van Workfront voor auto-provisioned gebruikers vormen. In het vervolgkeuzemenu Workfront-gebruikerskenmerken waarin u gebruikerskenmerken toewijst (Setup > Systeem > Single Sign-On), is een nieuw menu-item &quot;NWE Layout Template&quot; nu beschikbaar voor het maken van deze configuratie. Eerder, kon u lay-outmalplaatjes voor auto-provisioned gebruikers slechts in Workfront Klassiek vormen.

Zie voor instructies over het toewijzen van gebruikerskenmerken [Kenmerken van gebruikers toewijzen en nieuwe gebruikers automatisch instellen](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## In het nieuwe veld worden de groepen weergegeven waartoe uw gebruikers behoren

Nu is het gemakkelijk om te weten te komen tot welke groepen uw gebruikers behoren. In een rapport of een weergave waarin gebruikers worden vermeld, kunt u een kolom maken met het nieuwe veld Andere groepen. In dit veld worden de groepen weergegeven waarin elke gebruiker lid is.

Voor informatie over het gebruik van rapporten en weergaven raadpleegt u [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) en [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Op de pagina Blauwdrukdetails wordt nu een afbeelding weergegeven

De detailspagina voor elke blauwdruk toont nu een beeld van het projectmalplaatje dat met de blauwdruk geïnstalleerd is. De afbeelding bevat een voorvertoning van de blauwdrukinhoud, zodat u weet wat u gaat installeren. U kunt desgewenst een voorvertoning van de volledige afbeelding weergeven in de browser of de afbeelding downloaden.

Zie voor meer informatie [Overzicht van blauwdrukken](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Voorkeuren voor blauwdrukken voor nieuwe uitgaven

Voor sommige blauwdrukken zijn nu nieuwe uitgiftevoorkeuren beschikbaar. Ze worden standaard geïnstalleerd, maar u kunt de installatie van de voorkeuren uitschakelen wanneer u de installatiegegevens configureert.

De voorkeur omvat groepen van het rijonderwerp, rijonderwerpen, en het verpletteren van regels om de correcte informatie te verzamelen wanneer een kwestie of een verzoek wordt voorgelegd, en de kwestie of het verzoek naar de correcte baanrol of het team te verzenden. Het gebruik van de voorkeuren draagt bij aan consistentie in de manier waarop nieuwe problemen of verzoeken worden vastgelegd voor uw projecten.

Merk op dat het gebruiken van deze voorkeur niet de projecten maakt die van het malplaatje in verzoekrijen worden gecreeerd.

Zie voor meer informatie [Een blauwdruk configureren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Nieuw voor groepsbeheerders: onlangs verwijderde en herstelde items van een groep weergeven en beheren

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

We maken het nog steeds eenvoudiger om uw groepen en de bijbehorende objecten op één locatie te beheren. Nu kunt u de onlangs verwijderde en herstelde items van een groep weergeven en bewerken in het gebied Groepen. Hierdoor hoeft u niet naar het gebied Onlangs verwijderd of Onlangs hersteld in Setup te gaan om deze items te beheren. En het houdt de lijst van groepspunten u met werkt gescheiden van andere schrapte en herstelde punten in het systeem.

Zie voor meer informatie [Onlangs verwijderde items van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) en [Onlangs herstelde items van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Nieuw voor groepsbeheerders: groepsvoorkeuren zijn nu van invloed op groepssjablonen

Het is nu gemakkelijker om ervoor te zorgen dat de projectmalplaatjes van uw groep aan de behoeften van uw groep voldoen. Wanneer u een nieuw projectmalplaatje aan een groep op het tijdstip toewijst dat u het creeert, erft het malplaatje de volgende montages van het project en de taakvoorkeur van de groep:

* Prestatiesindexmethode
* Type voorwaarde
* Schema vanuit
* Gebruikerstijd uitgeschakeld
* Type bijwerken
* Instellingen voor toegang

Wanneer u een nieuwe malplaatjetaak binnen een projectmalplaatje creeert dat met een groep wordt geassocieerd, erft de malplaatjetaak de volgende montages van de de taakvoorkeur van de groep:

* Duur
* Type inkomsten
* Kostensoort

Eerder, werden de projectmalplaatjes en de taken van het projectmalplaatje geërft deze montages van het project en de taakvoorkeur die op het systeemniveau wordt geplaatst.

Als u een malplaatje of malplaatjetaak zonder een groep-voor voorbeeld, van de belangrijkste pagina van Malplaatjes creeert-hierboven montages van het project en de taakvoorkeur op systeemniveau worden geërft. Nochtans, als u later een groep aan het malplaatje of malplaatjetaak toewijst, beïnvloeden de voorkeur van de groep niet het.

Voor meer informatie, zie de sectie hoe de voorkeur op malplaatjes en malplaatjetaken in het artikel van toepassing is [De projectsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Nieuw voor beheerders: zoek op welke aangepaste formulieren een aangepast veld gebruiken

Het is nu eenvoudiger om een aangepast veld te wijzigen in een aangepast formulier. Met één klik in het aangepaste formulier kunt u meer informatie vinden over andere aangepaste formulieren die ook het veld gebruiken. Het is belangrijk om te beoordelen of die formulieren aanpassingen nodig hebben om correct te blijven werken nadat u de wijziging hebt aangebracht.

Zie voor meer informatie [Alle aangepaste formulieren weergeven die een bepaald aangepast veld of een bepaalde aangepaste widget gebruiken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Nieuw voor groepsbeheerders: Project, taak en uitgiftevoorkeuren voor een groep vergrendelen en ontgrendelen

Nu kunt u ervoor zorgen dat iedereen in de subgroepen onder uw groep dezelfde voorkeursinstellingen gebruikt, of u kunt deze gebruikers toestaan een voorkeursinstelling te configureren voor hun unieke workflows.

* Nadat een beheerder van Workfront een voorkeur op systeemniveau ontgrendelt, kunt u het voor alle subgroepen onder uw groep vormen en dan sluiten. Hoewel u de vergrendelde voorkeur nog steeds kunt aanpassen, kunnen beheerders van lagere subgroepen dit niet doen voor hun groepen.

  Omgekeerd kunt u een voorkeur voor uw groep ontgrendelen. Dit staat subgroepbeheerders toe om het voor hun unieke project, taak, of de behoeften van het probleemwerkschema te vormen.

  Zie voor meer informatie [Een project, taak of uitgave van subgroepen vergrendelen of ontgrendelen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Als u een Workfront-beheerder bent, hoeft u niet naar het gebied Groepen te gaan om de voorkeuren van een subgroep te configureren. In het gedeelte met voorkeuren voor het hoofdproject, de voorkeuren voor Taken en problemen of Tijdschema&#39;s en Uren kunt u het zoekvak boven aan de pagina gebruiken om de subgroep te zoeken en de voorkeuren te configureren.

  Zie voor meer informatie [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) en [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Nieuw voor groepsbeheerders: sjablonen maken en bewerken in het gebied Groepen

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Workfront-ervaring.

We maken het nog steeds eenvoudiger om uw groepen en de bijbehorende objecten op één locatie te beheren. Nu kunt u met de malplaatjes van een groep van het gebied van Groepen in Opstelling bekijken en werken. Hierdoor hoeft u niet naar het gebied Sjablonen te gaan om de sjablonen van een groep te beheren. En het houdt de lijst van groepsmalplaatjes u aan werkt gescheiden van de anderen door het systeem.

Zie voor meer informatie [De projectsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Gegevens invoeren en opslaan in één aangepast formulier tegelijk

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

Het is nu gemakkelijker om informatie in de sectie Details voor een voorwerp te verstrekken: Type en sparen informatie in één enkel douanegebied of uitbreidbaar gebied (zoals Overzicht en Financiën), zelfs als de vereiste gebieden in andere douaneformulieren op het voorwerp nog niet worden ingevuld.

Eerder, toen u informatie in één douaneformulier of uitbreidbaar gebied voor een voorwerp inging, gingen alle douaneformulieren in bijlage aan het voorwerp op bewerkingswijze en al hun vereiste gebieden moesten worden voltooid alvorens u uw veranderingen kon bewaren. Dit was een probleem als u een vereist veld niet kon voltooien omdat het voor een andere gebruiker was bedoeld.

Als u alle aangepaste formulieren en uitbreidbare gebieden in de sectie Details voor een object wilt bewerken, klikt u op Alles bewerken in het nieuwe menu Bewerken dat we aan het pictogram Bewerken hebben toegevoegd. U kunt ook in hetzelfde menu op een naam klikken om naar het aangepaste formulier of de aangepaste sectie te bladeren waar u wijzigingen wilt aanbrengen

>[!NOTE]
>
>Deze functie is oorspronkelijk vrijgegeven voor Voorvertoning met versie 21.3.

Om het voor alle niveaus van een organisatie gemakkelijker te maken om hun werkschema&#39;s onafhankelijk te beheren en te controleren, hebben wij de capaciteit geïntroduceerd om statussen voor subgroepen tot stand te brengen en te beheren. Nu, van de sectie van Groepen in Opstelling, kunt u het volgende voor groepen doen u op om het even welk niveau beheert:

* Een status voor een groep maken, bewerken, verwijderen en verbergen
* Een status vergrendelen voor een groep, zodat alle onderliggende subgroepen deze op dezelfde manier kunnen gebruiken
* Ontgrendel een status voor een groep zodat beheerders van lagere subgroepen deze kunnen aanpassen aan hun unieke behoeften
* De status van een groep instellen als standaardstatus
* De weergave van groepsstatussen op objecten opnieuw ordenen en verbergen

Workfront-beheerders kunnen dit ook doen (voor alle groepen).

Eerder was deze functionaliteit alleen beschikbaar voor groepen op hoofdniveau.

Zie voor meer informatie [Groepsstatussen beheren](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Nieuw voor Workfront-beheerders: Migreer lay-outsjablonen van Workfront Classic naar uw nieuwe Workfront-ervaring

>[!NOTE]
>
>Deze functie is op 1 juli 2021 beschikbaar gesteld voor de voorvertoningsomgeving. Het zal op 15 juli 2021 worden vrijgegeven in de productieomgeving.

Om u te helpen lay-outsjablonen te beheren terwijl uw gebruikers overstappen op het gebruik van de nieuwe Workfront-ervaring, hebben we een knop gemaakt waarmee u lay-outsjablonen kunt migreren van Workfront Classic naar de nieuwe ervaring zonder op de klantenondersteuning van Workfront te vertrouwen.

Eerder kon alleen Workfront Customer Support uw lay-outsjablonen migreren van Workfront Classic naar de nieuwe Workfront-ervaring.

## Wanneer het associëren van een malplaatje met een groep, selecteer een proces van de groepsgoedkeuring in de Details van de Rij en de Onderwerpen van de Rij

We hebben een nieuwe optie toegevoegd aan het proces waarbij een sjabloon aan een groep wordt gekoppeld. Nu kunt u groep-specifieke goedkeuringsprocessen voor kwesties in de Details van de Rij van het malplaatje of in één van zijn Onderwerpen van de Rij selecteren.

In 21.3, toen wij de capaciteit toevoegden om een groepsmalplaatje met een groep te associëren, kon u een groep-specifiek goedkeuringsproces in het malplaatje selecteren, maar u kon dit niet in de Details van de Rij van het malplaatje of de Onderwerpen van de Rij doen.

Zie voor meer informatie [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
