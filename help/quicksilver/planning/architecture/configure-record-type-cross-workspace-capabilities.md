---
title: Mogelijkheden tussen werkruimten configureren voor recordtype
description: U kunt instellen dat een recordtype wordt toegevoegd aan een andere werkruimte of dat het wordt verbonden met een andere werkruimte.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Mogelijkheden tussen werkruimten configureren voor recordtypen

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt recordtypen configureren om te werken in meerdere werkruimten.

Hieronder vindt u de mogelijkheden van recordtypen tussen werkruimten:

* U kunt een recordtype instellen als gecentraliseerd. Gebruikers kunnen gecentraliseerde recordtypen toevoegen aan andere werkruimten die zij kunnen beheren.
* U kunt een recordtype aanwijzen als een aanpasbare record. Gebruikers kunnen vanuit andere werkruimten verbinding maken met dit recordtype.

U moet eerst de mogelijkheden voor de werkruimte van een recordtype definiëren voordat werkruimtemanagers deze kunnen verbinden vanuit of toevoegen aan andere werkruimten.

U definieert de mogelijkheden voor de werkruimte van een recordtype wanneer u een recordtype maakt of bewerkt.

Zie een van de volgende artikelen voor meer informatie:

* [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)
* [Recordtypen bewerken](/help/quicksilver/planning/architecture/edit-record-types.md)

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul><li><p>Willekeurig Workfront-pakket</p></li>
<p>en</p>
<li><p>Willekeurig planningspakket om verbindingbare recordtypen te maken</p></li>
<li><p>Planning Plus-pakket om gecentraliseerde recordtypen te maken</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningspakket wordt opgenomen. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Gecentraliseerde recordtypen configureren

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

Als werkruimtemanager, kunt u een verslagtype vormen om een gecentraliseerd verslagtype te zijn. Een gecentraliseerd recordtype kan aan andere werkruimten worden toegevoegd.

Een werkruimtemanager kan een gecentraliseerd recordtype toevoegen aan een werkruimte die zij beheren. De oorspronkelijke velden van het recordtype worden ook toegevoegd.

Gebruikers kunnen records toevoegen aan een gecentraliseerd recordtype vanuit elke werkruimte die zij met Contribute-machtigingen hebben en waarin het gecentraliseerde recordtype is toegevoegd, inclusief de oorspronkelijke werkruimte. Zij kunnen verslagen van werkruimte bekijken zij slechts toestemmingen van de Mening hebben aan.

