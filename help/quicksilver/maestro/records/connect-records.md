---
title: Connect-records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '2912'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connect-records

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt Adobe Maestro-records met elkaar of met objecten van andere toepassingen verbinden.

U moet eerst twee recordtypen met elkaar verbinden of een recordtype verbinden met een objecttype vanuit een andere toepassing. Vervolgens kunt u de tabelweergave van het recordtype gebruiken om records met elkaar te verbinden of records met andere objecten te verbinden.

Voor informatie over het verbinden van verslagtypes met elkaar of aan objecten types van andere toepassingen, zie [Verbind recordtypen](../architecture/connect-record-types.md).

Zie voor een voorbeeld van het verbinden van recordtypen [Voorbeeld van het verbinden van recordtypen en records](../architecture/example-connect-record-types-and-records.md).

U kunt het volgende verbinden:

* Operationele Maestro-gegevens
* Operationele gegevens van Maestro naar taxonomische gegevens
* Operationele Maestro-records en objecten van andere toepassingen.

  U kunt Maestro-records vanuit de volgende toepassingen verbinden met objecten van de onderstaande typen:

   * Adobe Workfront

      * Projecten
      * Portfolio&#39;s
      * Programma&#39;s
      * Bedrijf
      * Groep

   * Adobe Experience Manager Assets

      * Afbeeldingsbestanden
      * Mappen



  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
<td>Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Als u Maestro-records wilt verbinden met Experience Manager Assets, hebt u een Adobe Experience Manager Assets-licentie nodig en moet het exemplaar van Workfront van uw organisatie zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Connect-records

### Overwegingen bij het verbinden van records

* Nadat u recordtypen hebt verbonden, worden de verbonden recordtypen weergegeven als gekoppelde recordvelden in de tabel met de recordtypen waarvan ze zijn gekoppeld.
* U kunt records en objecten van de gekoppelde record- en objecttypen bladeren en deze toevoegen vanuit de gekoppelde recordvelden.
* U kunt velden van de gekoppelde recordtypen toevoegen aan de tabel van het recordtype waarvan u een koppeling maakt.
* U kunt de waarden van gekoppelde velden niet handmatig bijwerken in de records waarvan u een koppeling maakt.

  De waarden van de verbonden gebieden van de verbonden verslagen bevolken het verslag Maestro dat u van automatisch van de werkruimte van Maestro verbindt u of van de derdetoepassing vormt.

* Iedereen met toegang tot de Maestro- en beheermachtigingen voor de werkruimte kan de verbindingen zien die u maakt tussen Maestro-records of tussen Maestro-records en andere toepassingsobjecten. Ze kunnen verbonden records en objecten weergeven, ongeacht hun machtigingen voor de externe toepassingen waarmee u verbinding maakt. <!--check with PM-->
* U kunt de verbindingen van alle anderen weergeven en bewerken als u beheerdersmachtigingen hebt voor de werkruimte waar de verbonden records zich bevinden.
* U kunt één Maestro-record verbinden met een of meerdere objecten vanuit een andere toepassing.
* Als u Maestro-records wilt koppelen aan andere records of objecten, moet u over het volgende beschikken:

   * Ten minste één Maestro-werkruimte, recordtype en record.

     Raadpleeg de volgende artikelen voor meer informatie:

      * [Werkruimten maken](../architecture/create-workspaces.md)
      * [Recordtypen maken](../architecture/create-record-types.md)
      * [Records maken](../records/create-records.md)

   * Verbindingen tussen recordtypen of tussen recordtypen en objecten uit andere toepassingen. Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md)

### Connect Maestro-records

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. (Optioneel) Voeg records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. Ga vanuit een record in de tabelweergave naar de gekoppelde recordkolom en houd de cursor boven de cel die overeenkomt met de record die u wilt koppelen aan andere records, en klik vervolgens op de knop **+** pictogram.

   De **Objecten verbinden** wordt weergegeven.

   ![](assets/connected-objects-table-for-records.png)

