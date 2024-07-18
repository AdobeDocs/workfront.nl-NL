---
title: De kalenderweergave beheren
description: U kunt records en de bijbehorende velden weergeven in een kalenderweergave.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# De kalenderweergave beheren

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

U kunt records en de bijbehorende velden weergeven in een kalenderweergave, vanaf de pagina met recordtypen.

Voor informatie over de meningen van de Planning van Adobe Workfront en hoe te om hen te beheren, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven in de vroege toegangsfase voor Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> Er zijn geen toegangscontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren voor een weergave</p>  
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> <p>Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een kalenderweergave beheren {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Overweeg het volgende:

* U kunt alleen een kalenderweergave maken wanneer u ten minste twee datumvelden hebt die zijn gekoppeld aan een recordtype. Wanneer u een of geen datumvelden hebt gekoppeld aan een recordtype, wordt de optie voor de kalenderweergave grijs weergegeven.

  U kunt uit de gebieden van de verslagdatum, of raadplegingsdatumgebieden van verbonden verslag of objecten types selecteren.
* De volgende scenario&#39;s bestaan:

   * Wanneer zowel de begin- als einddatum geen waarden hebben, worden de records niet weergegeven in de kalender
   * Als de begin- of einddatum geen waarde hebben, wordt de record weergegeven als een eendaagse gebeurtenis
   * Wanneer de begindatum na de einddatum ligt, wordt de record niet weergegeven in de kalender.

Een kalenderweergave beheren:

1. Ga naar de recordtypepagina waarvoor u de kalender wilt bekijken.
1. Creeer een kalendermening, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden in een kalender weergegeven als balken. De kleur van de balken komt overeen met de kleur van het recordpictogram.

1. Voer een van de volgende handelingen uit om door de kalender te navigeren:

   * Klik op de pictogrammen links en rechts of gebruik de horizontale schuifbalk om naar voren en naar achteren in de kalender te gaan.
   * Klik **vandaag** om de kalender aan de datum van vandaag te centreren.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor de tijd om de tijdstappen bij te werken:

      * Maand
1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [ Filters ](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Filters toevoegen

U kunt de hoeveelheid informatie die op het scherm wordt weergegeven verminderen door filters te gebruiken.

Houd rekening met het volgende wanneer u werkt met filters in de kalenderweergave:

<!-- this list is almost identical to the one for the table view - update both-->

* De filters die u voor een kalenderweergave maakt, werken onafhankelijk van de filters in een andere weergave die op hetzelfde recordtype is toegepast.

* De filters zijn uniek voor de weergave die u selecteert. Op twee kalenderweergaven van hetzelfde recordtype kunnen verschillende filters worden toegepast.

* Twee gebruikers die naar dezelfde kalenderweergave kijken, zien hetzelfde filter dat op dat moment wordt toegepast.

* U kunt de filters die u maakt voor een kalenderweergave niet een naam geven.

* Als u filters verwijdert, worden deze verwijderd van iedereen die hetzelfde recordtype als u benadert en die dezelfde weergave als u weergeeft.

* Het toevoegen van filters in de kalenderweergave is hetzelfde als het toevoegen van filters in de tabelweergave.

  Voor meer informatie, zie &quot;filters&quot;sectie in artikel [ toevoegen de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) leidt.

* U kunt filteren op gekoppelde recordvelden of opzoekvelden.

* U kunt filteren door velden op te zoeken waarin meerdere waarden worden weergegeven.
