---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 4 releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de 2017.3 bèta 4-release. De functionaliteit op deze pagina is in de week van 25 september 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin november 2017 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# 2017.3 Beta 4 releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de 2017.3 bèta 4-release. De functionaliteit op deze pagina is in de week van 25 september 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal begin november 2017 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2017.3 zijn aangebracht, raadpleegt u  [Overzicht van releaseactiviteiten 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

De 2017.3 bèta 4-versie bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**Voor beheerders**

* [Het nieuwe gebied van de Voorkeur van het Beheer van het Middel in het Gebied van de Opstelling](#new-resource-management-preferences-area-in-the-setup-area)

**Voor alle gebruikers**

* [Taken dupliceren](#duplicate-tasks)
* [Toewijzingen automatiseren tijdens het plannen van bronnen](#automate-assignments-when-scheduling-resources)
* [Toewijzingen wijzigen voor meerdere taken bij het plannen van bronnen](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [FTE-distributie toepassen op de bronnenplanner](#apply-fte-distribution-to-the-resource-planner)
* [Sectie Functie voor gebruikersinstellingen bevat percentage van FTE-beschikbaarheid](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Filters opslaan en beheren in het gebruiksrapport van een project](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Aanvullende filteropties in het gebruiksrapport](#additional-filtering-options-in-the-utilization-report)
* [Het gebruiksrapport per programma of Portfolio weergeven](#view-the-utilization-report-by-program-or-portfolio)
* [Originele informatie over problemen tonen in project- en taakrapporten](#show-original-issue-information-in-project-and-task-reports)
* [De Updates van het Systeem van de filter in de Stroom van de Update zijn nu Blijvend over Voorwerpen](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Rapport over actieve proefboekfasen in Workfront](#report-on-active-proof-stages-within-workfront)
* [Aangepaste Workfront Proef-machtigingsprofielen toewijzen aan gebruikers in Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Uur-bron toegevoegd aan abonnementen voor gebeurtenissen](#hour-resource-added-to-event-subscriptions)

## Taken dupliceren {#duplicate-tasks}

U kunt nu snel een taak of een set taken in een project dupliceren. Met deze handeling wordt een taak gemaakt die identiek is aan de oorspronkelijke taak. Er zijn geen extra opties tijdens het duplicatieproces waarmee u wijzigingen kunt aanbrengen in de nieuwe taak.  

Voorafgaand aan deze verandering, kon u een taak aan of een nieuw project, of het bestaande project kopiëren en sommige informatie wijzigen aangezien u het kopieerde.

Zie voor meer informatie over het dupliceren van taken [Taken kopiëren en dupliceren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Toewijzingen automatiseren tijdens het plannen van bronnen {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie [Overzicht van de werklastbalans](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

U kunt Workfront nu toestaan om taken voor niet toegewezen taken en kwesties automatisch voor te stellen wanneer het plannen van middelen voor veelvoudige projecten (van het Plannende lusje) of wanneer het plannen van middelen voor één enkel project (van het het Stafsen lusje).

Workfront analyseert de huidige werktoewijzingen voor alle beschikbare gebruikers en stelt intelligente, logische toewijzingen voor voor alle taken of problemen die nog niet zijn toegewezen. U kunt voorgestelde of bestaande toewijzingen wijzigen voordat u de toewijzingen voltooit.

Zie &quot;Niet-toegewezen taken en problemen in de planningsgebieden handmatig toewijzen&quot; voor meer informatie.

## Toewijzingen wijzigen voor meerdere taken bij het plannen van bronnen {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Wanneer het toewijzen van, het ruilen van, of het ongedaan maken van gebruikers in bulk wanneer het plannen van middelen (of van het Plannende lusje of het het Vouwen lusje), kunt u taken voor specifieke taken nu wijzigen die u (met inbegrip van alle subtaken en bijbehorende kwesties) binnen één of meerdere projecten aanwijst.

Voorafgaand aan deze verandering, kon u taken aan taken en kwesties slechts over volledige projecten wijzigen (u kon geen specifieke taken binnen een project aanwijzen).

Zie &quot;Niet-toegewezen taken en problemen in de planningsgebieden handmatig toewijzen&quot; voor meer informatie.

## FTE-distributie toepassen op de bronnenplanner {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Deze functionaliteit is momenteel niet beschikbaar in Voorvertoning voor alle clusters.

U kunt de correcte hoeveelheid Beschikbare Uren voor elke rol van de gebruiker nu tonen die op het Percentage van VTE Beschikbaarheid voor elke rol wordt gebaseerd, wanneer de gebruikers meer dan één rol hebben.

Bijvoorbeeld, als het programma van een gebruiker erop wijst dat zij 100 uren in één maand beschikbaar zijn te werken, en hun percentage van VTE Beschikbaarheid voor de Primaire Rol 75% is en het percentage van de Beschikbaarheid FTE van hun Andere Rol 25% is, zal de Planner van het Middel de gebruiker met 75 Beschikbare Uren onder hun Andere Rol en met 25 Beschikbare Uren een lijst maken.

Voorafgaand aan deze verandering, werd de naam van de gebruiker die in de Planner van het Middel slechts voor de Primaire Rol wordt getoond, en de volledige beschikbaarheid van de gebruiker die op hun programma (100 uren) wordt gebaseerd geassocieerd slechts met de Primaire Rol. De andere Rol van de gebruiker die in de Planner van het Middel slechts wordt getoond als de gebruiker aan een taak in die rol werd toegewezen en de Beschikbare Uren voor de gebruiker in de Andere Rol nul was.

Voor meer informatie over hoe Beschikbare Uren en Beschikbare FTEs voor gebruikers en rollen in de Planner van het Middel worden berekend, zie [Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Sectie Functie voor gebruikersinstellingen bevat percentage van FTE-beschikbaarheid {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Deze functionaliteit is momenteel niet beschikbaar in Voorvertoning voor alle clusters.

Wanneer u nu een gebruikersprofiel bijwerkt, kunt u extra taakrollen aan een gebruiker toevoegen en het percentage van de FTE definiëren dat aan elke taakrol wordt toegewezen.

Vóór deze wijziging kon u geen specifieke hoeveelheid VTE toewijzen aan een van de taakrollen waaraan de gebruiker was gekoppeld.

Voor meer informatie over het bijwerken van het Percentage van Beschikbaarheid FTE voor de de baanrollen van de gebruiker, zie [Gebruikersprofiel bewerken](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) of [Mijn instellingen configureren](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Het nieuwe gebied van de Voorkeur van het Beheer van het Middel in het Gebied van de Opstelling {#new-resource-management-preferences-area-in-the-setup-area}

U kunt een nieuw gebied in Opstelling nu vinden genoemd het Beheer van het Middel. Op dit gebied, hebben wij een het plaatsen geïntroduceerd die u toestaat om te specificeren hoe te om gebruikersbeschikbaarheid in de Planner van het Middel te berekenen. U kunt de berekening als volgt uitvoeren:

* Handmatig: het standaardschema van het systeem wordt naast de afzonderlijke VTE van de gebruiker gebruikt om de beschikbaarheid van het uur van de gebruiker in de Planner van het Middel te bepalen. Het schema van de gebruiker wordt genegeerd.
* Automatisch: Het Programma van de gebruiker wordt gebruikt om de uurbeschikbaarheid van de gebruiker in de Planner van het Middel te bepalen. De beschikbaarheid van FTE wordt berekend gebaseerd op het Programma van de gebruiker en het Standaard Programma. De waarde van de gebruiker FTE wordt genegeerd. 

Zie voor meer informatie over het configureren van voorkeuren voor het beheer van bronnen voor uw systeem [Voorkeuren voor beheer van bronnen configureren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Filters opslaan en beheren in het gebruiksrapport van een project {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Nu kunt u filters bewaren die u in het rapport van het Gebruik creeert. Bovendien kunt u de naam van een opgeslagen filter wijzigen, een opgeslagen filter dupliceren, een opgeslagen filter verwijderen of een opgeslagen filter wijzigen.

Eerder, moest u individuele filteropties specificeren telkens als u het rapport van het Gebruik filtreerde.

Zie voor meer informatie over het opslaan en beheren van filters in het gebruiksrapport [Overzicht van het verslag over het gebruik van hulpbronnen](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overzicht van het verslag over het gebruik van hulpbronnen](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Aanvullende filteropties in het gebruiksrapport {#additional-filtering-options-in-the-utilization-report}

Nu wanneer het runnen van het rapport van het Gebruik, zijn de nieuwe het filtreren gebieden voor Portfolio&#39;s, Programma&#39;s, en Projecten nu beschikbaar wanneer het creëren van uw filter, naast de de Taken, Kwesties, en gebieden van Rollen die eerder beschikbaar waren.

Voorafgaand aan deze verandering, kon u filtreren door portefeuille, programma, en project slechts door een nieuwe filterregel toe te voegen.

Zie voor meer informatie [Overzicht van het verslag over het gebruik van hulpbronnen](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overzicht van het verslag over het gebruik van hulpbronnen](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Het gebruiksrapport per programma of Portfolio weergeven {#view-the-utilization-report-by-program-or-portfolio}

U kunt nu een gebruiksrapport per programma of portfolio weergeven. Dit laat u toe om informatie van veelvoudige projecten binnen één enkel Rapport van het Gebruik te zien.

Om deze verandering te vergemakkelijken, is het lusje van het Gebruik nu beschikbaar zowel in het Rapporterende gebied binnen Workfront, als binnen een individueel project.

Voorafgaand aan deze verandering, konden de Rapporten van het Gebruik slechts binnen een project worden betreden.

Zie voor meer informatie  [Overzicht van het verslag over het gebruik van hulpbronnen](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Originele informatie over problemen tonen in project- en taakrapporten {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Deze functionaliteit is momenteel niet beschikbaar in Voorvertoning voor alle clusters.

U kunt nu de volgende informatie over de originele kwestie in een project of taakrapport, voor de projecten en de taken vinden die door een kwestie om te zetten werden gecreeerd:

* Oorspronkelijke invoerdatum afgifte
* Oorspronkelijke naam van uitgave
* Oorspronkelijke ID van maker van uitgave

Deze informatie kan in een taak of een projectrapport of een lijst worden getoond door een douanemening op tekstwijze te bouwen.

Voor deze wijziging kon je deze gegevens niet melden.

Voor meer informatie over het bouwen van de de wijze van de douanetekst mening die de informatie van de originele kwestie vangt, zie [Weergave: oorspronkelijke informatie weergeven over taken en projectlijsten](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## De Updates van het Systeem van de filter in de Stroom van de Update zijn nu Blijvend over Voorwerpen {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Deze functionaliteit is niet vrijgegeven voor de voorvertoningsomgeving met Bèta 4. Deze is beschikbaar in Voorvertoning in de eerste helft van oktober.

De optie Systeemupdates filteren is nu blijvend in alle objecten op de Workfront-site. Hierdoor kunt u systeemupdates verbergen en alleen gebruikersopmerkingen in de updatestroom voor één object weergeven. Deze instelling blijft behouden wanneer u naar andere objecten bladert.

Voordat u deze wijziging aanbracht, moest u de systeemupdates voor elk object uitfilteren terwijl u door de Workfront-site bladerde.

Zie voor meer informatie [Werk bijwerken](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Rapport over actieve proefboekfasen in Workfront {#report-on-active-proof-stages-within-workfront}

Wanneer u een rapport van de documentversie maakt in Workfront, wordt nu een kolom met de naam Actieve proefdrukfasen weergegeven. In deze kolom kunt u het proefdrukwerkgebied weergeven dat momenteel actief is op elke documentversie in het rapport. De naam van het werkgebied wordt weergegeven in de kolom &quot;Actieve proefdrukstadia&quot;. Als er momenteel geen werkgebied actief is in de documentversie, is de kolom leeg.

Zie voor meer informatie over beschikbare velden in weergaven en rapporten [Woordenlijst met Adobe Workfront-terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Aangepaste Workfront Proef-machtigingsprofielen toewijzen aan gebruikers in Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Wanneer u nu proofingmogelijkheden inschakelt voor een gebruiker in Workfront, kunt u een aangepast Workfront Proof-machtigingsprofiel toewijzen. 

Voorafgaand aan deze verandering, slechts waren de volgende toestemmingsprofielen beschikbaar: Supervisor, Manager, Beheerder.

## Uur-bron toegevoegd aan abonnementen voor gebeurtenissen {#hour-resource-added-to-event-subscriptions}

Met de nieuwe Uur-bron kunt u nu een gebeurtenisabonnement maken om uw factureringstoepassing synchroon te houden met Workfront.

Zie voor meer informatie over gebeurtenisabonnementen [API voor abonnementen voor gebeurtenissen](../../../../wf-api/general/event-subs-api.md).
