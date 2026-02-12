---
title: Overzicht recordtype tussen werkruimten
description: U kunt recordtypen globaal of verbindingsbaar maken. Algemene recordtypen kunnen vanuit een centrale of primaire werkruimte in Adobe Workfront-planning worden toegevoegd aan meerdere werkruimten, terwijl verbindingbare recordtypen kunnen worden verbonden met andere werkruimten dan de eigen werkruimte.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 5a725e747e8776a867cb0dc4129544f6a28ce8e0
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 0%

---


# Overzicht van recordtypen voor verschillende werkruimten

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span> -->

{{planning-important-intro}}

U kunt mogelijkheden voor de verschillende werkruimten inschakelen voor een recordtype in Adobe Workfront Planning. Er kan naar een recordtype voor meerdere werkruimten worden verwezen of het kan vanuit meerdere werkruimten worden geopend.

>[!IMPORTANT]
>
>Uw organisatie moet de volgende pakketten aanschaffen om de mogelijkheden van werkruimten voor recordtypen te kunnen inschakelen:
>
>Verbindbare recordtypen configureren:
>
>
>* Alle Workfront-pakketten en alle planningspakketten
>
>   of
>
>* Willekeurige workflow en planningpakket voor Prime of Ultimate
>
>Globale recordtypen configureren:
>
>* Willekeurig Workfront-pakket en een plannings Plus-pakket
>     
>   of
>
>* Willekeurige workflow en planningpakket voor Prime of Ultimate
>
>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger.
>Voor informatie, zie [ het toegangsoverzicht van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/access-overview.md).

Hieronder vindt u de mogelijkheden van recordtypen tussen werkruimten:

* **Globale verslagtypes**: De gebruikers kunnen globale verslagtypes aan andere werkruimten toevoegen zij leiden.

* **Verbonden verslagtypes**: De gebruikers kunnen met dit verslagtype van andere werkruimten verbinden.

In dit artikel vindt u een overzicht van recordtypen tussen werkruimten. Voor informatie over het bepalen van de mogelijkheden van de dwars-werkruimte van een verslagtype, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

## Overzicht van algemene recordtypen

Algemene recordtypen kunnen vanuit een centrale of primaire werkruimte in Workfront Planning aan meerdere werkruimten worden toegevoegd.

Wanneer het uitvoeren van de Planning van Workfront voor een multi-teamorganisatie met gemeenschappelijke werkschema&#39;s, zou u een samenhangende structuur en meta-gegevens voor zeer belangrijke verslagtypes (zoals Campagnes of Deliverables) kunnen moeten bepalen die aan de werkruimten van elk team kunnen worden toegevoegd om hun werk te vangen en te beheren.

U zou het werk van elk team ook kunnen nodig hebben om tot een centraal niveau te rollen.

In zo&#39;n werkschema, kunt u ervoor zorgen dat de teams hun werk constant vangen terwijl het ontgrendelen van dwars-teamzicht, zonder de behoefte om alles aan één werkruimte, of iedereen in de organisatie aan elke werkruimte toe te voegen. Hiervoor kunt u algemene recordtypen gebruiken.

Ga als volgt te werk om algemene recordtypen te gebruiken:

1. Van een werkruimte u beheert, vorm een verslagtype om globaal te zijn.

   Een werkruimtemanager kan toestemmingen aan gebruikers met een Standaardvergunning, of teams, groepen, rollen, en bedrijven geven om een gekozen verslagtype aan een werkruimten toe te voegen zij leiden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte, maar wordt in andere werkruimten weergegeven.

   Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Voeg een recordtype aan een secundaire werkruimte van bestaande toe die als globaal verslagtype is gevormd.

   Het recordtype bestaat in de volgende werkruimten:

   * Zijn originele werkruimte waar het als globaal verslagtype werd aangewezen.
   * Een secundaire werkruimte.

   Voor informatie, zie [ bestaande verslagtypes van een andere werkruimte ](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md) toevoegen.

   De volgende secties beschrijven overwegingen over globale verslagtypes en hoe zij in of hun originele of secundaire werkruimten functioneren.

### Overwegingen over de algemene recordtypen in hun oorspronkelijke primaire werkruimte

Het recordtype dat globaal wordt geconfigureerd, heeft de volgende eigenschappen:

