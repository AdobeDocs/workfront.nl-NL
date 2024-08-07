---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta Final
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de release 2017.2. De functionaliteit op deze pagina is op 28 juni 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal op 26 juli 2017 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# 2017.2 Beta Final

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de voorvertoningsomgeving met de release 2017.2. De functionaliteit op deze pagina is op 28 juni 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal op 26 juli 2017 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
>De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst van alle veranderingen die in 2017.2 worden aangebracht, zie [ 2017.2 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

De slotversie van Beta van 2017.2 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders:**

* [ bepaalt de Beschikbaarheid van de HTML5 Video het proef kijker (ProofHK en Workfront) ](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [ steun SHA-256 certificaten voor SAML 2.0 ](#support-sha-256-certificates-for-saml-2-0)
* [ Type-Ahead voor de Attributen van de Toewijzing ](#type-ahead-for-mapping-attributes)
* [API-verbetering: toegang tot gebruikerstoewijzingen](#api-enhancement-access-user-allocations)

**voor Alle Gebruikers:**

* [ Planner van het Middel ](#resource-planner)
* [ Nieuw plannend Gebied in een Project (de Bouwer van het Team) ](#new-scheduling-area-in-a-project-team-builder)
* [ Middel die plant: Toon Minder Punten door Standaard ](#resource-scheduling-show-fewer-items-by-default)
* [ Middel die plant: De Indicator van de Daling van de vertoning en over-toewijzing wanneer het slepen van Taken en Kwesties ](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [ Middel die plant: De Toewijzingen van de gebruiker zijn niet meer gerond aan het Dichtstbijzijnde Half uur ](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [ de Uitvoer het Rapport van het Gebruik in TSV en de Formaten van PDF ](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [ 2017.2 Definitief Beta ](#user-calendar-enhancements-in-the-my-work-area%22)
* [ 2017.2 Definitief Beta ](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [ de Beslissingsvertoningen van het Bewijs op het Mijn Gebied van het Werk (Workfront) ](#proof-decision-displays-in-the-my-work-area-workfront)
* [ Proofs van de Media van de Mening Rich in Vooraf ingestelde Resoluties (ProofHK en Workfront) ](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [ Mening URL aan Subpagina&#39;s in Commentaren op Rijke Proofs van Media (ProofHK en Workfront) ](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [ creeer de Mening van de Douane die op Bestaande Standaardmeningen (ProofHQ) wordt gebaseerd ](#create-custom-views-based-on-existing-standard-views-proofhq)
* [ filter het Rapporterende Gebied (ProofHQ) ](#filter-the-reporting-area-proofhq)
* [ Minimale en Maximale Waarden van de Vertoning in Rapporten (ProofHQ) ](#display-minimum-and-maximum-values-in-reports-proofhq)
* [ Meldingen in-app voor Goedkeuring van proef ](#in-app-notification-for-proof-approval)
* [ Mobiele Verbeteringen ](#mobile-improvements)
* [ Snede die aan de Verklaringen van de Filter voor de Waarden van het Gebied wordt toegevoegd die komma&#39;s ](#slash-added-to-filter-statements-for-field-values-that-contain-commas) bevatten
* [ Veelvoudige het Factureren Tarieven ](#multiple-billing-rates)
* [ Nieuw Middel het Beoogde Gebogen Gebied van het Uur ](#new-resource-budgeted-hour-field)
* [Functie gebruikerstaak weergeven in gebied &#39;Toegewezen aan&#39; op de detailpagina voor taken en problemen](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werklast gebruiken, zie [ Overzicht van de Balancer van de Werkbelasting ](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nieuw planningsgebied in een Project (Teambouwer) {#new-scheduling-area-in-a-project-team-builder}

Het plannende gebied in een project (vroeger genoemd geworden Bouwer van het Team) is opnieuw ontworpen met een bijgewerkt en intuïtiever gebruikersinterface. De nieuwe planningsfunctionaliteit past nu meer bij de functie Resource Scheduling die momenteel beschikbaar is in andere delen van Workfront.

Tot de verbeteringen behoren:

* Huidige middeltoewijzingen voor leden van het projectteam bekijken, toestaand u om geïnformeerde besluiten te nemen wanneer het nemen van taken
* Visuele vertegenwoordiging van taakduur op de het plannen chronologie
* De informatie filteren die wordt weergegeven op de tijdlijn van de planning
* U kunt eenvoudig gebruikers toevoegen aan en verwijderen uit het projectteam, rechtstreeks uit de tijdlijn die u wilt plannen

De volgende functionaliteit is beschikbaar op andere gebieden van het hulpmiddel wanneer het plannen van middelen, maar is niet beschikbaar wanneer het plannen van middelen in het Team dat gebied plant:

* Bovenliggende taken configureren voor weergave op de tijdlijn van de planning
* Projectnamen configureren voor weergave op de geplande tijdlijn
* Gebruikerstoewijzingen wijzigen met het gereedschap Omwisselen
* Filteren op portfolio, programma&#39;s en projecten

Voor meer informatie over functionaliteit beschikbaar in het Team dat gebied plant, zie &quot;begonnen worden met Middel het Plannen&quot;.

## Bronnen plannen: Standaard minder items tonen {#resource-scheduling-show-fewer-items-by-default}

Standaard worden er maximaal 10 tijdelijke items per dag weergegeven op de tijdlijn voor de planning voor een bepaalde gebruiker. U kunt de lijst uitvouwen om alle taken en problemen weer te geven die momenteel aan die gebruiker zijn toegewezen.

Hierdoor kunt u gemakkelijker door de tijdlijn bladeren waarin de gebruikers een groot aantal taken en problemen hebben toegewezen.

Vóór deze wijziging werden alle taken en problemen altijd voor alle gebruikers weergegeven.

Zie &quot;Niet-toegewezen taken en problemen in de planningsgebieden handmatig toewijzen&quot; voor meer informatie over het toewijzen van taken en problemen aan gebruikers in de tijdlijn van de planning.

## Bronnen plannen: de indicator voor neerzetten en de overtoewijzing weergeven bij het slepen van taken en problemen {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Wanneer u via slepen en neerzetten een taak of uitgave toewijst aan een gebruiker op de tijdlijn van de planning, wordt nu de volgende informatie weergegeven voordat de taak of uitgave wordt vrijgegeven en de toewijzing wordt voltooid:

* Er wordt een neerzetindicator weergegeven in de rij van de gebruiker. Hierdoor kunt u zien waar een item wordt toegewezen voordat u de toewijzing maakt.
* Als gebruikerstoewijzingen zijn ingeschakeld op de tijdlijn van de planning, worden de rode overtoewijzingsindicatoren weergegeven als het voltooien van de toewijzing ertoe zal leiden dat de gebruiker te veel wordt toegewezen.

Vóór deze wijzigingen werd geen informatie weergegeven voordat de taak of uitgave werd vrijgegeven.

Zie &quot;Niet-toegewezen taken en problemen in de planningsgebieden handmatig toewijzen&quot; voor meer informatie over het toewijzen van taken en problemen aan gebruikers in de tijdlijn van de planning.

## Bronplanning: Toewijzingen van gebruikers worden niet meer afgerond naar het dichtstbijzijnde halve uur {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Wanneer meerdere gebruikers zijn toegewezen aan een taak of uitgave, of wanneer een taak of uitgave meerdere dagen omvat, probeert Workfront geplande uren gelijkmatig te verdelen over de toegewezen gebruikers en dagen. Uren worden standaard afgerond naar de dichtstbijzijnde honderdste (bijvoorbeeld 1,33).

Eerder, wanneer u manueel verdeelde uren veranderde, worden de uren aangepast en afgerond aan het dichtstbijzijnde half uur (bijvoorbeeld, wordt 1.33 afgerond aan 1.5).

Uren worden nu niet meer aangepast en afgerond naar het dichtstbijzijnde halfuur (1,33 blijft bijvoorbeeld 1,33).

## API-verbetering: toegang tot gebruikerstoewijzingen {#api-enhancement-access-user-allocations}

U hebt nu toegang tot schaduw voor gebruikerstoewijzingen via de Workfront API.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exporteer het gebruiksrapport in de indeling TSV en PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

U kunt het rapport van het Gebruik over een project in TSV en PDF formaten, naast het formaat XLSX nu uitvoeren.

Voorafgaand aan deze verandering, kon u het rapport van het Gebruik slechts in formaat XLSX uitvoeren.

Voor meer informatie over het uitvoeren van het rapport van het Gebruik, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [ Overzicht van het rapport van het Gebruik van het Middel ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Het besluit van het bewijs verschijnt in het Mijn Gebied van het Werk (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Wanneer het bekijken van het proefdrukken goedkeuringen in Mijn Goedkeuringen lusje in uw Mijn Gebied van het Werk, wordt het proefdrukbesluit getoond in uw Mijn Gebied van het Werk en blijft tot u de nieuwe Refresh knoop binnen Workfront klikt of tot de volgende tijd u de browser pagina vernieuwt.

Voorafgaand aan deze wijziging was er geen aanwijzing dat er al een besluit was genomen over de proefdruk en dat de proefdruk op het tabblad Mijn goedkeuringen bleef staan totdat u de browser vernieuwde.

Voor meer informatie, zie [ goedkeurend het werk ](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [ het goedkeuren van het werk ](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Proefdrukken voor rijke media weergeven in Vooraf ingestelde resoluties (proefdrukken van hoofdletters en kleine letters, Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

In een vroegere versie aan het milieu van de Voorproef, introduceerden wij de capaciteit om de resolutie van de proeven van rijke Media aan te passen hetzij door een douaneresolutie te specificeren, of door het beeld aan de gewenste resolutie te slepen.

U kunt nu opties voor vooraf ingestelde resolutie selecteren voor verschillende telefoons, tablets, laptops en desktops.

Voor meer informatie, zie &quot;het Bekijken van een Vooraf ingestelde Resolutie&quot;in [ de interactieve proefdrukresolutie van de Verandering in de het proef kijker ](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## URL naar subpagina&#39;s weergeven in opmerkingen op proefdrukken voor rijke media (proefdrukken van hoofdletters en kleine letters en Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Deze functie is momenteel beschikbaar in de productieomgeving.

Wanneer u nu een opmerking maakt op een subpagina in een proefdruk van rijke media, wordt de URL naar de subpagina weergegeven op de opmerking.

Vóór deze wijziging was niet duidelijk naar welke subpagina de opmerking verwees.

Zie voor meer informatie

## Bepaal de Beschikbaarheid van de HTML5 Video Proofing Viewer (ProefHQ en Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Als beheerder van Workfront in ProofHQ, kunt u bepalen of de gebruikers in uw organisatie toegang tot de nieuwe HTML5 het proefdrukken kijker voor videoproeven hebben.

Zie voor meer informatie over het configureren van deze optie in Workfront.

## Aangepaste weergaven maken op basis van bestaande standaardweergaven (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Nu kunt u een aangepaste weergave maken op basis van een standaardweergave. De opties Kolommen, Sorteren en Filters uit de standaardweergave worden standaard in de nieuwe weergave opgenomen.

Voordat u deze wijziging aanbracht, moest u de weergave helemaal opnieuw maken om een aangepaste weergave te maken. 

Voor meer informatie, zie [ Creërend een Mening van de Douane ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) in [ creeer en beheer de Mening van de Douane in het Bewijs van Workfront Proof ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Het rapportgebied filteren (ProefHQ) {#filter-the-reporting-area-proofhq}

Standaard bevatten de gegevens die op het tabblad Rapporten worden weergegeven, alle gegevens van uw ProofingHQ-systeem. U kunt nu filters gebruiken om alleen informatie weer te geven die relevant is voor uw behoeften. 

Voor meer informatie, zie [ Filtrerend Rapporten ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) binnen  [ de Rapporten van de Looppas in Workfront Proof ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Minimum- en maximumwaarden weergeven in rapporten (proefdrukken van hoofdletters en kleine letters) {#display-minimum-and-maximum-values-in-reports-proofhq}

U kunt nu configureren of minimum- en maximumwaarden in de grafiek worden weergegeven wanneer u rapporten weergeeft.

Voor meer informatie, zie [ Bekijkend Rapporten ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) in  [ de Rapporten van de Looppas in Workfront Proof ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Ondersteuning voor SHA-256-certificaten voor SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

We ondersteunen nu Secure Hash Algorithm 256 (SHA-256) bij het configureren van Workfront voor SSO met SAML 2.0. Voorafgaand aan deze versie, steunden wij slechts Veilig Algorithm 1 van de Hash (SHA-1).

Voor meer informatie over het vormen van Workfront met SAML 2.0, zie [ Adobe Workfront met SAML 2.0 vormen ](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Type vooruit voor toewijzingskenmerken {#type-ahead-for-mapping-attributes}

Het veldtype Standaardwaarde in het dialoogvenster Kenmerktoewijzing is bijgewerkt naar een typeveld. Vóór deze wijziging was het type van het veld Standaardwaarde een vervolgkeuzelijst.

Deze wijziging geldt voor de volgende SSO-protocollen:

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 ondersteunt geen kenmerktoewijzing.

## Mobiele verbeteringen {#mobile-improvements}

>[!NOTE]
>
> De mobiele toepassing wordt onafhankelijk van de Workfront-hoofdtoepassing uitgebracht. De functionaliteit die in deze sectie wordt beschreven, wordt begin augustus uitgebracht.

De volgende toegevoegde functionaliteit wordt weergegeven op de mobiele apps, voor zowel de Android- als de iOS-platforms:

* Verzoeken verzenden vanuit de mobiele app
* Timesheet New Entry op de mobiele app
* Aangepaste formulierbewerking vanuit de mobiele app
* Goedkeuringsaanvragen proefdrukken voor de mobiele app

Voor sommige van deze functies wordt een openbaar bètaprogramma voor het Android-platform uitgevoerd.

Voor meer informatie over het aanstaande bètaprogramma voor mobiele apparaten raadpleegt u de  [ &quot;Bèta&quot;](https://support.workfront.com/hc/en-us/sections/115000743248) pagina.

Zie voor meer informatie over het gebruik van de mobiele Workfront-app.  

## Snede die aan de Verklaringen van de Filter voor Gebiedswaarden wordt toegevoegd die komma&#39;s bevatten {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Wanneer u een filter maakt in de tekstmodus en filtert voor veldwaarden die komma&#39;s bevatten, moet u een schuine streep (&quot;/&quot;) toevoegen vóór de komma&#39;s die de waarden scheiden, om ervoor te zorgen dat de waarde als één filteroptie wordt gelezen. Dit geldt alleen voor de volgende veldtypen:

* Vervolgkeuzelijsten
* Keuzerondjes
* Selectievakjes

Voorafgaand aan deze wijziging kon u niet filteren op velden met opties met komma&#39;s.

Voor meer informatie over deze verandering, zie [ Overzicht van Filters ](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Meerdere factureringssnelheden {#multiple-billing-rates}

U kunt nu meerdere overschrijvingen van factureringssnelheden toevoegen voor dezelfde taakrol op projectniveau. Met deze nieuwe functionaliteit kunt u datumbereiken definiëren voor elke overschrijving. Tijdens de gespecificeerde datumwaaier, wordt een verschillend factureringspercentage toegepast op de baanrol die aan taken op een project wordt toegewezen. De factureringstarieven worden vermenigvuldigd met uren op het project om opbrengst te berekenen. Opbrengsten die zijn berekend binnen het datumbereik van een factureringssnelheid, blijven vergrendeld bij dat tarief en worden niet bijgewerkt als de percentages van de taakrollen in de projectupdate. In het geval van werkelijke inkomsten worden geen uren die zijn geregistreerd voordat de factureringssnelheid wordt overschreden, opnieuw berekend op basis van de huidige factureringsgraad. De uren die vóór de het facturerings tariefopheffing werden geregistreerd werden toegevoegd aan het project zullen met het facturerings tarief van de baanrol op dat ogenblik worden geassocieerd.

Voorafgaand aan deze verandering, kon u het factureringspercentage van een baanrol slechts eenmaal met voeten treden, en de Ware Ontvangsten zouden opnieuw berekenen om het huidige factureringspercentage voor alle uren te weerspiegelen die alvorens het het factureringspercentage werd geregistreerd werd veranderd.

Voor meer informatie over de Tarieven en de Inkomsten van het Factureren, zie [ Overzicht van Facturering en Inkomsten ](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Voor meer informatie over het met voeten treden van factureringspercentages voor baanrollen op het projectniveau, zie [ Overzicht van het met voeten treden van de FactureringsRates van de Rol van de Taak en het berekenen van Inkomsten op een project ](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Resource Planner {#resource-planner}

Met deze versie, introduceren wij de eerste fase van de Planner van het Middel, die deel van het herontwerp van het nieuwe lusje van de Planning in het gebied van Mensen uitmaakt. Door de Planner van het Middel te gebruiken, kunt u de hoeveelheid uren begroten de gebruikers in uw Pools van het Middel in alle huidige projecten worden toegewezen waarvoor u de Manager van het Middel bent. U kunt de volgende toewijzingsaantallen door project, baanrol, en door gebruiker zien, in de Planner van het Middel:

* Beschikbare uren
* Geplande uren
* Geforceerde uren
* Uur-variantie (tussen de begrote en de geplande uren)
* Nettouurverschil (tussen de beschikbare en de begrote uren uren)

Voor meer informatie over het gebruiken van de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nieuw veld voor rondgerichte uren van bronnen {#new-resource-budgeted-hour-field}

Om de nieuwe functionaliteit van de Planning en de Planner van het Middel te steunen, is een nieuw gebied toegevoegd aan de Bouwer van het Rapport, die u toestaat om over het Middel te rapporteren Gefedgeted Uren. In dit veld wordt het aantal uren vastgelegd waarvoor een bron in een project wordt opgenomen. Dit veld is niet beschikbaar wanneer bronnen worden gebudgetteerd met behulp van de functie Oude bronnenplanning.

Voor meer informatie over het gebruiken van Begroeide Uren in de Planner van het Middel, zie [ overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Melding in de app voor goedkeuring proef {#in-app-notification-for-proof-approval}

Wanneer u als fiatteur voor een bewijs wordt aangewezen, ontvangt u een bericht in de app over de proefdrukgoedkeuring die op uw besluit wacht. In het bericht wordt de volgende tekst weergegeven: `<User name>` wil dat u deze proefdruk goedkeurt.&quot; Als de gebruikersinformatie niet beschikbaar is, verandert het bericht in &quot;Dit bewijs vereist uw goedkeuring.&quot;

Voorafgaand aan deze verbetering, was de enige visuele aanwijzing dat u als fiatteur op een bewijs werd aangewezen een nieuw proefdrukverzoek in uw Mijn Gebied van het Werk.

Voor meer informatie over in-app berichten, zie [ Mening en beheer in-app berichten ](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Functie gebruikerstaak weergeven in gebied &#39;Toegewezen aan&#39; op de detailpagina voor taken en problemen {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Wanneer u nu de detailpagina van een taak of uitgave weergeeft, wordt een taakrol weergegeven onder de naam van de toegewezen persoon in het gebied Toegewezen aan. Deze taakrol vertegenwoordigt de taakrol van de gebruiker die de taakroltoewijzing van de taak of kwestie aanpast. Als de taak of kwestie niet aan een baanrol wordt toegewezen, wordt de primaire baanrol van de toegewezen gebruiker getoond.

Vóór deze wijziging werd alleen de titel van de gebruiker weergegeven onder de naam van de gebruiker in het gebied Toegewezen aan. 
