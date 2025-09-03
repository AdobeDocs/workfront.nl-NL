---
title: Overzicht van gecentraliseerde recordtypen
description: De gecentraliseerde verslagtypes kunnen aan veelvoudige werkruimten van een centrale of primaire werkruimte in de Planning van Adobe Workfront worden toegevoegd.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
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

Ook, zou u het werk van elk team kunnen nodig hebben om tot een centraal, meer globaal niveau te rollen.

In deze workflow kunt u ervoor zorgen dat teams hun werk consistent vastleggen en tegelijkertijd de zichtbaarheid van verschillende teams ontgrendelen, zonder dat iedereen in de organisatie aan één werkruimte moet worden toegevoegd.

Ga als volgt te werk om gecentraliseerde recordtypen te gebruiken:

1. Configureer een recordtype dat moet worden gecentraliseerd.

   Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.
1. Voeg een bestaand recordtype van gecentraliseerde toe.

   Voor informatie, zie [ bestaande verslagtypes ](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md) toevoegen.




・ Een nieuwe instelling &quot;Toestaan dat het recordtype in andere werkruimten wordt toegevoegd&quot; is beschikbaar in Geavanceerde instellingen voor recordtypen.

・ Indien toegelaten, kan de werkruimtemanager gebruikers met Standaardvergunning, teams, groepen, rollen, of bedrijven selecteren die het verslagtype in de werkruimten kunnen toevoegen zij leiden.

・ De werkruimtebeheerder die de instelling bewerkt, wordt standaard automatisch toegevoegd aan de lijst met geselecteerde gebruikers

o Werkruimtemanager kan zijn eigen naam verwijderen nadat het minstens 1 andere entiteit heeft toegevoegd

o Er moet ten minste 1 gebruiker/team/... geselecteerd zijn om de instelling op te slaan

o Wanneer het recordtype in ten minste 1 andere werkruimte is toegevoegd, kunnen alle geselecteerde gebruikers worden verwijderd

§ Dit wordt gedaan zodat het mogelijk is om het globale verslagtype in nieuwe werkruimten te verhinderen toe te voegen maar het te houden in werkruimten die het reeds gebruiken.

・ In fase 1 worden alle records van de verbonden recordtypen automatisch gedeeld met elke werkruimte waarin het recordtype is toegevoegd.

・ Als het recordtype is ingeschakeld als een cross-workspace, wordt een door het systeem gegenereerd &quot;Workspace&quot; veld toegevoegd aan het recordtype

o Het toont de werkruimte van waar elke record is gemaakt.

o Dit veld is alleen-lezen en kan niet worden verwijderd.

o Deze kan worden verborgen in weergavevelden.

o Het werkruimteveld kan worden gebruikt voor filteren, groeperen en sorteren, en in alle weergave-instellingen, zoals in andere velden.


Typen records van verschillende Workspace in lokale werkruimten

・ Bij het toevoegen van een nieuw recordtype aan hun werkruimte zien lokale werkruimtemanagers een optie uit de lijst van globale verslagtypes te selecteren die voor hen beschikbaar zijn

・ Wanneer ze een van de algemene recordtypen selecteren, wordt deze direct toegevoegd aan de werkruimte

・ Het is mogelijk het algemene recordtype naar een willekeurige sectie en positie in de lokale werkruimte te verplaatsen


Machtigingen voor het algemene recordtype in lokale werkruimten

Binnen lokale werkruimten winnen de leden na toegang tot het globale verslagtype:

・ In Fase 1 krijgen lokale werkruimtebeheerders Contribute-machtigingen. Dit betekent:

o Lokale werkruimtemanagers kunnen:

§ Voeg het algemene recordtype toe

§ Alle records in het algemene recordtype toevoegen/bewerken/verwijderen, ongeacht de werkruimte waaruit de record is toegevoegd.

§ Verwijder het algemene recordtype uit de lokale werkruimte

o Beheerders van lokale werkruimten kunnen:

§ Velden toevoegen, bewerken, verwijderen

§ De vormgeving en het label van het recordtype bijwerken

§ Zie de geavanceerde instellingen voor het recordtype

§ Automatisering beheren

§ Aanvraagformulieren beheren

§ Het delen van het recordtype aanpassen voor het bereik van de werkruimte

§ Schakel de instelling voor het algemene recordtype uit in de geavanceerde instellingen.

・ Medewerkers in de lokale werkruimte krijgen Contribute-machtiging voor het algemene recordtype en kunnen hierin records toevoegen en beheren

・ Gebruikers in de lokale werkruimte krijgen Weergavemachtiging voor het algemene recordtype

・ Zodra een record vanuit een lokale werkruimte aan het algemene recordtype is toegevoegd, wordt die naam in het Workspace-veld weergegeven

o Op dit moment is het niet mogelijk het werkruimteveld te bewerken en te wijzigen

・ De verslagen die aan lokale werkruimten worden toegevoegd worden allen opgerold en getoond in de primaire werkruimte, en alle leden van de primaire werkruimte krijgen meningstoegang tot het.

・ Records die zijn toegevoegd in lokale werkruimten, worden niet weergegeven in andere lokale werkruimten met hetzelfde algemene recordtype en hun leden krijgen geen toegang tot de records.



Toegang tot verbindingen:

・ MVP-bereik

o De recordtypen die met het algemene recordtype zijn verbonden, worden zichtbaar voor lokale werkruimten waar het algemene recordtype is toegevoegd, zodat zij de verbindingsvelden kunnen gebruiken voor het toevoegen van tags


API-gedrag

Als de gebruiker via API records probeert te maken in een algemeen recordtype zonder de werkruimte-id op te geven, controleert het systeem of de gebruiker toegang heeft om records te maken in de primaire werkruimte (waar een algemeen recordtype wordt gemaakt)

・ Zo ja, dan wordt de record gemaakt in de primaire werkruimte

・ Als dat niet het geval is, krijgt de gebruiker een validatiefout die hij niet kan gebruiken voor de primaire werkruimte en moet hij de werkruimte-id opgeven waar hij toegang heeft om te maken.