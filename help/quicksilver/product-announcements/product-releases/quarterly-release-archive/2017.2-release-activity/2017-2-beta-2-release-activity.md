---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 2 releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die beschikbaar zijn in de voorvertoningsomgeving met de 2017.2 bèta 2-release. De functionaliteit op deze pagina is op 24 mei 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal tussen eind juli en begin augustus 2017 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 2017.2 Beta 2 releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die beschikbaar zijn in de voorvertoningsomgeving met de 2017.2 bèta 2-release. De functionaliteit op deze pagina is op 24 mei 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal tussen eind juli en begin augustus 2017 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
>De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst van alle wijzigingen die in 2017.2 zijn aangebracht, raadpleegt u [Overzicht van releaseactiviteiten 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

De 2017.2 bèta 2-versie bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**Voor beheerders:**

* [API-verbetering: gebeurtenisabonnementen](#api-enhancement-event-subscriptions)

**Voor alle gebruikers:**

* [Abonneren op projecten](#subscribe-to-projects)
* [Abonnement op objecten opzeggen via e-mail](#unsubscribe-from-items-from-email)
* [Configureer hoe mijlpalen worden weergegeven op de Gantt-grafiek](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Bronpaginasjablonen](#resource-pools-templates)
* [Versies van gecontroleerde documenten weergeven in Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nieuw object Request in goedkeuringsrapport voor proef](#new-requester-object-in-proof-approval-report)

## API-verbetering: gebeurtenisabonnementen {#api-enhancement-event-subscriptions}

Wanneer een actie op een voorwerp van Workfront voorkomt dat door gebeurtenisabonnementen wordt gesteund, kunt u Workfront nu vormen om een reactie naar uw gewenste eindpunt te verzenden. Dit betekent dat uw integratie in real-time kan communiceren met de Workfront API.

Zie voor meer informatie [API voor abonnementen voor gebeurtenissen](../../../../wf-api/general/event-subs-api.md). 

## Abonneren op projecten {#subscribe-to-projects}

U kunt nu op nieuwe commentaren op projecten intekenen waarvoor u geen deel van het projectteam uitmaakt. Vóór deze release kon u zich alleen abonneren op opmerkingen over problemen en taken.

Zie voor meer informatie over abonnementen op objecten [Abonneren op objecten in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Abonnement op objecten opzeggen via e-mail {#unsubscribe-from-items-from-email}

Je kunt je abonnement op objecten opzeggen via de link Abonnement opzeggen in het e-mailbericht met abonnement. Eerder kon je je abonnement op een object alleen opzeggen via de Workfront-interface.

Meer informatie over het opzeggen van abonnementen op e-mailberichten voor abonnementen vindt u in de sectie &quot;Opting out of Email Notification&quot; in [Adobe Workfront-berichten](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Configureer hoe mijlpalen worden weergegeven op de Gantt-grafiek {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORRECTIE **: Deze functie bevindt zich momenteel niet in de omgeving van de voorvertoningssandbox. Het is de bedoeling dat het op een later tijdstip, in de maand juni 2017, wordt vrijgegeven.*

Er zijn nu twee opties voor het weergeven van mijlpaalinformatie in een Gantt-grafiek. U kunt een van de volgende mijlpaalindicatoren configureren of beide:

* Mijlsteendiamanten (pictogram)

  Dit pictogram wordt weergegeven in het Gantt-diagram na elke taak die aan een mijlpaal is gekoppeld.

* Mijlsteenlijnen

  Een lijnvertoningen na om het even welke taak verbonden aan de mijlpaal, over alle taken in de grafiek van Gantt.

Vóór deze wijziging was er slechts één optie om Mijlpalen toe te laten om op een grafiek van Gantt te tonen, genoemd &quot;Mijlpalen.&quot; Deze optie maakte zowel het milestone diamond icon als de milestone line mogelijk. Deze indicatoren konden niet van elkaar worden gescheiden. De twee opties zijn nu beschikbaar op alle Gantt-grafieken, inclusief alle projectlijsten en -rapporten. 

Voor meer informatie over het vormen hoe de informatie in de grafiek van Gantt toont, zie [Vorm hoe de informatie op de Grafiek van Gantt toont](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Bronpaginasjablonen {#resource-pools-templates}

U kunt nu bronnenpools opgeven voor sjablonen. Voorafgaand aan deze versie, kon u de Pools van het Middel slechts met gebruikers en projecten associëren.

Voor meer informatie over Brongroepen raadpleegt u [Overzicht van bronnenpools](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Versies van gecontroleerde documenten weergeven in Workfront {#view-versions-of-proofed-documents-within-workfront}

U kunt nu proefdrukken van alle versies van een proefdocument weergeven in de Workfront-interface. 

Voordat u deze wijziging aanbrengt, kunt u alleen de laatste versie van het proefdocument weergeven.

Gebruikers zonder proeflicentie kunnen:

* Een proefdruk openen op een vorige versie van een proefdocument

Gebruikers met een proeflicentie kunnen het volgende doen:

* Een proefdruk openen op een vorige versie van een proefdocument
* De proefdrukdetails weergeven in een vorige versie van een proefdocument

Zie voor meer informatie [Documentversies beheren](../../../../documents/managing-documents/manage-document-versions.md) in [Documentversies beheren](../../../../documents/managing-documents/manage-document-versions.md).

## Nieuw object Request in goedkeuringsrapport voor proef {#new-requester-object-in-proof-approval-report}

Wanneer u nu een Proefgoedkeuringsrapport maakt, is er een nieuw object Requester. Met dit object kunt u gegevens rapporteren over de gebruiker die de proefdrukgoedkeuring heeft aangevraagd. 

Het nieuwe object Requester in het rapport Goedkeuring proef bevat alle velden die beschikbaar zijn met het bestaande object User in andere typen objectrapporten.

>[!NOTE]
>
> Deze informatie is alleen beschikbaar in het rapport vanaf het moment dat deze functie voor het eerst werd geïntroduceerd in de respectievelijke voorvertoning- of productieomgevingen. Informatie in rapporten over het object Requester vóór de introductie van deze functie is niet beschikbaar.

U krijgt toegang tot het object Requester wanneer u een goedkeuringsrapport maakt, zoals wordt beschreven in [Een aangepast rapport maken](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Voor meer informatie over het rapport van het object Goedkeuringen proef raadpleegt u de [Objecten in Adobe Workfront begrijpen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) sectie in [Objecten in Adobe Workfront begrijpen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
