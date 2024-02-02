---
title: Connect-records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '2396'
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
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connect-records

{{maestro-important-intro}}

U kunt Adobe Maestro-records met elkaar of met objecten van andere toepassingen verbinden.

U moet eerst twee recordtypen met elkaar verbinden of een recordtype met een objecttype vanuit een andere toepassing. Hiermee maakt u gekoppelde recordvelden. U kunt records vervolgens met elkaar verbinden of records met andere objecten vanuit een andere toepassing verbinden met behulp van de gekoppelde recordvelden.

Voor informatie over het verbinden van verslagtypes met elkaar of aan objecten types van andere toepassingen, zie [Verbind recordtypen](../architecture/connect-record-types.md).

Zie voor een voorbeeld van het verbinden van recordtypen [Voorbeeld van het verbinden van recordtypen en records](../architecture/example-connect-record-types-and-records.md).

U kunt het volgende verbinden:

* Operationele Maestro-gegevens
* Operationele Maestro-gegevens met taxonomische gegevens
* Maestro taxonomies
* Operationele Maestro-records of taxonomieën met objecten uit andere toepassingen.

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

* Nadat u recordtypes verbindt, tonen de verbonden verslagtypes als verbonden verslaggebieden in de lijst van de verslagtypes zij van en op de pagina van Details van de verslagen worden verbonden zij van en verbonden.
* U kunt records en objecten van de gekoppelde record- en objecttypen bladeren en deze toevoegen vanuit de gekoppelde recordvelden.
* U kunt velden van de gekoppelde recordtypen toevoegen aan de tabel van het recordtype waarvan u een koppeling maakt.
* U kunt de waarden van gekoppelde velden niet handmatig bijwerken in de records waarvan u een koppeling maakt.

  De waarden van de verbonden gebieden van de verbonden verslagen bevolken het verslag Maestro dat u van automatisch van de werkruimte van Maestro verbindt u of van de derdetoepassing vormt.

* Iedereen met toegang tot Maestro en Mening of hogere toestemmingen aan de werkruimte kan de verbindingen zien die u tussen verslagen Maestro of tussen verslagen Maestro en de voorwerpen van andere toepassingen maakt. Ze kunnen verbonden records en objecten weergeven, ongeacht hun machtigingen voor de externe toepassingen waarmee u verbinding maakt.
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
1. Van een verslag in de lijstmening wordt vermeld, ga naar de verbonden verslagkolom en klik binnen het verbonden verslaggebied, dan klik **+** pictogram.

   ![](assets/connected-objects-table-for-records.png)

   >[!TIP]
   >
   >    U kunt de pagina Details van een record openen, het gekoppelde recordveld zoeken en op de knop **+** in het veld om records van het aangesloten record- of objecttype toe te voegen.

   De **Objecten verbinden** wordt weergegeven.

1. Typ de naam van een record in het zoekvak en selecteer de naam wanneer de record in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere records in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   Het volgende wordt toegevoegd:

   * De gekoppelde records worden weergegeven in het gekoppelde recordveld van de record die u in stap 6 hebt geselecteerd. <!--accurate?--> Wanneer u de gekoppelde records bijwerkt, worden de gekoppelde velden bijgewerkt voor de records die u automatisch koppelt. U kunt gekoppelde velden niet handmatig bewerken.

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

>[!NOTE]
>
>U kunt Workfront-objecten niet verbinden met Maestro-records uit Workfront.


