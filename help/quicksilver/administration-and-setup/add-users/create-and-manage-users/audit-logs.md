---
title: Overzicht controlelogboeken
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als beheerder van Adobe Workfront, kunt u gebruiker-veranderingen volgen die in het systeem tijdens de afgelopen 90 dagen worden teweeggebracht gebruikend controlelogboeken.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 85c6985d27ef0806e9152ecf2cbd90ca63a588c6
workflow-type: tm+mt
source-wordcount: '1523'
ht-degree: 0%

---

# Overzicht van auditlogboeken

<!--Audited: 08/2025-->

Als beheerder van Adobe Workfront, kunt u gebruiker-veranderingen volgen die in het systeem tijdens de afgelopen 90 dagen worden teweeggebracht gebruikend de hieronder beschreven controlelogboeken.

Voor instructies bij het bekijken van en het filtreren wat u in deze controlelogboeken wilt zien, zie [ de controlelogboeken van de Mening en van de uitvoer ](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## De informatie u in een controlelogboek kunt vinden

De volgende gebieden worden geregistreerd in elke ingang van het controlelogboek:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datum en tijd</td> 
   <td>Wanneer de handeling heeft plaatsgevonden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Logbestandstype</td> 
   <td>Type van het controlelogboek, zoals het Niveau van de Toegang of de Vorm van de Douane.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gebruikersnaam</td> 
   <td> <p>Naam van de gebruiker die de handeling heeft uitgevoerd.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Handeling</td> 
   <td> Handelingen die door de gebruiker worden uitgevoerd, zoals Wijzigen, Maken en Verwijderen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object</td> 
   <td> Naam van het object dat wordt beïnvloed door de handeling. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Details</td> 
   <td>Aanvullende details over de handeling. Plaats de muis boven de tekst om het volledige bericht te lezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP-adres</td> 
   <td> <p>IP adres van de gebruiker die de actie op het tijdstip van de actie uitvoerde.</p> <p>Het IP-adres is niet beschikbaar voor bepaalde systeemhandelingen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Controlelogbestandstypen en de acties die deze activeren

* [ Niveau van de Toegang ](#access-level)
* [Zakelijke regels](#business-rules)
* [ Bedrijf ](#company)
* [ Voorwaarde ](#condition)
* [ Douane Gebied ](#custom-field)
* [ Vorm van de Douane ](#custom-forms)
* [ Sectie van de Douane ](#custom-section)
* [ Wisselkoers ](#exchange-rate)
* [ Groep ](#group)
* [ Rol van de Baan ](#job-role)
* [ Prioriteit ](#priority)
* [ Voorkeur van het Project ](#project-preference)
* [ Ernst ](#severity)
* [ Status ](#status)
* [ Taken &amp; de Voorkeur van Kwesties ](#tasks-issues-preferences)
* [Gebruiker](#user)
<!--* [Login Attempt](#login-attempt) -->

### Toegangsniveau {#access-level}

Het systeem produceert een het logboekingang van het Niveau van de Toegang wanneer een gebruiker één van de volgende acties doet:

* Creeert een toegangsniveau
* Hiermee wordt een toegangsniveau verwijderd
* Wijzigt een toegangsniveau:

   * Hiermee wordt het licentietype gewijzigd
   * Hiermee wijzigt u machtigingen voor projecten, taken, problemen, portfolio&#39;s, programma&#39;s, rapporten, documenten, gebruikers of sjablonen

     >[!NOTE]
     >
     >Het systeem registreert geen toestemmingsveranderingen in Financiële Gegevens of binnen de volgende toegangstypes: Mening en geeft uit.
     >
     >Als een gebruiker bijvoorbeeld het toegangstype Planner wijzigt van Weergave in Bewerken, geeft het systeem geen informatie weer die in het vervolgkeuzemenu Instellingen nauwkeurig instellen staat.

### Zakelijke regels

Zakelijke regels zijn alleen beschikbaar voor klanten die een Ultimate Workfront-abonnement hebben aangeschaft. Voor meer informatie, zie [ bedrijfsregels ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md) creëren en uitgeven.

Het systeem produceert een ingang van het de controlelogboek van de BedrijfsRegel wanneer een gebruiker één van het volgende doet:

* Creeert een bedrijfsregel
* Bewerkt een bedrijfsregel:

   * Wijzigt de naam
   * Expressies toevoegen of verwijderen
   * Hiermee wordt een trigger gewijzigd

* Verwijdert een bedrijfsregel

### Bedrijf {#company}

Het systeem produceert een ingang van het de controlelogboek van het Bedrijf wanneer een gebruiker één van het volgende doet:

* Creeert een bedrijf
* Wijzigt een bedrijf:

   * Wijzigt de naam
   * Leden toevoegen of verwijderen
   * Hiermee wordt de waarde in het veld Groep toegevoegd, bewerkt of verwijderd
   * Voegt een tarief van het bedrijf voor een baanrol toe of geeft uit
   * Hiermee verwijdert u een factureringstarief voor een functie
   * Hiermee stelt u het in als het primaire bedrijf voor de organisatie
   * Hiermee voegt u een aangepast formulier toe of verwijdert u dit

* Een bedrijf verwijderen

Voor meer informatie over statussen, zie [ Overzicht van Statussen ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Voorwaarde {#condition}

Het systeem produceert een ingang van het de controlelogboek van de Voorwaarde wanneer een gebruiker één van de volgende acties doet:

* Maakt een voorwaarde
* Hiermee wijzigt u een voorwaarde:

   * De naam wijzigen
   * De kleur wijzigen
   * Hiermee wordt deze ingesteld als standaard
   * Hiermee wordt de beschrijving van de voorwaarde gewijzigd of verwijderd
   * Hiermee wordt de voorwaarde verborgen of weergegeven

* Hiermee wordt een voorwaarde verwijderd

Voor meer informatie over het vormen van baanrollen, zie [ een douanevoorwaarde ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) creëren of uitgeven.

### Aangepast veld {#custom-field}

Het systeem genereert een controlelogbestandvermelding Aangepast veld wanneer een gebruiker een van de volgende handelingen uitvoert:

* Hiermee maakt u een aangepast veld
* Hiermee wijzigt u een aangepast veld:

   * De naam, het label, de instructies of de indeling wijzigen
   * Hiermee wordt het weergavetype gewijzigd

     Dit is alleen beschikbaar als het veld een van de volgende typen is: één regel, alinea, vervolgkeuzelijst, selectievakje, keuzerondje

   * De veldgrootte wijzigen

     Dit is alleen beschikbaar als het veld een van de volgende typen is: één regel, alinea, tekst met opmaak

   * Hiermee voegt u een veldkeuze toe, verwijdert of verbergt u deze
   * Hiermee bewerkt u een label of waarde voor een veldkeuze
   * Hiermee configureert u de veldoptie die u wilt selecteren
   * Vormt een drop-down gebied om veelvoudige selecties of één enkele selectie toe te staan
   * Vormt een datumveld om de tijd van de dag al dan niet weer te geven
   * Hiermee bewerkt u de hyperlink of wijzigt u de waarde in een beschrijvend tekstveld

* Hiermee verwijdert u een aangepast veld
* Deelt een aangepast veld

### Aangepast formulier {#custom-form}

Het systeem genereert een aangepaste Forms-controlelogbestandvermelding wanneer een gebruiker een van de volgende handelingen uitvoert:

* Hiermee maakt u een aangepast formulier
* Een aangepast formulier wijzigen:

   * De naam of beschrijving wijzigen
   * Schakelt actief in of uit
   * Hiermee wordt een veld of sectie toegevoegd of verwijderd
   * Voor een aangepaste sectie wijzigt u een instelling onder Aanvullende instellingen
   * Een veld wijzigen in vereist of niet vereist
   * Hiermee wordt een berekening in een aangepast veld gewijzigd
   * Hiermee verbergt of geeft u de formule weer die is gekoppeld aan een berekend veld in de aanwijstekst
   * Hiermee schakelt u vorige berekeningen bijwerken in of uit
   * Hiermee voegt u logica of weergavelogica over het overslaan of wijzigen

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Hiermee verwijdert u een aangepast formulier
* Hiermee deelt u een aangepast formulier

### Aangepaste sectie {#custom-section}

Het systeem produceert een ingang van het de controlelogboek van de Sectie van de Douane wanneer een gebruiker één van de volgende acties in een douaneformulier doet:

* Hiermee maakt u een aangepaste sectie
* De naam of beschrijving van een aangepaste sectie wijzigen
* Hiermee verwijdert u een aangepaste sectie

Voor informatie over douanesecties in douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

### Wisselkoers {#exchange-rate}

Het systeem produceert een ingang van het de controlelogboek van het Tarief van de Uitwisseling wanneer een gebruiker één van de volgende acties doet:

* Maakt een wisselkoers
* Verandert een wisselkoers:

   * Hiermee wordt een valuta toegevoegd
   * Verandert de koers van de valuta
   * Hiermee wordt de valuta ingesteld als de basisvaluta (standaardvaluta) voor alle projecten en rapporten in het hele systeem

* Verwijdert een wisselkoers

Voor meer informatie over het vormen van wisselkoersen, zie [ de wisselkoers van de Opstelling ](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Groep {#group}

Het systeem produceert een ingang van het de controlelogboek van de Groep wanneer een gebruiker één van de volgende acties doet:

* Hiermee wordt een groep gemaakt
* Hiermee wordt een groep verwijderd
* Een groep wijzigen:

   * Gebruikers toevoegen of verwijderen
   * Subgroepen toevoegen of verwijderen

### Taken rollen {#job-role}

Het systeem produceert een ingang van het de controlelogboek van de Rollen van de Baan wanneer een gebruiker één van de volgende acties doet:

* Hiermee wordt een taakrol gemaakt
* Hiermee wijzigt u een taakrol:

   * De naam wijzigen
   * Hiermee voegt u de beschrijving toe, wijzigt u deze of verwijdert u deze.
   * Hiermee voegt u de kosten per uur toe, wijzigt u deze of verwijdert u deze. (Kosten/uur)
   * Voegt, verandert, of verwijdert het factureringstarief (Rekening/Hr.) toe

* Hiermee wordt een taakrol verwijderd

Voor meer informatie over het vormen van baanrollen, zie [ baanrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.

### Aanmeldingspoging {#login-attempt}

Het systeem genereert een logbestandvermelding van een Login-poging wanneer een gebruiker een van de volgende handelingen uitvoert:

* Meld u aan, meldt u zich af of mislukt een aanmeldingspoging in Workfront (in een browser en in de mobiele app)
* Meld u aan, meldt u zich af of mislukt een aanmeldingspoging bij Workfront-integratie (zoals Workfront voor Slack)
* Aanmelden of zich afmelden bij de Workfront API

Login Attempt Logs registreert niet wanneer een beheerder van Workfront Login als eigenschap gebruikt.

>[!NOTE]
>
>Dit is niet beschikbaar als uw organisatie is aangemeld bij de Adobe Admin Console. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

### Prioriteit {#priority}

Het systeem produceert een ingang van het Prioritair controlelogboek wanneer een gebruiker één van de volgende acties doet:

* Maakt een prioriteit
* Hiermee wijzigt u een prioriteit:

   * De naam wijzigen
   * De kleur wijzigen
   * Hiermee wordt deze ingesteld als standaard
   * Hiermee voegt u een beschrijving van de prioriteit toe, wijzigt u deze of verwijdert u deze
   * Hiermee verbergt of toont u de prioriteit

* Hiermee wordt een prioriteit verwijderd

Voor meer informatie over het vormen van prioriteiten, zie [ prioriteiten ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md) creëren en aanpassen.

### Projectvoorkeur {#project-preference}

Het systeem produceert een ingang van het de controlelogboek van de Voorkeur van het Project wanneer een gebruiker één van de volgende acties doet:

* Hiermee maakt u een aangepast kwartaal
* Hiermee wijzigt u een projectvoorkeur:

   * Hiermee vergrendelt of ontgrendelt u het
   * Hiermee wijzigt u een van de instellingen
   * Hiermee schakelt u het bestand in, uit of bewerkt het
   * Hiermee wordt een tijdlijnberekening bewerkt

* Hiermee wordt een aangepast kwartaal verwijderd

Voor meer informatie over projectvoorkeur, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

### Ernst {#severity}

Het systeem genereert een item in het log voor de controle van de ernst wanneer een gebruiker een van de volgende handelingen uitvoert:

* Hiermee maakt u een prioriteitsniveau in de uitgave
* Hiermee wijzigt u de ernst van een uitgave:

   * De naam wijzigen
   * De kleur wijzigen
   * Hiermee wordt deze ingesteld als standaard
   * Hiermee wordt de beschrijving van de ernst gewijzigd of verwijderd
   * Hiermee verbergt of toont u de ernst

* Hiermee verwijdert u de ernst van een uitgave

Voor meer informatie over het vormen van baanrollen, zie [ tot stand brengen of passen de controles van de kwestie ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md) aan.

### Status {#status}

Het systeem produceert een ingang van het de controlelogboek van de Status wanneer een gebruiker één van de volgende acties doet:

* Maakt een status op systeem- of groepsniveau
* Wijzigt een status op systeem- of groepsniveau:

   * Wijzigt de naam
   * Maakt van het tot een standaardstatus
   * Hiermee vergrendelt of ontgrendelt u het
   * Hiermee verbergt of verbergt u deze
   * Hiermee wijzigt u de kleur of beschrijving

* Hiermee wordt een status op systeem- of groepsniveau verwijderd

Voor meer informatie over statussen, zie [ Overzicht van Statussen ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Voorkeuren voor taken en problemen {#tasks-issues-preferences}

Het systeem genereert een controlelogbestandvermelding voor taken en problemen wanneer een gebruiker een voorkeur voor Taken en problemen op een van de volgende manieren wijzigt:

* Een voorkeur vergrendelen of ontgrendelen
* Hiermee wordt de instelling voor een voorkeur gewijzigd
* Hiermee wijzigt u de instelling Toegang voor taken, problemen of verzoeken

Voor meer informatie over taak en uitgevende voorkeur, zie [ taak voor het hele systeem vormen en voorkeur uitgeven ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Gebruiker {#user}

Het systeem produceert een ingang van het de controlelogboek van de Gebruiker wanneer een gebruiker één van de volgende acties doet:

* Hiermee wordt een gebruiker gemaakt

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Dit is niet beschikbaar als uw organisatie is aangemeld bij de Adobe Admin Console. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

* Hiermee wordt een gebruiker verwijderd
* Hiermee wijzigt u het toegangsniveau, het bedrijf, het team of de groep van een gebruiker
* Hiermee wordt een gebruiker geactiveerd
* Hiermee wordt een gebruiker gedeactiveerd
