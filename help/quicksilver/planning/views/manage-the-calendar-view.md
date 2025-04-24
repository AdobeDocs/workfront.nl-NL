---
title: De kalenderweergave beheren
description: U kunt records en de bijbehorende velden weergeven in een kalenderweergave. In dit artikel wordt beschreven hoe u een kalenderweergave kunt maken en een bestaande weergave kunt bewerken of verwijderen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: f171db8474df703fddbf63a673f9bfbd2ab2db27
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# De kalenderweergave beheren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->

{{planning-important-intro}}

U kunt records en de bijbehorende velden weergeven in een kalenderweergave, vanaf de pagina met recordtypen.

Voor informatie over de meningen van de Planning van Adobe Workfront en hoe te om hen te beheren, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

## Toegangsvereisten

+++ Breid uit om toegangsvereisten te bekijken..

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
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

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

   ![ de meningsvoorbeeld van de Kalender ](assets/calendar-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden in een kalender weergegeven als balken. De kleur van de balken komt overeen met de kleur van het recordpictogram.

1. Voer een van de volgende handelingen uit om door de kalender te navigeren:

   * Klik op de pictogrammen links en rechts of gebruik de horizontale schuifbalk om naar voren en naar achteren in de kalender te gaan.
   * Klik **vandaag** om de kalender aan de datum van vandaag te centreren.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor de tijd om de tijdstappen bij te werken:

      * **Maand**: De vertoningen van verslagen in een maandelijkse kalender.


      * **Week**: De vertoning van verslagen op de volgende gebieden:

         * Records die zich uitstrekken over meerdere dagen worden boven aan de kalender weergegeven.
         * Records die een dag of minder duren, worden weergegeven in de onderste helft van de kalenderweergave. Als u hebt opgegeven dat u het uur van de begin- en einddatum wilt weergeven, wordt de record op het juiste tijdstip weergegeven binnen de dag dat deze plaatsvindt.


1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [Filters](#add-filters)
   * [ Montages ](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
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

### De instellingen van de kalenderweergave bewerken

Het bewerken van de instellingen van de kalenderweergave is vergelijkbaar met het bewerken van de instellingen van een tijdlijnweergave.

Voor meer informatie, zie &quot;uitgeven de sectie van de chronologiemening&quot;in artikel [ de chronologiemening ](/help/quicksilver/planning/views/manage-the-timeline-view.md) beheert.