* Alle gegevens (weergave, oorspronkelijke velden) kunnen alleen worden bewerkt in de oorspronkelijke werkruimte.

* U kunt de volgende handelingen uitvoeren op het algemene recordtype vanuit de oorspronkelijke werkruimte:

   * Bewerk het

     Het bewerken van een algemeen recordtype omvat het bewerken van de weergave, de mogelijkheden van de werkruimte en alle velden die in de oorspronkelijke werkruimte zijn gemaakt.
   * Delen

     Wanneer u een recordtype deelt, worden gebruikers aan de werkruimte toegevoegd en worden de records ook met die gebruikers gedeeld.
   * Verwijderen

     U kunt een globaal recordtype van zijn originele werkruimte slechts schrappen nadat u alle instanties van als van alle secundaire werkruimten schrapt waar het werd toegevoegd.

     Voor meer informatie, zie [ verslagtypes van de Schrapping ](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Maakt het van andere werkruimten aansluit
   * Aanvraagformulieren maken en beheren
   * Automatisering maken en beheren

* De volgende records worden weergegeven in de primaire werkruimte van een algemeen recordtype:

   * Records die zijn toegevoegd van het algemene recordtype in de primaire werkruimte
   * Records die zijn toegevoegd van algemene recordtypen in de secundaire werkruimten waar deze zijn toegevoegd

     De verslagen die u van een secundaire werkruimte toevoegt rollen omhoog en tonen in de primaire werkruimte. Alle leden van de originele primaire werkruimte krijgen de toestemmingen van de Mening aan hen en de verslagen zijn zichtbaar aan hen slechts van de Primaire werkruimte, zelfs wanneer zij geen toestemmingen aan de secundaire werkruimte hebben.
* De volgende scenario&#39;s bestaan voor welk soort toestemmingen u aan de verslagen hebt die in de primaire werkruimte worden getoond, afhankelijk van waar zij van werden toegevoegd:

   * U hebt dezelfde machtigingen voor de records die in de primaire werkruimte zijn gemaakt als voor de werkruimte en het oorspronkelijke algemene recordtype.
   * U hebt de zelfde toestemmingen aan de verslagen in een secundaire werkruimte worden gecreeerd aangezien u aan de secundaire werkruimte en aan het globale verslagtype in die ruimte moet.

<!--Removed this as this was too confusing: 

* When the original global record type is added to multiple secondary workspaces, users gain the following visibility to the records added to the global record types: 

    * Members of the original workspace automatically gain View permissions to all records added from any workspace, even if they are  not members of those workspaces. They can view these records in the following workspaces, only if they are a member of these following workspaces: 
        * The primary workspace
        * The secondary workspace where the records were added. Secondary workspace members can view only records from workspaces where they are a member.-->

* De recordtypen die zijn verbonden met een algemeen recordtype, worden beschikbaar voor verbinding vanuit de werkruimten waar dit recordtype wordt toegevoegd.

  Bijvoorbeeld, als u een globaal verslagtype van de Campagne hebt dat een verbinding met een type van het verslag van Gebieden heeft, en u het type van het verslag van de Campagne aan een secundaire werkruimte toevoegt, zullen de Gebieden dwars-werkruimte verbindbaar van de secundaire werkruimte worden. De leden van de secundaire werkruimte kunnen nu campagnes maken en deze koppelen aan gebieden.

* Velden die in de oorspronkelijke werkruimte voor een algemeen recordtype zijn gemaakt, zijn zichtbaar in alle werkruimten waar het recordtype is toegevoegd.

  U kunt de veldinstellingen alleen vanuit de oorspronkelijke werkruimte bewerken.

  De montages van de gebieden die in de originele werkruimte worden gecreeerd zijn read-only in de secundaire werkruimten voor alle leden, ongeacht hun toestemmingen op de secundaire werkruimte.

  Secundaire werkruimtemanagers kunnen de veldinstellingen niet wijzigen voor velden die zijn geconfigureerd in de oorspronkelijke werkruimte. Alleen de werkruimtebeheerders van de oorspronkelijke werkruimte kunnen de veldinstellingen in de oorspronkelijke werkruimte wijzigen.

### Overwegingen over globale verslagtypes in een secundaire werkruimte

* Secundaire werkruimtegangers krijgen Contribute-toestemming voor het algemene recordtype in de werkruimte van hun team. Zij kunnen verslagen in het van de secundaire werkruimte toevoegen en beheren.

* Secundaire werkruimtevieken krijgen Weergavemachtiging voor het algemene recordtype in de werkruimte van hun team. Ze kunnen er geen records in toevoegen en beheren.

* Secundaire werkruimtemanagers kunnen de volgende extra acties op het verslagtype uitvoeren dat van een globaal verslagtype in een secundaire werkruimte wordt toegevoegd:

   * Verwijder het bestand.

     Als u het recordtype uit een secundaire werkruimte verwijdert, wordt dit alleen verwijderd uit de secundaire werkruimte. De records en velden die er vanuit de secundaire werkruimte aan worden toegevoegd, worden ook verwijderd uit de secundaire ruimte. De records die in de secundaire ruimte worden toegevoegd, blijven in de primaire werkruimte. Hierdoor wordt het recordtype niet verwijderd uit de oorspronkelijke werkruimte of uit andere secundaire werkruimten waar het is toegevoegd.

     Voor meer informatie, zie [ verslagtypes van de Schrapping ](/help/quicksilver/planning/architecture/delete-record-types.md).

   * Delen

     Door een globaal recordtype in een secundaire werkruimte te delen, komt het volgende ook voor:

      * Gebruikers worden met weergavemachtigingen toegevoegd aan de werkruimte.
      * De gebruikers ontvangen de zelfde toestemmingen aan alle verslagen van het globale verslagtype in de secundaire werkruimte.
   * Deel de weergaven van de recordtypen.

     U kunt een mening niet openbaar van een globaal verslagtype in een secundaire werkruimte delen. U kunt weergaven alleen intern delen vanuit een secundaire werkruimte. U kunt een weergave intern en openbaar delen voor een algemeen recordtype in de oorspronkelijke werkruimte.

     Voor informatie, zie [ meningen van het Aandeel ](/help/quicksilver/planning/access/share-views.md).


<!--when they will be able to add fields to the secondary space, this bullet will need this extra information: 
    After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added.-->

<!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
* Add new fields
    Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
* Add request forms to it
* Add automations to it-->

* Geen enkele gebruiker kan de volgende handelingen uitvoeren op een algemeen recordtype in een secundaire werkruimte:

   * Bewerk het

     U kunt de weergave, de mogelijkheden van de werkruimte of de toegevoegde velden niet bewerken vanuit de oorspronkelijke werkruimte.
   * Aanvraagformulieren maken en beheren
   * Automatisering maken en beheren

* De verslagen die in een secundaire werkruimte worden toegevoegd zijn zichtbaar van de volgende werkruimten, wanneer u Mening of hogere toestemmingen aan deze werkruimten hebt:

   * De secundaire plaats waar ze zijn toegevoegd
   * De oorspronkelijke primaire werkruimte van het algemene recordtype

* De volgende scenario&#39;s bestaan voor de toegang tot van verslagen die in secundaire werkruimten werden gecreeerd:

   * Als u beheermachtigingen hebt voor de oorspronkelijke werkruimte en geen machtigingen voor een secundaire werkruimte, kunt u records weergeven die zijn toegevoegd vanuit de secundaire werkruimten in de oorspronkelijke werkruimte, maar kunt u deze records niet vanuit de oorspronkelijke werkruimte beheren.
   * Als u beheerdersmachtigingen hebt voor het origineel en de secundaire werkruimten, kunt u de records beheren vanuit de oorspronkelijke werkruimte van het algemene recordtype en vanuit de secundaire werkruimte waar ze zijn toegevoegd.
     <!--not anymore: * You can view the records in additional secondary workspaces where the global record type is added only if you have View permissions to those workspaces-->
* U kunt geen meningen van een globaal verslagtype in een secundaire werkruimte openbaar delen.

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

   Een werkruimtemanager kan selecteren met welke werkruimten een bepaald recordtype beschikbaar is om te verbinden.

   Het oorspronkelijke recordtype bestaat in de oorspronkelijke werkruimte en kan toegankelijk zijn om verbinding te maken met een andere werkruimte.

   Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Verbind met een verslagtype dat als aansluit van een andere werkruimte wordt aangewezen u beheert.

   Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
