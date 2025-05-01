---
title: Records delen
description: U kunt records met anderen delen om de samenwerking te verbeteren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Records delen

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Als u met andere gebruikers wilt samenwerken, kunt u records met anderen delen.

U kunt een Adobe Workfront-planningsrecord op de volgende manieren delen:

* Kopieer de koppeling van de recordpagina vanuit uw browser wanneer de pagina is geopend.

* Kopieer een koppeling naar de pagina van de record wanneer u records bekijkt in de tabelweergave van het recordtype.

* U kunt alle verslagen in een werkruimte met andere gebruikers delen door de werkruimte <span class="preview"> en het verslagtype te delen.</span>

  Zie de volgende artikelen voor meer informatie:

   * [Een werkruimte delen](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [Een recordtype delen](/help/quicksilver/planning/access/share-record-types.md)

  </div>

In dit artikel wordt beschreven hoe u een koppeling naar de pagina van een record kunt kopiëren vanuit de tabelweergave van een recordtype.

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
   <td><p> Medewerker of hogere licentie </p>
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
   <td>  <p>De mening of hogere toestemmingen aan een werkruimte <span class="preview"> en verslagtype </span> om te delen   een record met behulp van een koppeling </p>
   <p>Beheer toestemmingen aan een werkruimte <span class="preview"> en verslagtype </span> om de verslagen in de werkruimte te delen </p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>In het milieu van de Productie, moeten alle gebruikers met inbegrip van de beheerders van het Systeem aan een lay-outmalplaatje worden toegewezen dat de gebieden van de Planning omvat.</p>
   <div class="preview">
<p> In het milieu van de Voorproef, moeten de gebruikers met een Licht of de vergunning van de Medewerker een lay-outmalplaatje worden toegewezen dat Planning omvat.</p>

<p>De standaardgebruikers en de Beheerders van het Systeem hebben Planning die door gebrek wordt toegelaten.</p></div>

<p>Voor meer informatie, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md"> lay-outmalplaatjes </a> creëren en beheren.</p></td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Recordkoppelingen delen vanuit de tabelweergave van het recordtype

{{step1-to-planning}}

De werkruimte die u het laatst hebt geopend.
1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) van **Mening** drop-down menu in de hoger-juiste hoek van de lijst, selecteer een lijstmening. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik met de rechtermuisknop op een recordrij

   of

   Beweeg over de naam van een verslag, klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **verbinding van het Exemplaar**.

   ![ Contextueel menu voor verslagrij ](assets/contextual-menu-for-record-row.png)

   De koppeling wordt naar het klembord gekopieerd.

1. Plak de koppeling in een e-mail- of chatvenster om deze met andere gebruikers te delen. Wanneer gebruikers de koppeling ontvangen, wordt de recordpagina geopend.

   >[!TIP]
   >
   >De velden op de recordpagina zijn dezelfde velden die beschikbaar zijn in de tabelweergave van de record.


   <!--add there when it will be available: if they have access to this record-->

## Alle records in een werkruimte delen door de werkruimte te delen

U kunt alle records in een werkruimte delen wanneer u de werkruimte deelt met anderen.

Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen deze delen met anderen.

Voor meer informatie, zie [ een werkruimte ](/help/quicksilver/planning/access/share-workspaces.md) delen.


<div class="preview">

## Alle records in een recordtype delen door het recordtype te delen

In het milieu van de Productie, erven de verslagen toestemmingen van de werkruimte.

In de voorvertoningsomgeving nemen records rechten over van het recordtype.

Standaard nemen recordtypen machtigingen van de werkruimte over.

U kunt echter een van de volgende handelingen uitvoeren:

* Schakel overgeërfde machtigingen van de werkruimte op een recordtype uit. Dit verwijdert hogere toestemmingen aan de verslagen, maar houdt de toestemmingen van de Mening aan de werkruimte, verslagtype, en verslagen.
* Hiermee geeft u gebruikers handmatig machtigingen voor een recordtype, zelfs als ze geen machtigingen voor de werkruimte hebben. Dit geeft hen automatisch de toestemmingen van de Mening aan de werkruimte. Hierdoor krijgen gebruikers machtigingen voor de records.

Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen hun recordtypen en records delen met anderen.

Voor meer informatie, zie [ recordtypes van het Aandeel ](/help/quicksilver/planning/access/share-record-types.md).

</div>
