---
title: Recordweergaven beheren
description: U kunt records in een tabel-, tijdlijn- of kalenderweergave weergeven wanneer u Adobe Workfront-planning gebruikt. In dit artikel wordt beschreven hoe u een weergave kunt maken en een bestaande weergave kunt bewerken of verwijderen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 0d968a3f398c2e7dc4154cd5a16acf35ca7c86f5
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 0%

---


# Recordweergaven beheren

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


{{planning-important-intro}}

Nadat u een recordtype hebt geselecteerd in het gedeelte Adobe Workfront Planning, kunt u alle records van dat type weergeven in de volgende weergaven:

* Tabel

  Voor meer informatie, zie [ de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

* Tijdlijn

  Voor meer informatie, zie [ de chronologiemening ](/help/quicksilver/planning/views/manage-the-timeline-view.md) leiden.

* Kalender

  Voor meer informatie, zie [ de kalendermening ](/help/quicksilver/planning/views/manage-the-calendar-view.md) leiden.

In dit artikel wordt de volgende informatie over recordweergaven beschreven:

* [ creeer en geef een mening ](#create-or-edit-record-views) uit
* [Een weergave verwijderen](#delete-views)
* [Een weergave dupliceren](#duplicate-a-view)
* [ laat de aanwezigheidsindicatoren in real time in een mening toe ](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard </p>
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
   <td>   <p>Rechten beheren voor een weergave</p>  
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen of te dupliceren</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>In het milieu van de Productie, moeten alle gebruikers met inbegrip van de Beheerders van het Systeem aan een lay-outmalplaatje worden toegewezen dat Planning omvat.</p>
<p><span class="preview">In het milieu van de Voorproef, hebben de Standaardgebruikers en de Beheerders van het Systeem Planning die door gebrek wordt toegelaten.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het werken met recordweergaven

* Weergaven in Workfront Planning zijn specifiek voor records. U kunt niet dezelfde weergave toepassen op twee verschillende recordtypen.
* Weergaven die u maakt, zijn alleen zichtbaar voor u en gebruikers met wie u de weergaven deelt.
* Wanneer u een weergave wijzigt of verwijdert, wordt deze gewijzigd en verwijderd voor alle gebruikers die machtigingen hebben voor de weergave.
* Elke gebruiker kan maximaal 100 weergaven maken. U kunt meer dan 100 weergaven weergeven voor een recordtype, maar één gebruiker kan slechts 100 weergaven maken.
* U kunt weergaven die u maakt met anderen delen. Voor informatie, zie [ meningen van het Aandeel ](/help/quicksilver/planning/access/share-views.md).
* De volgende elementen zijn uniek voor elke recordweergave:

   * Filter
   * Groepering
   * Sorteren
   * De vormgeving van de balk (voor de tijdlijnweergave)

  <!-- some of these are not available in all of the views - edit above-->

  Wanneer u bijvoorbeeld een filter maakt in een tabelweergave, zijn de filterresultaten alleen zichtbaar in de geselecteerde weergave en niet in alle weergaven die aan het recordtype zijn gekoppeld.

  >[!NOTE]
  >
  > Sommige weergave-elementen zijn mogelijk niet voor alle weergaven beschikbaar.


## Gelijksoortigheid en verschillen tussen recordweergaven

In de volgende tabel worden de overeenkomsten en verschillen tussen de tabel-, tijdlijn- en kalenderweergave weergegeven:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Functie | Tabelweergave | Tijdlijnweergave | Kalenderweergave |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Records in een lijst of tabel weergeven | ✓ |              | |
| Alle velden standaard weergeven als kolommen in de tabel | ✓ |              |    |
| Velden (of kolommen) verbergen of weergeven | ✓ |               |    |
| Veldwaarden bewerken voor elke record | ✓ |               |             |
| Records toevoegen als nieuwe rijen in de weergave | ✓ |               |        |
| Velden toevoegen als nieuwe kolommen in de weergave | ✓ |               |         |
| Rijen kopiëren uit een externe lijst en deze in een tabel plakken | ✓ |               |          |
| Records in een tijdlijn weergeven |            | ✓ |             |
| Filterrecords | ✓ | ✓ | ✓ |
| Records weergeven op een kalender |           |              | ✓ |
| Groepsrecords | ✓ | ✓ |
| Records sorteren | ✓ |              |
| Kleurcoderecords |           | ✓ | ✓ |
| Kleurcodegroepen |           | ✓ |
| Specifieke records zoeken | ✓ | ✓ |
| De weergave delen met anderen | ✓ | ✓ | ✓ |
| De recordpagina openen vanuit de weergave | ✓ | ✓ |    |
| Records weergeven per jaar en kwartaal |           | ✓ |    |
| Records weergeven per maand |           | ✓ | ✓ |
| Records per week weergeven |           |               | ✓ |


## Weergaven maken of bewerken {#create-or-edit-views}

{{step1-to-planning}}


1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Klik op **+ Weergave** om een nieuwe weergave toe te voegen.
1. Selecteer een van de volgende typen weergaven:

   * Tabel
   * Tijdlijn
   * Kalender

   Er wordt een nieuw tabblad gemaakt met de geselecteerde weergave.

   Afhankelijk van de breedte van uw scherm, zouden de extra meningen in **Meer** menu ![ Meer menu ](assets/more-menu.png) kunnen tonen.


>[!TIP]
>
>Wanneer u een recordtype maakt, wordt de tabelweergave ook standaard gemaakt.
>
>Als u een tijdlijn of een kalenderweergave wilt maken, moet het recordtype waarvoor u de weergave maakt, ten minste twee datumvelden hebben.
>
>Anders worden de opties Tijdlijn en Kalender grijs weergegeven.
>

![ de types van Mening drop-down van verslagtype lijst ](assets/view-types-drop-down-from-record-type-list.png)

1. (Voorwaardelijk) klik **daarna**, wanneer het creëren van een chronologie of een kalendermening.

   Standaard geeft Workfront de weergave een van de volgende namen:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Het getal is een automatisch gegenereerde toename.

1. (Voorwaardelijk) selecteer het **Begin** en **Eind data** voor de verslagen die in de chronologie of kalendermening zullen tonen.

   >[!TIP]
   >
   >    U kunt uit de gebieden van de verslagdatum, of raadplegingsdatumgebieden van verbonden verslag of objecten types selecteren. U moet aggregators voor datumgebieden (MAX of MIN) gebruiken wanneer u raadplegingsgebieden als Begin en Eind data voor de chronologie en kalendermeningen selecteert. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klik **creëren**.

   De weergave wordt weergegeven als een nieuw tabblad. De weergaven worden in chronologische volgorde weergegeven vanaf het moment waarop ze zijn gemaakt of met u zijn gedeeld.
1. (Facultatief) klik **Meer** menu ![ meer inlasteken neer pictogrammeningen ](assets/more-caret-down-icon-views.png) naast de laatste mening om alle meningen voor het geselecteerde verslagtype te tonen.

   De extra meningsvertoning onder **Meer** menu na het laatste meningslusje. Het aantal naast **meer** menu toont het aantal extra meningen.
1. (Facultatief) om een mening anders te noemen nadat het wordt gecreeerd, klik het meningsdrop-down menu, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) > **anders noemen** om de meningsnaam bij te werken

   of

   Dubbelklik op de weergavenaam en typ de nieuwe naam.  <!--ensure there is not another saving step here?!-->

1. (Optioneel) Raadpleeg de volgende artikelen voor informatie over het beheren van een bepaald weergavetype:

   * [De tabelweergave beheren](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [De tijdlijnweergave beheren](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [De kalenderweergave beheren](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## Weergaven verwijderen

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Beweeg over één van de namen van de mening in het meningslusje, dan klik **Meer** ![ Meer menu ](assets/more-menu.png) links van de meningsnaam, dan klik **Schrapping**.
Eerst, zou u **Meer** aan de linkerzijde van het laatste lusje kunnen moeten klikken om de mening te vinden u wilt schrappen.

1. Klik **Schrapping** om te bevestigen. <!--ensure there is not another saving step here?!-->

   De weergave wordt verwijderd voor alle gebruikers die toegang hebben tot het recordgebied en kan niet worden hersteld.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Een weergave dupliceren

Als u meerdere versies van een weergave wilt behouden en kleine wijzigingen wilt aanbrengen tussen de versies, kunt u een weergave dupliceren.

Als u een weergave dupliceert, worden identieke kopieën van een bestaande weergave gemaakt.

De machtigingen voor delen van de oorspronkelijke weergave worden niet overgedragen naar de gedupliceerde weergave.

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Beweeg over het lusje van de mening u wilt dupliceren, en **klikken Meer** menu ![ ](assets/more-menu.png) rechts van de meningsnaam, dan **** dupliceert.

   ![ Mening meer menu met dubbele optie ](assets/view-more-menu-with-duplicate-option.png)


   De weergave wordt gedupliceerd en de naam van de nieuwe weergave volgt het volgende patroon: `Original view's name (Copy)` . Het nieuwe meningslusje toont aan het eind van alle meningslusjes.

## De real-time aanwezigheidsindicator in een weergave inschakelen

De avatars van andere gebruikers die recordinformatie uitgeven tezelfdertijd zoals u in de hoger-juiste hoek van alle verslagmeningen toont, door gebrek.

Wanneer u de tabelweergave weergeeft, kunt u ook bekijken welk veld een andere gebruiker bewerkt op het moment dat u de record weergeeft.

1. Ga naar een pagina met recordtypen en open een weergave.
1. (Voorwaardelijk) Als er andere gebruikers zijn die de records van het geselecteerde type tegelijkertijd bewerken, worden hun avatars in de rechterbovenhoek van de weergave weergegeven.
1. Klik het drop-down menu naast avatars, selecteren **samenwerkers** knevel tonen. De schakeloptie is standaard geselecteerd.

   ![ toon geselecteerde samenwerkersknevel ](assets/show-collaborators-toggle-selected.png)

1. (Voorwaardelijk) Open een lijstmening, en het gebied dat een andere persoon actief uitgeeft wordt benadrukt in de kleur die aan de contour van hun avatar in de lijstmening beantwoordt.

   Als de markeerkleur van de avatar grijs is, is de gebruiker meer dan 30 seconden geleden gestopt met het actief bewerken van de record.

   ![ Echte - tijd het gebied van de indicatorlijst en avatar verbinding ](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >U kunt **selecteren toont samenwerkers** knevel van om het even welke mening. Het veld dat momenteel door anderen wordt bewerkt, wordt alleen in de tabelweergave weergegeven.
