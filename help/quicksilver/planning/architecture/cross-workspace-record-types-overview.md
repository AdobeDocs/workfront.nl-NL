---
title: Overzicht recordtypen tussen werkruimten
description: De gecentraliseerde verslagtypes kunnen aan veelvoudige werkruimten van een centrale of primaire werkruimte in de Planning van Adobe Workfront worden toegevoegd.
hidefromtoc: true
hide: true
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1349'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Overzicht van recordtypen voor verschillende werkruimten

In de Planning van Adobe Workfront, kunt u dwars-werkruimtemogelijkheden voor een verslagtype toelaten dat u om een verslagtype in meer dan één werkruimte van verwijzingen kunt voorzien.

Hieronder vindt u de mogelijkheden van recordtypen tussen werkruimten:

* U kunt een recordtype instellen als gecentraliseerd. Gebruikers kunnen gecentraliseerde recordtypen toevoegen aan andere werkruimten die zij beheren.

  >[!IMPORTANT]
  >
  >U moet beschikken over een Workfront Planning Plus-pakket, naast een Workfront-pakket om gecentraliseerde recordtypen te kunnen gebruiken.
  >
  >Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningspakket wordt opgenomen.

* U kunt een recordtype aanwijzen als aanpasbaar. Gebruikers kunnen vanuit andere werkruimten verbinding maken met dit recordtype.

In dit artikel vindt u een overzicht van recordtypen tussen werkruimten. Voor informatie over het bepalen van de mogelijkheden van de dwars-werkruimte van een verslagtype, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.


## Overzicht van gecentraliseerde recordtypen

De gecentraliseerde verslagtypes kunnen aan veelvoudige werkruimten van een centrale of primaire werkruimte in de Planning van Workfront worden toegevoegd.

Wanneer het uitvoeren van de Planning van Workfront voor een multi-teamorganisatie met gemeenschappelijke werkschema&#39;s, zou u een samenhangende structuur en meta-gegevens voor zeer belangrijke verslagtypes (zoals Campagnes of Deliverables) kunnen moeten bepalen die aan de werkruimten van elk team kunnen worden toegevoegd om hun werk te vangen en te beheren.

Ook, zou u het werk van elk team kunnen nodig hebben om tot een centraal niveau te rollen.

In zo&#39;n werkschema, kunt u ervoor zorgen dat de teams hun werk constant vangen terwijl het ontgrendelen van dwars-teamzicht, zonder de behoefte om alles aan één werkruimte, of iedereen in de organisatie aan elke werkruimte toe te voegen. Hiervoor kunt u gecentraliseerde recordtypen gebruiken.

Ga als volgt te werk om gecentraliseerde recordtypen te gebruiken:

1. Configureer een recordtype dat in een specifieke werkruimte moet worden gecentraliseerd.

   Een werkruimtemanager kan toestemmingen aan gebruikers met een Standaardvergunning, of teams, groepen, rollen, en bedrijven geven om een gekozen verslagtype aan een werkruimten toe te voegen zij leiden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte, maar wordt in andere werkruimten weergegeven.

   Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Voeg een recordtype aan een secundaire werkruimte van bestaande toe die als gecentraliseerd verslagtype is gevormd.

   Het recordtype bestaat in de volgende werkruimten:

   * Zijn originele werkruimte waar het als gecentraliseerd verslagtype werd aangewezen.
   * Een secundaire werkruimte.

   Voor informatie, zie [ bestaande verslagtypes van een andere werkruimte ](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md) toevoegen.

   De volgende secties beschrijven overwegingen over gecentraliseerde verslagtypes en hoe zij in of hun originele of secundaire werkruimten functioneren.

### Overwegingen over de gecentraliseerde recordtypen in hun oorspronkelijke werkruimte

Het recordtype dat is geconfigureerd om te worden gecentraliseerd, heeft de volgende eigenschappen:

* Alle gegevens (weergave, oorspronkelijke velden) kunnen alleen worden bewerkt in de oorspronkelijke werkruimte.

* U kunt de volgende handelingen uitvoeren op het gecentraliseerde recordtype vanuit de oorspronkelijke werkruimte van een gecentraliseerd recordtype:

   * Bewerk het

     Het bewerken van een gecentraliseerd recordtype omvat het bewerken van de weergave, de mogelijkheden van de werkruimte en alle velden die in de oorspronkelijke werkruimte zijn gemaakt.
   * Aanvraagformulieren maken
   * Aanvraagformulieren beheren

* U kunt een gecentraliseerd recordtype alleen verwijderen als het niet is toegevoegd aan een secundaire werkruimte. Nadat het aan een andere werkruimte wordt toegevoegd, zal het proberen om het van de originele werkruimte te schrappen een fout veroorzaken.

  Dit wordt gedaan zodat het gecentraliseerde verslagtype in de werkruimten kan blijven waar het reeds is toegevoegd.
* De verslagen die u aan een gecentraliseerd verslagtype toevoegt zijn zichtbaar slechts aan gebruikers die de toestemmingen van de Mening aan de werkruimte hebben waar zij werden toegevoegd.
* De verslagen die u van een secundaire werkruimte toevoegt rollen omhoog en tonen in de originele werkruimte. Alle leden van de oorspronkelijke werkruimte krijgen weergavemachtigingen.

* De aangesloten recordtypen van een gecentraliseerd recordtype worden beschikbaar voor verbinding vanuit de werkruimten waar dit recordtype wordt toegevoegd.

  Bijvoorbeeld, als u een type van het verslagverslag van de Campagne hebt dat een verbinding met het verslagtype van Gebieden heeft, en u het type van het verslag van de Campagne aan een secundaire werkruimte toevoegt, zullen de Gebieden dwars-werkruimte verbindbaar voor de secundaire werkruimte worden. De leden van de secundaire werkruimte kunnen nu campagnes maken en deze koppelen aan gebieden.

