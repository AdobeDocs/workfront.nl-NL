---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 1-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de release 2017.3. De functionaliteit op deze pagina is op 9 augustus 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin november 2017 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# 2017.3 Beta 1-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de release 2017.3. De functionaliteit op deze pagina is op 9 augustus 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin november 2017 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2017.3 zijn aangebracht, raadpleegt u  [ 2017.3 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

De Beta 1-release van 2017.3 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders:**

* [ verhindert taken en kwesties worden geschrapt wanneer de uren worden geregistreerd ](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [ Verwijdering van het &quot;Vroege Toegang&quot;Plaatsen van het Gebied van de Opstelling ](#removal-of-the-early-access-setting-from-the-setup-area)
* [Workfront - standaard e-mailadres wijzigen](#workfront-default-email-address-change)

**voor Alle Gebruikers:**

* [ de Plannende Verbeteringen van het Middel ](#resource-scheduling-improvements)
* [ Vertoning Breedbeeld ](#widescreen-display)
* [ Resize en maak Kolommen in Rapporten en Lijsten opnieuw in orde ](#resize-and-reorder-columns-in-reports-and-lists)
* [ Duidelijke Optie van Gegevens van de Douane wanneer het kopiëren van Taken en Kwesties ](#clear-custom-data-option-when-copying-tasks-and-issues)
* [ creeer direct een Project van een Malplaatje ](#create-a-project-directly-from-a-template)
* [ In-App Bericht voor Geabonneerde Voorwerpen ](#in-app-notification-for-subscribed-objects)
* [@Tagging momenteel niet beschikbaar in de voorvertoningsomgeving ](#tagging-currently-not-available-in-the-preview-environment)
* [Gegevens over gebruikerstoewijzing opnemen in het gebruiksrapport van een project](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Verbeteringen in bronnenplanning {#resource-scheduling-improvements}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [ Overzicht van de Balancer van de Werkbelasting ](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

De volgende middelen die verbeteringen plannen zijn beschikbaar wanneer het plannen van middelen voor een team, voor een project, of voor veelvoudige projecten als middelmanager:

* [ Mening die Gebied op het Volledige Scherm plant Wijze ](#view-scheduling-area-in-full-screen-mode)
* [ Meer Opties van de Waaier van de Datum om het Middel te bekijken die Gebied ](#more-date-range-options-for-viewing-the-resource-scheduling-area) plannen
* [Geprojecteerde datums weergeven op de geplande tijdlijn](#view-projected-dates-on-the-scheduling-timeline)

### Gebied voor planning weergeven in de modus Volledig scherm {#view-scheduling-area-in-full-screen-mode}

U kunt de tijdlijn van de planning weergeven in de modus Volledig scherm, zodat u meer informatie kunt zien in één weergave. 

Voor meer informatie, zie &quot;Begonnen met het Plannen van het Middel&quot;.

### Meer Opties van de Waaier van de Datum voor het Bekijken van het Gebied van de Planning van het Middel {#more-date-range-options-for-viewing-the-resource-scheduling-area}

U kunt de volgende aanvullende opties voor het datumbereik weergeven wanneer u de tijdlijn van de planning bekijkt:

* Weergave één dag
* Weergave van 4 weken
* Weergave van 6 weken

Voorafgaand aan deze wijziging kon u de planningstijdlijn alleen bekijken in een weergave van 1 week, 2 week of 3 weken. Deze datumbereiken zijn nog steeds beschikbaar naast de nieuwe datumbereiken.

Wanneer u de plantijdlijn in een weergave van één dag weergeeft, kunnen gebruikerstoewijzingen (inclusief dagelijkse totale uren) niet worden weergegeven.

Voor meer informatie, zie &quot;Begonnen met het Plannen van het Middel&quot;.

### Geprojecteerde datums weergeven op de geplande tijdlijn {#view-projected-dates-on-the-scheduling-timeline}

Nu kunt u de planningschronologie vormen om de Geprojecteerde Datums eerder dan de Geplande Datums voor taken en kwesties te tonen. 

Vóór deze wijziging werden taken en problemen in de tijdlijn van de planning alleen weergegeven op Geplande datums.

Wanneer u de Geprojecteerde Datums op de planningschronologie bekijkt, kunnen de gebruikerstoewijzingen (met inbegrip van dagelijkse totale uren) niet worden getoond.

Voor meer informatie, zie &quot;Begonnen met het Plannen van het Middel&quot;.

## Breedbeeld {#widescreen-display}

Wanneer u een van de volgende objecten in Workfront weergeeft, wordt het volledige browservenster automatisch gevuld:

* Projecten
* Taken
* Problemen
* Rapporten
* Dashboards
* Kalenders

Vóór deze wijziging stonden aan beide zijden van het weergegeven gebied twee witte zijbalken. De breedbeeldweergave wordt nu dynamisch aangepast aan de breedte van het scherm en het browservenster.

## Kolommen in rapporten en lijsten vergroten/verkleinen en opnieuw ordenen {#resize-and-reorder-columns-in-reports-and-lists}

U kunt kolommen in een rapport of lijst nu opnieuw rangschikken en resize, zonder het moeten het rapport uitgeven. (Deze functionaliteit werd verwijderd met de veroudering van het milieu van de Vroege Toegang eerder dit jaar. Het wordt nu opnieuw ingevoerd.)

Deze functionaliteit is niet beschikbaar voor dashboardlijsten of -rapporten, omdat deze lijsten opnieuw zijn ontworpen in een nieuwe structuur van het gegevensraster. Voor alle andere lijsten is deze functionaliteit ingeschakeld met deze versie.

Voor meer informatie over het resizing en het opnieuw rangschikken van kolommen, zie [ kolombreedte en orde wijzigen ](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Optie Aangepaste gegevens wissen bij het kopiëren van taken en problemen {#clear-custom-data-option-when-copying-tasks-and-issues}

Wanneer u een taak of uitgave kopieert, kunt u nu een optie selecteren om aangepaste gegevens te wissen. Wanneer u de aangepaste gegevens van een taak of uitgave wist, wordt het formulier naar het nieuwe item gekopieerd, maar de aangepaste gegevens op het formulier niet. Het wissen van aangepaste gegevens heeft ook invloed op de aangepaste formulieren die zijn gekoppeld aan de documenten die aan de items zijn gekoppeld, of op de aangepaste formulieren die zijn gekoppeld aan de uitgaven voor de taak.

Vóór deze wijziging werden de aangepaste gegevens die in een aangepast formulier waren opgenomen, ook naar het nieuwe item gekopieerd toen u de taak of uitgave kopieerde. 

Voor meer informatie over het kopiëren van taken, zie [ Kopiëren en dupliceren taken ](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Voor meer informatie over het kopiëren van kwesties, zie [ kwesties van het Exemplaar ](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Een project rechtstreeks van een sjabloon maken {#create-a-project-directly-from-a-template}

U kunt nu een project van een malplaatje, op het malplaatjeniveau tot stand brengen.

Voorafgaand aan deze verandering, kon u een project van een malplaatje slechts op het lusje van Projecten in het gebied van Projecten van Workfront tot stand brengen, door het **Nieuwe Project van Malplaatje** optie te gebruiken.

Voor meer informatie over het creëren van een project van een malplaatje, zie [ een project creëren gebruikend een malplaatje ](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Voorkomen dat taken en problemen worden verwijderd wanneer de uren worden geregistreerd {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

U kunt Workfront nu configureren om taken en problemen waarvoor uren zijn geregistreerd, toe te staan of te verwijderen.

Voorafgaand aan deze verandering, toen u een taak of kwestie schrapte waar de uren werden geregistreerd, werden de uren of met de taak of de kwestie geschrapt, of zij werden verplaatst naar het project, afhankelijk van uw Voorkeur Timesheet &amp; van de Uren.

Voor meer informatie over het schrappen van taken, zie [ de taken van de Schrapping ](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Voor meer informatie over het schrappen van kwesties, zie [ kwesties van de Schrapping ](../../../../manage-work/issues/manage-issues/delete-issues.md).

Voor meer informatie over het toelaten van het systeem dat voor taak en uitgevende schrapping plaatst, zie [ de taak van het hele systeem vormen en voorkeur uitgeven ](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Verwijderen van de instelling &quot;Vroege toegang&quot; uit het installatiegebied {#removal-of-the-early-access-setting-from-the-setup-area}

We verwijderen de instelling waarmee Workfront-beheerders gebruikers konden inschrijven voor deelname aan de omgeving van Vroege toegang. Deze functionaliteit is sinds eind 2016 verouderd. We hebben in 2017 geen nieuwe functionaliteit vrijgegeven voor vroege toegang en alle functies die in die omgeving overbleven, zijn verplaatst naar Productie.

Voorafgaand aan deze wijziging konden Workfront-beheerders nog steeds gebruikers toevoegen aan de omgeving Vroege toegang, hoewel er geen nieuwe functies beschikbaar waren.

## Workfront - standaard e-mailadres wijzigen {#workfront-default-email-address-change}

Het standaard e-mailadres voor uitgaande post van Workfront is veranderd van [ noreply@attask.com ](mailto:noreply@attask.com) in [ noreply@my.workfront.com ](mailto:noreply@workfront.com).

Als u momenteel e-mailberichten filtert die vanuit Workfront worden verzonden, moet u het filter aanpassen aan het nieuwe standaardadres. 

De wijziging in het standaardadres heeft geen invloed op geconfigureerde Workfront-e-mailadressen. 

Zie voor meer informatie.

## Melding in app voor geabonneerde objecten {#in-app-notification-for-subscribed-objects}

Wanneer een gebruiker een opmerking maakt over projecten, taken en problemen waarvoor u een abonnement hebt, ontvangt u nu een melding in de app. Meer over abonnement in-app berichten leren, zie [ Mening en beheer in-app berichten ](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Afhankelijk van de functies die uw Workfront-beheerder heeft ingeschakeld, kunt u ook e-mailmeldingen ontvangen voor geabonneerde items. U kunt van een punt door een verbinding op een abonnements-e-mail gemakkelijk afmelden, zoals beschreven in [ Adobe Workfront-meldingen ](../../../../workfront-basics/using-notifications/wf-notifications.md) .

Vóór deze wijziging hebt u altijd een e-mailbericht voor geabonneerde items ontvangen. Er was geen optie om een melding in de app te ontvangen.

U kunt het e-mailbericht met een abonnement uitschakelen, maar u kunt meldingen in de app voor geabonneerde items niet uitschakelen. Voor meer informatie zie [ gebeurtenisberichten voor iedereen in het systeem ](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) vormen.

Meer leren over het intekenen op punten, zie [ aan punten in Adobe Workfront ](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md) intekenen.

## @Tagging is momenteel niet beschikbaar in de voorvertoningsomgeving {#tagging-currently-not-available-in-the-preview-environment}

Wanneer we werken om de updatestream Rich Text Format-functionaliteit te geven, kunt u tijdelijk het @-symbool niet gebruiken om andere gebruikers in de updatestream een tag toe te wijzen voor de volgende objecten in de Voorvertoningsomgeving:

* Project
* Taak
* Probleem
* Tijdschema

U kunt anderen nog etiketteren door **te klikken omvat anderen op dit pictogram van de Update**.

Voor meer informatie, zie [ Tags anderen op updates ](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Gegevens over gebruikerstoewijzing opnemen in het gebruiksrapport van een project {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [ Overzicht van de Balancer van de Werkbelasting ](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

In het gebruiksverslag voor een project wordt nu rekening gehouden met de vraag of de geplande uren tijdens de duur van een taak opnieuw zijn toegewezen. Wanneer de gebruikerstoewijzing voor uren is gewijzigd (zoals beschreven in &quot;Gebruikerstoewijzingen beheren in de planningsgebieden&quot;), kunnen de gegevens in het gebruiksrapport worden beïnvloed als de data die zijn geselecteerd in het gebruiksrapport slechts een deel van een taak bevatten.

Voor meer informatie, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