{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een **Tabel** van de **Weergave** vervolgkeuzelijst.

1. Voeg afzonderlijke records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. (Voorwaardelijk) Als u het geselecteerde recordtype hebt verbonden met een Workfront-object, gaat u naar de kolom met het gekoppelde object en plaatst u de cursor boven de cel die overeenkomt met de record die u wilt koppelen aan objecten uit Workfront. Klik vervolgens op de knop **+** pictogram.

   De **Objecten verbinden** wordt weergegeven.

   ![](assets/connect-objects-box-to-select-projects.png)

   >[!TIP]
   >
   >    U kunt de pagina Details van een record openen, het gekoppelde recordveld zoeken en op de knop **+** in het veld om objecten van het type verbonden object toe te voegen.

   Zie voor meer informatie over het verbinden van recordtypen met objecten uit een externe toepassing [Verbind recordtypen](../architecture/connect-record-types.md).

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
   * Een pagina met alleen-lezen details in Maestro voor het gekoppelde Workfront-object. U kunt tot deze pagina toegang hebben door de naam van een project van het verbonden gebied van een verslag van Maestro te klikken. Ga verder met stap 8. <!--accurate?-->

     Als u bijvoorbeeld een koppeling naar een Workfront-project maakt, worden er in Maestro de pagina&#39;s Details van die projecten gemaakt.

     >[!IMPORTANT]
     >
     > De pagina met alleen-lezen Workfront-objectdetails wordt alleen gemaakt wanneer afzonderlijke projecten aan Maestro-records worden toegevoegd. Als u een verbinding maakt tussen een Maestro-recordtype en een Workfront-objecttype, wordt het Workfront-recordtype niet gemaakt in Maestro.

1. (Optioneel) Klik op de naam van een Workfront-object dat is verbonden met een Maestro-record in het gekoppelde veld van een tabelweergave of in het dialoogvenster **Details** pagina van het verslag-Maestro.

   Dit opent de alleen-lezen Maestro **Details** pagina voor het gekoppelde Workfront-object. De velden die u als opzoekvelden hebt geselecteerd toen u het recordtype koppelde aan het Workfront-object, worden weergegeven op de pagina Details.

   >[!TIP]
   >
   >* Als u de instelling Meerdere records toestaan hebt ingeschakeld, worden de waarden van de meerdere objecten gescheiden door komma&#39;s weergegeven of worden ze samengevoegd volgens de gekozen aggregator.
   >
   >* Er wordt geen gekoppeld recordveld gemaakt voor de gekoppelde Workfront-objecten in Workfront.

1. (Optioneel) Als u het gekoppelde Workfront-object in Workfront wilt openen, klikt u op **Ga naar bron** in de rechterbovenhoek van de pagina Details van het Workfront-object.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Hiermee wordt de Workfront-objectpagina geopend als u minstens weergavemachtigingen hebt om het object weer te geven. U kunt informatie over het Workfront-object bewerken als u hiervoor gemachtigd bent.

1. (Optioneel) Houd de muisaanwijzer in de tabelweergave van het recordtype Maestro boven de kolomkop van het gekoppelde Workfront-object en klik op het vervolgkeuzemenu en klik vervolgens op **Opzoekvelden bewerken**.

1. Workfront-objectvelden toevoegen vanuit het menu **Niet-geselecteerde velden** gebied

   of

   Workfront-objectvelden verwijderen uit het dialoogvenster **Geselecteerde velden** gebied.

   Hiermee voegt u gekoppelde velden toe aan of verwijdert u deze uit de Maestro-records. De informatie die aan de verwijderde velden is gekoppeld, blijft in Workfront.


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

1. (Optioneel) Klik op **Nieuwe record** om nieuwe records toe te voegen aan het geselecteerde recordtype. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. (Voorwaardelijk) Als u het geselecteerde recordtype hebt verbonden met Experience Manager Assets, gaat u naar de gekoppelde objectkolom en beweegt u de cursor over de cel die overeenkomt met de record die u vanuit de Experience Manager wilt koppelen met andere objecten. Klik vervolgens op de knop **+** pictogram.

   >[!TIP]
   >
   >  U kunt toevoegen klik op **+** op het gekoppelde objectveld op de pagina Details van de Maestro-record om elementen aan de record te koppelen.

   De **Elementen selecteren** wordt weergegeven. <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   Voor meer informatie over het verbinden van verslagtypes met objecten types van een derdetoepassing, zie [Verbind recordtypen](../architecture/connect-record-types.md).

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
   * Een pagina met alleen-lezen details in Maestro voor het gekoppelde Experience Manager Assets-object. U kunt deze pagina openen door op de naam van een element in het gekoppelde veld van een Maestro-record te klikken. Ga verder met stap 8. <!--accurate?-->

     >[!IMPORTANT]
     >
     > De pagina Experience Manager Assets Details (alleen-lezen) van het gekoppelde recordtype wordt alleen gemaakt wanneer afzonderlijke elementen aan Maestro-records worden toegevoegd. Als u een verbinding maakt tussen een Maestro-recordtype en Experience Manager Assets, wordt het Experience Manager Assets-recordtype niet gemaakt.

     Eventuele bestaande informatie uit de velden van de elementen van de Experience Manager wordt weergegeven in de gekoppelde of opzoekvelden.

     >[!TIP]
     >
     >
     >* Als u de instelling Meerdere records toestaan hebt ingeschakeld, worden de waarden van de meerdere objecten gescheiden door komma&#39;s weergegeven.
     >
     >* Er wordt geen gekoppeld recordveld naar de Maestro-gekoppelde records gemaakt voor de gekoppelde Experience Manager-elementen in de Experience Manager Assets-toepassing.


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

1. (Optioneel) Als u de pagina Details van record voor Experience Manager-elementen in de Experience Manager wilt openen, gaat u naar de pagina Type record van de record waarvan u een koppeling maakt, klikt u op de naam van een element in het gekoppelde recordveld om het pop-upvenster te openen en klikt u vervolgens op de knop **Openen** pictogram ![](assets/open-asset-icon.png) om het element te openen.

   Hierdoor worden de elementen van de Experience Manager geopend **Details** pagina in Maestro.

1. Klikken **Ga naar bron** rechtsboven in het scherm.

   ![](assets/go-to-source-asset-maestro-details-page.png)

   Hierdoor wordt het element in Adobe Experience Manager Assets geopend als u toegang hebt om het te bekijken. U kunt het element in deze toepassing bijwerken als u hiervoor gemachtigd bent.

1. (Optioneel) Houd de muisaanwijzer boven de kolomkop van het gekoppelde Experience Manager-element in de tabelweergave van het maestro-recordtype en klik op het vervolgkeuzemenu en klik vervolgens op **Opzoekvelden bewerken**.

1. Experience Manager Assets-objectvelden toevoegen vanuit het menu **Niet-geselecteerde velden** gebied

   of

   Workfront-objectvelden verwijderen uit het dialoogvenster **Geselecteerde velden** gebied.

   Hiermee voegt u gekoppelde velden toe aan of verwijdert u deze uit de Maestro-records. De informatie die aan de verwijderde velden is gekoppeld, blijft in Adobe Experience Assets.
