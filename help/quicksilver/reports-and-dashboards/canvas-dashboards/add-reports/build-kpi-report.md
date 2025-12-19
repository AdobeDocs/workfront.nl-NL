---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Bouw een KPI- rapport in een dashboard van het Canvas
description: Een KPI-rapport waarin één geaggregeerde KPI prominent wordt weergegeven, kan worden toegevoegd aan een Canvasdashboard.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: d7caaa0871263fb8ef4224a9c298778f3ee2454a
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# Bouw een KPI- rapport in een dashboard van het Canvas

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Onderdelen van het onderdeel zijn mogelijk niet compleet of werken niet zoals bedoeld in deze fase. Gelieve te dienen om het even welke terugkoppelen betreffende uw ervaring door de instructies in [ te volgen verstrekt ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) sectie in het de bètaoverzichtsartikel van de dashboards van het Canvas.<br>
>Als u feedback hebt over een mogelijk probleem met een probleem of een technisch probleem, stuurt u een ticket naar Workfront Support. Voor meer informatie, zie [ de Steun van de Klant van het Contact ](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Deze bètaversie is niet beschikbaar op de volgende cloudproviders:
>
>* Je eigen sleutel voor Amazon Web Services
>* Azure
>* Google Cloud Platform

U kunt een PKI- rapport aan een Dashboard van het Canvas bouwen en toevoegen dat visueel uw zeer belangrijke gegevens van de prestatiesindicator als aantal vertegenwoordigt, dat u kunt dan gebruiken om te zien hoe uw projecten en teams presteren.

![ KPI- rapportvoorbeeld ](assets/kpi-example-main.png)

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

U moet een dashboard tot stand brengen alvorens u een KPI- rapport kunt bouwen.

## Bouw een KPI- rapport in een dashboard van het Canvas

Er zijn vele configuratieopties beschikbaar voor de bouw van een KPI- rapport. In deze sectie doorlopen we het algemene proces voor het maken van een sectie.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**

1. Klik **creëren**.

1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.

1. Voor de linkerkant, uitgezochte **KPI**.

1. In de hoger-juiste hoek, klik **creëren rapport**.

1. Volg hieronder de stappen om de **sectie van Details** te vormen:

   1. Ga een rapport **Naam** in.
   1. Ga een rapport **Beschrijving** in.

      >[!NOTE]
      >
      >De beschrijving wordt gebruikt als een bijschrift onder de KPI-waarde. Als u geen beschrijving opgeeft, wordt een bijschrift voor u gegenereerd op basis van het aggregator- en aggregatietype dat u in de volgende stappen selecteert.

1. Volg hieronder de stappen om de **Bouw KPI** sectie te vormen:

   1. In het linkerpaneel, klik het **Bouw KPI** ![ pictogram van KPI bouwen ](assets/build-kpi-icon.png).

   1. Klik **Uitgezochte gebied** en specificeer dan het gebied u aan het rapport wilt toevoegen.

   1. In het **type van Samenvoeging** drop-down, selecteer hoe de gegevens omhoog rollen om de output van KPI te veroorzaken. De opties in dit veld zijn afhankelijk van het type veld dat u in de vorige stap hebt geselecteerd.

1. Volg hieronder de stappen om de **sectie van de Filter** te vormen:

   1. In het linkerpaneel, klik het **pictogram van de Filter** ![ van de Filter ](assets/filter-icon.png).

   1. Selecteer **filter uitgeven**.

   1. Klik **toevoegen voorwaarde** en specificeer dan het gebied u tegen en de bepaling wilt filtreren die bepaalt welk soort voorwaarde het gebied moet ontmoeten.

   1. (Facultatief) klik **toevoegen filtergroep** om een andere reeks het filtreren criteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

      Voor meer informatie over filters, zie [ rapportfilters in een Dashboard van het Canvas ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md) uitgeven.

1. Volg hieronder de stappen om de **sectie van de Montages van de Kolom te vormen 0} Drilldown {:**

   1. In het linkerpaneel, klik het **Drilldown pictogram van Kolommen** ![ Drilldown kolommen ](assets/drilldown-column.png). De velden in het diagram worden automatisch als kolommen weergegeven in de voorbeeldsectie aan de rechterkant.

   1. (Facultatief) om het even welke bestaande kolomconfiguraties bij te werken, selecteer de kolom u in de **Huidige kolommen** sectie wilt bijwerken en dan de gewenste informatie (b.v. etiket, verbonden status, en het formatteren regels) bijwerken.

   1. Klik **toevoegen kolom** en selecteer dan het gebied u als kolom in de lijst wilt tonen. Herhaal dit proces voor elke kolom u wilt toevoegen.

1. Volg hieronder de stappen om de **sectie van de Montages van de Groep van de Drilldown** te vormen:

   1. In het linkerpaneel, klik het **** pictogram van de de groepengroep van de 1} Groep ![.](assets/drilldown-group-icon.png)

   1. Klik **toevoegen groeperend** knoop en dan het gebied selecteren u als groepering wilt tot stand brengen.

1. Klik **sparen** om het rapport tot stand te brengen en het toe te voegen aan het dashboard.

## Bouw een KPI- rapportvoorbeeld

In deze sectie, zullen wij de stappen gaan om een PKI- rapport tot stand te brengen dat hangende documentgoedkeuringen toont.

Voor meer informatie over KPI- rapportvoorbeelden, zie [ een rapportdashboard voor overzicht en goedkeuringen ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) creëren.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**

1. Klik **creëren**.

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
      ![ In afwachting van kpi filtervoorbeeld ](assets/pending-kpi-filter.png)
1. Klik **sparen** in de hoger-juiste hoek van het scherm.

## Overwegingen bij het bouwen van een KPI-rapport

### Rapporten met financiële gegevens

De gebruikers met Mening of geven toegang tot Financiële Gegevens in hun toegangsniveau uit zullen nog financiële gegevens in het dashboard van het Canvas visualisaties-zelfs zien als de de financieringstoestemming van de Mening op de taak of projectniveau wordt verwijderd.

* Gebruikers zonder financiële gegevensrechten op het niveau van de toegang zullen geen financiële gegevens in rapporten zien.
* Gebruikers die financiële gegevens zien, zijn beperkt tot records die ze al mogen bekijken (projecten, taken, problemen, enz.). Zij zullen geen financiële waarden zien voor verslagen zij niet kunnen toegang hebben tot.
* De makers van rapporten moeten voorzichtig zijn bij het opnemen van financiële gegevens in dashboards en zich bewust zijn van wie ze dashboards delen om onbedoelde toegang te voorkomen.

Dit is een bekende grens en we zijn van plan deze zo snel mogelijk aan te pakken.

### De veldkiezer gebruiken

De **secties** drop-down in de **Bouw KPI** sectie wordt ontworpen om de keuzen op een gebiedsselecteur te versmallen om een voorwerp gemakkelijker te maken om te vinden wanneer het bouwen van een lijstrapport. Om te beginnen selecteert u een basisentiteitsobject.

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