1. Typ de naam van een record in het zoekvak en selecteer de naam wanneer de record in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere records in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   Het volgende wordt toegevoegd:

   * De gekoppelde records worden weergegeven in het gekoppelde recordveld van de record die u in stap 5 hebt geselecteerd. <!--accurate?--> Wanneer u de gekoppelde records bijwerkt, worden de gekoppelde velden voor de records waarvan u een koppeling maakt, automatisch bijgewerkt. U kunt gekoppelde velden niet handmatig bewerken.

     >[!TIP]
     >
     >* We gebruiken onderling gekoppelde velden en opzoekvelden.
     >
     >* Als u de optie **Meerdere records toestaan** Wanneer u de recordtypen aansluit, worden de waarden van velden voor de meerdere geselecteerde objecten weergegeven met een komma van elkaar gescheiden of samengevoegd op basis van de gekozen aggregator.

1. (Optioneel) Sluit de pagina Type Maestro-record en ga naar de geselecteerde werkruimte.
1. Klik op de kaart voor het recordtype waarmee u een koppeling hebt gemaakt.

   Als u bijvoorbeeld verbinding hebt gemaakt met de **Campagne** record met de productrecord, klik op de knop **Product** kaart.

   Het recordtype moet worden geopend in de tabelweergave. Als dat niet het geval is, selecteert u een tabelweergave.

   Let erop dat de **Campagne** In het gekoppelde recordveld worden de namen weergegeven van de campagnes die u aan producten hebt gekoppeld op de pagina Type productrecord. Wanneer u de Campagnegegevens bijwerkt, wordt het aan Campagne gekoppelde recordveld voor het type productrecord automatisch bijgewerkt.

### Connect Maestro-records verbinden met Workfront-objecten

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Nadat u een verbinding hebt gemaakt tussen een Maestro-recordtype en een Workfront-objecttype, kunt u afzonderlijke Maestro-records verbinden met objecten in Workfront. De Workfront-velden die u hebt verbonden, worden automatisch ingevuld in de Maestro-records waarvan u de objecten koppelt.

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.

1. (Optioneel) Voeg afzonderlijke records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. (Voorwaardelijk) Als u het geselecteerde recordtype hebt verbonden met een Workfront-object, gaat u naar de kolom met het gekoppelde object en plaatst u de cursor boven de cel die overeenkomt met de record die u wilt koppelen aan objecten uit Workfront. Klik vervolgens op de knop **+** pictogram.

   De **Objecten verbinden** wordt weergegeven.

   ![](assets/connect-objects-box-to-select-projects.png)

   Zie voor meer informatie over het verbinden van recordtypen met objecten uit een externe toepassing [Verbind recordtypen](../architecture/connect-record-types.md).

1. Typ de naam van een Workfront-object in het zoekvak en selecteer het vervolgens wanneer het in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere objecten in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   Het volgende wordt toegevoegd:

   * De geselecteerde Workfront-objecten worden toegevoegd aan het gekoppelde recordveld.
   * Als u deze hebt toegevoegd toen u het recordtype verbond met Workfront, worden de gekoppelde velden (of de opzoekvelden) automatisch gevuld met informatie uit Workfront.
   * Er wordt een nieuw recordtype met de naam &quot;&lt; Naam van het Workfront-objecttype >&quot; gemaakt in dezelfde werkruimte als de Maestro-record waarvan u een koppeling maakt. De naam van het object maakt deel uit van de naam van dit recordtype. Als u bijvoorbeeld een koppeling naar een Workfront-project maakt, worden de **Project** recordtype in Maestro.

     Dit is een alleen-lezen recordtype en er worden Workfront-objecten weergegeven die zijn geselecteerd in het nieuwe gekoppelde objectveld dat u hebt gemaakt van de Maestro-record. De gekoppelde velden van het gekoppelde object worden ook weergegeven op de alleen-lezen gekoppelde Workfront-records.

     >[!IMPORTANT]
     >
     > Het alleen-lezen Workfront-objectrecordtype wordt alleen gemaakt wanneer afzonderlijke projecten aan Maestro-records worden toegevoegd. Het maken van een verbinding tussen een Maestro-recordtype en een Workfront-objecttype leidt niet tot het Workfront-recordtype.

     Eventuele bestaande informatie uit de velden van de Workfront-objecten wordt weergegeven in de gekoppelde of opzoekvelden.

     >[!TIP]
     >
     >
     >* Als u de instelling Meerdere records toestaan hebt ingeschakeld, worden de waarden van de meerdere objecten gescheiden door komma&#39;s weergegeven of worden ze samengevoegd volgens de gekozen aggregator.
     >
     >* Er wordt geen gekoppeld recordveld naar de Maestro-gekoppelde records gemaakt voor de gekoppelde Workfront-objecten in Workfront.


