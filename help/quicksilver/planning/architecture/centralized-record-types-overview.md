---
title: Overzicht van gecentraliseerde recordtypen
description: De gecentraliseerde verslagtypes kunnen aan veelvoudige werkruimten van een centrale of primaire werkruimte in de Planning van Adobe Workfront worden toegevoegd.
hidefromtoc: true
hide: true
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Overzicht van gecentraliseerde recordtypen

De gecentraliseerde verslagtypes kunnen aan veelvoudige werkruimten van een centrale of primaire werkruimte in de Planning van Adobe Workfront worden toegevoegd.

## Overzicht van gecentraliseerde recordtypen

Wanneer het uitvoeren van de Planning van Workfront voor een multi-teamorganisatie met gemeenschappelijke werkschema&#39;s, zou u een samenhangende structuur en meta-gegevens voor zeer belangrijke verslagtypes (zoals Campagnes of Deliverables) kunnen moeten bepalen die aan de werkruimten van elk team kunnen worden toegevoegd om hun werk te vangen en te beheren.

Ook, zou u het werk van elk team kunnen nodig hebben om tot een centraal niveau te rollen.

In zo&#39;n werkschema, kunt u ervoor zorgen dat de teams hun werk constant vangen terwijl het ontgrendelen van dwars-teamzicht, zonder de behoefte om alles aan één werkruimte, of iedereen in de organisatie aan elke werkruimte toe te voegen. Hiervoor kunt u gecentraliseerde recordtypen gebruiken.

Ga als volgt te werk om gecentraliseerde recordtypen te gebruiken:

1. Configureer een recordtype dat in een specifieke werkruimte moet worden gecentraliseerd.

   Een werkruimtemanager kan gebruikers met een Standaardvergunning, teams, groepen, rollen, of bedrijven selecteren om een gekozen verslagtype aan een werkruimten toe te voegen zij leiden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte, maar wordt zichtbaar gemaakt vanuit alle andere werkruimten.

   Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Voeg een bestaand verslagtype van bestaande toe die als gecentraliseerde aan de werkruimte van een team is gevormd.

   Het recordtype bestaat in de volgende werkruimten:

   * Zijn originele werkruimte waar het als gecentraliseerd verslagtype werd aangewezen.
   * De werkruimte van het team.

   Voor informatie, zie [ bestaande verslagtypes ](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md) toevoegen.

   De volgende secties beschrijven overwegingen over gecentraliseerde verslagtypes in of hun originele werkruimten of nadat zij aan de werkruimten van een team worden toegevoegd.

## Overwegingen over de gecentraliseerde recordtypen in hun oorspronkelijke werkruimte

Het recordtype dat is geconfigureerd om te worden gecentraliseerd, heeft de volgende eigenschappen:

* Alle gegevens kunnen alleen worden bewerkt in de oorspronkelijke werkruimte.

* U kunt de volgende handelingen uitvoeren op het gecentraliseerde recordtype vanuit de oorspronkelijke werkruimte van een gecentraliseerd recordtype:

   * Bewerk het

     Het bewerken van een gecentraliseerd recordtype omvat het bewerken van de weergave, de mogelijkheden van de werkruimte en alle velden die in de oorspronkelijke werkruimte zijn gemaakt.
   * Aanvraagformulieren maken
   * Aanvraagformulieren beheren

* U kunt een gecentraliseerd recordtype alleen verwijderen als het niet aan een teamwerkruimte is toegevoegd. Nadat het aan de werkruimte van een team wordt toegevoegd, zal het proberen om het van de originele werkruimte te schrappen een fout veroorzaken.

  Dit wordt gedaan zodat het gecentraliseerde verslagtype in de werkruimten kan blijven waar het reeds is toegevoegd.
* De verslagen die u aan een gecentraliseerd verslagtype toevoegt zijn zichtbaar slechts aan gebruikers die de toestemmingen van de Mening aan zijn originele werkruimte hebben.
* De verslagen die u van de werkruimte van het team toevoegt rollen omhoog en tonen in de originele werkruimte. Alle leden van de oorspronkelijke werkruimte krijgen hier weergavemachtigingen voor.

* De aangesloten recordtypen van een gecentraliseerd recordtype worden beschikbaar voor verbinding vanuit de werkruimten waar dit recordtype wordt toegevoegd.

