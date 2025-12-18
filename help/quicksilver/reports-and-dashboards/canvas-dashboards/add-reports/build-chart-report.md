---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Bouw een grafiekrapport in een dashboard van het Canvas
description: Een grafiekrapport dat uw gegevens visualiseert als bar, kolom, lijn, of cirkeldiagram kan aan een Dashboard van het Canvas worden toegevoegd.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: bb65fa45f6fce762920627ad0fb6fd1d832f23a3
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 0%

---

# Bouw een grafiekrapport in een dashboard van het Canvas

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Voorproef voor alle klanten.</span>

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Onderdelen van het onderdeel zijn mogelijk niet compleet of werken niet zoals bedoeld in deze fase. Gelieve te dienen om het even welke terugkoppelen betreffende uw ervaring door de instructies in [ te volgen verstrekt ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) sectie in het de bètaoverzichtsartikel van de dashboards van het Canvas.<br>
>Als u feedback hebt over een mogelijk probleem met een probleem of een technisch probleem, stuurt u een ticket naar Workfront Support. Voor meer informatie, zie [ de Steun van de Klant van het Contact ](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Deze bètaversie is niet beschikbaar op de volgende cloudproviders:
>
>* Je eigen sleutel voor Amazon Web Services
>* Azure
>* Google Cloud Platform

U kunt een grafiekrapport aan een dashboard van het Canvas bouwen en toevoegen om uw gegevens als bar, kolom, lijn, of cirkeldiagram visualiseren.

![ rapport van de Grafiek ](assets/chart-report-main.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td> 
   <td><p>Toegang tot rapporten, dashboards en kalenders bewerken</p>
  </td> 
  </tr>  
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Vereisten

U moet een dashboard tot stand brengen alvorens u een grafiekrapport kunt bouwen.

## Bouw een grafiekrapport in een dashboard van het Canvas

Er zijn vele configuratieopties beschikbaar voor het bouwen van een grafiekrapport. In deze sectie doorlopen we het algemene proces voor het maken van een sectie.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**

1. Klik **creëren**.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Grafiek**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. (Facultatief) volg de stappen hieronder om de **sectie van Details** te vormen:

   1. Ga een rapport **Naam** in.

   1. Ga een rapport **Beschrijving** in.

   1. Indien gewenst, uncheck **extra reeksen als &quot;Andere&quot;** doos tonen.

      >[!NOTE]
      >
      >Er is een maximumaantal 60 reeksen die in een grafiek kunnen worden getoond. Wanneer deze doos wordt gecontroleerd, worden om het even welke reeksen boven de grens geconsolideerd in a **Andere** groepering in de grafiek.
1. Kies welk type diagram u wilt maken:
   * [Staaf, kolom of lijndiagram](#bar-column-or-line-chart)
   * [Cirkeldiagram](#pie-chart)

### Staaf, kolom of lijndiagram

>[!NOTE]
>
>Afhankelijk van het geselecteerde veldtype kunnen er aanvullende velden zijn. De hieronder beschreven opties zijn standaard voor alle veldtypen.


1. In het linkerpaneel, klik het **bouwt grafiek** ![ het pictogram van de Grafiek ](assets/build-chart-icon.png) bouwen.

1. In het **type van Grafiek** drop-down, uitgezochte **Bar**, **Kolom**, of **Lijn**.
1. Selecteer in het tweede vervolgkeuzemenu de balk, kolom of het lijntype:
   * **Eenvoudig**
   * **Multi-series**
   * **Gestapeld**

1. In de **Onderste (X) as** sectie, selecteer het **gebied van de Update**, bepaal dan de plaats en selecteer van het gebied dat de gegevens bevat die in de grafiek zullen worden samengevat.
1. In het **type van Samenvoeging** drop-down, selecteer hoe de gegevens omhoog rollen om de grafiekoutput te veroorzaken.
1. <span class="preview"> (Optioneel) Voeg een aslabel toe aan de beschikbare ruimte. </span>
1. <span class="preview"> (Facultatieve) knevel **as van de Huid** op. </span>
1. <span class="preview"> (Facultatieve) Input a **de lijnwaarde van de Verwijzing** om een doel of een drempel op de grafiek te plaatsen.</span>
1. Kies het type van a **Lijn** van het drop-down menu.
1. Selecteer het **gebied van de Update** knoop onder de tweede sectie, bepaal de plaats en selecteer dan van het tweede gebied u in de grafiek wilt tonen.


### Cirkeldiagram

>[!NOTE]
>
>Afhankelijk van het geselecteerde veldtype kunnen er aanvullende velden zijn. De hieronder beschreven opties zijn standaard voor alle veldtypen.


1. In het linkerpaneel, klik het **bouwt grafiek** ![ het pictogram van de Grafiek ](assets/build-chart-icon.png) bouwen.

1. In het **type van Grafiek** drop-down, uitgezochte **Bar**.
1. In de **Metrische** sectie, selecteer het **gebied van de Update**, bepaal dan de plaats en selecteer van het gebied dat de gegevens bevat die in de grafiek zullen worden samengevat.
1. In het **type van Samenvoeging** drop-down, selecteer hoe de gegevens omhoog rollen om de grafiekoutput te veroorzaken.
1. In de **sectie van het Segment**, selecteer het **gebied van de Update**, bepaal dan de plaats en selecteer van het gebied dat de segmenten bevat u in het cirkeldiagram wilt tonen.
1. <span class="preview"> (Facultatief) in de **Schijf** sectie, knevel **segmentetiketten** op om segmentetiketten te tonen.</span>
1. <span class="preview"> (Facultatieve) knevel **tonen totaal** op om het totaal in het midden van de grafiek te tonen. Wanneer toegelaten, zijn er extra opties om een centrumetiket te tonen en het waardeformaat te kiezen.</span>

>[!NOTE]
>
>Samenvoegingstypen worden als volgt weergegeven:
>
>* De samenvoegingstypes van de telling: De getoonde centrumwaarde is een telling van alle segmenten van de grafiek.
>* Som-aggregatietypen: de weergegeven middenwaarde is het geaggregeerde totaal van de numerieke of valutawaarde.
>* Typen gemiddelde, maximale en minimale aggregatie: de middelste waarde geeft dienovereenkomstig het gemiddelde, de maximale of de minimale waarde weer.

1. <span class="preview"> (Facultatief) in de sectie van de Legende, knevel **legenda** tonen om de grafieklegenda te tonen.</span>

1. <span class="preview"> (Facultatief) kies a **positie van de Legenda** van het drop-down menu.</span>

## Aanvullende instellingen voor het diagramrapport configureren

### Filters

Volg hieronder de stappen om de **sectie van de Filter** te vormen:

1. In het linkerpaneel, klik het **pictogram van de Filter**![ van de Filter {](assets/filter-icon.png).
1. Selecteer **filter uitgeven**.
1. Klik **toevoegen voorwaarde** en specificeer dan het gebied u tegen en de bepaling wilt filtreren die bepaalt welk soort voorwaarde het gebied moet ontmoeten.
1. (Facultatief) klik **toevoegen filtergroep** om een andere reeks het filtreren criteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

### Instellingen voor drilldown

Volg hieronder de stappen om de **sectie van de Montages van de Kolom te vormen 0} Drilldown {:**

1. In het linkerpaneel, klik het **Drilldown pictogram van Kolommen** ![ Drilldown kolommen ](assets/drilldown-column.png). De velden in het diagram worden automatisch als kolommen weergegeven in de voorbeeldsectie aan de rechterkant.

1. (Facultatief) om het even welke bestaande kolomconfiguraties bij te werken, selecteer de kolom u in de **Huidige kolommen** sectie wilt bijwerken en dan de gewenste informatie (b.v. etiket, verbonden status, en voorwaarden) bijwerken.

1. Klik **toevoegen kolom** en selecteer dan het gebied u als kolom in de lijst wilt tonen. Herhaal dit proces voor elke kolom u wilt toevoegen.

### Instellingen van de downgroep

Volg hieronder de stappen om de **sectie van de Montages van de Groep van de Drilldown** te vormen:

1. In het linkerpaneel, klik het **pictogram van de Montages van de Groep** ![ van de Montages van de Groep ](assets/drilldown-group-icon.png).

1. Klik **toevoegen groeperend** knoop en dan het gebied selecteren u als groepering wilt tot stand brengen.

1. Klik **sparen** om het rapport tot stand te brengen en het toe te voegen aan het dashboard.

## Een voorbeeld van een diagramrapport maken

In deze sectie, zullen wij over de stappen gaan om een kolomgrafiek tot stand te brengen die achterstallige taken door projecteigenaar toont.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**

1. Klik **creëren**.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **Grafiek**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Ga een rapport **Naam** in (b.v. *Verouderde Taken door de Eigenaar van het Project*).

   1. Ga een rapport **Beschrijving** in.

1. Volg hieronder de stappen om **bouwt grafiek** sectie te vormen:

   1. In het linkerpaneel, klik het **bouwt grafiek** pictogram.

   1. In het **type van Grafiek** drop-down, uitgezochte **Kolom**.

   1. In het **type van Kolom** drop-down, uitgezochte **Eenvoudig**.

   1. Selecteer het **gebied van de Update** knoop onder de **bodem (X) as** sectie, dan bepaal de plaats en selecteer van de **Taak** > **Project** > **Eigenaar** > **Naam** gebied.

      ![ gebied van de Update ](assets/bottom-x-axis.png)

   1. Klik het **Uitgezochte gebied** knoop onder de **Linkeras (Y)** sectie, dan bepaal de plaats en selecteer van de **Taak** > **het gebied van de Naam**.

   1. In het **type van Samenvoeging** drop-down, uitgezochte **Telling**.

      ![ het typegebied van de Samenvoeging ](assets/left-y-axis.png)

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter**.

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde**.

   1. Klik op het lege voorwaardengebied, dan selecteren het **Gebied van de Selectie**.

   1. Selecteer het **Volledige** gebied van de Percentage.

   1. In de **drop-down exploitanten**, uitgezocht **minder dan**, dan ga *100* op het evaluatorgebied in.

   1. Klik **toevoegen Voorwaarde**, dan **Gebied van de Selectie**.

   1. Selecteer het **Geplande gebied van de Datum van de Voltooiing**.

   1. In de **drop-down exploitanten**, uitgezochte **minder dan**.

   1. Knevel **Vastgestelde relatieve datum** aan ****.

   1. Ga *$$TODAY* op het evaluatiegebied in.

      Voor meer informatie over vervangingen, zie de sectie op datum-Gebaseerde variabelen van de vervangingsfilter in [ rapportfilters in een 1} artikel van het Dashboard van het Canvas uitgeven.](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md)

      ![ het gebied van de Evaluator ](assets/add-condition.png)

1. Volg hieronder de stappen om de **sectie van de Montages van de Kolom te vormen 0} Drilldown {:**

   1. In het linkerpaneel, klik het **Drilldown Kolommen** ![ Drilldown kolommen ](assets/drilldown-column.png) pictogram. De velden in het diagram worden automatisch als kolommen weergegeven in de voorbeeldsectie aan de rechterkant.

   1. Klik **toevoegen kolom**, dan selecteren **Toegewezen aan** > **Naam** gebied.

   1. Klik **toevoegen kolom**, dan selecteren het **Geplande gebied van de Datum van het Begin**.

   1. Klik **toevoegen kolom**, dan selecteren het **Geplande gebied van de Datum van de Voltooiing**.

   1. Klik **toevoegen kolom**, dan selecteren het **Laatste gebied van de Datum van de Update**.

   1. (Facultatief) om de updatetijd te tonen, selecteer de **Laatste optie van de Datum van de Update** op het **Huidige gebied van Kolommen**, dan selecteer een optie van de tijdwaarde in het **formaat van de Datum** drop-down.

1. Volg hieronder de stappen om de **sectie van de Montages van de Groep van de Drilldown** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Montages van de Groep** ![ van de Montages van de Groep ](assets/drilldown-group-icon.png).

   1. Klik **toevoegen groeperend** knoop en selecteer dan het **Project** > **gebied van de Naam**.

1. Klik **sparen** om het rapport tot stand te brengen en het toe te voegen aan het dashboard.

## Overwegingen bij het samenstellen van een grafiekrapport

### De veldkiezer gebruiken

De **secties** drop-down in de **bouwt grafiek** sectie wordt ontworpen om de keuzen op een gebiedsselecteur te versmallen om een voorwerp gemakkelijker te maken om te vinden wanneer het bouwen van een lijstrapport. Om te beginnen selecteert u een basisentiteitsobject.

* **Alle Secties**: Alle objecten types in het Werkschema van Workfront en de Planning van Workfront.
* **de Voorwerpen van Workfront**: De inheemse voorwerpen van het Werkschema van Workfront.
* **de Types van Verslag van de Planning**: De verslagtypes van Douane die in de Planning van Workfront worden bepaald.

![ drop-down Secties ](assets/sections-dropdown.png)

Zodra het voorwerp van de basisentiteit is geselecteerd, **secties** drop-down dan werkt met toepasselijke gebiedstype opties bij om van te kiezen.

* **Alle Secties**: Inheemse gebieden, douanegebieden, en verwante voorwerpen.
* **Alle Gebieden**: Zowel inheemse als douanegebieden (sluit verhoudingen) uit.
* **Gebieden van de Douane**: Klant-bepaalde gebieden of op een douanevorm of een verslag van de Planning.
* **de Gebieden van Workfront**: Eigen gebieden slechts.
* **Verhoudingen**: Verbonden verslagen.

![ Te Rapporteren objecten selectie ](assets/reportable-objects-selection.png)

### Verwijzen naar onderliggende objecten

De beschikbare verhoudingen voor extra kolommen, filteropties, en groeperingsattributen zijn over het algemeen beperkt tot voorwerpen hoger in de objecten van Workfront hiërarchie of anders één enkele selectie op het voorwerp van de basisentiteit van het rapport hebben. Hierop zijn enkele uitzonderingen van toepassing, waaronder:

* Project > Taken
* Documentgoedkeuring > Documentgoedkeuringsfasen
* Acties voor documentgoedkeuring > Deelnemers aan werkgebied voor documentgoedkeuring

Wanneer u een van de bovenstaande relaties van bovenliggend item naar onderliggend item gebruikt, wordt in de tabel een rij weergegeven voor elke onderliggende record die is verbonden met het bovenliggende object.