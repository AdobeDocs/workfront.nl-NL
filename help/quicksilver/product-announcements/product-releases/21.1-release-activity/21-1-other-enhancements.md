---
content-type: release-notes
keywords: notities,driemaandelijks,bijwerken
navigation-topic: product-releases
title: 21.1 Andere verbeteringen
description: Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de versie 21.1 voor de voorvertoningsomgeving. Deze verbeteringen zullen in de productieomgeving beschikbaar worden gesteld in de week van 15 februari 2021.
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1 Andere verbeteringen

Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de versie 21.1 voor de voorvertoningsomgeving. Deze verbeteringen zullen in de productieomgeving beschikbaar worden gesteld in de week van 15 februari 2021.

Voor een lijst met alle wijzigingen die beschikbaar zijn in de release 21.1 raadpleegt u [21.1 - releaseoverzicht](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Updates voor vereisten voor mislukte abonnementen voor gebeurtenissen

We werken de soft-disable vereisten van de mislukkingen van het Abonnement van de Gebeurtenis bij. Naast de bestaande vereisten worden abonnementen voor gebeurtenissen nu uitgeschakeld als ze er niet in slagen de levering binnen 2000 pogingen tot een succes te maken. Dit is de versterking van de bestaande 70%-regel voor mislukkingen, die onder bepaalde omstandigheden tot buitensporige hoeveelheden fouten kan leiden.

Bovendien voegen we vanaf februari 2021 vereisten voor hard-disable toe.

Voor meer informatie over de nieuwe soft-disable en hard-disable vereisten, zie [Veelgestelde vragen - Abonnementen voor gebeurtenissen](../../../wf-api/general/event-subs-faq.md).

## De nieuwe gebieden van het Team beschikbaar aan de Dagelijkse Samenvatting

We hebben velden voor teamgoedkeuring en toewijzingen toegevoegd aan de e-mail met dagelijkse controlesamenvatting voor handelingen.

Zie voor meer informatie [Meldingen: Actie vereist](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## POP-e-mailoptie vervangen in aanvraagwachtrij

We vervangen de e-mailoptie POP voor aanvraagwachtrijen door een nieuw Workfront-beheerd systeem. U kunt aanvragen nog steeds via e-mail verzenden, maar u moet in plaats daarvan een nieuw door Adobe Workfront beheerd e-mailadres instellen in het gebied Wachtrij aanvragen.

Deze wijzigingen kunt u testen in Voorvertoning.

E-mail wordt automatisch uitgeschakeld in alle voorvertoningsomgevingen. Ga voor testdoeleinden naar [Verzending van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Zie voor meer informatie [Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Voor meer informatie over waarom wij deze verandering aanbrengen, zie [Nieuw Adobe Workfront-systeem dat POP-e-mail voor aanvraaglijsten vervangt door 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Deze functie is nu opgenomen in het dialoogvenster [Wachtrijbeheer in de nieuwe Workfront-ervaring](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) leerpad op Workfront One.

## Uren bewerken op tijdbladen beperken

Om meer controle over timesheets en het uitgeven van uren te verstrekken, hebben wij een het plaatsen toegevoegd die u toestaat om het uitgeven van uren tot timesheet eigenaars en systeembeheerders te beperken.

Eerder konden gebruikers met de optie Timesheets &amp; Uren ingeschakeld in hun toegangsniveau uren op om het even welk timesheet uitgeven.

Zie voor meer informatie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Verbeterde filters en weergaven in het gebied Timesheets

Wij hebben de volgende verbeteringen toegevoegd wanneer u een Project, een Taak, of een Uitgave aan een Chronologie toevoegt:

* Filters: We hebben filters toegevoegd voor Projecten en problemen. Klik op Meer opties om deze filters weer te geven. Eerder, slechts hadden de Taken beschikbaar filtreren.
* Weergaven: We hebben opties voor weergave en groeperen toegevoegd aan de zoekpagina.

Zie voor meer informatie [Logtijd](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Het vak voor overwerk verbergen in de tijdbladen

U kunt het vak voor overuren nu verbergen om verwarring onder de gebruikers te voorkomen als u overuren in Workfront niet bijhoudt. U kunt de overloopdoos voor een enig-gebruik timesheet of in het Profiel van de Tijdopnemer verbergen:

* Tijdschema voor eenmalig gebruik: Wanneer u ervoor kiest om de overloopdoos in een individueel timesheet te verbergen, is het verborgen slechts voor dat timesheet. Zie voor meer informatie [Een timesheet voor eenmalig gebruik maken](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Tijdbladprofiel: Wanneer u ervoor kiest om het vak voor overwerk te verbergen in het tijdbladprofiel, wordt het vak voor overwerk niet weergegeven in alle toekomstige tijdbladen die worden gemaakt voor de gebruiker(s) die aan dat profiel is toegewezen. Zie voor meer informatie [Werkbladprofielen maken, bewerken en toewijzen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Eerder kon u het vak voor overwerk niet verbergen op tijdbladen.

## Items in de breedbandnavigatie uitvouwen of samenvouwen

Om het gemakkelijker bekijken van de volledige weg van breadcrumb toe te staan, hebben wij uitbreiding toegevoegd en functionaliteit samenvouwen.

Alle afgekapte items worden nu gegroepeerd vóór het project met de tekst &quot;Meer&quot;. Bijvoorbeeld, &quot;3 meer&quot;wijst erop dat er 3 voorwerpen zijn die niet tonen.

Eerder moest u op de ellips klikken om afgekapte objecten weer te geven in een vervolgkeuzemenu.

Als u alle items in de broodkruimel wilt weergeven, klikt u op Meer aan het begin van de broodkruimel om de items uit te vouwen. Nadat u de selectie hebt uitgevouwen, kunt u op &quot;Minder&quot; klikken om de items weer samen te vouwen.

## Nieuwe look en feel voor de navigatie door middel van ademkruimels

Om gebruikers te helpen beter te identificeren waar zij in Workfront zijn en gemakkelijker tussen voorwerpen te navigeren, hebben wij de volgende verbeteringen aan broodkruimelnavigatie aangebracht:

* Elk item in de broodkruimel bevat nu een objectlabel.
* De huidige pagina is nu opgenomen in de broodkruimel en cursief.
* Toetsenbordnavigatie en schermlezernavigatie zijn nu beschikbaar voor de broodkruimels.
* Extra kleine opmaakwijzigingen

