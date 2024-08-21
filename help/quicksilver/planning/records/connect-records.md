---
title: Connect-records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '2287'
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

In dit artikel wordt beschreven hoe u records kunt verbinden. Voor meer algemene informatie over het verbinden van verslagen, zie [ Verbonden verslagenoverzicht ](/help/quicksilver/planning/records/connected-records-overview.md).

U moet eerst twee recordtypen met elkaar verbinden of een recordtype met een objecttype vanuit een andere toepassing. Hiermee maakt u gekoppelde recordvelden. U kunt dan records met elkaar verbinden of records met andere objecten vanuit andere toepassingen verbinden met behulp van de gekoppelde recordvelden.

Het verbinden van records is vergelijkbaar met het verbinden van records met objecten vanuit een andere toepassing.

Voor informatie over het verbinden van verslagtypes met elkaar of aan objecten types van andere toepassingen, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

Voor een voorbeeld van het verbinden van verslagtypes, zie [ Voorbeeld van het verbinden van verslagtypes en verslagen ](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

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

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
   <p>Om Adobe Workfront Planningsverslagen met Experience Manager Assets te verbinden, moet u een vergunning van Adobe Experience Manager Assets hebben en de instantie van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezet. Voor informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>.</p>
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
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   <p>Huidig: Plan</p> 
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
   <p>U kunt machtigingen voor een werkruimte weergeven of vergroten als u alle verbindingen met objecten en velden vanuit andere toepassingen wilt weergeven, ongeacht de toegang die u hebt in de andere toepassing. </p>
   <p>Geef de objecten die u vanuit Workfront of Experience Manager Assets wilt koppelen weer of geef deze machtigingen hoger op. </p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Vereisten voor het verbinden van records

Als u records wilt verbinden met andere records of objecten, moet u over het volgende beschikken:

* Ten minste één werkruimte, recordtype en record.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Werkruimten maken](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [Recordtypen maken](/help/quicksilver/planning/architecture/create-record-types.md)
   * [Records maken](/help/quicksilver/planning/records/create-records.md)

* Verbindingen tussen recordtypen of tussen recordtypen en objecten uit andere toepassingen. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

## Connect-records van Workfront Planning

U kunt records vanuit Workfront Planning verbinden in de volgende gebieden:

* Van een verslag van de Planning in de Planning van Workfront op de verbonden verslaggebieden in de lijstmening.
* Van een verslag van de Planning in de Planning van Workfront in de verslagvoorproef of pagina in de verbonden verslaggebieden.
  <!--
  * From a Planning record in Workfront Planning in the record preview or page in the connected record fields on the Details tab.
  * From a Planning record in the record's preview or page on the Connections tab.-->

### Connect Adobe Workfront Planning-records vanuit de tabelweergave of de recordpagina <!--Details tab of the-->

{{step1-to-planning}}

1. Klik de werkruimte waarvan verslagen u wilt verbinden

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Klik de naam van de mening van de a **Lijst** om het te openen.
1. (Optioneel) Voeg records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
1. (Voorwaardelijk) Nadat u het geselecteerde recordtype met een ander recordtype hebt verbonden, ga naar de verbonden verslagkolom en klik de cel die met het verslag beantwoordt dat u met andere verslagen wilt verbinden.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Voer een van de volgende handelingen uit:

   * Klik in de lijst op de naam van een verbonden record om deze aan de geselecteerde record toe te voegen. De record wordt automatisch toegevoegd.
   * Typ de naam van een record en klik erop wanneer deze in de lijst wordt weergegeven. De record wordt automatisch toegevoegd.

   <!--1. (Optional) If you cannot find a record or an object to connect, and you want to add it, click **+ Add** to add a new record. For more information, see the "Create records as you connect them" in the article [Create records](/help/quicksilver/planning/records/create-records.md).
    
    You can also create projects and portfolios by adding them to a record in the connected record field. You can create only blank projects, without a template by adding them to a record. 
    
     -->

   >[!TIP]
   >
   >    U kunt de pagina van een verslag openen door de naam van het verslag in de mening te klikken, het verbonden verslaggebied te vinden en het gebied tweemaal te klikken (als er reeds verslagen zijn verbonden), of **te klikken verbindt verslagen** (als het gebied leeg is) om verslagen van het verbonden verslag of objecttype toe te voegen.
   >
   >![](assets/connect-records-from-record-page-field.png)

1. (Facultatief) klik **zie allen** om alle verslagen te tonen.

1. (Voorwaardelijk) als u **klikte zie allen** in de vorige stap, **verbind voorwerpen** vakvertoningen.

   ![](assets/connected-objects-table-for-records.png)

1. Typ de naam van een record in het zoekvak en selecteer de naam wanneer de record in de lijst wordt weergegeven

   of

   Selecteer de naam van één of veelvoudige verslagen in de doos, dan klik **verbind voorwerpen**.

   Het volgende wordt toegevoegd:

   * De gekoppelde records worden weergegeven in het gekoppelde recordveld van de record die u in een vorige stap hebt geselecteerd.
   * De gekoppelde velden worden gevuld met de informatie uit de gekoppelde records als u gekoppelde opzoekvelden hebt toegevoegd toen u de recordtypen aansloot.

   Wanneer u de gekoppelde records bijwerkt, worden de gekoppelde velden bijgewerkt voor de records die u automatisch koppelt. U kunt gekoppelde velden niet handmatig bewerken.

   >[!TIP]
   >
   >* We gebruiken onderling gekoppelde velden en opzoekvelden.
   >
   >* Wanneer u ervoor kiest om meerdere records te verbinden wanneer u de recordtypen hebt verbonden, worden de veldwaarden van de meerdere objecten gescheiden door komma&#39;s weergegeven of worden ze samengevoegd volgens de aggregator die u hebt gekozen.

1. (Optioneel) Sluit de pagina met recordtypen en ga naar de werkruimte die u hebt geselecteerd.
1. Klik op de kaart voor het recordtype waarmee u een koppeling hebt gemaakt.

   Bijvoorbeeld, als u het **Campagne** verslag met het verslag van het Product verbond, klik de **kaart van het Product**.

   Het recordtype moet worden geopend in de tabelweergave. Als dat niet het geval is, selecteert u een tabelweergave.

   Bericht dat het **verbonden verslaggebied van de Campagne** {de namen van de campagnes toont u met producten in de het verslagtype van het Product pagina verbond. Wanneer u de Campagnegegevens bijwerkt, wordt het aan Campagne gekoppelde recordveld voor het type productrecord automatisch bijgewerkt.

### Connect Adobe Workfront Planning-records vanuit de tabelweergave of de <!--Details tab of the--> recordpagina verbinden met Workfront-objecten

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Nadat u een verbinding hebt gemaakt tussen een recordtype en een Workfront-objecttype, kunt u afzonderlijke records verbinden met objecten in Workfront. De Workfront-velden die u hebt verbonden, worden automatisch ingevuld in de records waarvan u de objecten koppelt.

>[!NOTE]
>
>U kunt vanuit Workfront geen verbinding maken tussen Workfront-objecttypen en Workfront Planning-recordtypen.


{{step1-to-planning}}

1. Klik de werkruimte waarvan verslagen u wilt verbinden.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer a **de mening van de Lijst** van het **drop-down menu van de Mening**.

1. Klik **Nieuw verslag** om individuele verslagen aan het verslagtype toe te voegen dat u selecteerde. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
1. (Voorwaardelijk) Nadat u het geselecteerde recordtype hebt verbonden met een Workfront-objecttype, gaat u naar de gekoppelde objectkolom en dubbelklikt u op de cel die overeenkomt met de record die u wilt koppelen aan objecten uit Workfront.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Voer een van de volgende handelingen uit:

   * Klik op een object in de lijst om het toe te voegen aan de geselecteerde record. Objecten worden in alfabetische volgorde weergegeven. Het object wordt automatisch toegevoegd.
   * Typ de naam van een object en klik erop wanneer het wordt weergegeven in de lijst. Het object wordt automatisch toegevoegd.

   >[!TIP]
   >
   >U kunt de pagina van een verslag van de mening openen, het verbonden verslaggebied tweemaal klikken, of **verbinden** op het gebied klikken om voorwerpen van het verbonden objecten type toe te voegen.

1. (Facultatief) klik **zie allen** om alle voorwerpen te tonen u minstens toestemmingen aan mening hebt.

1. (Voorwaardelijk) als u **klikte zie allen** in de vorige stap, **verbind voorwerpen** vakvertoningen.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Typ de naam van een Workfront-object in het zoekvak en selecteer het vervolgens wanneer het in de lijst wordt weergegeven

   of

   Selecteer de naam van één of veelvoudige voorwerpen in de doos, dan klik **verbind voorwerpen**.

   >[!IMPORTANT]
   >
   >* U kunt alleen Workfront-objecten toevoegen die u kunt bekijken.
   >
   >* Nadat u Workfront-objecten hebt toegevoegd, kan iedereen met Weergave- of hogere machtigingen de Workfront-objecten en hun veldgegevens weergeven, ongeacht de machtigingen of toegang tot deze objecten in Workfront.

   Het volgende wordt toegevoegd:

   * De geselecteerde Workfront-objecten worden toegevoegd aan het gekoppelde recordveld.
   * Als u deze hebt toegevoegd toen u het recordtype verbond met Workfront, worden de gekoppelde velden (of de opzoekvelden) van de Workfront-objecten automatisch gevuld met informatie van Workfront.

   Voor meer informatie over het verbinden van verslagtypes met voorwerpen van een andere toepassing, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Optioneel) Klik op de naam van een Workfront-object dat is verbonden met een Workfront-planningsrecord in het gekoppelde veld van een tabelweergave of vanuit het gekoppelde veld op de recordpagina.

   Hiermee wordt het Workfront-object in Workfront geopend als u ten minste weergavemachtigingen voor het object hebt.

   >[!TIP]
   >
   >* Wanneer u ervoor kiest om meerdere records te verbinden bij het verbinden van de recordtypen, worden de waarden van de opzoekvelden gescheiden door komma&#39;s weergegeven of worden ze geaggregeerd volgens de aggregator die u hebt gekozen.
   >
   >* Er wordt geen gekoppeld recordveld gemaakt voor de gekoppelde Workfront-objecten in Workfront.

1. (Facultatief) van de lijstmening van het verslagtype, houd over de kolomkopbal van het verbonden voorwerp van Workfront, en klik het drop-down menu, dan klik **uitgezocht gebieden** uitgeven.

1. Voeg de objecten van Workfront gebieden van het **Niet geselecteerde gebied** toe

   of

   Verwijder de objecten van Workfront gebieden van het **Geselecteerde gebied**.

   Hiermee voegt u gekoppelde velden toe aan of verwijdert u deze uit de planningsrecords van Workfront. De informatie die aan de verwijderde velden is gekoppeld, blijft in Workfront.


### Connect Workfront Planning-records vanuit de tabelweergave of de <!--Details tab of the--> recordpagina verbinden met Adobe Experience Manager-objecten

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>U moet een Adobe Experience Manager Assets-licentie hebben en het Workfront-exemplaar van uw organisatie moet zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console om Workfront Planning-records te kunnen verbinden met Adobe Experience Manager Assets.
>
>Als u vragen over het aan boord gaan aan Adobe Admin Console hebt, zie [ Adobe Verenigde Veelgestelde vragen van de Ervaring ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Nadat u een verbinding hebt gemaakt tussen een recordtype en Adobe Experience Manager Assets, kunt u afzonderlijke records verbinden met Experience Manager-elementen. De elementvelden die u vanaf Experience Manager Assets hebt verbonden toen u de verbinding maakte, worden automatisch ingevuld in het recordtype waarvan u een koppeling hebt gemaakt.

>[!NOTE]
>
>De verslagen van de planning en hun gebieden zijn toegankelijk van Experience Manager Assets wanneer uw beheerder van Workfront de meta-gegevensafbeelding door de integratie tussen Workfront en Adobe Experience Manager Assets vormt. Voor meer informatie, zie [ activa meta-gegevensafbeelding tussen Adobe Workfront en Experience Manager Assets ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en) vormen.

Records verbinden met AEM elementen:

{{step1-to-planning}}

1. Klik de werkruimte waarvan verslagen u wilt verbinden.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer a **de mening van de Lijst** van de **drop-down menu van de Mening** in de hoger-juiste hoek van de verslagtype pagina.

1. (Facultatief) klik **Nieuw verslag** om nieuwe verslagen aan het verslagtype toe te voegen dat u selecteerde. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
1. (Voorwaardelijk) Nadat u het geselecteerde verslagtype met Experience Manager Assets aansloot, ga naar de verbonden objecten kolom en beweegt over de cel die aan het verslag beantwoordt dat u met andere voorwerpen van Experience Manager wilt verbinden, dan **+** pictogram klikken.

   >[!TIP]
   >
   >  U kunt op het pictogram **+** in het gekoppelde objectveld in de recordpagina klikken om elementen aan de record te koppelen.

   De **Uitgezochte Assets** vakvertoningen. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Klik om een aantal van de volgende typen elementen te selecteren:

   * Afbeeldingen
   * Mappen

   U kunt meerdere elementen selecteren.

   >[!IMPORTANT]
   >
   > U kunt alleen elementen verbinden die u in Experience Manager kunt bekijken. Zodra verbonden, kunnen alle gebruikers van de Planning van Workfront de activa in de Planning van Workfront, ongeacht hun toegang in Experience Manager Assets bekijken.

1. Klik **Uitgezocht**. <!-- we might change this to Connect-->

   Het volgende wordt toegevoegd:

   * De geselecteerde elementen van de Experience Manager worden toegevoegd aan het gekoppelde recordveld.
   * In de gekoppelde velden (of opzoekvelden) wordt informatie uit de aan de Experience Manager gekoppelde elementen ingevuld.

     Eventuele bestaande informatie uit de velden van de elementen van de Experience Manager wordt automatisch weergegeven in de gekoppelde of opzoekvelden.

     >[!TIP]
     >
     >* Wanneer u ervoor kiest om meerdere records te verbinden wanneer u de recordtypen verbindt, worden de waarden van de meerdere objecten gescheiden door komma&#39;s of samengevoegd volgens de door u gekozen aggregator weergegeven.
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

1. (Facultatief) om de pagina van het verslag van de activa van de Experience Manager in Experience Manager te openen, ga naar de verslagtype pagina van het verslag u van verbindt, klik de naam van een activa in het verbonden verslaggebied om het pop-up venster te openen, dan klik **Open in AEM** pictogram ![](assets/open-asset-icon.png) om de activa te openen.

   Hiermee opent u de Experience Manager-asset in Adobe Experience Manager Assets.

1. (Facultatief) van de lijstmening van het verslagtype, houd over de kolomkopbal van de verbonden activa van de Experience Manager, en klik het drop-down menu, dan klik **uitgezocht gebieden** uitgeven.

1. Voeg de objecten van Experience Manager Assets gebieden van het **Niet geselecteerde gebied** toe

   of

   Verwijder de objecten van Workfront gebieden van het **Geselecteerde gebied**.

   Hiermee voegt u gekoppelde velden toe aan of verwijdert u deze uit de records. De informatie die aan de verwijderde velden is gekoppeld, blijft in Adobe Experience Assets.

<!--
### Connect Workfront Planning records from the Connections tab of the record page

1. Go to any view of a record type that has been connected to other record types or object types from other applications. 
1. Follow the steps described in the previous subsections to find a record in the view that you want to connect with other records or objects. 
1. Click the name of a record. 

    The preview page opens. 
1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) to open the record's page. 
1. Click the **Connections** tab in the record's preview or page. 

    ![](assets/connections-tab-on-record-in-workfront-planning.png)

    All record or object types that are linked to the selected record type display as sections. Connected records or objects display under their record or object type names on cards. 

    >[!TIP]
    >
    >    Only connected records that have individual records connected display by default.

1. (Optional) Click **Show all connections** to show all connected record types, including the ones without connected records. 

1. (Optional) Click the downward-pointing arrow to the left of a section to collapse it. 

1. (Conditional) If there are records or objects connected to the selected record, click **Connect** to add more records or objects of the same type. 
    The Connect button does not display if there are no records currently connected to the selected record. 
1. Follow the steps describes in the previous sections to connect records from Workfront Planning or objects from Workfront or AEM Assets. 
    The records and objects are added immediately.
1. (Optional) Hover over the connected card of a record or object, then click the **Disconnect record** icon to disconnect it from the selected record. 

    ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

    The record is immediately disconnected from all areas of Workfront Planning or from other applications where it might show as connected. Any lookup field values are also removed. 

-->

## Connect-records van Workfront-objecten

U moet het volgende hebben om de verslagen van de Planning van Workfront van de voorwerpen van Workfront te verbinden:

* Verbindingen tussen recordtypen en Workfornt-objecttypen die zijn ingesteld in Workfront Planning.
* Uw Workfront of groepsbeheerder moet de sectie Planning toevoegen aan de Workfront-objecttypen die verbinding kunnen maken met de recordtypen voor planning in uw lay-outsjabloon.

Voor meer informatie, zie [ verslagen in de sectie van de Planning van de voorwerpen van Adobe Workfront beheren ](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
