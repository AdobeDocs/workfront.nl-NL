---
product-area: documents
navigation-topic: approvals
title: Een revisie- en goedkeuringsdashboard maken
description: U kunt goedkeuringsmetriek in de dashboards van het Canvas herzien.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 0b4884d6c9a88c096b15af65a2aff0a54ca66811
workflow-type: tm+mt
source-wordcount: '2520'
ht-degree: 0%

---

# Een rapportdashboard maken voor revisie en goedkeuring

U kunt een rapportdashboard in het gebied van de Dashboards van het Canvas tot stand brengen om zowel hoog als gedetailleerde informatie over overzichten en goedkeuringen met Verenigde functionaliteit van Goedkeuringen te tonen.

>[!IMPORTANT]
>
>Deze functionaliteit is beschikbaar slechts voor klanten die de Verenigde dienst van Goedkeuringen gebruiken en in de bèta van de Dashboards van het Canvas ingeschreven. Voor meer informatie, zie {de bètainformatie van de Dashboards van het 0} Canvas [.](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)


![ voorbeelddashboard ](assets/whole-dashboard.png)

## Een dashboard maken

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.
1. Klik **Nieuw Dashboard**.
1. Geef het dashboard een naam.
1. (Optioneel) Voeg een beschrijving toe.
1. Klik **creëren**.
   ![ voeg dashboardnaam en beschrijving ](assets/create-a-dashboard.png) toe

Nadat u een dashboard hebt gemaakt, kunt u beginnen met het toevoegen van KPI&#39;s, grafieken en tabellen. Zie de volgende secties voor meer informatie:

