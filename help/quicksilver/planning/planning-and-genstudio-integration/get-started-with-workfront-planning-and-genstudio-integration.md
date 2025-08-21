---
title: Aan de slag met de Workfront Planning and GenStudio for Performance Marketing Integration
description: De GenStudio for Performance Marketing-werkruimte is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft. Leer enkele basisbeginselen over hoe u uw workflows kunt stroomlijnen met deze integratie.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1475'
ht-degree: 0%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Ga aan de slag met de Adobe Workfront Planning and Adobe GenStudio for Performance Marketing integratie

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Organisaties die zowel Adobe Workfront Planning als Adobe GenStudio for Performance Marketing gebruiken, definiëren vaak meer gedetailleerd marketingconcepten zoals Campagnes, Producten en Persoonlijk dan wat GenStudio standaard ondersteunt.

Er is een native integratie tussen GenStudio for Performance Marketing en Workfront Planning. Dankzij deze integratie kunnen gebruikers in Workfront Planning de in GenStudio gebruikte campagnes, producten, persoonlijke instellingen, activering, kanalen en regio&#39;s beheren. Het laat hen ook toe om GenStudio te vormen om bestaande verslagtypes van de Planning van Workfront van verwijzingen te voorzien, creërend een meer verbonden en verenigbare marketing werkschema.

De GenStudio for Performance Marketing-werkruimte is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft.

## Integratievoordelen

Met de integratie tussen Workfront Planning en GenStudio for Performance Marketing kunt u:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Bekijk de GenStudio-werkruimte in Workfront Planning.
* Wijzig uw campagnes in GenStudio en heb updates in real time van de zelfde informatie in de Planning van Workfront.
* Wijzig uw campagnes in de Planning van Workfront en heb updates in real time van de zelfde informatie in GenStudio.
* Vermijd dubbele gegevensinvoer.
* Houd de afstemming over planning en activering.

## Integratievereisten

* Workfront en GenStudio for Performance Marketing moeten worden ingeschakeld bij dezelfde organisatie.

  Voor meer informatie over GenStudio, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)

* GenStudio is niet beschikbaar in Workfront Planning wanneer uw bedrijf meerdere Workfront-instanties heeft. <!--this will change-->

* De Workfront-instantie maakt deel uit van de Adobe Unified Experience, inclusief het gebruik van het Identity Management System (IMS).

  Voor informatie, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Gebruikers die zowel Planning als GenStudio gebruiken, kunnen binnen de IMS-organisatie tot slechts één Workfront-instantie behoren.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Toegangsvereisten

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Elk Adobe Workfront Workflow-pakket</p>
<p>Willekeurig Adobe Workfront-planningspakket</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio-pakket</p></td> 
   <td> 
<p>??? HEEFT GEN STUDIO EEN PAKKET DAT DIT ONDERSTEUNT?</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio-licentie</p></td> 
   <td><p> ??? VEREIST GEEN STUDIO EEN SPECIFIEKE LICENTIE DIE DIT ONDERSTEUNT?</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Aanvullende producten</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>  
   <p>Configuratie voor GenStudio: ???WAT BEHOEFT HET TOEGANGSNIVEAU VOOR GENS??</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen*</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Contribute of hoger machtigingen voor een werkruimte en recordtype  </p> </li> 
   <li><p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p></li>
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Eventuele machtigingen in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Machtigingen maken in Adobe GenStudio for Performance Marketing om items te maken</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Voor meer informatie over Adobe GenStudio for Performance Marketing, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)


## Overzicht van de integratie van Workfront Planning and GenStudio

In de volgende secties wordt het volgende beschreven:

* Mogelijkheden voor het bijwerken van Workfront Planning-informatie van GenStudio
* Mogelijkheden voor het bijwerken van GenStudio-informatie van Workfront Planning
* Beperkingen voor wat u in een GenStudio-werkruimte kunt en kunt beheren vanuit Workfront Planning.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### De GenStudio-werkruimte in Workfront Planning

* Als uw organisatie meerdere Workfront-instanties heeft, is de GenStudio-werkruimte niet zichtbaar vanuit een van uw Workfront-instanties. <!-- this might change-->
* De werkruimte van GenStudio geeft een visuele indicator weer die duidelijk maakt dat deze uit GenStudio is geïmporteerd. Voor informatie, zie [ de werkruimte van GenStudio in de Planning van Adobe Workfront ](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md) leiden.
* Alle gebruikers die toegang hebben tot zowel de Planning van GenStudio als van Workfront kunnen de werkruimte van GenStudio in de Planning van Workfront ook zien.
* Gebruikers van Workfront Planning moeten via het Adobe Identity Management System (IMS) worden beheerd om de GenStudio-werkruimte van Workfront te kunnen bekijken en gebruiken.

  Gebruikers die alleen voor Workfront werken, kunnen de GenStudio-werkruimte niet zien, zelfs niet als deze beschikbaar is in Workfront.

  Voor informatie, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Recordtypen

* U kunt de gegevens van GenStudio-recordtypen (bijvoorbeeld hun weergave) bewerken via Workfront Planning.
* U kunt GenStudio-recordtypen met anderen delen in Planning.
* U kunt recordtypen maken vanuit Planning in de GenStudio-werkruimte. Deze recordtypes blijven slechts in Planning. Ze worden niet weergegeven in GenStudio.
* De types van verslag die met GenStudio worden gesynchroniseerd tonen een visuele indicator in de Planning van Workfront die het duidelijk maakt dat de verslagtypes uit GenStudio worden ingevoerd.

