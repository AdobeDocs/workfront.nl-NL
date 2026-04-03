---
title: Tweede kwartaal 2026 Rapportverbeteringen
description: Tweede kwartaal 2026 Rapportverbeteringen
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 1ef6ead705231a41cbf62b8a8b35f480da004970
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Tweede kwartaal 2026 Rapportverbeteringen

Op deze pagina worden de verbeteringen beschreven die zijn aangebracht in de release Tweede kwartaal 2026 voor Voorvertoning. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving, zoals vermeld.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Tweede Kwartaal 2026 versiecyclus, zie [ Tweede Kwartaal 2026 releaseoverzicht ](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Huidig versieveld voor documentversies

>[!NOTE]
>
>Voorbeeld: 2 april 2026
>Snelle productie: 15 april 2026
>Productie voor iedereen: 16 april 2026

We hebben een Booleaans veld `currentVersion` toegevoegd aan het object Document Version om het gemakkelijker te maken om de laatste versie van een document te identificeren en hierover te rapporteren.
Met deze update:

* U kunt `currentVersion` gebruiken in filters, weergaven, groepen en grafieken.
* Het veld is beschikbaar in de keuzelijst Canvas-veld voor rapporten documentversie.

* Wanneer een nieuwe versie wordt geüpload:

   * De nieuwe versie is gemarkeerd als `TRUE`
   * Eerdere versies worden gemarkeerd als `FALSE`

* Rapporten kunnen de huidige versies op de dashboards van Canvas en erfenisrapportering consistent identificeren

Bestaande filters voor klassieke rapporten met `isCurrentVersion` of `isDocumentCurrentVersion` werken nog steeds zoals beschreven.

## De geplande Levering van het Rapport steunt nu verbinding-Gebaseerde E-mail

>[!NOTE]
>
>Voorbeeld: 3 april 2026
>Snelle productie: 15 april 2026
>Productie voor iedereen: 16 april 2026

Workfront omvat nu een nieuw leveringstype van de Verbinding voor geplande rapporten. In plaats van het produceren van en het vastmaken van een dossier, verzendt deze optie een e-mail die een directe verbinding aan het rapport in Workfront bevat, toestaand ontvangers om {{$include }} de huidigste gegevens in de toepassing te bekijken.

De optie van de Verbinding is nu het standaardleveringstype voor nieuw gecreeerd gepland rapport leveringsregels, terwijl de bestaande op dossier-gebaseerde formaten (HTML, PDF, Excel, en TSV) beschikbaar blijven.

Met deze verandering, hebben wij ook de blik-en-mening van de e-mail van de rapportlevering bijgewerkt.

Voor meer informatie, zie [ Plan een automatische rapportlevering ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Rapporten uitvoeren als een specifieke gebruiker in Canvasdashboards

>[!NOTE]
>
>Voorbeeld: 2 april 2026
>Snelle productie: 15 april 2026
>Productie voor iedereen: 16 april 2026
>
>Canvasdashboards worden momenteel in bèta weergegeven.

U kunt rapporten op de dashboards van het Canvas nu vormen om als specifieke gebruiker in werking te stellen. Wanneer toegelaten, toont het rapport gegevens die op de geselecteerde gebruiker toegang in plaats van de toestemmingen van de kijker worden gebaseerd.

Dit verzekert consistentere en betrouwbaardere gegevens over dashboardkijkers, zelfs wanneer de toegang tot de werkruimten van de Planning, verslagtypes, of vergunningsmontages verschilt.

Voor meer informatie, zie [ een KPI- rapport in een Dashboard van het Canvas ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md) bouwen, [ een grafiekrapport in een Dashboard van het Canvas ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md), of [ bouwt een lijstrapport in een Dashboard van het Canvas ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

## Nieuwe verificatieopties voor gegevensverbinding

>[!NOTE]
>
>Voorbeeld: 12 maart 2026
>Snelle productie: 12 maart 2026
>Productie voor iedereen: 16 april 2026

U kunt nu verifiëren aan Gegevens verbinden gebruikend sleutels RSA of de verbindingen van de Tokens van de Toegang van de Programmatische (KLOPJE), toevoegend veiligere en flexibele alternatieven aan traditionele gebruikersbenaming/wachtwoordgeloofsbrieven.

Met deze nieuwe opties kunnen organisaties stabiele verbindingen onderhouden vanuit Power BI, Tableau en andere BI-tools van derden zonder te vertrouwen op gebruikersgebaseerde aanmeldingsmethoden.

>[!IMPORTANT]
>
>In juni 2026 zijn gebruikersgegevens/wachtwoordgegevens vereist voor het gebruik van meervoudige verificatie (MFA). Wij adviseren overschakeling aan of RSA of op PAT-Gebaseerde authentificatie voor de rekeningen van de de dienstgebruiker die worden gebruikt om gegevens van Gegevens te laden verbindt in derdevisualiseringshulpmiddelen, gegevensverwerkers, en manuscripten die niet met MFA in het authentificatieproces zullen werken.

## Aangepaste veldlabels die worden weergegeven bij het samenstellen van rapporten

>[!NOTE]
>
>Voorbeeld: 26 februari 2026
>Snelle productie: 12 maart 2026
>Productie voor iedereen: 16 april 2026

Het label van het aangepaste veld wordt nu vóór de veldnaam en het object weergegeven in de gereedschappen voor het samenstellen van rapporten, zodat u gemakkelijker velden kunt vinden. Veldlabels worden ook weergegeven wanneer u filters, weergaven en groepen in lijsten definieert.

Het label van het aangepaste veld is bedoeld voor de systeeminterface, terwijl de veldnaam vaak wordt gebruikt voor de API- en back-endopslagdoeleinden en wellicht niet zo nuttig is bij het zoeken naar een veld.

Voor meer informatie, zie [ een douanerapport ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Aandeelbare rapportmappen

>[!NOTE]
>
>Voorbeeld: 26 februari 2026
>Snelle productie: 12 maart 2026
>Productie voor iedereen: 16 april 2026

U kunt rapporten nu organiseren en delen met behulp van deelbare rapportmappen. Deze nieuwe eigenschap helpt teams die grote volumes van rapporten beheren scalable en verenigbare toegangsbeheer handhaven:

* **creeer georganiseerde omslagstructuren**: De beheerders van het systeem kunnen top-level omslagen tot stand brengen, en de gebruikers met beheerde toegang kunnen subfolders tot 4 niveaus diep tot stand brengen.
* **korrelige toestemmingscontroles**: De omslagen van het aandeel met twee toestemmingsniveaus:
   * Weergeven: gebruikers kunnen rapporten openen en mappen delen
   * Beheer: gebruikers kunnen mapgegevens bewerken, items toevoegen/verwijderen en automatisch beheertoegang tot alle rapporten in de map ontvangen
* **Geërfte toestemmingen**: De toestemmingen trapsgewijs van ouderomslagen aan alle subfolders en rapporten binnen de omslagboom
* **Verbeterde lijstervaring**: Wanneer u sharable omslagen toelaat, zult u toegang tot de verbeterde lijstervaring hebben. Voor meer informatie, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Voor meer informatie, zie [ Gebruik shareable rapportomslagen ](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Verbeterde datumlabels voor grafiekgroepen in canvasdashboards

>[!NOTE]
>
>Voorbeeld: 26 februari 2026
>Snelle productie: 12 maart 2026
>Productie voor iedereen: 16 april 2026

>[!NOTE]
>
>Canvasdashboards worden momenteel in bèta weergegeven.

Grafieken die gegevens op datum groeperen tonen nu duidelijkere, beter leesbare datumetiketten. Met deze update worden datumlabels dynamisch aangepast op basis van de geselecteerde groep per optie, zoals dag, week, maand of jaar, zodat grafieken in één oogopslag beter leesbaar en interpreteerbaar zijn:

<table> <tbody> <tr> <td>Dag</td> <td>Geeft de volledige datum weer. Voorbeeld: 12-3-2026</td> </tr> <tr> <td>Week</td> <td>Geeft een opgemaakte begindatum van de week weer. Voorbeeld, 8 maart 2026</td> </tr> <tr> <td>Maand</td> <td>Geeft de maand en het jaar weer. Voorbeeld maart 2026</td> </tr> <tr> <td>Jaar</td> <td>Hiermee geeft u alleen het jaar weer. Voorbeeld: 2026</td> </tr> </tbody> </table>

Eerder, toonden de grafiekgroepen altijd de begindatum van de geselecteerde periode in een numeriek formaat.
