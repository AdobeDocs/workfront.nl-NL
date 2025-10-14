---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 1-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die beschikbaar zijn in de voorvertoningsomgeving met de Beta 1-release van 2017.2. De functionaliteit op deze pagina is op 10 mei 2017 beschikbaar gesteld in de voorvertoningsomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# 2017.2 Beta 1-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die beschikbaar zijn in de voorvertoningsomgeving met de Beta 1-release van 2017.2. De functionaliteit op deze pagina is op 10 mei 2017 beschikbaar gesteld in de voorvertoningsomgeving.

>[!IMPORTANT]
>
>De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

De Beta 1-release van 2017.2 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders:**

* [&#x200B; herstelt Documenten &#x200B;](#restore-documents)
* [&#x200B; Nieuwe Banner van de Voorproef met de Informatie van de Versie &#x200B;](#new-preview-banner-with-release-information) 
* [Beschikbaarheid API 7](#api-7-availability)

**voor Alle Gebruikers:**

* [&#x200B; abonneert aan Taken en Kwesties &#x200B;](#subscribe-to-tasks-and-issues)
* [&#x200B; de Plannende Verbeteringen van het Middel &#x200B;](#resource-scheduling-improvements)
* [&#x200B; vergelijk Proofs &#x200B;](#compare-proofs)
* [&#x200B; Nieuw Gebied voor de Pools van het Middel voor Gebruikers en Projecten &#x200B;](#new-field-for-resource-pools-for-users-and-projects)
* [&#x200B; Bijgewerkte Mening en Voel in de Lijst van het Dashboard &#x200B;](#updated-look-and-feel-in-the-dashboard-list)
* [&#x200B; Verwijderend de Functionaliteit van Endorsements in Workfront &#x200B;](#removing-the-endorsements-functionality-in-workfront)
* [Kolommen in een lijst opnieuw ordenen met Slepen en neerzetten (functionaliteit wordt verwijderd)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Documenten herstellen {#restore-documents}

Workfront-beheerders kunnen nu afzonderlijke documenten herstellen die in de afgelopen 30 dagen zijn verwijderd. 

Vóór deze wijziging konden Workfront-beheerders alleen projecten, taken en problemen herstellen (inclusief documenten die samen met het verwijderde project, de verwijderde taak of uitgave zijn verwijderd).

Voor meer informatie, zie [&#x200B; geschrapte punten &#x200B;](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.

## Nieuwe voorvertoningsbanner met releasegegevens {#new-preview-banner-with-release-information}

De blauwe banner boven aan de omgeving van de voorvertoningssandbox geeft nu de naam en het versienummer van de voorvertoningsomgeving weer. Als u op de naam van de release klikt, gaat u naar een artikel op de Help-site waar u meer informatie kunt vinden over de huidige release Voorvertoning. Voor meer informatie over het Milieu van Sandbox van de Voorproef, zie [&#x200B; het Milieu van Sandbox van de Voorproef van Adobe Workfront &#x200B;](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## Beschikbaarheid API 7 {#api-7-availability}

API 7 is nu beschikbaar en bevat nieuwe en bijgewerkte objecten.

Voor meer informatie, zie [&#x200B; wat in API Versie 7 &#x200B;](../../../../wf-api/api/new-api-version-7.md) Nieuw is.

## Abonneren op taken en problemen {#subscribe-to-tasks-and-issues}

Workfront stuurt meldingen over objecten die je hebt toegewezen aan of die je hebt.

Vanaf de huidige release kunt u zich op deze items abonneren als u onderdelen wilt volgen die niet aan u zijn toegewezen, maar die van invloed kunnen zijn op uw werk.

U kunt zich abonneren op uitgaven en taken waarvoor u minstens de machtiging Beeld hebt. Wanneer een nieuwe opmerking wordt toegevoegd aan de uitgave of taak waarop u zich abonneert, wordt u in een e-mail op de hoogte gesteld van die opmerking.

Voor meer informatie over het intekenen aan kwesties en taken, zie [&#x200B; aan punten in Adobe Workfront &#x200B;](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md) intekenen

## Verbeteringen in bronnenplanning {#resource-scheduling-improvements}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [&#x200B; Overzicht van de Balancer van de Werkbelasting &#x200B;](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

De volgende verbeteringen zijn beschikbaar wanneer het plannen van middelen:

* [&#x200B; Mening Meer Punten op het Middel die Chronologie in Één enkele Mening plannen &#x200B;](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [&#x200B; vorm de Naam van het Project aan Vertoning op Taken en Kwesties op de Plannende Chronologie &#x200B;](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [&#x200B; vormt of de Ouderlijke Taken op de Plannende Chronologie &#x200B;](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline) worden getoond
* [&#x200B; breidt of vouwt gemakkelijk Alle Taken en Kwesties op de Plannende Chronologie uit &#x200B;](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Rol- en gebruikersgegevens blijven boven aan de geplande tijdlijn tijdens schuiven](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Meer Punten op het Middel die Chronologie in Één enkele Mening plannen {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Wanneer het plannen van middelen voor een team of voor om het even welke projecten waarvoor u de Manager van het Middel bent, verbruiken de taken en de kwesties nu minder verticale ruimte op de het plannen chronologie. Hierdoor kunt u meer taken en problemen in één weergave bekijken.

Als u besluit om projectnamen op elke taak en kwestie op de het plannen chronologie te tonen, wordt de verticale ruimte van elke taak en kwestie uitgebreid, resulterend in minder taken en kwesties die in één enkele mening tonen.

Voor meer informatie over het plannen van middelen, zie  &quot;Ga aan de slag met Resource Scheduling.&quot;

### Vorm de Naam van het Project aan Vertoning op Taken en Kwesties op de Plannende Chronologie {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Wanneer het plannen van middelen voor een team of voor om het even welke projecten waarvoor u de Manager van het Middel bent, kunt u de projectnaam aan vertoning op elke taak en kwestie op de het plannen chronologie nu vormen. Dit staat gebruikers toe die de het plannen chronologie bekijken om de naam van het project snel te zien waar de taak of de kwestie verblijft.

Voor meer informatie, zie &quot;Begonnen met het Plannen van het Middel&quot;.

### Configureer of bovenliggende taken worden weergegeven op de geplande tijdlijn {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Wanneer het plannen van middelen voor projecten waarvoor u de Manager van het Middel bent, kunt u nu vormen of de oudertaken op de het plannen chronologie tonen wanneer de Summiere optie van de Wijze van de Voltooiing op het project aan Handboek wordt geplaatst.

Vóór deze verandering, oudertaken altijd getoond op de het plannen chronologie wanneer de Summiere Wijze van de Voltooiing op het project aan Handboek werd geplaatst. 

Wanneer de Summiere Wijze van de Voltooiing op het project aan Automatisch wordt geplaatst, kunnen de oudertaken niet op de het plannen chronologie worden getoond. Deze ervaring is niet veranderd.

Voor meer informatie, zie &quot;Begonnen met het Plannen van het Middel&quot;.

### U kunt alle taken en problemen op de geplande tijdlijn eenvoudiger uitvouwen of samenvouwen {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Er is een nieuwe koppeling beschikbaar waarmee u alle taken en problemen in de tijdlijn van de planning eenvoudiger kunt samenvouwen.

Voor meer informatie, zie &quot;Begonnen met het Plannen van het Middel&quot;.

### Rol- en gebruikersgegevens blijven boven aan de geplande tijdlijn tijdens schuiven {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Nu wanneer het scrollen neer op de het plannen chronologie om extra informatie te bekijken, blijven de rolnaam en de gebruikersnaam bij de bovenkant van de Gebruikers en het gebied van Rollen op de het plannen chronologie, die het gemakkelijker maken om te zien welke gebruiker en rol de taken en kwesties worden geassocieerd met.

Vóór deze wijziging zouden de rolnaam en de gebruikersnaam uit de huidige weergave schuiven.

Voor meer informatie over het plannen van middelen, zie  &quot;Ga aan de slag met Resource Scheduling.&quot;

## Proofs vergelijken {#compare-proofs}

U kunt nu twee documentproeven binnen om het even welke enige documentlijst, zoals binnen het lusje van Documenten in een project, een taak, een kwestie, een portefeuille, of binnen het belangrijkste gebied van Documenten in de Globale Bar van de Navigatie vergelijken. 

De twee proefdrukken worden weergegeven met het gereedschap Revisie en Goedkeuring en u kunt elk document proeflezen terwijl u de proefdrukken in een weergave Naast elkaar vergelijkt.

Voor meer informatie, zie [&#x200B; proef &#x200B;](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md) vergelijken.

## Nieuw veld voor bronnenpools voor gebruikers en projecten {#new-field-for-resource-pools-for-users-and-projects}

De R1.5 versie introduceerde nieuwe functionaliteit rond de Planning van het Middel aan het milieu van de Voorproef. Met deze functionaliteit kunt u nieuwe bronnenpools maken. Dit zijn verzamelingen van gebruikers.

Nu kunt u deze Groepen van Middel met projecten, evenals met gebruikers associëren. U zult nu een nieuw gebied genoemd &quot;Groepen van het Middel&quot;op het project, evenals op het gebruikersvoorwerp zien.

Voor meer informatie over de nieuwe Groepen van het Middel en hoe zij met projecten en gebruikers kunnen worden geassocieerd, zie [&#x200B; overzicht van de Groepen van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Bijgewerkte weergave en weergave in de dashboardlijst {#updated-look-and-feel-in-the-dashboard-list}

Wanneer u een dashboardlijst bekijkt, is het uiterlijk moderner en schaalbaarder.

Deze functionaliteit was eerder alleen beschikbaar voor gebruikers die waren ingeschreven voor Vroege toegang. Dit is nu beschikbaar voor alle gebruikers in de voorvertoningsomgeving. Deze zal met de release van 2017.2 beschikbaar worden gesteld aan alle gebruikers in de productieomgeving. 

Voor meer informatie over dashboards, zie [&#x200B; een dashboard &#x200B;](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

## Verwijderen van de Endorsements-functionaliteit in Workfront {#removing-the-endorsements-functionality-in-workfront}

Bij het evalueren van de functionaliteit in de updatestream, hebben wij verbeteringen geïdentificeerd als een lage toepassing en een laag gebruikskenmerk. In 2017.2 wordt de volgende functionaliteit rondom Endorsements verwijderd uit Workfront vanaf de release 2017.2 (deze functionaliteit is niet meer beschikbaar in Voorvertoning):

* Het tabblad Bijschriften in het gebied met gebruikersprofielen.
* Het Endorsements-object wordt verwijderd uit de API-verkenner. Als u momenteel API-rapporten aantrekt voor de objecten &quot;Endorsement&quot; of &quot;Endorsement Share&quot;, zijn de aanroepen ongeldig nadat dit object is verwijderd.

De volgende functionaliteit blijft in de webtoepassing:

* De goedkeuring van een gebruiker door een andere gebruiker die vóór de verwijdering van deze eigenschap werd gemaakt zal in de updatestroom van de aantekenaar blijven. 

Aantekeningen zijn geen te rapporteren object geweest, dus er zijn geen wijzigingen in de rapportage voor dit object.

## Kolommen in een lijst opnieuw ordenen met Slepen en neerzetten (functionaliteit wordt verwijderd) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

De functionaliteit voor het wijzigen van de volgorde van kolommen in een lijst door een kolom van de ene locatie te slepen en in een andere plaats neer te zetten, wordt verwijderd uit Vroege toegang in de productieomgeving met de release van 2017.2 en is niet meer beschikbaar voor gebruikers. 

Voor meer details over deze functionaliteit, zie [&#x200B; kolombreedte en orde wijzigen &#x200B;](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
