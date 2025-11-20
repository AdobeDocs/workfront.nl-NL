---
title: Records delen
description: U kunt verslagen delen gebruikend de knoop van het Aandeel om samenwerking in de Planning van Adobe Workfront te verhogen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---


<!--update metadata with real information at release-->

# Records delen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


{{planning-important-intro}}

U kunt de toestemmingen van mensen aan individuele verslagen in een verslagtype aanpassen. O

U kunt een Adobe Workfront-planningsrecord op de volgende manieren delen:

* Een koppeling naar de record delen.

  Voor meer informatie, zie [ verslagen van het Aandeel gebruikend een verbinding ](/help/quicksilver/planning/records/share-records.md).

* Deel alle records in een werkruimte met andere gebruikers door de werkruimte en het recordtype te delen.

  Zie de volgende artikelen voor meer informatie:

   * [Een werkruimte delen](/help/quicksilver/planning/access/share-workspaces.md)

   * [Een recordtype delen](/help/quicksilver/planning/access/share-record-types.md)

* Deel een verslag gebruikend de **optie van het Aandeel**.

  Dit artikel beschrijft hoe u een verslag met anderen kunt delen gebruikend de **optie van het Aandeel**.

>[!IMPORTANT]
>
>Gebruikers met toegang tot een werkruimte krijgen automatisch minstens weergavemachtigingen voor alle records in de werkruimte.
>Als u weergaven deelt, geeft u gebruikers geen machtigingen voor records. Alleen werkruimten delen kan gebruikers machtigingen verlenen voor het opnemen van typen en records.
>
>Voor algemene informatie over het delen van voorwerpen in de Planning van Workfront, zie ook [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront- en planningspakketten</p> 
of
<p>Willekeurig workflowpakket en planningspakket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Alle</p> 
   <p><b>OPMERKING</b></p>
   <p>Alleen personen met een standaardlicentie kunnen beheermachtigingen voor records krijgen. Alle andere licenties kunnen alleen weergavemachtigingen hebben en de optie Beheren is voor deze licenties grijs.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  <p>Rechten voor een werkruimte, een recordtype en de record beheren</p>  
   <p><b>BELANGRIJK</b></p>
   <p>Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen een record delen</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van records

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* U kunt records delen met de volgende entiteiten: personen, groepen, teams, bedrijven of functies.
* Als u een werkruimte deelt met gebruikers, ontvangen zij standaard dezelfde machtigingen voor de records in de werkruimte.
* Wanneer u een entiteit uit een werkruimte verwijdert, worden alle machtigingen voor delen verwijderd uit de recordtypen en alle records in de werkruimte.
* De toegang van een gebruiker tot de record wordt bepaald door de combinatie van de volgende drie instellingen:

   * Hun rechten worden overgenomen van het recordtype en de werkruimte
   * Machtigingen die afzonderlijk zijn toegevoegd in het dialoogvenster voor het delen van records
   * De volgende machtigingen:

      * **iedereen in de werkruimte kan** bekijken: Dit maakt het verslag viewable door iedereen in de werkruimte <!-- is this OK to say "workspace? should it be "record"??-->
      * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: Dit wordt geselecteerd door gebrek en staat het beperken van toegang tot het verslag tot specifieke mensen toe.

* U kunt de volgende machtigingsniveaus aan een record toekennen:

   * Weergave
   * Beheren

* Wanneer u een record deelt met een gebruiker, worden deze gegevens standaard toegevoegd met dezelfde machtigingen als voor het recordtype.

  Bijvoorbeeld:

   * Als zij de toestemmingen van de Mening aan het verslagtype hebben, krijgen zij de toestemmingen van de Mening aan het verslag
   * Als zij over Contribute- of beheermachtigingen voor het recordtype beschikken, krijgen zij beheermachtigingen voor de record

* Als werkruimtebeheerder kunt u een record delen met een gebruiker die geen deel uitmaakt van de werkruimte. In dit geval, is er een waarschuwing naast de toegevoegde entiteit op de hoogte brengend dat zij geen toegang tot de werkruimte hebben. U kunt accepteren dat de gebruiker aan zowel de record als de werkruimte wordt toegevoegd, of u kunt weigeren deze aan de werkruimte toe te voegen, zodat de gebruiker ook uit de record wordt verwijderd.

* Wanneer u een record deelt met gebruikers die beheermachtigingen hebben voor de werkruimte, krijgen zij ook standaard beheermachtigingen voor de record. De machtiging Weergeven is grijs.

* Als u geen toestemmingen hebt om mensen aan de werkruimte toe te voegen, zult u slechts gebruikers, teams, groepen, rollen, en bedrijven zien en toevoegen die reeds aan de werkruimte worden toegevoegd. U kunt geen andere entiteit toevoegen die nog geen deel uitmaakt van de werkruimte.

* U kunt overgeërfde toestemmingen voor één enkel verslag onbruikbaar maken, in welk geval u hen kunt individueel toestemmingen geven, of zij kunnen toestemmingen verkrijgen als zij tot &quot;iedereen in de werkruimte&quot;optie behoren. <!-- is this OK to say "workspace? should it be "record"??-->

* Als meerdere machtigingen voor delen van toepassing zijn op dezelfde gebruiker, krijgen ze de hoogste machtigingen voor die machtigingen.

  Als een record bijvoorbeeld wordt gedeeld met een gebruiker met weergavemachtigingen en hun groep met beheertoegang, krijgen ze beheermachtigingen voor de record.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Als een formuleveld of een raadplegingsgebied van een verbonden verslag op een gebied op een verslag gebaseerd is waarover u geen toestemmingen hebt, zult u de correcte berekening zien welke factoren in het verslag u anders niet kunt toegang hebben.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Recordmachtigingen delen