* [Voeg overzichts- en goedkeuringsinformatie op hoog niveau toe met KPI&#39;s en grafieken](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Gedetailleerde revisie- en goedkeuringsinformatie toevoegen met tabellen](#add-detailed-review-and-approval-information-with-tables)

## Voeg overzichts- en goedkeuringsinformatie op hoog niveau toe met KPI&#39;s en grafieken

U kunt informatie op hoog niveau over documentgoedkeuringen met KPIs en grafieken bekijken.

Voor meer informatie, zie [ een KPI- rapport ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md) bouwen en [ bouwen een grafiekrapport ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

### KPI&#39;s

![ KPI voorbeelden ](assets/kpi-dashboard.png)

#### Goedkeuringen in behandeling

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **KPI**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type *in afwachting van* op het **3} gebied van de Naam {.**
   1. Het type *wacht goedkeuringen* op het **gebied van de Beschrijving** in behandeling. Dit wordt weergegeven als een bijschrift onder de KPI-waarde.

1. Volg hieronder de stappen om de **Bouw KPI** sectie te vormen:

   1. In het linkerpaneel, klik **Bouw KPI** ![ bouwt KPI pictogram ](assets/build-kpi-icon.png).

   1. Klik **Uitgezochte gebied**.

   1. Bepaal en selecteer de **omslag van de Goedkeuring van het Document**.

   1. Selecteer **Status**.

   1. In het **type van Samenvoeging** drop-down, uitgezochte **Telling**.

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter** ![ van de Filter ](assets/filter-icon.png).

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde**.

   1. Klik in de lege voorwaardenfilter, klik **Kiep een Gebied**, dan kies **Status**.
   1. Verlaat de exploitant als **Gelijk**, dan type _in afwachting van overzicht_ in textbox.
      ![ hangend kpi filtervoorbeeld ](assets/pending-kpi-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.


#### Achterstallige betalingen

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **KPI**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _achterstallig_ op het **gebied van de Naam**.
   1. De Deadline van het Stadium van de Goedkeuring van het type _in het verleden_ op het **3} gebied van de Beschrijving {.** Deze beschrijving wordt weergegeven als een bijschrift onder de KPI-waarde.

1. Volg hieronder de stappen om de **Bouw KPI** sectie te vormen:

   1. In het linkerpaneel, klik **Bouw KPI** ![ bouwt KPI pictogram ](assets/build-kpi-icon.png).

   1. Klik **Uitgezochte gebied**.

   1. Bepaal en selecteer de **omslag van de Goedkeuring van het Document**.

   1. Selecteer **Status**.

   1. In het **type van Samenvoeging** drop-down, uitgezochte **Telling**.

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter** ![ van de Filter ](assets/filter-icon.png).

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde**.

   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.

   1. Selecteer **Stadium van de Goedkeuring** > **Deadline**.
   1. Verander de exploitant in **minder dan**.
   1. Knevel **Vastgestelde relatieve datum** aan ****, toen type _$$TODAY_ in textbox.
      ![ achterstallig kpi filtervoorbeeld ](assets/overdue-kpi-filter.png)
   1. Klik **toevoegen voorwaarde**.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **Status**.
   1. Verander de exploitant in **niet bevat**, dan type _goedgekeurd_ in textbox.
      ![ achterstallig kpi filtervoorbeeld 2 ](assets/overdue-kpi-filter-2.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.


#### Voltooide goedkeuringen


1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **KPI**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _voltooide_ op het **gebied van de Naam**.
   1. De Telling van de Status van de Goedkeuring van het type __ op het **3} gebied van de Beschrijving.** Deze beschrijving wordt weergegeven als een bijschrift onder de KPI-waarde.

1. Volg hieronder de stappen om de **Bouw KPI** sectie te vormen:

   1. In het linkerpaneel, klik **Bouw KPI** ![ bouwt KPI pictogram ](assets/build-kpi-icon.png).

   1. Klik **Uitgezochte gebied**.

   1. Bepaal en selecteer de **omslag van de Goedkeuring van het Document**.

   1. Selecteer **Status**.

   1. In het **type van Samenvoeging** drop-down, uitgezochte **Telling**.

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter** ![ van de Filter ](assets/filter-icon.png).

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde**.

   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.

   1. Selecteer **Status**.

   1. Verander de exploitant in **bevat**, en type _goedgekeurd_ in textbox.
      ![ voltooid kpi filtervoorbeeld ](assets/completed-kpi-filter.png)
   1. Klik **toevoegen voorwaarde**.
   1. Klik **en** om het in **of** te veranderen.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **Status**.
   1. Verander de exploitant in **Gelijk**, toen type _herzien_ in textbox.
      ![ voltooid kpi filtervoorbeeld ](assets/completed-kpi-filter-2.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

#### Verlaten goedkeuringen

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **KPI**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _verliet_ op het **3} gebied van de Naam {.**
   1. De deadline van de Goedkeuring van het type _over 2 weken voorbij_ op het **3} gebied van de Beschrijving {.** Deze beschrijving wordt weergegeven als een bijschrift onder de KPI-waarde.

1. Volg hieronder de stappen om de **Bouw KPI** sectie te vormen:

   1. In het linkerpaneel, klik **Bouw KPI** ![ bouwt KPI pictogram ](assets/build-kpi-icon.png).

   1. Klik **Uitgezochte gebied**.

   1. Zoek en selecteer de **omslag van het de goedkeuringsstadium van 0} Document.**

   1. Selecteer **Deadline**.

   1. In het **type van Samenvoeging** drop-down, uitgezochte **Telling**.

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter** ![ van de Filter ](assets/filter-icon.png).

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde**.

   1. Klik in de lege voorwaardenfilter, klik **kiezen een Gebied**.

   1. Selecteer **Status**.

   1. Verander de exploitant in **niet bevat**, en type _goedgekeurd_ in textbox.
      ![ verlaten kpi filtervoorbeeld ](assets/abandoned-kpi-filter.png)
   1. Klik **toevoegen voorwaarde**.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **Deadline**.
   1. Verander de exploitant in **minder dan**, dan knevel **plaats relatieve datum** aan ****.
   1. Typ _$$TODAY-2w_ in het tekstvak.
      ![ verlaten kpi filtervoorbeeld ](assets/abandoned-kpi-filter-2.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

### Grafieken

![ de voorbeelden van de Grafiek ](assets/chart-dashboard.png)

#### Goedkeuringen op basis van het diagram van de beslissingsbalk

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Grafiek**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _keurt door besluit_ op het **gebied van de Naam** goed.
   1. (Facultatief) Type een beschrijving op het **gebied van de Beschrijving**. Deze tekst wordt als knopinfo naast de naam van het diagram weergegeven.
1. Volg hieronder de stappen om **bouwt grafiek** sectie te vormen:

   1. In het linkerpaneel, klik het **bouwt grafiek** ![ het pictogram van de Grafiek ](assets/build-chart-icon.png) bouwen.

   1. In het **type van Grafiek** drop-down menu, verlaten **Geselecteerde Bar**.
   1. In het **type van Bar** drop-down menu, verlaat **Eenvoudig** geselecteerd.
   1. Klik **gebied van de Update** voor de **Onderste (X) as**, dan de uitgezochte **Goedkeuring van het Document** > **Status**.
   1. Plaats het **type van Samenvoeging** aan **Telling**.
   1. Klik **gebied van de Update** voor de **Linkeras (Y)**, dan selecteren **Status**.
1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:
   1. In het linkerpaneel, klik het **** pictogram van het filterlusje van de Filter ![ pictogram.](assets/filter-tab.png)
   1. Klik **uitgeven Filter**, dan **voeg voorwaarde** toe.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **Versie van het Document** > **Versie**.
   1. Verander de exploitant in **is niet Null**.
      ![ filtervoorbeeld ](assets/approvals-by-decision-chart-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.


#### Revisitiebalkdiagram

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Grafiek**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _Herzieningen_ op het **gebied van de Naam**.
   1. Type _Aantal revisies voor documenten met onvolledige besluiten die vóór het eind van deze maand_ op het **3} gebied van de Beschrijving {worden gepland.** Deze tekst wordt als knopinfo naast de naam van het diagram weergegeven.

1. Volg hieronder de stappen om **bouwt grafiek** sectie te vormen:

   1. In het linkerpaneel, klik het **bouwt grafiek** ![ het pictogram van de Grafiek ](assets/build-chart-icon.png) bouwen.

   1. In het **type van Grafiek** drop-down menu, verlaten **Geselecteerde Bar**.
   1. In het **type van Bar** drop-down menu, verlaat **Eenvoudig** geselecteerd.
   1. Klik **gebied van de Update** voor de **Onderste (X) as**, dan de uitgezochte **Goedkeuring van het Document** > **Versie van het Document** > **Versie**.
   1. Plaats het **type van Samenvoeging** aan **Telling**.
   1. Klik {het gebied van de Update 1} voor de **Linker (Y) as**, dan selecteren de uitgezochte **Goedkeuring van het Document** > **Versie van het Document** > **Document** > **Naam**.****

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:
   1. In het linkerpaneel, klik het **** pictogram van het filterlusje van de Filter ![ pictogram.](assets/filter-tab.png)
   1. Klik **uitgeven Filter**, dan **voeg voorwaarde** toe.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.

   1. Selecteer **het stadium van de Goedkeuring** > **deelnemers van het stadium van de Goedkeuring** > **Datum van het Besluit**.

   1. Verander de exploitant in **is Null**.
      ![ het filtervoorbeeld van het revisiesdiagram ](assets/revision-chart-filter.png)
   1. Klik **toevoegen voorwaarde**.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **het stadium van de Goedkeuring** > **Deadline**.
   1. Verander de exploitant in **minder dan of Gelijk**, dan knevel **plaats relatieve datum** aan ****.
   1. Typ _$$TODAYem_ in het tekstvak.
      ![ het filtervoorbeeld van het grafiekfilter van Herzieningen ](assets/revision-chart-filter-2.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

## Gedetailleerde revisie- en goedkeuringsinformatie toevoegen met tabellen

Voor meer informatie bij de bouw van een lijstrapport, zie [ een lijstrapport ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md) bouwen.

![ lijstvoorbeeld ](assets/table-dashboard.png)

### Goedkeuringslijst in behandeling

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.
1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Lijst**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _wacht goedkeuringen_ op het **gebied van de Naam** in behandeling.
   1. Typ een beschrijving op het **gebied van de Beschrijving**. Deze tekst wordt als knopinfo naast de naam van het diagram weergegeven.

1. Volg hieronder de stappen om de **bouwt lijst** sectie te vormen:

   1. In het linkerpaneel, klik het **kolommen van de Lijst** ![ pictogram van de kolommen van de Lijst ](assets/drilldown-column.png).
   1. Klik **toevoegen kolom**.
   1. De rol neer en selecteert **Goedkeuringen van het Document** > **Status**.
   1. Voeg de volgende kolommen toe:

   <table>
    <tr>
    <td><strong>Projectnaam</strong></td>
    <td>Documentversie &gt; Document &gt; Project &gt; Naam</td>
    </tr>
    <tr>
    <td><strong>Documentnaam</strong></td>
    <td>De Versie van het document &gt; Document &gt; type <em> Naam </em> in het onderzoeksvakje.</td>
    </tr>
    <tr>
    <td><strong>Documentversie</strong></td>
    <td>Documentversie &gt; Document &gt; Versie</td>
    </tr>
    <tr>
    <td><strong>Deadline</strong></td>
    <td>Documentgoedkeuring &gt; Goedkeuringswerkgebied &gt; Deadline</td>
    </tr>
    <tr>
    <td><strong>Gevraagd door</strong></td>
    <td>De Goedkeuring van het document &gt; het Stadium van de Goedkeuring &gt; de Deelnemers van het Stadium van de Goedkeuring * &gt; Vraag &gt; type <em> Naam </em> in het onderzoeksvakje.</td>
    </tr>
    <tr>
    <td><strong>Aangevraagde datum</strong></td>
    <td>Document Approval &gt; Approval Stage &gt; Approval Stage Participants* &gt; Created at</td>
    </tr>
    <tr>
    <td><strong>Fiatteur</strong></td>
    <td>De Goedkeuring van het document &gt; het Stadium van de Goedkeuring &gt; de Deelnemers* &gt; de Gebruiker van de Deelnemer &gt; type <em> Naam </em> in het onderzoeksvakje.</td>
    </tr>
    </table>


   *De Deelnemers van het Stadium van de goedkeuring worden beknot aan _Pa van het Stadium van de Goedkeuring._


1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:
   1. In het linkerpaneel, klik het **** pictogram van het filterlusje van de Filter ![ pictogram.](assets/filter-tab.png)
   1. Klik **uitgeven Filter**, dan **voeg voorwaarde** toe.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **Status**.
   1. Verander de exploitant in **Gelijk**, dan type _in afwachting van goedkeuring_ in textbox.
      ![ hangende het filtervoorbeeld van de goedkeuringstabel ](assets/pending-approval-table-filter.png)
   1. (Facultatief) voeg extra filters toe zoals die in de **Facultatieve hieronder sectie van filters** worden beschreven.
1. Klik **sparen** in de hoger-juiste hoek van het scherm.


**Facultatieve filters**

Als u meer specifieke informatie wilt weergeven, afhankelijk van het gebruik, kunt u extra filtervoorwaarden toevoegen. U kunt de tabel opnieuw maken en nieuwe filtervoorwaarden per gebruik toevoegen.

+++ Uitbreiden om extra filteropties weer te geven

**Mijn Projecten**

1. Klik **uitgeven Filter** > **toevoegt voorwaarde**:
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **versie van het Document** > **Document** > **Project** > **Eigenaar** > type _Naam_ in het onderzoeksvakje.
   1. Verander de exploitant in **Gelijk**, dan kies **me (Logged in gebruiker)** aan vertoningsprojecten in Workfront waar u als projecteigenaar wordt gemerkt.
      ![ hangende het filtervoorbeeld van de goedkeuringstabel ](assets/pending-approvals-my-project-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

**Goedkeuringen ik heb voorgelegd**

1. Klik **uitgeven Filter** > **toevoegt voorwaarde**:
   1. Klik in de lege voorwaardenfilter, klik **kiezen een Gebied**.
   1. Selecteer **>** de Deelnemers van het Stadium van de Goedkeuring **>** Vraag **> type** Naam _in het onderzoeksvakje._
   1. Verander de exploitant in **Gelijk**, dan kies **me (Logged in gebruiker)** aan vertoningsprojecten in Workfront waar u als projecteigenaar wordt gemerkt.
      ![ hangende het filtervoorbeeld van de goedkeuringstabel ](assets/pending-approvals-my-project-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

+++

### Achterstallige goedkeuringenlijst

1. [ creeer een dashboard ](#create-a-dashboard) zoals die in de sectie hierboven wordt beschreven.

1. In de hoger-juiste hoek van de pagina van de dashboarddetails, klik **voeg rapport** toe.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Lijst**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Het type _achterstallige goedkeuringen_ op het **gebied van de Naam**.
   1. (Facultatief) Type een beschrijving op het **gebied van de Beschrijving**. Deze tekst wordt als knopinfo naast de naam van het diagram weergegeven.

1. Volg hieronder de stappen om de **bouwt lijst** sectie te vormen:

   1. In het linkerpaneel, klik het **kolommen van de Lijst** ![ pictogram van de kolommen van de Lijst ](assets/drilldown-column.png).
   1. Klik **toevoegen kolom**.
   1. De rol neer en selecteert **Goedkeuringen van het Document** > **Status**.
   1. Voeg de volgende kolommen toe:

      <table>
        <tr>
        <td><strong>Projectnaam</strong></td>
        <td>Documentversie &gt; Document &gt; Project &gt; Naam</td>
        </tr>
        <tr>
        <td><strong>Documentnaam</strong></td>
        <td>De Versie van het document &gt; Document &gt; type <em> Naam </em> in het onderzoeksvakje.</td>
        </tr>
        <tr>
        <td><strong>Documentversie</strong></td>
        <td>Documentversie &gt; Document &gt; Versie</td>
        </tr>
        <tr>
        <td><strong>Deadline</strong></td>
        <td>Document &gt; Approval Stage &gt; Deadline</td>
        </tr>
        <tr>
        <td><strong>Gevraagd door</strong></td>
        <td>Document &gt; het Stadium van de Goedkeuring &gt; de Deelnemers van het Stadium van de Goedkeuring * &gt; Vraag &gt; type <em> Naam </em> in het onderzoeksvakje.</td>
        </tr>
        <tr>
        <td><strong>Aangevraagde datum</strong></td>
        <td>Document &gt; Approval Stage &gt; Approval Stage Participants* &gt; Created at</td>
        </tr>
        <tr>
        <td><strong>Fiatteur</strong></td>
        <td>Document &gt; het Stadium van de Goedkeuring &gt; de Deelnemers van het Stadium van de Goedkeuring * &gt; de Gebruiker van de Deelnemer &gt; type <em> Naam </em> in het onderzoeksvakje.</td>
        </tr>
        </table>

      *De Deelnemers van het Stadium van de goedkeuring worden beknot aan _Pa van het Stadium van de Goedkeuring._

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:
   1. In het linkerpaneel, klik het **** pictogram van het filterlusje van de Filter ![ pictogram.](assets/filter-tab.png)
   1. Klik **uitgeven Filter**, dan **voeg voorwaarde** toe.
   1. Klik in de lege voorwaardenfilter, dan klik **kiezen een Gebied**.
   1. Selecteer **Stadium van de Goedkeuring** > **Deadline**.
   1. Verander de exploitant in **minder dan**, dan knevel **plaats relatieve datum** aan ****.
   1. Typ _$$TODAY_ in het tekstveld.
      ![ achterstallig het filtervoorbeeld van de goedkeuringstabel ](assets/overdue-approval.png)
   1. (Facultatief) voeg extra filters toe zoals die in de **Facultatieve hieronder sectie van filters** worden beschreven.
1. Klik **sparen** in de hoger-juiste hoek van het scherm.



**Facultatieve filters**

Als u meer specifieke informatie wilt weergeven, afhankelijk van het gebruik, kunt u extra filtervoorwaarden toevoegen. U kunt de tabel opnieuw maken en nieuwe, optionele filtervoorwaarden per geval toevoegen.

+++ Uitbreiden om extra filteropties weer te geven

**Mijn Projecten**

1. Klik **uitgeven Filter** > **toevoegt voorwaarde**:
   1. Klik in de lege voorwaardenfilter, klik **kiezen een Gebied**.
   1. Selecteer **versie van het Document** > **Document** > **Project** > **Eigenaar** > type _Naam_ in het onderzoeksvakje.
   1. Verander de exploitant in **Gelijk**, dan kies **me (die in Gebruiker wordt geregistreerd)** aan vertoningsprojecten in Workfront waarin u als projecteigenaar duidelijk bent.
      ![ hangende het filtervoorbeeld van de goedkeuringstabel ](assets/pending-approvals-my-project-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

**Goedkeuringen ik heb voorgelegd**

1. Klik **uitgeven Filter** > **toevoegt voorwaarde**:
   1. Klik in de lege voorwaardenfilter, klik **kiezen een Gebied**.
   1. Selecteer **>** de Deelnemers van het Stadium van de Goedkeuring **>** Vraag **> type** Naam _in het onderzoeksvakje._
   1. Verander de exploitant in **Gelijk**, dan kies **me (die in Gebruiker wordt geregistreerd)** aan vertoningsprojecten in Workfront waarin u als projecteigenaar duidelijk bent.
      ![ hangende het filtervoorbeeld van de goedkeuringstabel ](assets/pending-approvals-my-project-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

**Mijn team**

1. Klik **uitgeven Filter** > **toevoegt voorwaarde**:
   1. Klik in de lege voorwaardenfilter, klik **kiezen een Gebied**.
   1. Selecteer **>** de Deelnemers van het Stadium van de Goedkeuring van het Stadium van de Goedkeuring **>** Team van de Deelnemer **> type** Naam _in het onderzoeksvakje._
   1. Verander de exploitant aan **Gelijk**, dan kies **Mijn standaardteams (die in Gebruiker)** of **Mijn andere teams (die in Gebruiker) worden geregistreerd** aan vertoningsprojecten die aan of uw standaardteam of andere teams worden toegewezen u bent.
      ![ hangende het filtervoorbeeld van de goedkeuringstabel ](assets/approvals-ive-submitted-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.
+++
