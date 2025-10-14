---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 3-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die beschikbaar zijn in de voorvertoningsomgeving met de Beta 2-release van 2017.2. De functionaliteit op deze pagina is op 24 mei 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal tussen eind juli en begin augustus 2017 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# 2017.2 Beta 3-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die beschikbaar zijn in de voorvertoningsomgeving met de Beta 2-release van 2017.2. De functionaliteit op deze pagina is op 24 mei 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal tussen eind juli en begin augustus 2017 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
>De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst van alle veranderingen die in 2017.2 worden aangebracht, zie [&#x200B; 2017.2 overzicht van de versieactiviteit &#x200B;](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

De Beta 2-release van 2017.2 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders:**

* [&#x200B; het Terugzetten van Punten in Bulk van de Bak van de Recycling &#x200B;](#restoring-items-in-bulk-from-the-recycle-bin)
* [Gebruikersgegevens zijn gesynchroniseerd van Workfront naar ProofHQ (ProofHQ en Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**voor Alle Gebruikers:** 

* [&#x200B; Mening Geabonneerde Gebruikers &#x200B;](#view-subscribed-users)
* [&#x200B; vormt hoe de Mijlpalen op de Grafiek van Gantt &#x200B;](#configure-how-milestones-are-displayed-on-the-gantt-chart) worden getoond
* [&#x200B; omvat de Gantt Legende van de Grafiek wanneer het Uitvoeren naar PDF &#x200B;](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [&#x200B; Goedkeuringen van het Bewijs van de Mening in het Mijn Gebied van het Werk (Workfront) &#x200B;](#view-proof-approvals-in-the-my-work-area-workfront)
* [&#x200B; Namen van de Gebruiker van de Mening wanneer het richten van het Bewijzen van de Verzoeken van de Goedkeuring van het Mijn Gebied van het Werk (Workfront) &#x200B;](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [&#x200B; Verbeterde het proeven kijker voor VideoProofs (ProefHK en Workfront) &#x200B;](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [&#x200B; Proofs van de Media van de Mening Rich in Afwisselende Resoluties (ProofHK en Workfront) &#x200B;](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [&#x200B; Nieuw voorwerp &quot;van de Auteur van het Bewijs&quot;in het Rapport van de Versie van het Document (Workfront) &#x200B;](#new-proof-creator-object-in-document-version-report-workfront)
* [Nieuwe functie Bronpool tijdelijk uit voorvertoning verwijderd](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Items in bulk herstellen vanuit de prullenbak {#restoring-items-in-bulk-from-the-recycle-bin}

U kunt nu maximaal 10 verwijderde projecten, taken, problemen of documenten tegelijk herstellen.

Voordat u deze wijziging aanbrengt, kunt u slechts één verwijderd item tegelijk herstellen.

Voor meer informatie over het herstellen van punten, zie [&#x200B; geschrapte punten &#x200B;](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.

## Geabonneerde gebruikers weergeven {#view-subscribed-users}

U kunt nu zien wie op een punt door het aantal abonnees intekent uit te breiden die naast de abonnementverbinding verschijnen.

Vóór deze verbetering, had u geen zicht in wie aan om het even welke punten wordt geabonneerd.

Voor meer informatie over het intekenen op punten, zie [&#x200B; aan punten in Adobe Workfront &#x200B;](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md) intekenen. 

## Configureer hoe mijlpalen worden weergegeven op de Gantt-grafiek {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Er zijn nu twee opties voor het weergeven van mijlpaalinformatie in een Gantt-grafiek. U kunt een van de volgende mijlpaalindicatoren configureren of beide:

* Mijlsteendiamanten (pictogram)

  Dit pictogram wordt weergegeven in het Gantt-diagram na elke taak die aan een mijlpaal is gekoppeld.

* Mijlsteenlijnen

  Een lijnvertoningen na om het even welke taak verbonden aan de mijlpaal, die alle taken in de grafiek van Gantt overspannen.

Vóór deze wijziging was er slechts één optie om Mijlpalen toe te laten om op een grafiek van Gantt te tonen, genoemd &quot;Mijlpalen.&quot; Deze optie maakte zowel het milestone diamond icon als de milestone line mogelijk. Deze indicatoren konden niet van elkaar worden gescheiden.

Voor meer informatie over het vormen hoe de informatievertoningen in de grafiek van Gantt, zie [&#x200B; vormen hoe de informatievertoningen op de Grafiek van Gantt &#x200B;](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## De Gantt Chart Legend opnemen bij exporteren naar PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Wanneer u het Gantt-diagram naar een PDF exporteert, kunt u nu selecteren of u ook de legenda van het diagram samen met het diagram zelf wilt exporteren. De punten inbegrepen in de legenda zijn slechts die opties u hebt toegelaten om in de grafiek van de Gantt in UI te worden getoond. Deze opties worden opgenomen in de legenda als deze bestaan voor de taken van het project. Als u bijvoorbeeld Mijlpalen in het Gantt-diagram wilt weergeven, worden deze ook door de legenda weergegeven, maar alleen als er ten minste één taak aan een mijlpaal is gekoppeld.

Voorafgaand aan deze wijziging kon u de legenda niet uitsluiten van de geëxporteerde PDF. De legenda bevatte alle mogelijke opties en markeringen van de Gantt, ongeacht of deze waren ingeschakeld of in de UI bestonden.

Voor meer informatie over het uitvoeren van de grafiek van Gantt, zie [&#x200B; de Grafiek van Gantt naar PDF &#x200B;](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md) uitvoeren.

## Gebruikersgegevens zijn gesynchroniseerd van Workfront naar ProofHQ (ProofHQ en Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Gebruikersgegevens (naam en e-mail) worden nu gesynchroniseerd van Workfront naar ProofHQ wanneer gebruikers worden gemaakt of bijgewerkt in Workfront. 

Voor meer informatie over gebruikerssynchronisatie van Workfront aan ProofHQ, zie.

## Nieuw object Proefmaker in documentversierapport (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Wanneer u nu een rapport Documentversie maakt, is er een nieuw object Proefmaker. Met dit object kunt u informatie rapporteren over de gebruiker die de proefdruk heeft gemaakt. 

Het nieuwe Proefdrukobject in het rapport Documentversie bevat alle velden die beschikbaar zijn met het bestaande object Gebruiker in andere typen objectrapporten.

>[!NOTE]
>
> Deze informatie is alleen beschikbaar in het rapport vanaf het moment dat deze functie voor het eerst werd geïntroduceerd in de respectievelijke voorvertoning- of productieomgevingen. Informatie in rapporten over het object Requester vóór de introductie van deze functie is niet beschikbaar.

U hebt toegang tot het voorwerp van de Maker van het Bewijs wanneer het creëren van een rapport van de Versie van het Document, zoals die in [&#x200B; wordt beschreven creeer een douanerapport &#x200B;](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Voor meer informatie over het de objecten van de Versie van het Document rapport, zie [&#x200B; voorwerpen in Adobe Workfront &#x200B;](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) sectie in [&#x200B; begrijpen voorwerpen in Adobe Workfront &#x200B;](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.

## Goedkeuringen proef bekijken in Mijn werkgebied (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Alle proefgoedkeuringen u voor goedkeuring hebt voorgelegd worden nu getoond in het Mijn gebied van het Werk, in het **Werk ik voor Goedkeuring** tabel heb voorgelegd.

Voorafgaand aan deze verandering, het **Werk ik voor Goedkeuring** lusje heb voorgelegd omvatte proefgoedkeuringen niet.

Goedkeuringen van proefdrukken worden alleen weergegeven als aan de volgende criteria is voldaan:

* De goedkeuring is momenteel in afwachting van goedkeuring
* Het goedkeuringsproces wordt toegewezen aan een gebruiker die een in licentie gegeven Workfront-gebruiker is (Goedkeuringsprocessen die zijn toegewezen aan gebruikers die geen Workfront-gebruikers met licentie hebben, worden niet weergegeven)
* De goedkeuringsprocessen zijn gestart nadat deze functionaliteit is vrijgegeven (goedkeuringsprocessen die zijn gestart voordat deze functionaliteit wordt vrijgegeven, worden niet weergegeven)

Voor meer informatie, zie [&#x200B; goedkeuringen van de Mening &#x200B;](../../../../review-and-approve-work/manage-approvals/view-approvals.md) in [&#x200B; goedkeuringen van de Mening &#x200B;](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Gebruikersnamen weergeven bij het indienen van aanvragen voor proefdrukken in het gebied Mijn werk (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Bij het goedkeuren van testgoedkeuringen in het gebied Mijn werk wordt nu de naam van de gebruiker die goedkeuring heeft aangevraagd, weergegeven.

Voor meer informatie, zie [&#x200B; goedkeurend het werk &#x200B;](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [&#x200B; het goedkeuren van het werk &#x200B;](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Verbeterde proefdrukviewer voor videoproefdrukken (proefdrukken van hoofdletters en kleine letters, Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

De proefdrukviewer in zowel Workfront als ProofHQ wordt bijgewerkt met een nieuwe look and feel, HTML5-architectuur voor betere prestaties en ondersteuning voor nieuwe functionaliteit.

De nieuwe proefdrukviewer bevat de volgende verbeteringen:

* Frame-voor-frame proefdrukken
* Video bufferen
* Functionaliteit zoeken in de lijst met opmerkingen
* Alle acties die zijn ingesteld op de opmerking, worden weergegeven op elke opmerking in de lijst met opmerkingen
* Modus Volledig scherm
* Inhoud sneller of langzamer controleren
* Spellingcontrole bij het toevoegen van opmerkingen en antwoorden

### Voorvertoning

De nieuwe proefdrukviewer is beschikbaar om te testen in de volgende voorvertoningsomgevingen:

* Voorvertoningsomgeving voor hoofdkwartier proefdrukken

  Voor meer informatie over het milieu van de Voorproef ProofHQ, zie [&#x200B; het Testen van Sandbox van de Voorproef Milieu - Workfront Proof &#x200B;](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Workfront Preview-omgeving, wanneer uw account is ingeschakeld met proefdrukken

  Zie voor meer informatie over de Workfront Preview-omgeving  [&#x200B; de zandbakmilieu van de Voorproef van Adobe Workfront &#x200B;](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

In deze versie ondersteunt de nieuwe proefdrukviewer alleen videoproeven. Dit betekent dat alle videoproeven hefboomwerking de nieuwe het proefdrukken kijker, terwijl alle statische en rijke media proefdrukken blijven hefboomwerking de bestaande het proefdrukken kijker.

### Productie

Wanneer ze met de release 17.2 naar de productieomgeving worden vrijgegeven, kunnen beheerders kiezen of de nieuwe of verouderde proefdrukviewer geschikt is voor de gebruikers in hun organisatie. Standaard wordt de verouderde proefdrukviewer gebruikt.

Ga voor informatie over het gebruik van de nieuwe video-proefdrukviewer naar  

## Proofs voor rijke media weergeven in alternatieve resoluties (proefdrukken van hoofdvragen en Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

U kunt nu de resolutie van Rich Media-proefdrukken aanpassen door een aangepaste resolutie op te geven of door de afbeelding naar de gewenste resolutie te slepen.

Voordat u deze wijziging aanbrengt, kunt u proefdrukken alleen bekijken met de resolutie die inherent is aan het scherm of apparaat waarop u de inhoud controleert.

U kunt de modus Vergelijken gebruiken om verschillende resoluties van proefdrukken te vergelijken.

Voor meer informatie, zie [&#x200B; Open proeven in de Desktop het Proofing Kijker &#x200B;](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Nieuwe functie Bronpool tijdelijk uit voorvertoning verwijderd {#new-resource-pool-functionality-temporarily-removed-from-preview}

Vanwege ontwikkelingsuitdagingen hebben we besloten het nieuwe tabblad Bronplanning te verwijderen en de naam van het tabblad Oudere bronnenplanning te wijzigen in de oorspronkelijke naam van &quot;Bronplanning&quot;.

De nieuwe functionaliteit Brongroepen is ook verwijderd met deze wijziging. Het nieuwe lusje van de Planning van het Middel en de functionaliteit van de Pools van het Middel zullen aan het milieu van de Sandbox van de Voorproef eind juni, 2017 terugkeren.