* Velden die voor een gecentraliseerd recordtype zijn gemaakt in de oorspronkelijke werkruimte, zijn zichtbaar in alle werkruimten waar het recordtype is toegevoegd. De gebiedsmontages van een originele werkruimte zijn read-only in de secundaire werkruimten.

### Overwegingen over gecentraliseerde recordtypen na het toevoegen van deze aan een secundaire werkruimte

* Secundaire werkruimtegangers krijgen Contribute-toestemming voor het gecentraliseerde recordtype in de werkruimte van hun team. Zij kunnen verslagen in het van de secundaire werkruimte toevoegen en beheren.

* Secundaire werkruimtevieken krijgen Weergavemachtiging voor het gecentraliseerde recordtype in de werkruimte van hun team. Ze kunnen er geen records in toevoegen en beheren.

* Secundaire werkruimtemanagers kunnen de volgende extra acties op het verslagtype uitvoeren dat van een gecentraliseerd verslagtype in een secundaire werkruimte wordt toegevoegd:

   * Verwijder het bestand.

     Als u het recordtype uit een secundaire werkruimte verwijdert, wordt dit alleen verwijderd uit de secundaire werkruimte. De records die vanuit de secundaire werkruimte aan de werkruimte worden toegevoegd, worden ook verwijderd. Hierdoor wordt het recordtype niet verwijderd uit de oorspronkelijke werkruimte of uit andere secundaire werkruimten waar het is toegevoegd.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Geen enkele gebruiker kan de volgende handelingen uitvoeren op het recordtype dat vanuit een gecentraliseerd recordtype in een secundaire werkruimte wordt toegevoegd:

   * Bewerk het

     U kunt de weergave, de mogelijkheden van de werkruimte of de toegevoegde velden niet bewerken vanuit de oorspronkelijke werkruimte.
   * Aanvraagformulieren maken en beheren
   * Automatisering maken en beheren

* De verslagen die in secundaire werkruimten worden toegevoegd zijn zichtbaar van de volgende werkruimten, slechts als u Mening of hogere toestemmingen aan deze werkruimten hebt:

   * De secundaire werkruimte waar ze worden toegevoegd.
   * De oorspronkelijke werkruimte van het gecentraliseerde recordtype.
   * Alle andere werkruimten waar de gecentraliseerde werkruimte wordt toegevoegd.

* De volgende scenario&#39;s bestaan voor verslagen die in secundaire werkruimten worden gecreeerd:

   * Als u beheermachtigingen hebt voor de oorspronkelijke werkruimte en geen machtigingen voor een secundaire werkruimte, kunt u records weergeven die zijn toegevoegd vanuit de secundaire werkruimten in de oorspronkelijke werkruimte, maar kunt u deze records niet vanuit de oorspronkelijke werkruimte beheren.
   * Als u beheermachtigingen hebt voor de secundaire werkruimte, kunt u de records beheren in de oorspronkelijke werkruimte van het gecentraliseerde recordtype of vanuit de werkruimte waar ze zijn toegevoegd.
   * U kunt de verslagen in extra secundaire werkruimten bekijken waar het gecentraliseerde verslagtype wordt toegevoegd slechts als u de toestemmingen van de Mening aan die werkruimten hebt.

### Toegang tot de verbindingen van een gecentraliseerd recordtype

Recordtypen die zijn verbonden met het gecentraliseerde recordtype in de oorspronkelijke werkruimte, worden zichtbaar vanuit andere werkruimten waar het gecentraliseerde recordtype wordt toegevoegd.

### API-toegang van een gecentraliseerd recordtype

Bij het toevoegen van records aan een gecentraliseerd recordtype vanuit een secundaire werkruimte met de Workfront Planning API, controleert het systeem of de gebruiker toegang heeft om records te maken in de oorspronkelijke werkruimte van het gecentraliseerde recordtype.

De volgende gevallen bestaan:

* Als de gebruiker toegang heeft, wordt de record gemaakt in de oorspronkelijke werkruimte van de gecentraliseerde recordtypen.

* Als de gebruiker geen toegang heeft, krijgt de gebruiker een fout dat zij geen toegang tot de originele werkruimte van het gecentraliseerde verslagtype hebben en zij moeten werkruimte identiteitskaart verstrekken waar zij toegang hebben om verslagen tot stand te brengen.

## Overzicht van typen met verbonden records

U kunt vanuit elke werkruimte die u beheert verbinding maken met een recordtype dat is gedefinieerd als verbindingsbaar.

Uw teams zouden hun verslagen kunnen nodig hebben verbonden aan verslagtypes van andere werkruimten of meningsinformatie die op verslagen wordt gevangen die tot verslagen in andere werkruimten behoren. U kunt deze configuratie bereiken door een verslagtype als verbindingsbaar aan te wijzen.

Ga als volgt te werk om verbindingbare recordtypen te gebruiken:

1. Configureer een recordtype dat in een specifieke werkruimte kan worden verbonden.

   Een werkruimtenmanager kan selecteren welke werkruimten een bepaald verslagtype beschikbaar is om met van andere werkruimten te verbinden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte en wordt toegevoegd als een gekoppeld recordtype aan een andere werkruimte.

   Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Verbind met een verslagtype dat als aansluit van een andere werkruimte wordt aangewezen u beheert.

   Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