### Records

Het volgende is mogelijk voor verslagen die tot de verslagtypes behoren van GenStudio die zowel in de Planning van GenStudio als Workfront tonen:

* U kunt records toevoegen of verwijderen in GenStudio en deze worden weergegeven in (of verwijderd uit) Workfront Planning.
* U kunt records toevoegen of verwijderen in Workfront Planning en deze worden weergegeven in (of verwijderd uit) GenStudio.
* Wanneer u verslagen van of de Planning van Workfront of GenStudio schrapt, worden zij geplaatst in de Planning van Workfront onlangs schrapte bak 30 dagen. GenStudio heeft geen recent verwijderde opslagmap.
* Als u een record uit de recent verwijderde opslagmap herstelt, worden deze weer geplaatst in Workfront Planning en GenStudio.
* U kunt verslagen van de Planning van Workfront op de volgende manieren toevoegen:

   * Handmatig, geheel nieuw, vanuit elke weergave met de knop Nieuwe record
   * Door ze te importeren met een CSV- of Excel-bestand
   * Handmatig, inline, in de tabelweergave
   * Handmatig, rechtstreeks in de tijdlijn- of kalenderweergave <!--ensure the calendar is released when this releases-->

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* U kunt activeringsrecords niet maken of verwijderen via Workfront Planning.
* U kunt recordinformatie over alle records in de GenStudio-werkruimte in Planning bewerken in alle zichtbare velden vanuit Workfront Planning.

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Velden

* Recordvelden worden geïmporteerd uit GenStudio. U kunt GenStudio-veldinstellingen bewerken via Workfront Planning.
* U kunt velden maken voor GenStudio-recordtypen in Workfront Planning als u beheertoegang hebt in Gen Studio.
* Wanneer u gebieden voor de verslagtypes van GenStudio in Planning creeert, zijn zij zichtbaar van de volgende gebieden:
   * Weergaven plannen
   * Recorddetailpagina&#39;s plannen
   * GenStudio-recorddetailpagina&#39;s

  >[!TIP]
  >
  >Velden die zijn gemaakt in Workfront Planning zijn niet zichtbaar in de lijstweergave van GenStudio.

* U kunt velden in de tabelweergave van een GenStudio-recordtype verbergen in Planning.
* U kunt geen velden verwijderen die vanuit GenStudio zijn geïmporteerd vanuit Workfront Planning.
* U kunt velden die zijn gemaakt in Workfront Planning for GenStudio-recordtypen verwijderen uit Workfront Planning.

### De velden Gemaakt door en goedgekeurd door

* U kunt de velden Gemaakt door en Goedgekeurd door de recordtypen van GenStudio vanuit Workfront Planning toevoegen in Workfront Planning.
* De verslagen die in de het verslagtypes van het Kanaal en van het Gebied tonen &quot;Systeem&quot;als Gemaakt door gebruiker. Deze records worden automatisch gemaakt wanneer de GenStudio-werkruimte wordt gemaakt in Workfront Planning.
* De records die in GenStudio zijn gemaakt nadat de werkruimte in Workfront Planning beschikbaar is gemaakt, geven de naam weer van de IMS-gebruiker die de record heeft gemaakt in het veld Gemaakt op, zelfs als de gebruiker de records in GenStudio heeft gemaakt en geen Workfront-gebruiker is.
* In het veld Goedgekeurd door wordt de naam van de fiatteur weergegeven wanneer een aanvraagformulier wordt verzonden om een record te maken in het GenStudio-recordtype in Workfront Planning.

### Weergaven

* U kunt weergaven maken voor GenStudio-recordtypen.

  Voor informatie, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

* Het delen van de weergave van een GenStudio-recordtype is hetzelfde als het delen van een weergave voor een planningsrecordtype.
* In GenStudio kunt u geen meerdere weergaven maken.

### Verbindingen

* U kunt de volgende verbindingen maken tussen GenStudio-recordtypen en andere record- of objecttypen in Workfront Planning:

   * Twee GenStudio-recordtypen
   * Een GenStudio-recordtype en een planningsrecordtype vanuit dezelfde werkruimte
   * Een GenStudio-recordtype en een planningsrecordtype van een andere werkruimte, als de recordtypen zijn geconfigureerd om verbinding te maken met een andere werkruimte.
   * Een GenStudio-recordtype en een Workfront-objecttype (projecten, portfolio&#39;s, programma&#39;s, bedrijven, groepen)
   * A GenStudio record type and an AEM Assets object type.

### Formulieren en automatisering aanvragen

* U kunt aanvraagformulieren toevoegen aan een GenStudio-recordtype in Workfront Planning.
* U kunt automatiseringen voor een GenStudio verslagtype in de Planning van Workfront vormen.

### De voorvertoningsomgeving

* De GenStudio-werkruimte die vanuit uw productieomgeving toegankelijk is, wordt ook weergegeven in uw voorvertoningsomgeving.
* U kunt alle activiteiten uitvoeren die in dit artikel worden beschreven op de GenStudio-werkruimte in Workfront Planning in uw Voorvertoningsomgeving, maar deze wijzigingen worden niet overgedragen naar GenStudio.
Alleen wijzigingen die u aanbrengt in items in de synchronisatie van de productieomgeving tussen Workfront Planning en GenStudio.
GenStudio heeft geen voorvertoningsomgeving.

