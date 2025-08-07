---
title: Aan de slag met de Workfront Planning and GenStudio for Performance Marketing Integration
description: De GenStudio for Performance Marketing-werkruimte is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft. Leer enkele basisbeginselen over hoe u uw workflows kunt stroomlijnen met deze integratie.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 36cd1c23dfb6e01dc1016a6a12ae47e4f9172d20
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 0%

---

# Ga aan de slag met de Workfront Planning and GenStudio for Performance Marketing integratie

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

Organisaties die zowel Adobe Workfront Planning als Adobe GenStudio for Performance Marketing gebruiken, definiëren vaak meer gedetailleerd marketingconcepten zoals Campagnes, Producten en Persoonlijk dan wat GenStudio standaard ondersteunt.

Er is een native integratie tussen GenStudio for Performance Marketing en Workfront Planning. Dankzij deze integratie kunnen gebruikers in Workfront Planning de in GenStudio gebruikte campagnes, producten, persoonlijke instellingen, activering, kanalen en regio&#39;s beheren. Het laat hen ook toe om GenStudio te vormen om bestaande verslagtypes van de Planning van Workfront van verwijzingen te voorzien, creërend een meer verbonden en verenigbare marketing werkschema.

Dankzij deze integratie kunt u dubbele gegevensinvoer voorkomen, de planning en activering op elkaar afstemmen en kunt u uw marketingsysteem ondersteunen.

De GenStudio for Performance Marketing-werkruimte is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft.

Met de integratie tussen Workfront Planning en GenStudio for Performance Marketing kunt u:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Bekijk de GenStudio-werkruimte in Workfront Planning.
* Wijzig uw campagnes in GenStudio en heb updates in real time van de zelfde informatie in de Planning van Workfront.
* Wijzig uw campagnes in de Planning van Workfront en heb updates in real time van de zelfde informatie in GenStudio.

## Integratievereisten

* Workfront en GenStudio for Performance Marketing moeten worden ingeschakeld bij dezelfde organisatie.

  Voor meer informatie over GenStudio, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

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
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront-planningspakket</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningspakket wordt opgenomen. </p> 
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
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p> Systeembeheerder</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Contribute of hoger machtigingen voor een werkruimte en recordtype  </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


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

* U kunt recordtypegegevens (bijvoorbeeld hun weergave) bewerken in GenStudio in Workfront Planning.
* U kunt GenStudio-recordtypen met anderen delen in Planning.  <!--checking with Ani H.-->
* U kunt recordtypen maken vanuit Planning in de GenStudio-werkruimte. <!-- checking with Ani where these show up in GenS-->
* Recordtypen die met GenStudio worden gesynchroniseerd, geven een visuele indicator weer die duidelijk maakt dat de recordtypen uit GenStudio worden geïmporteerd.

### Records

* U kunt records toevoegen of verwijderen in GenStudio en deze worden weergegeven in (of verwijderd uit) Workfront Planning.
U kunt records toevoegen of verwijderen in Workfront Planning en deze worden weergegeven in (of verwijderd uit) GenStudio.
* U kunt verslagen van de Planning van Workfront op de volgende manieren toevoegen:

   * Handmatig, geheel nieuw, vanuit elke weergave met de knop Nieuwe record
   * Door ze te importeren met een CSV- of Excel-bestand
   * Handmatig, inline, in de tabelweergave
   * Handmatig, rechtstreeks in de tijdlijnweergave

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* U kunt activeringsrecords niet maken of verwijderen via Workfront Planning.
* U kunt recordinformatie over alle records in de GenStudio-werkruimte in Planning bewerken in alle zichtbare velden vanuit Workfront Planning.

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Velden

* Recordvelden worden geïmporteerd uit GenStudio. U kunt de gebiedsmontages in de Planning van Workfront uitgeven.
* U kunt meer gebieden voor de verslagtypes van GenStudio in de Planning van Workfront tot stand brengen als u Manage toegang in Gen Studio hebt.
* Wanneer u gebieden voor de verslagtypes van GenStudio in Planning creeert, zijn zij zichtbaar van de volgende gebieden:
   * Weergaven plannen
   * Recorddetailpagina&#39;s plannen
   * GenStudio-recorddetailpagina&#39;s

  >[!TIP]
  >
  >Velden die zijn gemaakt in Workfront Planning zijn niet zichtbaar in de lijstweergave van GenStudio.

* U kunt velden verbergen in de tabelweergave van een GenStudio-recordtype in Planning, maar u kunt geen velden verwijderen uit Workfront Planning.


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Weergaven

* U kunt weergaven maken voor GenStudio-recordtypen.

  Voor informatie, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

* U kunt de mening van een het recordtype van GenStudio delen aangezien u een mening voor een het verslagtype van de Planning zou delen.

### Verbindingen

* U kunt de volgende verbindingen maken tussen GenStudio-recordtypen en andere record- of objecttypen in Workfront Planning:

   * Twee GenStudio-recordtypen en
   * Een GenStudio-recordtype en een planningsrecordtype vanuit dezelfde werkruimte
   * Een GenStudio-recordtype en een planningsrecordtype van een andere werkruimte, als de recordtypen zijn geconfigureerd om verbinding te maken met een andere werkruimte.
   * Een GenStudio-recordtype en een Workfront-objecttype (projecten, portfolio&#39;s, programma&#39;s, bedrijven, groepen)