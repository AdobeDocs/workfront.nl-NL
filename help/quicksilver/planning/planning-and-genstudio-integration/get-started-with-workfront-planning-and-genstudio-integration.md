---
title: Aan de slag met de Workfront Planning and GenStudio for Performance Marketing Integration
description: De GenStudio for Performance Marketing-werkruimte is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft. Leer enkele basisbeginselen over hoe u uw workflows kunt stroomlijnen met deze integratie.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4745b93e02c9de087afbee752e0303280e52d688
workflow-type: tm+mt
source-wordcount: '1765'
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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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

Uw organisatie moet voldoen aan de volgende vereisten voor de integratie tussen Workfront Planning en GenStudio for Performance Marketing om te kunnen bestaan:

* Workfront en GenStudio for Performance Marketing moeten worden ingeschakeld bij dezelfde organisatie.

  Voor meer informatie over GenStudio, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Uw Workfront-instantie maakt deel uit van de Adobe Unified Experience, inclusief het gebruik van het Identity Management System (IMS).

  Voor informatie, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Gebruikers die zowel Planning als GenStudio gebruiken, moeten tot slechts één Workfront-instantie binnen de IMS-organisatie behoren.

  Gebruikers die alleen voor Workfront werken, kunnen de GenStudio-werkruimte niet zien, zelfs niet als deze beschikbaar is in Workfront.

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
<p>Willekeurig Workfront-pakket</p>
<p>Willekeurig planningspakket</p>

</td> </tr>
   <tr> 
<td> 
   <p> Aanvullende producten</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-gebruikersrollen</p></td> 
   <td><p><ul><li>Elke GenStudio-gebruikersrol voor toegang tot campagnes, producten en persoonlijke instellingen</li>
   <li>GenSudio System Manager toegang tot activeringen en gebeurtenissen</li></ul>
   Voor informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> de rollen en de toestemmingen van de Gebruiker </a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Rechten voor de GenStudio-werkruimte beheren om de architectuur van de werkruimte, de recordtypen en velden te wijzigen</p></li>
   <li><p>Contribute-machtigingen voor de GenStudio-werkruimte voor het toevoegen, bijwerken of verwijderen van records in de GenStudio-recordruimte</p> </li>  
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Eventuele machtigingen in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Machtigingen maken in Adobe GenStudio for Performance Marketing om items te maken</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

Voor informatie over de toegang van de Planning van Adobe Workfront, zie [ Adobe Workfront het toegangsoverzicht van de Planning ](/help/quicksilver/planning/access/access-overview.md).

Voor meer informatie over Adobe GenStudio for Performance Marketing, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)


## Overzicht van de integratiemogelijkheden van Workfront Planning and GenStudio

Afhankelijk van het aantal Workfront-instanties in uw organisatie, hebt u automatisch de volgende machtigingen voor de GenStudio-werkruimte in Planning:

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Eén exemplaar van Workfront</p></td> 
   <td> 
<p>Er is één GenStudio-werkruimte in Workfront Planning</p>
<p>Alle gebruikers met toegang tot GenStudio en Workfront Planning beschikken over beheermachtigingen in de GenStudio-werkruimte</p> 
</td> </tr>
   <tr> 
<td> 
   <p> Meerdere versies van Workfront</p> </td> 
   <td> 
   <p>Er is één GenStudio-werkruimte in elke Workfront Planning-instantie</p>
<p>Alle gebruikers met toegang tot GenStudio en Workfront Planning beschikken over Contribute-machtigingen voor de GenStudio-werkruimte van elk exemplaar</p> </td> 
  </tr>

</tbody> 
</table>

Voor informatie over de toestemmingen van de Planning van Workfront, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

In de onderstaande secties wordt het volgende beschreven:

* Mogelijkheden voor het bijwerken van Workfront Planning-informatie van GenStudio
* Mogelijkheden voor het bijwerken van GenStudio-informatie van Workfront Planning
* Beperkingen voor wat u in een GenStudio-werkruimte kunt en kunt beheren vanuit Workfront Planning.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### De GenStudio-werkruimte

* Als u de GenStudio-werkruimte in GenStudio bijwerkt, worden de wijzigingen weergegeven in de GenStudio-werkruimte in Planning.
* De werkruimte van GenStudio toont een visuele indicator in de Planning van Workfront om het als dusdanig te identificeren.

  ![ kaart van GenStudio in Planning ](assets/genstudio-card-with-tag-highlighted.png)

  Voor informatie, zie [ de werkruimte van GenStudio in de Planning van Adobe Workfront ](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md) leiden.
