---
title: Overzicht recordtype tussen werkruimten
description: Algemene recordtypen kunnen vanuit een centrale of primaire werkruimte in Adobe Workfront Planning aan meerdere werkruimten worden toegevoegd.
hidefromtoc: true
hide: true
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Overzicht van recordtypen voor verschillende werkruimten

{{planning-important-intro}}

U kunt mogelijkheden voor de verschillende werkruimten inschakelen voor een recordtype in Adobe Workfront Planning. Er kan naar een recordtype voor meerdere werkruimten worden verwezen of het kan vanuit meerdere werkruimten worden geopend.

>[!IMPORTANT]
>
>Er zijn uitgebreide Workfront-pakketvereisten om cross-workspace mogelijkheden voor recordtypen in uw systeem in te schakelen. Voor informatie, zie [&#x200B; het toegangsoverzicht van de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/access/access-overview.md).


Hieronder vindt u de mogelijkheden van recordtypen tussen werkruimten:

* **Globale verslagtypes**: De gebruikers kunnen globale verslagtypes aan andere werkruimten toevoegen zij leiden.

* **Verbonden verslagtypes**: De gebruikers kunnen met dit verslagtype van andere werkruimten verbinden.

In dit artikel vindt u een overzicht van recordtypen tussen werkruimten. Voor informatie over het bepalen van de mogelijkheden van de dwars-werkruimte van een verslagtype, zie [&#x200B; mogelijkheden van de dwars-werkruimte voor verslagtypes &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

## Overzicht van algemene recordtypen

Algemene recordtypen kunnen vanuit een centrale of primaire werkruimte in Workfront Planning aan meerdere werkruimten worden toegevoegd.

Wanneer het uitvoeren van de Planning van Workfront voor een multi-teamorganisatie met gemeenschappelijke werkschema&#39;s, zou u een samenhangende structuur en meta-gegevens voor zeer belangrijke verslagtypes (zoals Campagnes of Deliverables) kunnen moeten bepalen die aan de werkruimten van elk team kunnen worden toegevoegd om hun werk te vangen en te beheren.

Ook, zou u het werk van elk team kunnen nodig hebben om tot een centraal niveau te rollen.

In zo&#39;n werkschema, kunt u ervoor zorgen dat de teams hun werk constant vangen terwijl het ontgrendelen van dwars-teamzicht, zonder de behoefte om alles aan één werkruimte, of iedereen in de organisatie aan elke werkruimte toe te voegen. Hiervoor kunt u algemene recordtypen gebruiken.

Ga als volgt te werk om algemene recordtypen te gebruiken:

1. Van een werkruimte u beheert, vorm een verslagtype om globaal te zijn.

   Een werkruimtemanager kan toestemmingen aan gebruikers met een Standaardvergunning, of teams, groepen, rollen, en bedrijven geven om een gekozen verslagtype aan een werkruimten toe te voegen zij leiden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte, maar wordt in andere werkruimten weergegeven.

   Voor informatie, zie [&#x200B; mogelijkheden van de dwars-werkruimte voor verslagtypes &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Voeg een recordtype aan een secundaire werkruimte van bestaande toe die als globaal verslagtype is gevormd.

   Het recordtype bestaat in de volgende werkruimten:

   * Zijn originele werkruimte waar het als globaal verslagtype werd aangewezen.
   * Een secundaire werkruimte.

   Voor informatie, zie [&#x200B; bestaande verslagtypes van een andere werkruimte &#x200B;](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md) toevoegen.

   De volgende secties beschrijven overwegingen over globale verslagtypes en hoe zij in of hun originele of secundaire werkruimten functioneren.

### Overwegingen over de algemene recordtypen in hun oorspronkelijke werkruimte

Het recordtype dat globaal wordt geconfigureerd, heeft de volgende eigenschappen:

* Alle gegevens (weergave, oorspronkelijke velden) kunnen alleen worden bewerkt in de oorspronkelijke werkruimte.

* U kunt de volgende handelingen uitvoeren op het algemene recordtype vanuit de oorspronkelijke werkruimte:

   * Bewerk het

     Het bewerken van een algemeen recordtype omvat het bewerken van de weergave, de mogelijkheden van de werkruimte en alle velden die in de oorspronkelijke werkruimte zijn gemaakt.
   * Aanvraagformulieren maken
   * Aanvraagformulieren beheren

* U kunt een algemeen recordtype alleen verwijderen als het niet is toegevoegd aan een secundaire werkruimte. U moet het eerst verwijderen (door het te schrappen) uit de secundaire werkruimten alvorens u het uit de originele werkruimte kunt schrappen.
* De records die u toevoegt aan een algemeen recordtype zijn alleen zichtbaar voor gebruikers die weergavemachtigingen hebben voor de werkruimte waar ze zijn toegevoegd.
* De verslagen die u van een secundaire werkruimte toevoegt rollen omhoog en tonen in de originele werkruimte. Alle leden van de oorspronkelijke werkruimte krijgen weergavemachtigingen.
* Als het originele globale verslagtype aan veelvoudige secundaire werkruimten wordt toegevoegd, kunt u de verslagen bekijken die aan andere werkruimten slechts van de originele werkruimte of van werkruimten worden toegevoegd waar u minstens toestemmingen aan Mening hebt.
* De verbonden verslagtypes van een globaal verslagtype zullen beschikbaar voor verbinding van de werkruimten worden waar dit verslagtype wordt toegevoegd.

  Bijvoorbeeld, als u een globaal verslagtype van de Campagne hebt dat een verbinding met een type van het verslag van Gebieden heeft, en u het type van het verslag van de Campagne aan een secundaire werkruimte toevoegt, zullen de Gebieden dwars-werkruimte verbindbaar van de secundaire werkruimte worden. De leden van de secundaire werkruimte kunnen nu campagnes maken en deze koppelen aan gebieden.

* Velden die in de oorspronkelijke werkruimte voor een algemeen recordtype zijn gemaakt, zijn zichtbaar in alle werkruimten waar het recordtype is toegevoegd. De gebiedsmontages van een originele werkruimte zijn read-only in de secundaire werkruimten.

### Overwegingen over globale verslagtypes in een secundaire werkruimte

* Secundaire werkruimtegangers krijgen Contribute-toestemming voor het algemene recordtype in de werkruimte van hun team. Zij kunnen verslagen in het van de secundaire werkruimte toevoegen en beheren.

* Secundaire werkruimtevieken krijgen Weergavemachtiging voor het algemene recordtype in de werkruimte van hun team. Ze kunnen er geen records in toevoegen en beheren.

* Secundaire werkruimtemanagers kunnen de volgende extra acties op het verslagtype uitvoeren dat van een globaal verslagtype in een secundaire werkruimte wordt toegevoegd:

   * Verwijder het bestand.

     Als u het recordtype uit een secundaire werkruimte verwijdert, wordt dit alleen verwijderd uit de secundaire werkruimte. De records en velden die er vanuit de secundaire werkruimte aan worden toegevoegd, worden ook verwijderd. Hierdoor wordt het recordtype niet verwijderd uit de oorspronkelijke werkruimte of uit andere secundaire werkruimten waar het is toegevoegd.

  <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* Geen enkele gebruiker kan de volgende handelingen uitvoeren op het recordtype dat vanuit een algemeen recordtype in een secundaire werkruimte wordt toegevoegd:

   * Bewerk het

     U kunt de weergave, de mogelijkheden van de werkruimte of de toegevoegde velden niet bewerken vanuit de oorspronkelijke werkruimte.
   * Aanvraagformulieren maken en beheren
   * Automatisering maken en beheren

* De verslagen die in een secundaire werkruimte worden toegevoegd zijn zichtbaar van de volgende werkruimten, slechts als u Mening of hogere toestemmingen aan deze werkruimten hebt:

   * De secundaire werkruimte waar ze worden toegevoegd.
   * De oorspronkelijke werkruimte van het algemene recordtype.
   * Alle andere werkruimten waar de algemene werkruimte wordt toegevoegd.

* De volgende scenario&#39;s bestaan voor verslagen die in secundaire werkruimten worden gecreeerd:

   * Als u beheermachtigingen hebt voor de oorspronkelijke werkruimte en geen machtigingen voor een secundaire werkruimte, kunt u records weergeven die zijn toegevoegd vanuit de secundaire werkruimten in de oorspronkelijke werkruimte, maar kunt u deze records niet vanuit de oorspronkelijke werkruimte beheren.
   * Als u beheermachtigingen hebt voor de secundaire werkruimte, kunt u de records beheren in de oorspronkelijke werkruimte van het algemene recordtype of vanuit de werkruimte waar ze zijn toegevoegd.
   * U kunt de verslagen in extra secundaire werkruimten bekijken waar het globale verslagtype slechts wordt toegevoegd als u de toestemmingen van de Mening aan die werkruimten hebt.

### Toegang tot de verbindingen van een globaal recordtype

Recordtypen die zijn verbonden met het algemene recordtype in de oorspronkelijke werkruimte, worden zichtbaar vanuit andere werkruimten waar het algemene recordtype wordt toegevoegd en zijn beschikbaar voor verbindingen vanuit de secundaire werkruimten waar het algemene recordtype wordt toegevoegd.

### API-toegang van een algemeen recordtype

Wanneer het toevoegen van verslagen aan een globaal verslagtype van een secundaire werkruimte gebruikend de Planning API van Workfront, controleert het systeem of de gebruiker toegang heeft om verslagen in de originele werkruimte van het globale verslagtype tot stand te brengen.

De volgende gevallen bestaan:

* Als de gebruiker toegang heeft, wordt de record gemaakt in de oorspronkelijke werkruimte van de algemene recordtypen.

* Als de gebruiker geen toegang heeft, krijgt de gebruiker een fout dat zij geen toegang tot de originele werkruimte van het globale verslagtype hebben en zij moeten werkruimte identiteitskaart verstrekken waar zij toegang hebben om verslagen tot stand te brengen.

## Overzicht van typen met verbonden records

U kunt vanuit elke werkruimte die u beheert verbinding maken met een recordtype dat is gedefinieerd als verbindingsbaar.

Uw teams zouden hun verslagen kunnen nodig hebben verbonden aan verslagtypes van andere werkruimten of meningsinformatie die op verslagen wordt gevangen die tot verslagen in andere werkruimten behoren. U kunt deze configuratie bereiken door een verslagtype als verbindingsbaar aan te wijzen.

Ga als volgt te werk om verbindingbare recordtypen te gebruiken:

1. Configureer een recordtype dat in een specifieke werkruimte kan worden verbonden.

   Een werkruimtenmanager kan selecteren welke werkruimten een bepaald verslagtype beschikbaar is om met te verbinden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte en kan toegankelijk zijn om verbinding te maken met een andere werkruimte.

   Voor informatie, zie [&#x200B; mogelijkheden van de dwars-werkruimte voor verslagtypes &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Verbind met een verslagtype dat als aansluit van een andere werkruimte wordt aangewezen u beheert.

   Voor informatie, zie [&#x200B; verbind verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
