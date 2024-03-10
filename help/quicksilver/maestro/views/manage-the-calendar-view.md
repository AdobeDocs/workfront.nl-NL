---
title: De kalenderweergave beheren
description: U kunt records en de bijbehorende velden weergeven in een kalenderweergave.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 26d6fecf02541fff649deabe61e65dbe5ae5f688
workflow-type: tm+mt
source-wordcount: '360'
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

{{maestro-important-intro}}

U kunt records en de bijbehorende velden weergeven in een kalenderweergave, vanaf de pagina met recordtypen.

Ga voor informatie over de planningsmogelijkheden van Adobe Workfront en hoe u deze kunt beheren naar [Recordweergaven beheren](../views/manage-record-views.md).

## Toegangsvereisten

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het gesloten bètaprogramma voor Adobe Workfront-planningsmogelijkheden. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuratie op toegangsniveau</td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de planningsmogelijkheden van Adobe Workfront  </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten voor de weergave beheren</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## Een kalenderweergave beheren {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Overweeg het volgende:

* U kunt alleen een kalenderweergave maken wanneer u ten minste twee datumvelden hebt die zijn gekoppeld aan een recordtype. Wanneer u een of geen datumvelden hebt gekoppeld aan een recordtype, wordt de optie voor de kalenderweergave grijs weergegeven.
* De volgende scenario&#39;s bestaan:

   * Wanneer zowel de begin- als einddatum geen waarden hebben, worden de records niet weergegeven in de kalender
   * Als de begin- of einddatum geen waarde hebben, wordt de record weergegeven als een eendaagse gebeurtenis
   * Wanneer de begindatum na de einddatum ligt, wordt de record niet weergegeven in de kalender.

Een kalenderweergave beheren:

1. Ga naar de recordtypepagina waarvoor u de kalender wilt bekijken.
1. Een kalenderweergave maken, zoals wordt beschreven in het artikel [Recordweergaven beheren](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden in een kalender weergegeven als balken. De kleur van de balken komt overeen met de kleur van het recordpictogram.

1. Voer een van de volgende handelingen uit om door de kalender te navigeren:

   * Klik op de pictogrammen links en rechts of gebruik de horizontale schuifbalk om naar voren en naar achteren in de kalender te gaan.
   * Klikken **Vandaag** om de kalender te centreren op de datum van vandaag.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor de tijd om de tijdstappen bij te werken:

      * Maand