* Wanneer u beheerdersmachtigingen hebt voor de GenStudio-werkruimte in Planning, kunt u:

   * De GenStudio-werkruimte in Planning bijwerken (naam, beschrijving, pictogram)
   * Secties maken
   * Recordtypen toevoegen
   * Delen met anderen

     U kunt de GenStudio-werkruimte delen met anderen die geen GenStudio-account hebben. U kunt deze alleen delen met gebruikers die beschikbaar zijn in het Identity Management System (IMS) van uw organisatie. <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Als u over Contribute-machtigingen voor de GenStudio-werkruimte in Planning beschikt, kunt u de werkruimte niet wijzigen vanuit Planning.

### Typen opnemen in de GenStudio-werkruimte

* Als u de GenStudio-recordtypen bewerkt in GenStudio, worden de wijzigingen weergegeven in de GenStudio-werkruimte bij Planning.
* Recordtypen die zowel in GenStudio als in Planning zichtbaar zijn, hebben een GenStudio-indicator in Workfront Planning.

  ![ het verslagtype van GenStudio kaart in de Planning van Workfront ](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Wanneer u beheerdersmachtigingen hebt voor de GenStudio-werkruimte in Planning, kunt u het volgende doen via Workfront Planning:
   * Gegevens over GenStudio-recordtypen bewerken (weergave, geavanceerde instellingen).
   * GenStudio-recordtypen delen met anderen.
   * Recordtypen maken. Deze recordtypen blijven alleen beschikbaar in Workfront Planning. Ze worden niet weergegeven in GenStudio.
* Als u over Contribute-machtigingen voor de GenStudio-werkruimte in Planning beschikt, kunt u de GenStudio-recordtypen niet wijzigen vanuit Planning.

### Records in de GenStudio-werkruimte

* Wanneer u GenStudio-records bewerkt in GenStudio, zijn de wijzigingen zichtbaar in alle GenStudio-werkruimten in al uw exemplaren van Workfront.
* U kunt activeringsrecords niet maken of verwijderen via Workfront Planning.
* Als u beheerdersmachtigingen of Contribute voor de GenStudio-werkruimte hebt bij Planning, kunt u het volgende doen via Workfront Planning:
   * Records toevoegen of verwijderen die zichtbaar worden in (of worden verwijderd uit) GenStudio.

     Verwijderde records uit Workfront Planning of GenStudio worden gedurende 30 dagen in de Workfront Planning Onlangs verwijderd bin geplaatst. GenStudio heeft geen recent verwijderde opslagmap.
   * Herstel een record uit het recent verwijderde vak. Door verwijderde records te herstellen, worden ze weer geplaatst in Workfront Planning en GenStudio.
   * Voeg records op de volgende manieren toe:

      * Handmatig, geheel nieuw, vanuit elke weergave met de knop Nieuwe record
      * U kunt de bestanden importeren met een CSV- of Excel-bestand in de tabelweergave
      * Handmatig, in elke weergave in Workfront Planning
      * Door een aanvraag in te dienen bij een aanvraagformulier voor een recordtype in Workfront.

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* U kunt recordgegevens van alle records in de GenStudio-werkruimte bewerken via Workfront Planning.

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

### Velden met recordtypen in de GenStudio-werkruimte

* GenStudio-recordvelden worden standaard geïmporteerd naar Workfront Planning.
* U kunt geen velden toevoegen aan recordtypen in GenStudio.
* Wanneer u beheerdersmachtigingen hebt voor de GenStudio-werkruimte in Planning, kunt u het volgende doen via Workfront Planning:

   * GenStudio-veldinstellingen bewerken.
   * Maak velden voor GenStudio-recordtypen als u beheertoegang hebt in Gen Studio.

     Wanneer u gebieden voor de verslagtypes van GenStudio in Planning creeert, zijn zij zichtbaar van de volgende gebieden:

      * Weergaven Workfront Planning
      * Workfront Planning-recorddetailpagina&#39;s
      * GenStudio-recorddetailpagina&#39;s

     >[!TIP]
     >
     >Velden die zijn gemaakt in Workfront Planning zijn niet zichtbaar in de lijstweergave van GenStudio.

   * Velden verbergen in de tabelweergave van een GenStudio-recordtype in Planning.
&lt;!—* Velden die zijn gemaakt in Workfront Planning for GenStudio verwijderen uit Workfront Planning. — dit is niet mogelijk, per Iskuhi; de link is er, maar het zal een fout genereren—>

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Als u beschikt over Contribute-machtigingen voor de GenStudio-werkruimte in Planning:

   * U kunt in Workfront Planning geen velden bewerken die zijn ingesteld, verwijderen of toevoegen vanuit de GenStudio-werkruimte.
   * U kunt velden verbergen in de tabelweergave in Workfront Planning.

#### De velden Gemaakt door en goedgekeurd door

* U kunt de velden Gemaakt door en Goedgekeurd door de recordtypen van GenStudio vanuit Workfront Planning toevoegen in Workfront Planning.
* De verslagen die in de het verslagtypes van het Kanaal en van het Gebied tonen &quot;Systeem&quot;als Gemaakt door gebruiker. Deze records worden automatisch gemaakt wanneer de GenStudio-werkruimte wordt gemaakt in Workfront Planning.
* De records die in GenStudio zijn gemaakt nadat de werkruimte in Workfront Planning beschikbaar is gemaakt, geven de naam weer van de IMS-gebruiker die de record heeft gemaakt in het veld Gemaakt op, zelfs als de gebruiker de records in GenStudio heeft gemaakt en geen Workfront-gebruiker is.
* In het veld Goedgekeurd door wordt de naam van de fiatteur weergegeven wanneer een aanvraagformulier wordt verzonden om een record te maken in het GenStudio-recordtype in Workfront Planning.

### Weergaven opnemen in de GenStudio-werkruimte

>[!NOTE]
>
>De GenStudio-recordtypen worden weergegeven in de standaardtabelweergave die is geïmporteerd uit GenStudio.
>
>U kunt de oorspronkelijke tabelweergave die standaard uit GenStudio is geïmporteerd, niet verwijderen.

* In GenStudio kunt u geen meerdere weergaven maken.

* Wanneer u beheerdersmachtigingen hebt voor de GenStudio-werkruimte in Planning, kunt u het volgende doen in Workfront Planning:

   * Weergaven maken voor GenStudio-recordtypen.

     Voor informatie, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

   * Wijzig de namen van aangepaste weergaven in de GenStudio-recordtypen, deel ze, exporteer ze, dupliceer ze of verwijder ze.

* Als u over Contribute-machtigingen voor de GenStudio-werkruimte in Planning beschikt, kunt u het volgende doen in Workfront Planning:

   * Weergaven maken voor GenStudio-recordtypen.

     Voor informatie, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

   * U kunt aangepaste weergaven hernoemen, exporteren, dupliceren of verwijderen uit de GenStudio-recordtypen.

     U kunt geen weergaven delen vanuit de GenStudio-werkruimte in Workfront Planning

### Verbindingen opnemen in de GenStudio-werkruimte

U kunt verbindingen maken tussen recordtypen in GenStudio-werkruimten waar u beheermachtigingen hebt.

U kunt de volgende verbindingen maken tussen GenStudio-recordtypen en andere record- of objecttypen in Workfront Planning:

* Twee GenStudio-recordtypen
* Een GenStudio-recordtype en een planningsrecordtype vanuit dezelfde werkruimte
* Een GenStudio-recordtype en een planningsrecordtype van een andere werkruimte, als de recordtypen zijn geconfigureerd om verbinding te maken met een andere werkruimte.
* Een GenStudio-recordtype en een Workfront-objecttype (projecten, portfolio&#39;s, programma&#39;s, bedrijven, groepen)
* A GenStudio record type and an AEM Assets object type.

### Formulieren en automatisering aanvragen in het GenStudio-recordtype

* U kunt aanvraagformulieren toevoegen aan een GenStudio-recordtype in Workfront Planning.

  Voor informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
* U kunt automatiseringen voor een GenStudio verslagtype in de Planning van Workfront vormen.

  Voor informatie, zie [ de automatisering van de Planning van Adobe Workfront ](/help/quicksilver/planning/records/configure-automations-to-create-records.md) vormen.

## De voorvertoningsomgeving

* De GenStudio-werkruimte die toegankelijk is vanuit de productieomgeving, wordt ook weergegeven in de voorbeeldomgeving van hetzelfde Workfront-exemplaar.
* U kunt alle activiteiten uitvoeren die in dit artikel worden beschreven op de GenStudio-werkruimte in Workfront Planning in uw Voorvertoningsomgeving, maar deze wijzigingen zijn niet zichtbaar vanuit GenStudio.

  Alleen wijzigingen die u aanbrengt in items in de synchronisatie van de productieomgeving tussen Workfront Planning en GenStudio.

  GenStudio heeft geen voorvertoningsomgeving.

