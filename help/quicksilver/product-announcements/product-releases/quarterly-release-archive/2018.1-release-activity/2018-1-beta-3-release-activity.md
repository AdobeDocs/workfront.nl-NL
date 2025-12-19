---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 3-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 3-release van 2018.1. De functionaliteit is op 7 januari 2018 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin 2018 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# 2018.1 Beta 3-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 3-release van 2018.1. De functionaliteit is op 7 januari 2018 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin 2018 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2018.1 zijn aangebracht, raadpleegt u  [&#x200B; 2018.1 overzicht van de versieactiviteit &#x200B;](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

De Beta 3-release van 2018.1 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders**

* [de Verbeteringen van de groepsbeheerder](#group-administrator-improvements)

**voor Alle Gebruikers**

* [&#x200B; HTML5 die de Verbeteringen van de kijker het proef &#x200B;](#html5-proofing-viewer-improvements)
* [&#x200B; het Bewijzen Verbeteringen binnen Workfront &#x200B;](#proofing-improvements-within-workfront)
* {de Verbeteringen van het 0} Gebied van het Huis [&#x200B; &#x200B;](#home-area-improvements)
* [&#x200B; de Verbeteringen van de Gelijkheid &#x200B;](#agile-improvements)
* [&#x200B; de Verbeteringen van de Grafiek van de Gantt &#x200B;](#gantt-chart-improvements)
* [Verbeteringen voor middelenplanner](#resource-planner-improvements)

## de Verbeteringen van de groepsbeheerder {#group-administrator-improvements}

* [&#x200B; Wachtwoord UI van het Terugstellen voor groepsbeheerders &#x200B;](#reset-password-ui-updated-for-group-administrators) bijgewerkt
* [&#x200B; de Opties van de Opstelling van het Niveau van de Toegang voor groepsbeheerders &#x200B;](#access-level-setup-options-for-group-administrators)
* [&#x200B; creeer de Profielen van de Chronologie voor Groepen &#x200B;](#create-timesheet-profiles-for-groups)
* [Verwijderde items herstellen voor gebruikers als groepsbeheerder](#recover-deleted-items-for-users-as-a-group-administrator)

### Gebruikersinterface voor wachtwoorden opnieuw instellen voor groepbeheerders {#reset-password-ui-updated-for-group-administrators}

Als groepsbeheerder, wanneer u het wachtwoord voor een andere gebruiker terugstelt, wordt u veroorzaakt voor uw eigen wachtwoord alvorens u hun kunt veranderen. De gebruikersinterface is bijgewerkt met deze functionaliteit. Voorafgaand aan deze wijziging toonde de gebruikersinterface aan dat het Workfront-beheerderswachtwoord vereist was.

Voor meer informatie over het terugstellen van wachtwoorden voor andere gebruikers, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

Voor meer informatie over de mogelijkheden van een groepsbeheerder, zie de &quot;Mogelijkheden van de sectie van groepsbeheerders&quot;in [&#x200B; een groep &#x200B;](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

### De Opties van de Opstelling van het Niveau van de toegang voor groepsbeheerders {#access-level-setup-options-for-group-administrators}

Als Workfront-beheerder kunt u nu bepalen of groepsbeheerders zich kunnen aanmelden als andere gebruikers of dat ze de wachtwoorden van andere gebruikers kunnen herstellen. We hebben een nieuwe instelling toegevoegd in het toegangsniveau om deze toegang in of uit te schakelen. Voorafgaand aan deze wijziging konden alle groepsbeheerders zich aanmelden als andere gebruikers en de wachtwoorden van andere gebruikers standaard herstellen. Deze wijziging heeft alleen invloed op het toegangsniveau van de Planner.

Voor meer informatie over het vormen van toegangsniveau voor gebruikers, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Voor meer informatie over de mogelijkheden van een groepsbeheerder, zie de &quot;Mogelijkheden van de sectie van groepsbeheerders&quot;in [&#x200B; een groep &#x200B;](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

### Tijdlijnprofielen maken voor groepen {#create-timesheet-profiles-for-groups}

Als groepsbeheerder kunt u nu tijdlijnprofielen maken voor de groepen die u beheert en deze koppelen aan groepen die u beheert, of aan gebruikers van deze groepen. Met tijdbladprofielen zorgt u ervoor dat tijdbladen automatisch worden gemaakt voor de gebruikers die aan tijdbladen zijn gekoppeld.

Vóór deze wijziging kon alleen een Workfront-beheerder tijdbladprofielen maken.

Voor meer informatie over het creëren van de Profielen van de Chronologie, zie [&#x200B; creëren, uitgeven, en toewijzen timesheet profielen &#x200B;](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Voor meer informatie over de mogelijkheden van een groepsbeheerder, zie de &quot;Mogelijkheden van de sectie van groepsbeheerders&quot;in [&#x200B; een groep &#x200B;](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

### Verwijderde items herstellen voor gebruikers als groepsbeheerder {#recover-deleted-items-for-users-as-a-group-administrator}

Als een project met een Groep wordt geassocieerd waarvoor u de groepsbeheerder bent, kunt u het project, of om het even welk van zijn geschrapte taken, kwesties, of documenten van de Bak van de Recycling terugkrijgen. Vóór deze wijziging kon alleen een Workfront-beheerder items uit de prullenbak herstellen.

Voor meer informatie over het terugkrijgen van geschrapte punten in Workfront, zie [&#x200B; geschrapte punten &#x200B;](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.

Voor meer informatie over de mogelijkheden van een groepsbeheerder, zie de &quot;Mogelijkheden van de sectie van groepsbeheerders&quot;in [&#x200B; een groep &#x200B;](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren. 

## Verbeteringen in de HTML5-testviewer  {#html5-proofing-viewer-improvements}

* [&#x200B; vergelijk Wijze &#x200B;](#compare-mode)
* [&#x200B; filter de Lijst van de Commentaar &#x200B;](#filter-the-comment-list)
* [Lijst met opmerkingen wordt doorzocht nadat het eerste teken is ingevoerd](#comment-list-is-searched-after-the-first-character-is-entered)

### Vergelijkingsmodus {#compare-mode}

U kunt de vergelijkingsmodus nu gebruiken in de HTML5-proefdrukviewer wanneer u statische en videoproefdrukken weergeeft. 

De vergelijkingsmodus in de HTML5-proefdrukviewer verschilt op de volgende manieren van de verouderde proefdrukviewer:

* Wanneer u de vergelijkingsmodus start, wordt de nieuwere versie naar rechts verplaatst en wordt de versie die u aan de linkerkant vergelijkt, geopend.

  Eerder werd de nieuwere versie naar links verplaatst, met de versie die u aan de rechterkant vergelijkt.

* U kunt kiezen welke versie van een proefdruk u direct van de het proefdrukken kijker wilt vergelijken. 
* Het huidige zoomniveau en de huidige positie van proefdrukken in de proefdrukviewer blijven behouden wanneer u gelijktijdige navigatie invoert.
* Nieuwe optie Herstellen bij gelijktijdige navigatie.
* Bij het afsluiten van de vergelijkingsmodus kunt u kiezen welke proef u wilt sluiten. 

  Eerder was de oudere versie altijd gesloten.

* Verschillende verbeteringen op het gebied van uiterlijk en bruikbaarheid.

Voor meer informatie, zie [&#x200B; proefdrukken in de het proef kijker &#x200B;](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md) vergelijken.

### De lijst met opmerkingen filteren {#filter-the-comment-list}

U kunt nu opmerkingen filteren in de lijst met opmerkingen. U kunt filteren op gebruiker, handelingen, ongelezen en meer.

### Lijst met opmerkingen wordt doorzocht nadat het eerste teken is ingevoerd {#comment-list-is-searched-after-the-first-character-is-entered}

Wanneer u nu in de lijst met opmerkingen zoekt, wordt de lijst automatisch gefilterd nadat u het eerste teken hebt getypt.

Voordat deze wijziging werd doorgevoerd, moest u ten minste drie tekens in het zoekveld typen voordat de lijst met opmerkingen werd gefilterd.

Zie voor meer informatie in .

## Verbeteringen voor proefdrukken in Workfront {#proofing-improvements-within-workfront}

* [&#x200B; Proefdrukken van de Verbinding van Workfront Proof aan Workfront &#x200B;](#link-proofs-from-workfront-proof-to-workfront)
* [&#x200B; kan niet meer een Bewijs uit een Document verwijderen &#x200B;](#can-no-longer-remove-a-proof-from-a-document)
* [Bijgewerkte look and Feel bij het genereren en openen van proefdrukken](#updated-look-and-feel-when-generating-and-opening-proofs)

### Proefdrukken van Workfront Proof naar Workfront koppelen {#link-proofs-from-workfront-proof-to-workfront}

U kunt nu documentproefdrukken die al in uw Workfront Proof-account bestaan, koppelen aan Workfront.

Vóór deze wijziging was er geen toegang tot proefdrukken die al in Workfront Proof in Workfront bestonden. 

Voor meer informatie, zie [&#x200B; documenten van de Verbinding van externe toepassingen &#x200B;](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) in [&#x200B; documenten van de Verbinding van externe toepassingen &#x200B;](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Kan proefdrukken niet meer verwijderen uit een document {#can-no-longer-remove-a-proof-from-a-document}

U kunt een proefdruk niet meer uit een document verwijderen. Als u een proefdruk wilt verwijderen, moet u het hele document verwijderen.

Deze verbetering vermindert het risico dat gebruikers per ongeluk alle versies van een proefdocument verwijderen. 

Voor informatie over het schrappen van een document, zie [&#x200B; een proef &#x200B;](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) in [&#x200B; Schrapping een proef &#x200B;](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Bijgewerkte look and Feel bij het genereren en openen van proefdrukken {#updated-look-and-feel-when-generating-and-opening-proofs}

Er wordt nu een bijgewerkte animatiespeler weergegeven wanneer een proefdruk wordt gegenereerd.

## Verbeteringen in het thuisgebied {#home-area-improvements}

De volgende verbeteringen zijn aangebracht in het gebied Home:

* [&#x200B; Goedkeuringen van het Bewijs van de Mening van het Gebied van het Huis &#x200B;](#view-proof-approvals-from-the-home-area)
* [Standaardvelden worden weergegeven bij het configureren van de lay-outsjabloon voor items in het begingebied](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Goedkeuringen van proefdrukken weergeven vanuit het thuisgebied {#view-proof-approvals-from-the-home-area}

Naast de standaardgoedkeuringen kunt u nu proefdrukgoedkeuringen bekijken in het gebied Home.

Eerder kon u Workfront-goedkeuringen bekijken, maar geen goedkeuringen voor een proefdruk bekijken.  

Voor meer informatie, zie [&#x200B; Gebruik het gebied van het Huis &#x200B;](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Standaardvelden worden weergegeven bij het configureren van de lay-outsjabloon voor items in het begingebied {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Eerder waren de standaardvelden niet zichtbaar in de lay-outsjabloon.

Zie &quot;Lay-outsjablonen maken en beheren&quot; voor meer informatie.

## Agile-verbeteringen {#agile-improvements}

* [&#x200B; voegt Taken en Kwesties aan de Herhaling direct van de Pagina van de Details van de Taak of van de Uitgave &#x200B;](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page) toe
* [&#x200B; omvat Kwesties op de Achtergrond en de Raad van het Verhaal van het Trommel voor een Geniel Team &#x200B;](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [&#x200B; pas Groepen en Filters op Backlog voor een Gelijk Team &#x200B;](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team) toe
* [&#x200B; creeer een Lege Herhaling en werk het later &#x200B;](#create-a-blank-iteration-and-update-it-later) bij
* [De velden &quot;Focus&quot; en &quot;Capaciteit&quot; worden vooraf ingevuld bij het maken van een herhaling](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Voeg Taken en Kwesties aan de Herhaling direct van de Pagina van de Details van de Taak of van de Uitgave toe {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

U kunt nu taken en problemen die momenteel zijn toegewezen aan een team van Adobe rechtstreeks vanuit de taak of uitgave toevoegen aan een herhaling.

Eerder kon u taken alleen vanuit de achterstand aan een herhaling toevoegen. 

Voor meer informatie, zie [&#x200B; een herhaling &#x200B;](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) in [&#x200B; creëren een herhaling &#x200B;](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Inclusief problemen op de scrum Backlog en Story Board voor een flexibel team {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Problemen worden nu standaard opgenomen in de achterstand van uw Agile-team bij het gebruik van de methode Scrum Agile (problemen worden niet weergegeven op de achterstand van een Agile-team bij het gebruik van de Kanban-methode).

Voorafgaand aan deze wijziging konden alleen taken aan de achterstand worden toegevoegd. Als u een uitgave wilt toevoegen, moest u eerst de kwestie in een taak omzetten alvorens het kon worden toegevoegd.

Voor informatie over het gebruiken van kwesties op de achtergrond, zie  [&#x200B; beheert de Gelijke achterstand &#x200B;](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Groepen en filters toepassen op de achtergrond voor een flexibel team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

De opties Groeperen en Filter zijn nu beschikbaar op de Google-achterstand, zodat u uw achterstand kunt indelen op groepen en filteren op specifieke taken en problemen.

Voordat u deze wijziging aanbrengt, kunt u de weergaven toepassen op de Agile-achterstand.

Zie voor meer informatie  [&#x200B; beheert de Agile backlog &#x200B;](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) binnen  [&#x200B; beheert de Gelijke achterstand &#x200B;](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Een lege herhaling maken en deze later bijwerken {#create-a-blank-iteration-and-update-it-later}

U hoeft geen taak of uitgave meer toe te voegen aan een herhaling om deze te maken. U kunt een lege herhaling maken en taken en problemen op een later tijdstip toevoegen.

Voor meer informatie, zie [&#x200B; een herhaling &#x200B;](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) creëren.

### De velden &quot;Focus&quot; en &quot;Capaciteit&quot; worden vooraf ingevuld bij het maken van een herhaling {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Wanneer u een herhaling maakt, worden de velden &quot;Focus&quot; en &quot;Capaciteit&quot; vooraf gevuld met de gemiddelde waarden voor alle herhalingen uit het verleden die uw team heeft gemaakt. Als uw team geen eerdere herhalingen heeft gemaakt, worden deze velden weergegeven als 0.

Eerder waren deze velden altijd ingesteld op 0.

Voor meer informatie, zie [&#x200B; een herhaling &#x200B;](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) creëren.

## Verbeteringen in Gantt Chart {#gantt-chart-improvements}

* [&#x200B; laat Edit Wijze in de Grafiek van Gantt &#x200B;](#enable-edit-mode-in-the-gantt-chart) toe
* [Voorgangers verwijderen bij het bewerken van het Gantt-diagram](#remove-predecessors-when-editing-the-gantt-chart)

### Bewerkmodus inschakelen in Gantt-diagram {#enable-edit-mode-in-the-gantt-chart}

Als u de bewerkingsmodus inschakelt in het Gantt-diagram, kunt u de informatie in het diagram wijzigen. Vóór deze wijziging kon u de gegevens in het Gantt-diagram niet bewerken. U kunt alleen taakgegevens in de takenlijst bewerken.

Voor meer informatie over het uitgeven van de grafiek van Gantt, zie [&#x200B; informatie van de Update in de Grafiek van Gantt van de taaklijst &#x200B;](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Voorgangers verwijderen bij het bewerken van het Gantt-diagram {#remove-predecessors-when-editing-the-gantt-chart}

Gebruikend de Edit wijze voor de grafiek van Gantt, kunt u voorgangersverhoudingen tussen taken in de grafiek van Gantt van een project nu verwijderen. Voorafgaand aan deze verbetering, kon u de voorgangersverhouding slechts in de taaklijst, of op het taakniveau verwijderen.

Voor meer informatie over het uitgeven van de grafiek van Gantt, zie [&#x200B; informatie van de Update in de Grafiek van Gantt van de taaklijst &#x200B;](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Verbeteringen voor middelenplanner {#resource-planner-improvements}

* [&#x200B; Begroting met Nul Duur in de Planner van het Middel &#x200B;](#budget-with-zero-duration-in-the-resource-planner)

* [Gegevens op kosten weergeven in de bronnenplanner](#show-data-by-cost-in-the-resource-planner)

### Begroting met Duur Nul in de Planner van het Middel {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Deze functie is verwijderd uit de voorvertoningsomgeving en wordt vrijgegeven met versie 18.1.

U kunt uw middelen in de Planner van het Middel voor om het even welke datum, binnen of buiten het tijdkader van het project nu begroten. Voorafgaand aan deze verbetering, kon u uw middelen slechts voor de data binnen het tijdkader van het project begroten.

Voor meer informatie over het in de begroting opnemen van middelen in de Planner van het Middel, zie de &quot;Begrotende Middelen in de sectie van de Planner van het Middel&quot;in [&#x200B; overzicht van de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Gegevens op kosten weergeven in de bronnenplanner {#show-data-by-cost-in-the-resource-planner}

U kunt de informatie in de Planner van het Middel nu tonen door Kosten, naast Uren en FTE waarden. U kunt kosten in de Planner van het Middel tonen wanneer u het in de Mening door Project of Mening door de meningen van de Rol bekijkt. U kunt geen Kosten tonen wanneer u de Planner van het Middel in de Mening door de mening van de Gebruiker bekijkt.

Voor meer informatie over het bekijken van de Planner van het Middel door Uren, VTE, of de waarden van Kosten, zie [&#x200B; het navigatieoverzicht van de Planner van het Middel &#x200B;](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