1. (Optioneel) Sluit de pagina Type Maestro-record en ga naar de geselecteerde werkruimte.
1. (Optioneel) Klik op de kaart voor het recordtype van het Workfront-object. Klik bijvoorbeeld op de knop **Project** als u een koppeling hebt gemaakt naar Workfront-projecten. Het Workfront-recordtype alleen-lezen moet worden geopend in de tabelweergave.

   De records in de Workfront-recordtypepagina zijn alleen-lezen Workfront-objecten die zijn gekoppeld vanuit Maestro-records. De velden die zijn gekoppeld via het Workfront-recordtype, worden ook weergegeven als alleen-lezen kolommen en worden automatisch ingevuld wanneer ze in Workfront worden ingevuld.

1. (Optioneel) Voer een van de volgende handelingen uit om de pagina met gegevens over Workfront-objectrecords te openen in Maestro:

   * Ga in het recordtype waarvan u een koppeling hebt gemaakt naar het aan een Workfront-object gekoppelde recordveld en klik op de naam van het Workfront-object.
   * Van de **Tabel** Klik op de naam van het Workfront-object in de weergave van het Workfront-recordtype

     of

     Klik op de knop **Meer** rechts van de naam van het Workfront-object en klikt u op **Weergave**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   Hiermee opent u de pagina Details van Maestro van het gekoppelde Workfront-object. Dit is een alleen-lezen pagina.

1. (Optioneel) Voer een van de volgende handelingen uit om het gekoppelde Workfront-object te openen in Workfront:

   * Van de **Tabel** Klik op de naam van het Workfront-object om de projectrecord in Maestro te openen

   of

   Klik op de knop **Meer** rechts van de naam van het Workfront-object, klikt u op **Ga naar bron**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Hierdoor wordt de Workfront-objectpagina geopend. U kunt informatie over het Workfront-object bewerken als u hiervoor gemachtigd bent.

1. (Optioneel) Klik op de pagina met alleen-lezen Workfront-objectrecords in Maestro op **Velden toevoegen** pictogram ![](assets/add-fields-icon.png) in de rechterbovenhoek van de tabelweergave om Workfront-velden toe te voegen aan of te verwijderen uit het Workfront-recordtype.

   >[!NOTE]
   >
   >  De velden die u toevoegt of verwijdert op de pagina met Workfront-objectrecordtypen, worden niet toegevoegd aan of verwijderd uit het Maestro-recordtype dat is gekoppeld aan het Workfront-objecttype. De velden zijn alleen zichtbaar op de pagina met alleen-lezen Workfront-recordtypen, zodat u ze in Maestro kunt bekijken.

1. (Optioneel en voorwaardelijk) Als u ten minste twee datumvelden hebt toegevoegd aan het Workfront-object, klikt u op de knop **Weergave** vervolgkeuzemenu op de pagina met recordtypen voor Workfront-objecten en selecteer de **Tijdlijn** of **Weergave maken** om een tijdlijnweergave te maken.  Zie voor meer informatie [De tijdlijnweergave beheren](/help/quicksilver/maestro/views/manage-the-timeline-view.md).

   De aan Workfront gekoppelde objecten worden in de tijdlijnweergave weergegeven.


