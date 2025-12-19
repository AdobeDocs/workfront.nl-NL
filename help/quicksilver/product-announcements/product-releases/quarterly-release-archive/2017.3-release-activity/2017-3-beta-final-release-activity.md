---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta Slotrelease
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de Beta Final release van 2017.3. De functionaliteit op deze pagina is op 12 september 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin november 2017 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 0%

---

# 2017.3 Beta Slotrelease

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de Beta Final release van 2017.3. De functionaliteit op deze pagina is op 12 september 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin november 2017 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2017.3 zijn aangebracht, raadpleegt u  [ 2017.3 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

De slotversie van Beta van 2017.3 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders**

* [ Nieuwe Configuratie voor het Terugroepen van Verzoeken op het Gebied van de Montages van de Goedkeuring ](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Standaardproefdrukrollen configureren](#configure-default-proof-roles)

**voor Alle Gebruikers**

* [ Gebied van het Huis (Bijgewerkt Mijn Gebied van het Werk) ](#home-area-updated-my-work-area)

* [ Bijgewerkt Malplaatje van de Lay-out om het Gebied van het Huis ](#updated-layout-template-to-support-the-home-area) te steunen

* [ Kanban voor Agile ](#kanban-for-agile)
* [ omvat Kwesties op de Achtergrond van het Trommel voor een Team van de Giel ](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [ omvat Kwesties op de Raad van het Verhaal van de Trommel ](#include-issues-on-the-scrum-agile-story-board)
* [ pas Groepen en Filters op Backlog voor een Gelijk Team ](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team) toe
* [ Verbeterde @Tagging Functionality Keert in het Milieu van de Voorproef ](#enhanced-tagging-functionality-returns-in-the-preview-environment) terug
* [ de Updates van het Systeem van de Filter in de Stroom van de Update is nu Persistent over Voorwerpen ](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [ visualiseer Gegevens in het Rapport van het Gebruik ](#visualize-data-in-the-utilization-report)
* [ de Verbetering van de Prestaties van het Rapport van het Gebruik ](#utilization-report-performance-improvement)
* [ de Verbeteringen van het Document: Gestroomlijnde Interface ](#document-enhancements-streamlined-interface)
* [ het Proofing Verbeteringen binnen Workfront ](#proofing-enhancements-within-workfront)
* [ het Proofing Verbeteringen binnen zowel Workfront Proof als Workfront ](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [ Rich Tekst die voor Updates en E-mail opmaakt ](#rich-text-formatting-for-updates-and-emails)
* [ Nieuwe Gantt Grafiek herontwerpen ](#new-gantt-chart-redesign)
* [ ingebouwde Rapporten bevatten bijgewerkte beschrijvingen ](#built-in-reports-contain-updated-descriptions)
* [ brandend in Geëxporteerde Rapporten, Lijsten, en Dashboards ](#branding-in-exported-reports-lists-and-dashboards)
* [ Verbeteringen wanneer het kopiëren van Taken en het bewegen van Taken of Kwesties ](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [ Nieuwe Groepering voor de Rapporten van het Huur van het Middel begrote: Datum van de toewijzing ](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* {de Verbeteringen van de Planner van 0} Middel [](#resource-planner-improvements)
* [ Mobiele Verbeteringen ](#mobile-improvements)
* [ de Integratie van Workfront met Slack ](#workfront-integration-with-slack)
* [ Vooruitzichten 365 Verbeteringen ](#outlook-365-improvements)
* [API-wijzigingen](#api-changes)

## Thuisgebied (Mijn werkgebied is bijgewerkt) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Deze functionaliteit wordt niet vrijgegeven in de productieomgeving met de release 17.3. De functionaliteit blijft in Voorvertoning tot begin 2018.

Het nieuwe gebied van het Huis verstrekt een afwisselende, verbeterde mening aan de zelfde gegevens die momenteel in het Mijn gebied van het Werk beschikbaar zijn. Het gebied van het Huis verstrekt de volgende voordelen over het Mijn Gebied van het Werk:

* Een meer gestroomlijnde en intuïtieve interface
* Verbeterde prestaties

De volgende functionaliteit is beschikbaar in het gedeelte Mijn werk, maar is nog niet geïmplementeerd in het gedeelte Home:

* Je persoonlijke kalender bekijken
* Taken en problemen met tekstopmaak bijwerken
* Proefdrukken goedkeuren
* Een lijst weergeven met werkzaamheden die u ter goedkeuring hebt ingediend
* Een ad-hocprobleem maken voor een project
* Alleen goedkeuringen weergeven die aan u zijn gedelegeerd

Voor meer informatie over het gebruiken van het nieuwe gebied van het Huis, zie [ Gebruik het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Bijgewerkte lay-outsjabloon ter ondersteuning van het thuisgebied {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Deze functionaliteit wordt niet vrijgegeven in de productieomgeving met de release 17.3. De functionaliteit blijft in Voorvertoning tot begin 2018.

Als beheerder van Workfront, kunt u bepalen of de gebruikers in uw organisatie toegang tot het gebied van het Huis hebben door het lay-outmalplaatje te vormen zij aan worden toegewezen. Gebruikers aan wie geen lay-outsjabloon is toegewezen, hebben altijd toegang tot het gebied Home.

Zie &quot;Home aanpassen&quot; in &quot;Lay-outsjablonen maken en beheren&quot; voor meer informatie.

## Kanban voor Agile  {#kanban-for-agile}

Agile-teams kunnen nu een Kanban-methodologie in Workfront gebruiken, naast de reeds ondersteunde methode voor de functie Scrum Agile.

De methoden Scrum en Kanban Agile in Workfront verschillen op de volgende manieren:

**Voordelen van het Gebruiken van Kanban in Workfront**

* Geef de achterstand weer op de Kanban Agile story board.

  Zie voor meer informatie in .

* Configureer items op de achtergrond die automatisch aan de Kanban Agile-artikelkaart moeten worden toegevoegd wanneer andere items naar een status worden verplaatst die gelijk is aan Voltooien.

  Voor meer informatie, zie [ verhalen vormen die automatisch van de achterstand ](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in [ worden toegevoegd vormt Kanban ](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configureer een WIP-limiet (Work In Progress) die moet worden weergegeven op de Kanban Agile-artikelkaart.

  Voor meer informatie, zie [ het werk momenteel (WIP) grens ](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [ vormen Kanban ](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Voordelen van het Gebruiken van Trommel in Workfront**

* Voeg een reeks artikelen toe aan een letterlijke tekst van het artikel en maak een artikelbord voor die herhaling.
* Neem problemen op het vel-artikelbord op.
* Neem problemen op in de achterstand van een Agile-team.

  Voor meer informatie, zie [ vormen hoe de data worden toegepast wanneer het toevoegen van het werkpunten aan een herhaling ](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [ vormen het Trommel ](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Subtaken kunnen worden weergegeven op het artikelbord van de scrum.
* Bekijk een uitvouwgrafiek om de vooruitgang tegen verhalen tijdens de herhaling te zien.

  Voor meer informatie, zie [ Overzicht van de de burndown grafiek van de Gelijkheid ](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Voor meer informatie over het toelaten van en het vormen Kanban voor een team van de Gelijkheid, zie [ Beslissen over een Gelijke methodologie ](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [ creeer een team van de Gelijkheid ](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Inclusief problemen op de scrubbacklog voor een flexibel team {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Deze functionaliteit is verwijderd uit de productieomgeving op 14 november 2017. Het is de bedoeling dat dit begin 2018 opnieuw wordt geïntroduceerd in de voorvertoningsomgeving met een verbeterd ontwerp en een grotere stabiliteit. Deze is beschikbaar in de productieomgeving met de release van 2018.1.

U kunt nu kwesties op de achterstand van uw team van de Gielen wanneer het gebruiken van de Methode van de Agile van het Trommel (de kwesties worden niet getoond op de achterstand van een team van de Genile wanneer het gebruiken van de methodologie Kanban). De bestaande teams van de Trommel moeten deze functionaliteit toelaten om kwesties worden omvat. De kwesties worden automatisch inbegrepen op de achterstand voor de teams van de Groep van de Trommel die na de versie van 2017.3 worden gecreeerd.

Voorafgaand aan deze wijziging konden alleen taken aan de achterstand worden toegevoegd. Als u een uitgave wilt toevoegen, moest u eerst de kwestie in een taak omzetten alvorens het kon worden toegevoegd.

Omdat u nu toegang tot meer dan enkel taken op de backlog hebt, worden om het even welke meningen van de douanetaak die eerder op de backlog beschikbaar waren gekopieerd en aan de backlog toegevoegd als de meningen van het Punt van het Werk van de Douane van de Achtergrond.

Voor informatie over het gebruiken van kwesties op de achtergrond, zie  [ beheert de Gelijke achterstand ](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Voor informatie over het toelaten van kwesties om op de achtergrond van een team van de Trommel van de Kracht beschikbaar te zijn, zie  [ vormt hoe de datums worden toegepast wanneer het toevoegen van het werkpunten aan een herhaling ](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [ Scrum ](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) vormt.

## Inclusief problemen op de prullenbak voor onscherpe artikelen {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Deze functionaliteit is verwijderd uit de productieomgeving op 14 november 2017. Het is de bedoeling dat dit begin 2018 opnieuw wordt geïntroduceerd in de voorvertoningsomgeving met een verbeterd ontwerp en een grotere stabiliteit. Deze is beschikbaar in de productieomgeving met de release van 2018.1.

U kunt nu problemen opnemen op het whiteboard wanneer u de methode voor het bepalen van de spreidingsschaal gebruikt.

Voor meer informatie, zie [ statuskolommen op de het verhaalraad van de Gelijkheid ](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [ vormen het Trommel ](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) vormen.

## Groepen en filters toepassen op de achtergrond voor een flexibel team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Deze functionaliteit is verwijderd uit de productieomgeving op 14 november 2017. Het is de bedoeling dat dit begin 2018 opnieuw wordt geïntroduceerd in de voorvertoningsomgeving met een verbeterd ontwerp en een grotere stabiliteit. Deze is beschikbaar in de productieomgeving met de release van 2018.1.

De opties Groeperen en Filter zijn nu beschikbaar op de Google-achterstand, zodat u uw achterstand kunt indelen op groepen en filteren op specifieke taken en problemen.

Voordat u deze wijziging aanbrengt, kunt u de weergaven toepassen op de Agile-achterstand.

Zie voor meer informatie  [ beheert de Agile backlog ](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) binnen  [ beheert de Gelijke achterstand ](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## RTF-opmaak voor updates en e-mails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Het opmaken van wijzigingen die u aanbrengt in de voorvertoningsomgeving, kan worden teruggezet naar de status zonder opmaak.

Nu kunt u belangrijke informatie benadrukken door de commentaren en updates te formatteren u aan de voorwerpen van Workfront aanbrengt. 

Met de gereedschappen voor RTF-bestanden kunt u opmaakkenmerken toepassen op tekst, lijsten met opsommingstekens en nummers maken en hyperlinks toevoegen aan extra bronnen.

Opmaak die wordt toegepast op opmerkingen in de updatestroom, wordt ook weergegeven in de e-mailmeldingen voor bijwerken. Om meer over het formatteren van uw commentaren te leren, zie [ het werk van de Update ](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Verbeterde @Tagging-functionaliteit Geeft als resultaat in de voorvertoningsomgeving {#enhanced-tagging-functionality-returns-in-the-preview-environment}

U kunt het symbool @ opnieuw gebruiken om andere gebruikers in de Stroom van de Update van alle voorwerpen in het milieu van de Voorproef te etiketteren. In het verleden heeft @tagging de voor- en achternaam van de gecodeerde gebruiker in de updatestroom geplaatst. De verbeterde functie @tagging geeft nu alleen de voornaam van de gebruiker weer. Meer over het etiketteren van gebruikers in updates leren, zie [ Tags anderen op updates ](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## De Updates van het Systeem van de filter in de Stroom van de Update zijn nu Blijvend over Voorwerpen {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

De optie Systeemupdates filteren is nu blijvend in alle objecten op de Workfront-site. Hierdoor kunt u systeemupdates verbergen en alleen gebruikersopmerkingen in de updatestroom voor één object weergeven. Deze instelling blijft behouden wanneer u naar andere objecten bladert.

Voordat u deze wijziging aanbracht, moest u de systeemupdates voor elk object uitfilteren terwijl u door de Workfront-site bladerde.

Voor meer informatie, zie [ het werk van de Update ](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Gegevens visualiseren in het gebruiksrapport {#visualize-data-in-the-utilization-report}

 U kunt de gebruiksinformatie nu weergeven in een grafiekweergave. 

Voor meer informatie, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Verbetering van de prestaties van het gebruiksrapport {#utilization-report-performance-improvement}

>[!NOTE]
>
>Deze functie is vrijgegeven in een patch na de laatste release van Beta.

Nu wanneer het runnen van een rapport van het Gebruik, wordt u ertoe aangezet om een filter vóór het rapport toe te passen dat loopt. Deze wijziging zorgt ervoor dat de meest relevante informatie zo snel mogelijk wordt gegenereerd in het gebruiksrapport.

Voor meer informatie over het in werking stellen van een rapport van het Gebruik, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Documentverbeteringen: gestroomlijnde interface {#document-enhancements-streamlined-interface}

De gebruikerservaring voor het toevoegen van documenten aan Workfront is nu gestroomlijnder en intuïtiever. Nu kunt u een document uploaden vanaf uw bestandssysteem, een document aanvragen of een bestand koppelen vanuit een externe toepassing (zoals Google of Dropbox), allemaal via een eenvoudig keuzemenu. 

Eerder waren deze opties beschikbaar door het dialoogvenster Documenten toevoegen te openen. 

Zie de volgende informatie voor meer informatie:

* [ voegt documenten aan Adobe Workfront van uw dossiersysteem ](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) toe
* [ Verzoek om een Document ](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [ de documenten van de Verbinding van externe toepassingen ](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Met deze wijziging is de optie voor het plakken van een afbeelding of document vanaf het klembord niet meer beschikbaar.

## Verbeteringen voor proefdrukken in Workfront {#proofing-enhancements-within-workfront}

* [ Verbeterde Ervaring van de Gebruiker en Extra Functionaliteit ](#improved-user-experience-and-additional-functionality)
* [ Deel direct van de het proef kijker ](#share-directly-from-the-proofing-viewer)
* [Standaardproefdrukrollen configureren](#configure-default-proof-roles)

### Verbeterde gebruikerservaring en extra functionaliteit {#improved-user-experience-and-additional-functionality}

Naast een verbeterde gebruikerservaring bij het maken van proefdrukken in Workfront, is nu de volgende aanvullende functionaliteit beschikbaar:

* Voeg meerdere afbeeldingen samen tot één proefdruk.
* Bewijs van websites in meerdere resoluties (meerdere resoluties kunnen worden gemaakt als afzonderlijke proefdrukken of kunnen worden gecombineerd tot één proefdruk).
* Bewerk de bestandsnaam tijdens het uploaden.
* Voeg aangepaste velden toe aan het proefdrukformulier.
* Voeg een aangepast bericht toe om e-mailmeldingen te controleren.
* Aanvullende proefinstellingen 
* Real-time foutvalidatie tijdens het controleren van een URL (voorheen moest u enkele minuten wachten voordat een fout werd weergegeven)

Zie voor meer informatie.

>[!NOTE]
>
> Wanneer u een nieuwe proefdruk maakt met een geautomatiseerde workflow, kunt u slepen en neerzetten niet gebruiken om gebruikers van het ene werkgebied naar het andere te verplaatsen. Verwijder in plaats daarvan de gebruiker uit de ene stap en voeg deze toe aan een andere stap.

*de optie om gebruikers van één stap aan een andere te bewegen gebruikend belemmering-en-daling zal met de versie 2018.1 opnieuw worden geïntroduceerd.*

### Direct delen vanuit de proefdrukviewer {#share-directly-from-the-proofing-viewer}

U kunt nu rechtstreeks vanuit de testviewer delen met specifieke Workfront-gebruikers.

>[!NOTE]
>
>Deze functionaliteit is alleen beschikbaar voor nieuwe proefdrukken (proefdrukken die worden gemaakt na de release van 2017.3) en alleen voor Workfront-instanties die zijn geïntegreerd met een Workfront Proof Premium-account.

Vóór deze wijziging kon u alleen delen door een koppeling te maken en die koppeling vervolgens met een gebruiker te delen. 

Voor meer informatie, zie [ een proef binnen Adobe Workfront ](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [ Deel een bewijs binnen Adobe Workfront ](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Standaardproefdrukrollen configureren {#configure-default-proof-roles}

U kunt nu de standaardproefrollen vormen die nieuwe gebruikers en gastgebruikers aan nieuwe proefdrukken binnen het systeem van Workfront moeten. 

Dit is de standaardrol waaraan gebruikers worden toegewezen op een proef wanneer de proef met hen wordt gedeeld. 

## Verbeteringen voor proefdrukken in zowel Workfront Proof als Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [ Begin en Skip in HTML5 Video het proef kijker (de Kortere weg van het Toetsenbord) ](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Updates van de HTML5-testviewer](#html5-proofing-viewer-updates)

### Opnieuw starten en overslaan in HTML5 Video Proofing Viewer (sneltoetsen) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Er zijn nu sneltoetsen in de HTML5 Proofing-viewer voor video waarmee u de video opnieuw kunt starten vanaf het begin en het einde van de video kunt overslaan.

Voor meer informatie over de beschikbare toetsenbordkortere weg, zie [ kortere weg van het Toetsenbord in de het proef Workfront Proof kijker ](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Updates van de HTML5-testviewer {#html5-proofing-viewer-updates}

De HTML5-viewer ondersteunt nu statische proefdrukken.

Vóór deze wijziging werd in de HTML5-viewer alleen videoproefdrukken ondersteund. 

De HTML-viewer bevat de volgende nieuwe functionaliteit wanneer u statische inhoud test:

* Eén opmerking maken met markeringen op meerdere pagina&#39;s in de weergave Eén

  Dit was eerder mogelijk alleen in de weergave Ononderbroken of Tijdschriftweergave

* Door proefdrukken navigeren via de proefdrukminiaturen

   * Eenvoudig het deel van het bewijs te identificeren dat wordt herzien. Dit is belangrijk, vooral wanneer gebruikers met grotere proefdrukken in bestandsindelingen en lange webpagina&#39;s werken, of op elk gewenst moment  er is meer zoomniveau nodig om de details te kunnen zien .
   * Het zoomniveau wijzigen
   * Inhoud pannen

* Aangepaste waarden opgeven in het gereedschap Meten
* Wanneer u tekst notiteert in een proefdruk in de testviewer in Workfront Proof, kunt u opties opnemen om aan te geven dat de tekst vet, cursief en onderstreept moet worden weergegeven.

De HTML5-viewer ondersteunt nog niet alle functionaliteit die momenteel beschikbaar is in de bestaande Flash-viewer. De volgende functionaliteit is momenteel niet beschikbaar, maar wordt in een toekomstige release opgenomen:

* Ondersteuning voor rijke mediabestanden
* Vergelijkingsmodus (Video en statisch)
* Opmerkingen filteren (video en statisch)
* Hyperlinks in documenten controleren (statisch)
* Vertalingen (video en statisch)
* Aanwezigheidsindicator waarmee gebruikers worden weergegeven die momenteel aan de proefdruk werken
* Proofs delen

Zie voor meer informatie over het proefdrukken van statische proefdrukken in de HTML5-viewer.

Als Workfront-beheerder in Workfront Proof kunt u bepalen of gebruikers in uw organisatie toegang hebben tot de nieuwe HTML5-proefdrukviewer voor videoproefdrukken.

## Nieuwe Gantt Chart Redesign {#new-gantt-chart-redesign}

Het nieuwe Gantt-diagram bevat de volgende verbeteringen:

* Nieuwe pictogrammen en markeringen
* Nieuwe optie voor in- en uitzoomen op een bepaald tijdframe
* Kleinere taakcellen in het lijstgedeelte van de grafiek
* Opnieuw ontworpen opties voor instellingen, afdrukken en schakelen naar geprojecteerde datums.

Voor meer informatie over het vormen van opties in de grafiek van Gantt, zie [ vormen hoe de informatievertoningen op de Grafiek van Gantt ](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Ingebouwde rapporten bevatten bijgewerkte beschrijvingen {#built-in-reports-contain-updated-descriptions}

We hebben de beschrijvingen voor onze systeemrapporten in Workfront bijgewerkt, zodat ze informatie bevatten over het type rapport en de velden die erin worden opgenomen.  

Vóór deze verandering hadden de meeste van onze ingebouwde rapporten geen of zeer beperkte beschrijvingen.

Voor meer informatie over ingebouwde rapporten, zie [ de ingebouwde rapporten van Adobe Workfront van het Gebruik ](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Markeren in Geëxporteerde rapporten, lijsten en dashboards {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Deze functie is momenteel niet beschikbaar voor alle clusters in de voorvertoningsomgeving.

Als u branding gebruikt in Workfront, wordt het logo dat u gebruikt in uw globale navigatiebalk nu opgenomen in de .pdf-bestanden die u exporteert vanuit Workfront.

De volgende .pdf-bestanden bevatten het logo van uw organisatie in het geëxporteerde document:

* Geëxporteerde lijsten
* Geëxporteerde en geleverde rapporten
* Afgedrukte dashboards

Voor meer informatie over het uitvoeren van gegevens van Workfront, zie [ Gegevens van de Uitvoer ](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Verbeteringen bij het kopiëren van Taken en het bewegen van Taken of Kwesties {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Wij hebben de manier verbeterd u een taak kopieert of een taak of een kwestie beweegt, om het gemakkelijker te maken om een ouder voor de gekopieerde of verplaatste taak of kwestie te selecteren. Wanneer het selecteren van een ouder terwijl het kopiëren van een taak, bijvoorbeeld, kunt u nu een hiërarchie van taken, met hun ouder - kindverhouding, evenals onderzoek naar een ouder in projecten met veel taken zien.

Voorafgaand aan deze verandering, was er geen gebied van het Onderzoek in **Uitgezocht een stap van de Ouder**, en de hiërarchie van taken was niet zichtbaar in de taaklijst.

Voor meer informatie over het kopiëren van taken, zie [ Kopiëren en dupliceren taken ](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Voor meer informatie over het bewegen van kwesties, zie [ kwesties van de Beweging ](../../../../manage-work/issues/manage-issues/move-issues.md).

## Nieuwe Configuratie voor het Herroepen van Verzoeken in het gebied van de Montages van de Goedkeuring {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

We hebben een nieuwe instelling in het gedeelte Goedkeuringsinstellingen op systeemniveau geïntroduceerd, zodat Workfront-beheerders kunnen beslissen of ze gebruikers moeten toestaan een probleem op te lossen of een verzoek in te dienen waarvan de eerste status in afwachting is van goedkeuring. Als het terugroepen wordt toegestaan, wordt de kwestie geschrapt; als het terugroepen niet wordt toegestaan, kunnen de gebruikers geen knoop van de Herhaling zien wanneer de eerste status van een kwestie in afwachting van goedkeuring is.

Voordat deze wijziging plaatsvond, was het altijd toegestaan om de kwestie te herhalen. Toen de goedkeuring werd teruggeroepen, werd de goedkeuring volledig omzeild en werd de kwestie in de eerste status geplaatst, zonder dat er goedkeuring was toegevoegd.

Voor meer informatie over goedkeuringsmontages, zie [ globale goedkeuringsmontages ](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md) vormen. 

>[!NOTE]
>
>Deze optie wordt standaard uitgeschakeld wanneer deze functie wordt uitgebracht. Momenteel wordt het herinneren van kwesties toegelaten door gebrek voor alle organisaties. Wanneer deze functie wordt uitgebracht, moet de Workfront-beheerder deze instelling handmatig inschakelen om de functionaliteit te behouden zoals in Workfront.

## Nieuwe groepering voor het Bron begrote Uren rapporteert: Datum van toewijzing {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Wij hebben de capaciteit toegevoegd om uw resultaten tegen de Datum van de Toewijzing te groeperen wanneer u een Bron Gefedgeted rapport van het Uur bouwt.

Voorafgaand aan deze wijziging kon u de Datum van Toewijzing in de mening van het rapport tonen, evenals het in een filter gebruiken, maar u kon dit gebied niet in een groepering gebruiken.

Voor meer informatie over de Datum van de Toewijzing, zie [ Verklarende woordenlijst van de terminologie van Adobe Workfront ](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Voor meer informatie over de bouw van een rapport, zie [ een douanerapport ](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Verbeteringen voor middelenplanner {#resource-planner-improvements}

* [ Planner van het Middel: Toon Gegevens door FTE ](#resource-planner-show-data-by-fte)
* [ Planner van het Middel: Toon Gegevens door Week en Kwartaal ](#resource-planner-show-data-by-week-and-quarter)
* [ Planner van het Middel: Mening door Gebruiker ](#resource-planner-view-by-user)
* [ Planner van het Middel: De belemmering en Daling Projecten om Prioriteit ](#resource-planner-drag-and-drop-projects-to-establish-priority) te vestigen
* [De Planner van het middel: Exporteer de gegevens in de Planner van het Middel aan Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Bronnen: Gegevens per FTE tonen {#resource-planner-show-data-by-fte}

U kunt de toewijzing en beschikbaarheid van uw middelen door FTE in de Planner van het Middel nu tonen. Vóór deze wijziging kon u de waarden alleen in uren weergeven.

Voor meer informatie over het gebruiken van de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Bronnen: Gegevens per week en per kwartaal weergeven {#resource-planner-show-data-by-week-and-quarter}

U kunt het tijdkaderinterval voor uw Planner van het Middel nu veranderen om het tegen week of kwartaal te bekijken. Voordat deze wijziging plaatsvond, kon u de toewijzing en beschikbaarheid van uw middelen bekijken en deze slechts per maand begroten.

Voor meer informatie over het gebruiken van de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resourceplanner: Weergeven op gebruiker {#resource-planner-view-by-user}

U kunt de informatie in de Planner van het Middel nu tonen door gebruiker, eerst, dan door projecten, rollen, en taken. U kunt ook een verschil weergeven tussen Geplande en Beschikbare uren of VTE voor gebruikers. Voorafgaand aan deze verandering, kon u de informatie in de Planner van het Middel door projecten en rollen tonen.

Voor meer informatie over het gebruiken van de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Bronnen: projecten slepen en neerzetten om prioriteit vast te stellen {#resource-planner-drag-and-drop-projects-to-establish-priority}

U kunt projecten nu in de gewenste volgorde van prioriteit slepen en neerzetten. Voorafgaand aan deze verandering, kon u de prioriteit van projecten vestigen slechts door hen manueel een aantal toe te wijzen.

Voor meer informatie over het gebruiken van de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### De Planner van het middel: Exporteer de gegevens in de Planner van het Middel aan Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

U kunt de informatie in de Planner van het Middel nu naar een dossier van Excel uitvoeren.

Voor meer informatie over het gebruiken van de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Mobiele verbeteringen {#mobile-improvements}

We hebben de mogelijkheid toegevoegd om toegang te krijgen tot uw projecten en deze te beheren vanuit de Workfront Mobile-app. U kunt nu het volgende doen met de mobiele app Workfront:

* Toegang tot een lijst met uw projecten
* Heb toegang tot een lijst van taken en subtaken op een project
* Toegang tot een lijst met problemen in een project
* Een nieuw probleem in een project vastleggen

U kunt deze functionaliteit installeren wanneer u de mobiele Workfront-app bijwerkt. De update is in november 2017 beschikbaar in de mobiele winkels van Apple en Android.

## Workfront-integratie met Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>De Slack-integratie is momenteel niet beschikbaar. Het zal met uw milieu van de Productie in november 2017 beschikbaar zijn te gebruiken.

We lanceren een nieuwe integratie tussen Workfront en Slack. Als uw organisatie Slack al voor uw communicatie gebruikt, kunt u het nu integreren met Workfront en gemeenschappelijke acties van Workfront uitvoeren zonder uw communicatiekanalen in Slack te verlaten. U kunt nu de volgende handelingen uitvoeren vanaf uw Slack-account:

* Zoeken naar een object in Workfront
* Toegang tot uw werk- en goedkeuringslijsten
* Een taak maken
* Een uitgave maken
* Abonneren op een item vanuit een koppeling die met u wordt gedeeld aan dat item
* Taken en problemen toewijzen vanuit een koppeling die u met u deelt
* Uw werk goedkeuren
* Heb toegang tot uw Favorieten en uw Recente lijsten van Punten

Voor meer informatie over de toegang tot van Workfront van Slack, zie [ Gebruikend Workfront met Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Outlook 365-verbeteringen {#outlook-365-improvements}

We hebben de volgende verbeteringen aangebracht in de invoegtoepassing Workfront voor  Outlook 365:

* Voeg een taak of een kwestie aan een project in Workfront toe: U kunt een e-mail naar een taak of een kwestie in Workfront nu omzetten, gebruikend toe:voegen-binnen van Vooruitzichten 365. In dit proces, kunt u een project specificeren u de taak of de kwestie wilt worden toegevoegd aan, evenals een ontvanger en een vervaldatum. Voorafgaand aan deze verhoging, kon u een verzoek aan een verzoekrij slechts voorleggen of een persoonlijke taak toevoegen aan uw het Werken aan lijst van Vooruitzichten 365. 
* Een koppeling naar Workfront-objecten behouden in de oorspronkelijke e-mail die is geconverteerd naar taken, problemen of verzoeken: wanneer u een e-mail vanuit Outlook 365 converteert naar een taak, uitgave of aanvraag, blijft in Outlook 365 een koppeling behouden naar de taak of uitgave die vanuit die e-mail is geconverteerd in de oorspronkelijke e-mail. Voorafgaand aan deze verandering, was er geen aanwijzing in Vooruitzichten of een e-mail in een taak was omgezet of als verzoek ingediend. 

## API-wijzigingen {#api-changes}

* [ API 8 nu Beschikbaar ](#api-8-now-available)
* [ Verwijderd en Vervangen Versies van API ](#removed-and-deprecated-versions-of-the-api)
* [ 2017.3 de Eindversieactiviteit van Beta ](#updated-message-format-for-event-subscriptions)
* [Abonnement voor gebeurtenissen retourneert voor niet-leverbare berichten](#event-subscription-retries-for-undeliverable-messages)

### API 8 nu beschikbaar {#api-8-now-available}

Workfront API versie 8 is nu beschikbaar en biedt u nieuwe en bijgewerkte bronnen voor uw Workfront-integratie.

Voor een lijst van veranderingen die aan Workfront API worden aangebracht, zie [ Updates aan API Versie 8 ](../../../../wf-api/api/new-api-version-8-updates.md).

### Verwijderde en verwijderde versies van de API {#removed-and-deprecated-versions-of-the-api}

### Bijgewerkte berichtindeling voor abonnementen op gebeurtenissen

Om nuttiger informatie voor uw integratie te verstrekken die de API van de Abonnementen van de Gebeurtenis van Workfront omvatten, hebben wij het uitgaande berichtformaat voor gesteunde middelen veranderd door de oude en nieuwe waarden te omvatten verbonden aan die middelen. Om mislukking te vermijden, zullen om het even welke integraties u de Abonnementen API van de Gebeurtenis van Workfront gebruikt het nieuwe formaat moeten worden bijgewerkt, zoals die in [ wordt beschreven Abonnement API van de Gebeurtenis ](../../../../wf-api/general/event-subs-api.md).

### Abonnement voor gebeurtenissen retourneert voor niet-leverbare berichten {#event-subscription-retries-for-undeliverable-messages}

Het Workfront Event Subscription Framework biedt nu een mechanisme voor de afhandeling van door gebeurtenissen geïnitieerde uitgaande berichten die niet aan eindpunten van de klant worden geleverd. Om voortdurende berichtlevering te verzekeren, zouden de Klanten ervoor moeten zorgen dat om het even welke eindpunten die uitgaande berichten van gebeurtenisabonnementen verbruiken behoorlijk opstelling zijn. Voor meer informatie, zie [ het abonnementsretry van de Gebeurtenis ](../../../../wf-api/api/event-sub-retries.md).
