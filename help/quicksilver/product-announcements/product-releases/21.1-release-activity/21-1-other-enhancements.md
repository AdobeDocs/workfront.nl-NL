---
content-type: release-notes
keywords: notities,driemaandelijks,bijwerken
navigation-topic: product-releases
title: 21.1 Andere verbeteringen
description: Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de versie 21.1 voor de voorvertoningsomgeving. Deze verbeteringen zullen in de productieomgeving beschikbaar worden gesteld in de week van 15 februari 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 Andere verbeteringen

Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de versie 21.1 voor de voorvertoningsomgeving. Deze verbeteringen zullen in de productieomgeving beschikbaar worden gesteld in de week van 15 februari 2021.

Voor een lijst van alle veranderingen beschikbaar met de versie 21.1, zie [&#x200B; overzicht van de versie 21.1 &#x200B;](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Updates voor vereisten voor mislukte abonnementen voor gebeurtenissen

We werken de soft-disable vereisten van de mislukkingen van het Abonnement van de Gebeurtenis bij. Naast de bestaande vereisten worden abonnementen voor gebeurtenissen nu uitgeschakeld als ze er niet in slagen de levering binnen 2000 pogingen tot een succes te maken. Dit is de versterking van de bestaande 70%-regel voor mislukkingen, die onder bepaalde omstandigheden tot buitensporige hoeveelheden fouten kan leiden.

Bovendien voegen we vanaf februari 2021 vereisten voor hard-disable toe.

Voor extra informatie over nieuwe soft-disable en hard-disable vereisten, zie [&#x200B; FAQs - de Abonnementen van de Gebeurtenis &#x200B;](../../../wf-api/general/event-subs-faq.md).

## De nieuwe gebieden van het Team beschikbaar aan de Dagelijkse Samenvatting

We hebben velden voor teamgoedkeuring en toewijzingen toegevoegd aan de e-mail met dagelijkse controlesamenvatting voor handelingen.

Voor meer informatie, zie [&#x200B; Meldingen: Actie nodig &#x200B;](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## POP-e-mailoptie vervangen in aanvraagwachtrij

We vervangen de e-mailoptie POP voor aanvraagwachtrijen door een nieuw Workfront-beheerd systeem. U kunt aanvragen nog steeds via e-mail verzenden, maar u moet in plaats daarvan een nieuw door Adobe Workfront beheerd e-mailadres instellen in het gebied Wachtrij aanvragen.

Deze wijzigingen kunt u testen in Voorvertoning.

E-mail wordt automatisch uitgeschakeld in alle voorvertoningsomgevingen. Om e-mail voor het testen doeleinden toe te laten, zie [&#x200B; levering van e-mails van het milieu van de zandbak van de Voorproef &#x200B;](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md) toelaten.

Voor meer informatie, zie [&#x200B; gebruikers toelaten om een kwestie in een project van de Rij van het Verzoek &#x200B;](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md) te e-mailen.

Voor meer informatie over waarom wij deze verandering maken, zie [&#x200B; Nieuwe Adobe Workfront beheerde systeem om POP e-mail voor de Queues van het Verzoek met 21.1 te vervangen &#x200B;](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Deze eigenschap is nu inbegrepen in het [&#x200B; Beheer van de Rij in de nieuwe ervaring van Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-learn/tutorials-workfront/home) het leren weg op Workfront Één.

## Uren bewerken op tijdbladen beperken

Om meer controle over timesheets en het uitgeven van uren te verstrekken, hebben wij een het plaatsen toegevoegd die u toestaat om het uitgeven van uren tot timesheet eigenaars en systeembeheerders te beperken.

Eerder konden gebruikers met de optie Timesheets &amp; Uren ingeschakeld in hun toegangsniveau uren op om het even welk timesheet uitgeven.

Voor meer informatie, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

## Verbeterde filters en weergaven in het gebied Timesheets

Wij hebben de volgende verbeteringen toegevoegd wanneer u een Project, een Taak, of een Uitgave aan een Chronologie toevoegt:

* Filters: we hebben filters toegevoegd voor Projecten en problemen. Klik op Meer opties om deze filters weer te geven. Eerder, slechts hadden de Taken beschikbaar filtreren.
* Weergaven: We hebben weergave- en groeperingsopties toegevoegd aan de zoekpagina.

Voor meer informatie, zie [&#x200B; tijd van het Logboek &#x200B;](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Het vak voor overwerk verbergen in de tijdbladen

U kunt het vak voor overuren nu verbergen om verwarring onder de gebruikers te voorkomen als u overuren in Workfront niet bijhoudt. U kunt de overloopdoos voor een enig-gebruik timesheet of in het Profiel van de Tijdopnemer verbergen:

* Tijdsoverzicht voor eenmalig gebruik: wanneer u ervoor kiest om het vak voor overuren te verbergen in een afzonderlijk tijdblad, wordt dit alleen voor dat tijdsplaat verborgen. Voor meer informatie, zie [&#x200B; een enig-gebruiks timesheet &#x200B;](../../../timesheets/create-and-manage-timesheets/create-tmshts.md) creëren.
* Tijdbladprofiel: wanneer u ervoor kiest het vak voor overwerk te verbergen in het tijdbladprofiel, wordt het vak voor overwerk niet weergegeven in alle toekomstige tijdbladen die worden gemaakt voor de gebruiker(s) die aan dat profiel is toegewezen. Voor meer informatie, zie [&#x200B; creeer, geef uit, en wijs timesheet profielen &#x200B;](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe.

Eerder kon u het vak voor overwerk niet verbergen op tijdbladen.

## Items in de breedbandnavigatie uitvouwen of samenvouwen

Om het gemakkelijker bekijken van de volledige weg van breadcrumb toe te staan, hebben wij uitbreiding toegevoegd en functionaliteit samenvouwen.

Alle afgekapte items worden nu gegroepeerd vóór het project met de tekst &quot;Meer&quot;. Bijvoorbeeld, &quot;3 meer&quot;wijst erop dat er 3 voorwerpen zijn die niet tonen.

Eerder moest u op de ellips klikken om afgekapte objecten weer te geven in een vervolgkeuzemenu.

Als u alle items in de broodkruimel wilt weergeven, klikt u op Meer aan het begin van de broodkruimel om de items uit te vouwen. Nadat u de selectie hebt uitgevouwen, kunt u op Minder klikken om de items weer samen te vouwen.

## Nieuwe look en feel voor de navigatie door middel van ademkruimels

Om gebruikers te helpen beter te identificeren waar zij in Workfront zijn en gemakkelijker tussen voorwerpen te navigeren, hebben wij de volgende verbeteringen aan broodkruimelnavigatie aangebracht:

* Elk item in de broodkruimel bevat nu een objectlabel.
* De huidige pagina is nu opgenomen in de broodkruimel en cursief.
* Toetsenbordnavigatie en schermlezernavigatie zijn nu beschikbaar voor de broodkruimels.
* Extra kleine opmaakwijzigingen