### Connect Maestro-records verbinden met Adobe Experience Manager-objecten

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>U moet een Adobe Experience Manager Assets-licentie hebben en het Workfront-exemplaar van uw organisatie moet zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console om Maestro-records te kunnen verbinden met Adobe Experience Manager Assets.
>
>Als u vragen hebt over instaptoegang tot de Adobe Admin Console, raadpleegt u de [Veelgestelde vragen over Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Nadat u een verbinding hebt gemaakt tussen een Maestro-recordtype en Adobe Experience Manager Assets, kunt u afzonderlijke Maestro-records verbinden met Experience Manager-elementen. De elementvelden die u vanaf Experience Manager Assets hebt verbonden toen u de verbinding maakte, worden automatisch ingevuld in het Maestro-recordtype waarvan u een koppeling hebt gemaakt.

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.

1. (Optioneel) Voeg afzonderlijke records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. (Voorwaardelijk) Als u het geselecteerde recordtype hebt verbonden met Experience Manager Assets, gaat u naar de gekoppelde objectkolom en beweegt u de cursor over de cel die overeenkomt met de record die u vanuit de Experience Manager wilt koppelen met andere objecten. Klik vervolgens op de knop **+** pictogram.

   De **Elementen selecteren** wordt weergegeven. <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   Zie voor meer informatie over het verbinden van recordtypen met objecten uit een externe toepassing [Verbind recordtypen](../architecture/connect-record-types.md).

1. Klik om een aantal van de volgende typen elementen te selecteren:

   * Afbeeldingen
   * Mappen

   U kunt meerdere elementen selecteren.

   >[!IMPORTANT]
   >
   > U kunt alleen elementen verbinden die u in Experience Manager kunt bekijken. Zodra verbonden, kunnen alle gebruikers van Maestro de activa in Maestro, ongeacht hun toegang in Experience Manager Assets bekijken.

1. Klikken **Selecteren**.

   Het volgende wordt toegevoegd:

   * De geselecteerde elementen van de Experience Manager worden toegevoegd aan het gekoppelde recordveld.
   * In de gekoppelde velden (of opzoekvelden) wordt informatie uit de aan de Experience Manager gekoppelde elementen ingevuld.
   * Een nieuw recordtype met de naam &quot;Experience Manager Assets&quot; wordt gemaakt in dezelfde werkruimte als de Maestro-record waaruit u een koppeling maakt. <!--is this still added?-->

     Dit is een alleen-lezen recordtype en er worden Experience Manager-elementen weergegeven die zijn geselecteerd in het nieuwe gekoppelde objectveld dat u hebt gemaakt van de Maestro-record. De gekoppelde velden van het gekoppelde object worden ook weergegeven op de alleen-lezen gekoppelde Experience Manager-records.

     >[!IMPORTANT]
     >
     > Het Experience Manager Assets-recordtype alleen-lezen wordt alleen gemaakt wanneer afzonderlijke elementen aan Maestro-records worden toegevoegd. Als u een verbinding maakt tussen een Maestro-recordtype en Experience Manager Assets, wordt het Experience Manager Assets-recordtype niet gemaakt.

     Eventuele bestaande informatie uit de velden van de elementen van de Experience Manager wordt weergegeven in de gekoppelde of opzoekvelden.

     >[!TIP]
     >
     >
     >* Als u de instelling Meerdere records toestaan hebt ingeschakeld, worden de waarden van de meerdere objecten gescheiden door komma&#39;s weergegeven.
     >
     >* Er wordt geen gekoppeld recordveld naar de Maestro-gekoppelde records gemaakt voor de gekoppelde Experience Manager-elementen in de Experience Manager Assets-toepassing.


1. (Optioneel) Sluit de pagina Type Maestro-record en ga naar de geselecteerde werkruimte.
1. Klik op de kaart voor het Experience Manager Assets-recordtype. Het Experience Manager Assets-recordtype alleen-lezen moet worden geopend in de tabelweergave.

   De records in de Experience Manager Assets-recordtypepagina zijn alleen-lezen elementen. De velden die zijn gekoppeld via het Experience Manager Assets-recordtype, worden ook weergegeven als alleen-lezen kolommen en worden automatisch gevuld wanneer ze in de Experience Manager worden ingevuld.

1. (Optioneel) Ga naar het recordtype dat u vanuit Experience Manager Assets hebt gekoppeld en klik op de naam van een element in het gekoppelde recordveld. De details van de Experience Manager van de activa tonen in een pop-up venster. <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   De volgende velden worden weergegeven voor een afbeeldingsbestand:

   * Een miniatuur van de afbeelding
   * De naam van het afbeeldingsbestand
   * Dimensionen
   * Grootte
   * Beschrijving
   * Het bestandspad in Experience Manager
   * Het elementtype
   * Gemaakt op
   * Datum gewijzigd

1. (Optioneel) Ga als volgt te werk om de pagina Experience Manager Assets-recordgegevens te openen in Maestro:

   1. Ga naar de **Experience Manager Assets** Maestro-opnametype kaart in de werkruimte die u oorspronkelijk hebt geselecteerd en klik om de pagina met recordtypen te openen.
De Experience Manager Assets Maestro-recordtype pagina is alleen-lezen.
   1. Klik in de tabelweergave op de naam van een element

      of

      Houd de aanwijzer boven de naam van een element en klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de elementnaam klikt u op **Weergave**.\
      Hierdoor wordt de Maestro van het actief geopend **Details** pagina. Dit is een alleen-lezen pagina.
1. (Optioneel) Voer een van de volgende handelingen uit om de pagina Details van de record voor Experience Manager-elementen te openen in de Experience Manager:

   * Ga naar de pagina met het recordtype Maestro van de record waarvan u een koppeling maakt, klik op de naam van een element in het gekoppelde recordveld om het pop-upvenster te openen en klik vervolgens op de knop **Openen** pictogram ![](assets/open-asset-icon.png) om het element te openen.
   * Ga naar de **Experience Manager Assets** Maestro-opnametype kaart in de werkruimte die u oorspronkelijk hebt geselecteerd en klik om de pagina met recordtypen te openen, klik op de naam van een element om het Maestro-bestand te openen **Details** pagina, en klik vervolgens op **Ga naar bron** rechtsboven in het scherm.

     ![](assets/go-to-source-asset-maestro-details-page.png)
   * Ga naar de **Experience Manager Assets** Maestro-opnametype kaart in de werkruimte die u oorspronkelijk hebt geselecteerd en klik op de kaart om de Experience Manager Assets-recordtypepagina te openen, houd de muisaanwijzer boven de naam van een element en klik op de knop **Meer** en klik vervolgens op **Ga naar bron**.

     ![](assets/go-to-source-option-on-table-view.png)

   Het element wordt geopend in Experience Manager Assets.

1. (Optioneel) Klik op de knop **Velden toevoegen** pictogram ![](assets/add-fields-icon.png) in de rechterbovenhoek van de tabelweergave op de Experience Manager Assets-pagina met recordtypen om Experience Managers toe te voegen of te verwijderen.

   >[!NOTE]
   >
   >  De velden die u toevoegt of verwijdert op de Experience Manager Assets-recordtypepagina, worden niet toegevoegd aan of verwijderd uit het Maestro-recordtype dat is gekoppeld aan het Experience Manager-element. De velden zijn alleen zichtbaar op de pagina met alleen-lezen Experience Manager Assets-recordtypen, zodat u ze in Maestro kunt bekijken.

1. (Optioneel en voorwaardelijk) Als u ten minste twee datumvelden hebt toegevoegd aan het aan de Experience Manager gekoppelde element, klikt u op de knop **Weergave** vervolgkeuzemenu op de Experience Manager Assets-recordtypepagina en selecteer de **Tijdlijn** of **Weergave maken** om een tijdlijnweergave te maken.  Zie voor meer informatie [De tijdlijnweergave beheren](/help/quicksilver/maestro/views/manage-the-timeline-view.md).
De aan Experience Manager Assets gekoppelde elementen worden weergegeven in de tijdlijnweergave.