* Velden die voor een gecentraliseerd recordtype zijn gemaakt in de oorspronkelijke werkruimte, zijn zichtbaar in alle werkruimten waar het recordtype is toegevoegd.

## Overwegingen over gecentraliseerde verslagtypes na het toevoegen van hen aan de werkruimte van een team

* Deelnemers aan de teamwerkruimte krijgen Contribute-machtigingen voor het gecentraliseerde recordtype in de teamwerkruimte. Ze kunnen er records in toevoegen en beheren.

* De de werkruimtekijkers van het team krijgen de toestemming van de Mening aan het gecentraliseerde verslagtype in de teamwerkruimte. Ze kunnen er geen records in toevoegen en beheren.

* De werkruimtemanagers van het team kunnen de volgende acties op het verslagtype uitvoeren dat van een gecentraliseerd verslagtype in de werkruimte van een team wordt toegevoegd:

   * Nieuwe velden toevoegen

     Velden die vanuit een teamwerkruimte aan een gecentraliseerde record worden toegevoegd, zijn alleen zichtbaar vanuit de werkruimte van het team.
   * Delen
   * Verwijder het bestand.

     Als u het recordtype uit de werkruimte van een team verwijdert, wordt dit alleen verwijderd uit de werkruimte van het team. De records die vanuit de werkruimte van het team aan het team zijn toegevoegd, worden ook verwijderd. Hierdoor wordt het recordtype niet verwijderd uit de oorspronkelijke werkruimte of uit andere teamwerkruimten waar het is toegevoegd.

     Dit wordt gedaan zodat het mogelijk is om reeds toegevoegde gecentraliseerde verslagtype in werkruimten te houden die het reeds gebruiken.

* U kunt niet de volgende acties op het verslagtype uitvoeren dat van een gecentraliseerd verslagtype in de werkruimte van een team wordt toegevoegd:

   * Bewerk het

     U kunt de weergave, de mogelijkheden van de werkruimte of de velden die u uit de oorspronkelijke werkruimte hebt geïmporteerd, niet bewerken.
   * Aanvraagformulieren maken
   * Aanvraagformulieren beheren

* Records die zijn toegevoegd in de werkruimten van een team, zijn zichtbaar vanuit de volgende werkruimten als u over weergave of hogere machtigingen voor deze werkruimten beschikt:

   * De werkruimte van het team waar ze zijn toegevoegd.
   * De oorspronkelijke werkruimte van het gecentraliseerde recordtype.
   * Alle andere werkruimten waar de gecentraliseerde werkruimte wordt toegevoegd.

* De volgende scenario&#39;s bestaan voor verslagen die in de werkruimten van teams worden gecreeerd:

   * Als u beheermachtigingen hebt in de oorspronkelijke werkruimte en geen machtigingen hebt voor de werkruimten van de teams, kunt u records die zijn toegevoegd vanuit de werkruimten van het team weergeven in de oorspronkelijke werkruimte, maar kunt u deze records niet vanuit de oorspronkelijke werkruimte beheren.
   * Als u beheermachtigingen hebt in de werkruimte van het team, kunt u de records beheren in de oorspronkelijke werkruimte van het gecentraliseerde recordtype of vanuit de werkruimte waar ze zijn toegevoegd.

     U kunt de verslagen in extra teamwerkruimten bekijken waar het gecentraliseerde verslagtype slechts wordt toegevoegd als u de toestemmingen van de Mening aan die werkruimten hebt.

## Toegang tot verbindingen

Recordtypen die zijn verbonden met het gecentraliseerde recordtype in de oorspronkelijke werkruimte, worden zichtbaar voor teamwerkruimten waar het gecentraliseerde recordtype wordt toegevoegd.

## API-gedrag

Wanneer het toevoegen van verslagen aan een gecentraliseerd verslagtype van een teamwerkruimte gebruikend de Planning API van Workfront, controleert het systeem of de gebruiker toegang heeft om verslagen in de originele werkruimte van het gecentraliseerde verslagtype tot stand te brengen.

De volgende gevallen bestaan:

* Als de gebruiker toegang heeft, wordt de record gemaakt in de oorspronkelijke werkruimte van de gecentraliseerde recordtypen.

* Als de gebruiker geen toegang heeft, krijgt de gebruiker een fout dat zij geen toegang tot de originele werkruimte van het gecentraliseerde verslagtype hebben en zij moeten werkruimte identiteitskaart verstrekken waar zij toegang hebben om verslagen tot stand te brengen.