---
title: 22.3 Verbeteringen voor beheerders
description: 22.3 Verbeteringen voor beheerders
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 22.3 Verbeteringen voor beheerders

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de versie 22.3 voor de voorvertoningsomgeving. Deze verbeteringen zijn beschikbaar gesteld in de week van 11 juli 2022. Voor een lijst met alle wijzigingen die beschikbaar zijn in de release 22.3 gaat u naar [22.3 Overzicht van de release](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Adobe Workfront integreren met JumpSeat

U kunt nu JumpSeat integreren met Workfront om aangepaste, in-product richtlijnen voor uw gebruikers te maken. U hebt een Adobe Workfront Enterprise-licentie en een actief JumpSeat-abonnement nodig om de integratie in te schakelen.

Zie voor meer informatie [De integratie met JumpSeat configureren](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Standaardinstellingen van proefafdruk verplaatst naar Workfront

U kunt nu de volgende proefdrukinstellingen bewerken in het gedeelte Workfront instellen:

* Standaardinstellingen proefdrukken

* Instellingen voor proefafhandeling

Zie voor meer informatie [Standaardproefdrukinstellingen configureren](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Onvergrendelde statussen gebruiken in een goedkeuringsproces

**Opmerking:** Verwijderd uit de 22.3 Production release. Dit onderdeel zal naar verwachting op 15 september 2022 worden uitgebracht aan Production.

Om u meer controle over de goedkeuringsprocessen en statussen in uw systeem te geven, hebben wij het mogelijk gemaakt om een goedkeuringsproces tot stand te brengen dat op een open systeemstatus wordt gebaseerd. Bovendien kunt u nu elke status ontgrendelen die al in een goedkeuringsproces wordt gebruikt.

Eerder moest een systeemstatus die in een goedkeuringsproces werd gebruikt, worden gesloten. Dit maakte het beschikbaar voor alle groepen-zonder de mogelijkheid om het te verwijderen of anders te noemen-zodat konden de groepsbeheerders de lijst van statussen van hun groep niet stroomlijnen om hun specifieke behoeften te passen.

Raadpleeg de volgende artikelen voor meer informatie:

* [Een goedkeuringsproces voor werkitems maken](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Een status maken of bewerken](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Vergrendelde en ontgrendelde statussen op systeemniveau](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Een PDF-bestand toevoegen aan een aangepast formulier

We blijven u helpen aangepaste formulieren visueel en informatief te maken met nieuwe middelenwidgets die u kunt toevoegen, zoals afbeeldingen en video&#39;s. Nu kunt u een koppeling naar een PDF-bestand toevoegen aan een aangepast formulier. Wanneer het formulier aan een object is gekoppeld, kunnen gebruikers die met het object werken de PDF vanuit het formulier bekijken en ermee werken.

Zie voor meer informatie [Een afbeelding of andere middelenwidget toevoegen of bewerken in een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## In de berekeningeditor van het aangepaste formulierveld worden foutgegevens weergegeven

>[!NOTE]
>
>Deze functie is tijdelijk niet beschikbaar. Deze pagina wordt bijgewerkt wanneer de functie beschikbaar is.

Het bewerken van berekeningen voor aangepaste velden is nu gemakkelijker omdat nuttige foutinformatie rechtstreeks in de berekening wordt vermeld. Tijdens het maken van een berekend veld in een aangepast formulier worden fouten roze gemarkeerd. Wanneer u de muisaanwijzer op het gemarkeerde gedeelte plaatst, wordt knopinfo weergegeven waarin het probleem wordt beschreven.

Zie voor meer informatie [Berekende gegevens toevoegen aan een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Aanpassing van koptekst van project

Als Workfront- of groepsbeheerder kunt u nu de velden aanpassen die in de koptekst van een project worden weergegeven wanneer u een lay-outsjabloon gebruikt.

Deze update bevat de volgende verbeteringen:

* Verwijder bestaande gebieden uit de projectheader.

* Voeg nieuwe, niet-bewerkbare gebieden van het Overzicht van het Project toe. U kunt geen aangepaste velden of velden toevoegen die kunnen worden bewerkt. Bewerkbare velden die zich momenteel op de projectheader bevinden, kunnen op de koptekst blijven staan.

* De koptekst van het object kan maximaal vijf velden bevatten.


Vóór deze release konden de velden in de objectkoppen niet worden aangepast.

Zie voor meer informatie [Objectkoppen aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Besturing voor het maken van een leeg project

Als systeem of groepsbeheerder, kunt u nu controleren of de gebruikers lege projecten kunnen tot stand brengen, zonder een malplaatje te gebruiken. Wij hebben nieuw het plaatsen in het gebied van de Voorkeur van het Project van Opstelling geïntroduceerd die u toestaat om het creëren van lege projecten op de volgende gebieden onbruikbaar te maken:

* Van de Nieuwe optie van het Project in een lijst van projecten

* Wanneer het omzetten van een kwestie in een project van de uitgiftepagina


Het nieuwe plaatsen is &quot;staat gebruikers toe om projecten tot stand te brengen zonder een malplaatje te gebruiken&quot;en het wordt toegelaten door gebrek.

**Opmerking:** Gebruikers kunnen een taak nog steeds omzetten in een leeg project.

Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Een groep deactiveren op de pagina Groepen

Onlangs hebben we de mogelijkheid toegevoegd om groepen te deactiveren en opnieuw te activeren. Om die actie sneller en gemakkelijker te maken, hebben wij het aan de pagina van een groep toegevoegd. Nadat u op de naam van een groep hebt geklikt om naar de bijbehorende pagina te gaan, kunt u het menu Meer selecteren ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) naast de naam van de groep selecteert u Deactiveren of Opnieuw activeren.

Eerder kon u een groep alleen deactiveren of opnieuw activeren met het selectievakje Is actief op de pagina Details.

Zie voor meer informatie [Een groep deactiveren of opnieuw activeren](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Video&#39;s toevoegen aan aangepaste formulieren

Nu kunt u een nieuwe wijze van informatie, visuele interesse, en creativiteit aan een douaneformulier verstrekken door een video toe te voegen. Wanneer het formulier aan een object is gekoppeld, kunnen gebruikers die met het object werken de video op elk gewenst moment afspelen.

Eerder kon u alleen op tekst gebaseerde velden en afbeeldingen aan een aangepast formulier toevoegen.

Zie voor meer informatie [Een afbeeldings- of video-asset-widget toevoegen of bewerken in een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

