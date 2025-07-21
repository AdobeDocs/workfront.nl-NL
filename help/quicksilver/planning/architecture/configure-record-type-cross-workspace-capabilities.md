---
title: Mogelijkheden tussen werkruimten configureren voor recordtype
description: U kunt instellen dat een recordtype wordt toegevoegd aan een andere werkruimte of dat het wordt verbonden met een andere werkruimte.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# Mogelijkheden tussen werkruimten configureren voor recordtypen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt een recordtype toewijzen dat aan een andere werkruimte moet worden toegevoegd of dat via een andere werkruimte moet worden verbonden, in Adobe Workfront Planning.

U moet eerst de mogelijkheden voor de werkruimte van een recordtype definiëren voordat werkruimtemanagers deze kunnen verbinden vanuit of importeren in andere werkruimten.

U definieert de mogelijkheden voor de werkruimte van een recordtype wanneer u een recordtype maakt of bewerkt.

Zie een van de volgende artikelen voor meer informatie:

* [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)
* [Recordtypen bewerken](/help/quicksilver/planning/architecture/edit-record-types.md)

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configureer het toevoegen van een recordtype aan andere werkruimten

Als werkruimtemanager kunt u een recordtype configureren dat aan andere werkruimten wordt toegevoegd wanneer u een recordtype maakt of bewerkt.

Wanneer u het toevoegen van een recordtype aan andere werkruimten configureert, kan een werkruimtenmanager het recordtype en al zijn informatie in één van de werkruimten invoeren die zij leiden.

U kunt als volgt het toevoegen van een recordtype aan een andere werkruimte configureren wanneer u het recordtype bewerkt:

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype
of
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype.
1. Klik **uitgeven**.

   ![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card.png)

1. In **geef verslagtype** doos uit, selecteer de **Geavanceerde montages** tabel.
1. Laat **toe toestaan toevoegend dit verslagtype aan andere werkruimten** plaatsen.

   ![ geef recordtype Geavanceerde montages met toe voegen aan andere werkruimten laat ](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png) toe

1. In **Uitgezocht die dit verslagtype aan werkruimten kan toevoegen die zij** gebied beheren, voeg gebruikers toe die u wilt toestaan om dit verslagtype aan werkruimten toe te voegen die zij beheren.

   Uw naam wordt automatisch toegevoegd aan het veld.

   U kunt individuele gebruikers, of groepen, teams, baanrollen, of bedrijven toevoegen de waarvan gebruikers u wilt toestaan om dit verslagtype aan de werkruimten toe te voegen zij leiden.

   U kunt dit veld bewerken nadat u het recordtype hebt opgeslagen.
1. (Facultatief) verwijder uw naam uit **Uitgezocht die dit verslagtype aan werkruimten kan toevoegen zij** gebied beheren.

1. Klik **sparen**.

   De volgende dingen doen zich voor:

   * Het recordtype en de bijbehorende velden kunnen nu door de door u opgegeven personen worden toegevoegd aan een andere werkruimte.

   >[!NOTE]
   >
   >U kunt het recordtype en de bijbehorende velden alleen vanuit de oorspronkelijke werkruimte bewerken.

   * De kaart van het verslagtype toont een globaal pictogram ![ Globaal verslagtype pictogram ](assets/global-icon.png) om erop te wijzen dat het verslagtype beschikbaar is om aan om het even welke werkruimte worden toegevoegd de waarvan manager u in uw configuratie specificeerde.
   * Een systeem-geproduceerd **Workspace** gebied wordt toegevoegd aan het verslagtype.

     In het Workspace-veld wordt de werkruimte weergegeven van waaruit elke record is gemaakt.

     Dit veld is alleen-lezen en kan niet worden verwijderd.

## Verbinding maken met een recordtype vanuit andere werkruimten configureren

U kunt een recordtype configureren waarmee verbinding wordt gemaakt vanuit andere werkruimten wanneer u het recordtype maakt of bewerkt.

Om een verslagtype te vormen om met van andere werkruimten te verbinden wanneer u het verslagtype uitgeeft:

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **uitgeven**
of
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype, dan klik **uitgeven**.

   ![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card.png)

1. In **geef verslagtype** doos uit, selecteer de **Geavanceerde montages** tabel.
1. Laat **toe toestaan verbindend met dit verslagtype in andere werkruimten** plaatsen. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![ geef recordtype Geavanceerde montages tabel met verbinding van andere toegelaten werkruimten uit ](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Als deze optie is ingeschakeld, is het recordtype toegankelijk en kan het via andere werkruimten worden verbonden.

1. Kies van welke werkruimten het recordtype kan worden betreden. Kies een van de volgende opties:

   * **Systeem wijd**: De gebruikers kunnen met dit verslagtype van alle werkruimten verbinden waar zij toestemmingen beheren.
   * **Specifieke werkruimten**: Voeg de namen van de werkruimten toe waar de werkruimtemanagers met dit verslagtype kunnen verbinden.
1. Klik **uitgeven**.

   De volgende dingen doen zich voor:

   * Het recordtype en de bijbehorende velden zijn nu beschikbaar om verbinding te maken met de werkruimten die u hebt toegewezen.
   * De kaart van het verslagtype toont een pictogram van de dwars-werkruimteverbinding ![ het verbindingspictogram van de werkruimteverbinding ](assets/connect-from-other-workspaces-icon.png) om erop te wijzen dat het verslagtype beschikbaar is om van om het even welke werkruimte te worden verbonden u in uw configuratie hebt aangewezen.

   Het recordtype wordt beschikbaar om verbinding te maken vanuit de opgegeven werkruimten.