Voor meer informatie, zie [ overzicht van de types van het werkruimterecord over de werkruimte ](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Een recordtype als gecentraliseerd configureren:

{{step1-to-planning}}

1. Klik de werkruimte waarvan verslagtypes u als gecentraliseerd wilt vormen.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype.
1. Klik **uitgeven**.

   ![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >Als een recordtype al als een gecentraliseerd recordtype is aangewezen en het aan andere werkruimten is toegevoegd, wordt de Edit optie verduisterd.

1. In **geef verslagtype** doos uit, klik de **Geavanceerde montages** tabel.
1. Laat **toe toestaan toevoegend dit verslagtype aan andere werkruimten** plaatsen.

   ![ geef recordtype Geavanceerde montages met toe voegen aan andere werkruimten laat ](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png) toe

   >[!TIP]
   >
   >Nadat u een gecentraliseerd recordtype aan een andere werkruimte hebt toegevoegd, kan deze instelling niet meer worden uitgeschakeld.

1. In **Uitgezocht die dit verslagtype aan werkruimten kan toevoegen die zij** gebied beheren, voeg entiteiten toe die u wilt toestaan om dit verslagtype aan werkruimten toe te voegen die zij beheren.

   Uw naam wordt automatisch toegevoegd aan het veld.

   U kunt individuele gebruikers, of groepen, teams, baanrollen, of bedrijven toevoegen de waarvan gebruikers u wilt toestaan om dit verslagtype aan de werkruimten toe te voegen zij leiden.

   U moet minstens één entiteit (gebruiker, team, groep, rol, of bedrijf) aanwijzen om deze het plaatsen kunnen toelaten.

   U kunt dit veld bewerken nadat u het recordtype hebt opgeslagen.

1. (Facultatief) verwijder uw naam uit **Uitgezocht die dit verslagtype aan werkruimten kan toevoegen zij** gebied beheren.

1. Klik **sparen**.

   De volgende dingen doen zich voor:

   * Het recordtype en de bijbehorende velden kunnen nu door de door u opgegeven personen worden toegevoegd aan een andere werkruimte.

   >[!NOTE]
   >
   >U kunt de weergave en de instellingen van het recordtype en de oorspronkelijke velden alleen vanuit de oorspronkelijke werkruimte bewerken.

   * De kaart van het verslagtype toont een gecentraliseerd pictogram ![ Gecentraliseerd verslagtype pictogram ](assets/global-icon.png) om erop te wijzen dat het verslagtype beschikbaar is om aan andere werkruimten worden toegevoegd.
   * Een systeem-geproduceerd **Workspace** gebied wordt toegevoegd aan de lijstmening van het verslagtype en zijn verslagen&#39; details.

     In het Workspace-veld wordt de werkruimte weergegeven van waaruit elke record is gemaakt.

     Dit veld is alleen-lezen en kan niet worden verwijderd.
1. (Optioneel) Ga naar een andere werkruimte en maak een recordtype met een bestaand recordtype. Selecteer het recordtype dat u in de bovenstaande stappen hebt ingeschakeld.

   Voor informatie, zie [ bestaande verslagtypes van een andere werkruimte ](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md) toevoegen.

## Verbindbare recordtypen configureren

<!--this is a UI term; don't change the title of this section-->

U kunt een recordtype configureren waarmee verbinding wordt gemaakt vanuit andere werkruimten wanneer u het recordtype maakt of bewerkt.

Om een verslagtype te vormen om met van andere werkruimten te verbinden wanneer u het verslagtype uitgeeft:

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **uitgeven**
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype, dan klik **uitgeven**.

   ![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card.png)

1. In **geef verslagtype** doos uit, klik de **Geavanceerde montages** tabel.
1. Laat **toe toestaan verbindend met dit verslagtype in andere werkruimten** plaatsen. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![ geef recordtype Geavanceerde montages tabel met verbinding van andere toegelaten werkruimten uit ](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Als deze optie is ingeschakeld, is het recordtype toegankelijk en kan het via andere werkruimten worden verbonden.

1. Kies van welke werkruimten het recordtype kan worden betreden. Kies een van de volgende opties:

   * **Systeem wijd**: De gebruikers kunnen met dit verslagtype van alle werkruimten verbinden waar zij beheertoestemmingen hebben.
   * **Specifieke werkruimten**: Voeg de namen van de werkruimten toe waar de werkruimtemanagers met dit verslagtype kunnen verbinden.
1. Klik **sparen**.

   De volgende dingen doen zich voor:

   * Het recordtype en de bijbehorende velden zijn nu beschikbaar om verbinding te maken met de werkruimten die u hebt toegewezen.
   * De kaart van het verslagtype toont een pictogram van de dwars-werkruimteverbinding ![ het verbindingspictogram van de werkruimteverbinding ](assets/connect-from-other-workspaces-icon.png) om erop te wijzen dat het verslagtype beschikbaar is om met van om het even welke werkruimte te worden verbonden u in uw configuratie hebt aangewezen.

   Het recordtype wordt beschikbaar voor verbinding met de opgegeven werkruimten.
1. (Optioneel) Ga naar een andere werkruimte en voeg een verbinding toe aan het recordtype dat u in de bovenstaande stappen hebt ingeschakeld voor verbindingsbaarheid tussen werkruimten.

   Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).









