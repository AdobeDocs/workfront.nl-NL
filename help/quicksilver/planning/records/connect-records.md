---
title: Connect-records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 160bcc8796666c9615ebe8ead18813b96be26a71
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting records to one another, you can also connect records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connect-records

{{planning-important-intro}}

U kunt Adobe Workfront-planningsrecords met elkaar of met objecten van andere toepassingen verbinden.

U moet eerst twee recordtypen met elkaar verbinden of een recordtype met een objecttype vanuit een andere toepassing. Hiermee maakt u gekoppelde recordvelden. U kunt dan records met elkaar verbinden of records met andere objecten vanuit andere toepassingen verbinden met behulp van de gekoppelde recordvelden.

Het verbinden van records is vergelijkbaar met het verbinden van records met objecten vanuit een andere toepassing.

Voor informatie over het verbinden van verslagtypes met elkaar of aan objecten types van andere toepassingen, zie [Verbind recordtypen](/help/quicksilver/planning/architecture/connect-record-types.md).

Zie voor een voorbeeld van het verbinden van recordtypen [Voorbeeld van het verbinden van recordtypen en records](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

U kunt het volgende verbinden:

* Adobe Workfront-planningsrecords
* Adobe Workfront Planning registreert met voorwerpen van andere toepassingen.

  U kunt records verbinden met objecten van de onderstaande typen vanuit de volgende toepassingen:

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
   <p>Om Adobe Workfront Planningsverslagen met Experience Manager Assets te verbinden, moet u een vergunning van Adobe Experience Manager Assets hebben en de instantie van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezet. Zie voor meer informatie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience voor Workfront</a>.</p>
   </td>
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
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren voor een werkruimte om records te verbinden </p>  
   <p>U kunt machtigingen voor een werkruimte weergeven of vergroten als u alle verbindingen met objecten en velden vanuit andere toepassingen wilt weergeven, ongeacht de toegang die u hebt in andere toepassingen. </p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="/help/quicksilver/planning/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Overwegingen bij het verbinden van records

* Nadat u recordtypen hebt verbonden, worden de verbonden recordtypen weergegeven als gekoppelde recordvelden in de tabel met de recordtypen waarvan ze zijn gekoppeld en op de recordpagina&#39;s.
* U kunt records en objecten van de gekoppelde record- en objecttypen bladeren en deze toevoegen vanuit de gekoppelde recordvelden.
* U kunt velden van de gekoppelde recordtypen toevoegen aan de tabel van het recordtype waarvan u een koppeling maakt.
* U kunt de waarden van gekoppelde velden niet handmatig bijwerken in de records waarvan u een koppeling maakt.

  De waarden van de gekoppelde velden van de gekoppelde records vullen de Workfront-planningsrecord die u automatisch koppelt vanuit de oorspronkelijke record of het oorspronkelijke object.

* Iedereen met toegang tot de Planning van Workfront en Mening of hogere toestemmingen aan de werkruimte kan de verbindingen zien die u tussen verslagen of tussen verslagen en andere voorwerpen van toepassingen maakt. Ze kunnen verbonden records en objecten bekijken, ongeacht hun machtigingen in de toepassingen waarmee u verbinding maakt.
* U kunt de verbindingen van alle anderen weergeven en bewerken als u beheerdersmachtigingen hebt voor de werkruimte waar de verbonden records zich bevinden.
* U kunt één record verbinden met een of meerdere objecten vanuit een andere toepassing.
* Als u records wilt koppelen aan andere records of objecten, moet u over het volgende beschikken:

   * Ten minste één werkruimte, recordtype en record.

     Raadpleeg de volgende artikelen voor meer informatie:

      * [Werkruimten maken](/help/quicksilver/planning/architecture/create-workspaces.md)
      * [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)
      * [Records maken](/help/quicksilver/planning/records/create-records.md)

   * Verbindingen tussen recordtypen of tussen recordtypen en objecten uit andere toepassingen. Zie voor meer informatie [Verbind recordtypen](/help/quicksilver/planning/architecture/connect-record-types.md)
* U kunt objecten van Workfront verbinden met Workfront-planningsrecords in de volgende gebieden:
   * Uit een planningsrecord in Workfront Planning.
   * Vanuit het gedeelte Planning van een Workfront-object.

## Connect-records van Workfront Planning

### Connect Adobe Workfront-planningsrecords

{{step1-to-planning}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. (Optioneel) Voeg records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](/help/quicksilver/planning/records/create-records.md).
1. (Voorwaardelijk) Nadat u het geselecteerde recordtype met een ander recordtype hebt verbonden, ga naar de verbonden verslagkolom en klik de cel die met het verslag beantwoordt dat u met andere verslagen wilt verbinden.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Voer een van de volgende handelingen uit:

   * Klik in de lijst op de naam van een verbonden record om deze aan de geselecteerde record toe te voegen. De record wordt automatisch toegevoegd.
   * Typ de naam van een record en klik erop wanneer deze in de lijst wordt weergegeven. De record wordt automatisch toegevoegd.
   * Klikken **Alles bekijken** alle records weergeven.

1. (Voorwaardelijk) Als u hebt geklikt **Alles selecteren** in de vorige stap **Objecten verbinden** wordt weergegeven.

   ![](assets/connected-objects-table-for-records.png)

1. Typ de naam van een record in het zoekvak en selecteer de naam wanneer de record in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere records in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   >[!TIP]
   >
   >    U kunt de pagina van een record openen, het gekoppelde recordveld zoeken en op **Connect-records** in het veld om records van het verbonden record- of objecttype toe te voegen.
   >
   >![](assets/connect-records-from-record-page-field.png)

   Het volgende wordt toegevoegd:

   * De gekoppelde records worden weergegeven in het gekoppelde recordveld van de record die u in stap 6 hebt geselecteerd. <!--accurate?-->
   * De gekoppelde velden worden gevuld met de informatie uit de gekoppelde records als u gekoppelde opzoekvelden hebt toegevoegd toen u de recordtypen aansloot.

   Wanneer u de gekoppelde records bijwerkt, worden de gekoppelde velden bijgewerkt voor de records die u automatisch koppelt. U kunt gekoppelde velden niet handmatig bewerken.

   >[!TIP]
   >
   >* We gebruiken onderling gekoppelde velden en opzoekvelden.
   >
   >* Als u de optie **Meerdere records toestaan** Wanneer u de recordtypen aansluit, worden de waarden van velden voor de meerdere geselecteerde objecten weergegeven met een komma van elkaar gescheiden of samengevoegd op basis van de gekozen aggregator.

1. (Optioneel) Sluit de pagina met recordtypen en ga naar de werkruimte die u hebt geselecteerd.
1. Klik op de kaart voor het recordtype waarmee u een koppeling hebt gemaakt.

   Als u bijvoorbeeld verbinding hebt gemaakt met de **Campagne** record met de productrecord, klik op de knop **Product** kaart.

   Het recordtype moet worden geopend in de tabelweergave. Als dat niet het geval is, selecteert u een tabelweergave.

   Let erop dat de **Campagne** In het gekoppelde recordveld worden de namen weergegeven van de campagnes die u aan producten hebt gekoppeld op de pagina Type productrecord. Wanneer u de Campagnegegevens bijwerkt, wordt het aan Campagne gekoppelde recordveld voor het type productrecord automatisch bijgewerkt.

### Adobe Workfront-planningsrecords verbinden met Workfront-objecten

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Nadat u een verbinding hebt gemaakt tussen een recordtype en een Workfront-objecttype, kunt u afzonderlijke records verbinden met objecten in Workfront. De Workfront-velden die u hebt verbonden, worden automatisch ingevuld in de records waarvan u de objecten koppelt.

>[!NOTE]
>
>U kunt vanuit Workfront geen verbinding maken tussen Workfront-objecttypen en Workfront Planning-recordtypen.


{{step1-to-planning}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** vervolgkeuzelijst.

1. Klikken **Nieuwe record**  om afzonderlijke records toe te voegen aan het geselecteerde recordtype. Zie voor meer informatie [Records maken](/help/quicksilver/planning/records/create-records.md).
1. (Voorwaardelijk) Nadat u het geselecteerde recordtype hebt verbonden met een Workfront-objecttype, gaat u naar de gekoppelde objectkolom en dubbelklikt u op de cel die overeenkomt met de record die u wilt koppelen aan objecten uit Workfront.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Voer een van de volgende handelingen uit:

   * Klik op een object in de lijst om het toe te voegen aan de geselecteerde record. Objecten worden in alfabetische volgorde weergegeven. Het object wordt automatisch toegevoegd.
   * Typ de naam van een object en klik erop wanneer het wordt weergegeven in de lijst. Het object wordt automatisch toegevoegd.
   * Klikken **Alles bekijken** om alle objecten weer te geven die u ten minste gemachtigd bent te bekijken.

1. (Voorwaardelijk) Als u hebt geklikt **Alles bekijken** in de vorige stap **Objecten verbinden** wordt weergegeven.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Typ de naam van een Workfront-object in het zoekvak en selecteer het vervolgens wanneer het in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere objecten in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   >[!IMPORTANT]
   >
   >* U kunt alleen Workfront-objecten toevoegen die u kunt bekijken.
   >
   >* Nadat u Workfront-objecten hebt toegevoegd, kan iedereen met Weergave- of hogere machtigingen de Workfront-objecten en hun veldgegevens weergeven, ongeacht de machtigingen of toegang tot deze objecten in Workfront.

   Het volgende wordt toegevoegd:

   * De geselecteerde Workfront-objecten worden toegevoegd aan het gekoppelde recordveld.
   * Als u deze hebt toegevoegd toen u het recordtype verbond met Workfront, worden de gekoppelde velden (of de opzoekvelden) van de Workfront-objecten automatisch gevuld met informatie van Workfront.

   >[!TIP]
   >
   >U kunt de pagina van een record openen, het gekoppelde recordveld zoeken en op de knop **+** in het veld om objecten van het type verbonden object toe te voegen.

   Voor meer informatie over het verbinden van verslagtypes met voorwerpen van een andere toepassing, zie [Verbind recordtypen](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Optioneel) Klik op de naam van een Workfront-object dat is verbonden met een Workfront-planningsrecord in het gekoppelde veld van een tabelweergave of vanuit het gekoppelde veld op de recordpagina.

   Hierdoor wordt de pagina met alleen-lezen Workfront-planningsrecords geopend voor het gekoppelde Workfront-object. De velden die u als opzoekvelden hebt geselecteerd toen u het recordtype koppelde aan de weergave van het Workfront-object op de recordpagina Workfront Planning.

   >[!TIP]
   >
   >* Wanneer u de instelling Meerdere records toestaan inschakelt, worden de waarden van de opzoekvelden weergegeven, gescheiden door komma&#39;s, of worden ze samengevoegd volgens de aggregator die u hebt gekozen.
   >
   >* Er wordt geen gekoppeld recordveld gemaakt voor de gekoppelde Workfront-objecten in Workfront.

1. (Optioneel) Als u het gekoppelde Workfront-object in Workfront wilt openen, klikt u op **Ga naar bron** in de rechterbovenhoek van de recordpagina van het Workfront-object.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Hiermee wordt de Workfront-objectpagina geopend als u minstens weergavemachtigingen hebt om het object weer te geven. U kunt informatie over het Workfront-object bewerken als u hiervoor gemachtigd bent.

1. (Optioneel) Houd de muisaanwijzer in de tabelweergave van het recordtype boven de kolomkop van het gekoppelde Workfront-object en klik op het vervolgkeuzemenu en klik vervolgens op **Opzoekvelden bewerken**.

1. Workfront-objectvelden toevoegen vanuit het menu **Niet-geselecteerde velden** gebied

   of

   Workfront-objectvelden verwijderen uit het dialoogvenster **Geselecteerde velden** gebied.

   Hiermee voegt u gekoppelde velden toe aan of verwijdert u deze uit de planningsrecords van Workfront. De informatie die aan de verwijderde velden is gekoppeld, blijft in Workfront.


### Workfront-planningsrecords verbinden met Adobe Experience Manager-objecten

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>U moet een Adobe Experience Manager Assets-licentie hebben en het Workfront-exemplaar van uw organisatie moet zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console om Workfront Planning-records te kunnen verbinden met Adobe Experience Manager Assets.
>
>Als u vragen hebt over instaptoegang tot de Adobe Admin Console, raadpleegt u de [Veelgestelde vragen over Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Nadat u een verbinding hebt gemaakt tussen een recordtype en Adobe Experience Manager Assets, kunt u afzonderlijke records verbinden met Experience Manager-elementen. De elementvelden die u vanaf Experience Manager Assets hebt verbonden toen u de verbinding maakte, worden automatisch ingevuld in het recordtype waarvan u een koppeling hebt gemaakt.

{{step1-to-planning}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.

1. (Optioneel) Klik op **Nieuwe record** om nieuwe records toe te voegen aan het geselecteerde recordtype. Zie voor meer informatie [Records maken](/help/quicksilver/planning/records/create-records.md).
1. (Voorwaardelijk) Nadat u het geselecteerde recordtype met Experience Manager Assets hebt verbonden, ga naar de verbonden objecten kolom en beweegt over de cel die met het verslag beantwoordt dat u met andere voorwerpen van Experience Manager wilt verbinden, dan klik **+** pictogram.

   >[!TIP]
   >
   >  U kunt toevoegen klik op **+** op het gekoppelde objectveld in de recordpagina om elementen aan de record te koppelen.

   De **Elementen selecteren** wordt weergegeven. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Klik om een aantal van de volgende typen elementen te selecteren:

   * Afbeeldingen
   * Mappen

   U kunt meerdere elementen selecteren.

   >[!IMPORTANT]
   >
   > U kunt alleen elementen verbinden die u in Experience Manager kunt bekijken. Zodra verbonden, kunnen alle gebruikers van de Planning van Workfront de activa in de Planning van Workfront, ongeacht hun toegang in Experience Manager Assets bekijken.

1. Klikken **Selecteren**. <!-- we might change this to Connect-->

   Het volgende wordt toegevoegd:

   * De geselecteerde elementen van de Experience Manager worden toegevoegd aan het gekoppelde recordveld.
   * In de gekoppelde velden (of opzoekvelden) wordt informatie uit de aan de Experience Manager gekoppelde elementen ingevuld.

     Eventuele bestaande informatie uit de velden van de elementen van de Experience Manager wordt automatisch weergegeven in de gekoppelde of opzoekvelden.

     >[!TIP]
     >
     >* Als u de instelling Meerdere records toestaan hebt ingeschakeld, worden de waarden van de meerdere objecten gescheiden door komma&#39;s of samengevoegd volgens de gekozen aggregator weergegeven.
     >
     >* Een gekoppeld recordveld naar de aan Workfront Planning gekoppelde records wordt niet gemaakt voor de gekoppelde Experience Manager-elementen in de Experience Manager Assets-toepassing.

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

1. (Optioneel) Als u de recordpagina met Experience Manager-elementen in Experience Manager wilt openen, gaat u naar de pagina met recordtypen van de record waarvan u een koppeling maakt, klikt u op de naam van een element in het gekoppelde recordveld om het pop-upvenster te openen en klikt u vervolgens op de knop **Openen** pictogram ![](assets/open-asset-icon.png) om het element te openen.

   Hiermee opent u de Experience Manager-asset in Adobe Experience Manager Assets.

1. (Optioneel) Houd de muisaanwijzer in de tabelweergave van het recordtype boven de kolomkop van het gekoppelde Experience Manager-element en klik op het vervolgkeuzemenu en klik vervolgens op **Opzoekvelden bewerken**.

1. Experience Manager Assets-objectvelden toevoegen vanuit het menu **Niet-geselecteerde velden** gebied

   of

   Workfront-objectvelden verwijderen uit het dialoogvenster **Geselecteerde velden** gebied.

   Hiermee voegt u gekoppelde velden toe aan of verwijdert u deze uit de records. De informatie die aan de verwijderde velden is gekoppeld, blijft in Adobe Experience Assets.

## Connect-records van Workfront-objecten

U moet het volgende hebben om de verslagen van de Planning van Workfront van de voorwerpen van Workfront te verbinden:

* Verbindingen tussen recordtypen en Workfornt-objecttypen.
* Ten minste één verbinding tussen een record en een Workfront-object.
* Uw Workfront of groepsbeheerder moet de sectie Planning toevoegen aan de Workfront-objecttypen die verbinding kunnen maken met de recordtypen voor planning.

Zie voor meer informatie [Records beheren in het gedeelte Planning van Adobe Workfront-objecten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
