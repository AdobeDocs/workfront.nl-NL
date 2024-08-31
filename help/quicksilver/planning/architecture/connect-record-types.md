---
title: Recordtypen verbinden
description: Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Adobe Workfront Planning-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 78a54ec94dd5a5746144e99e14c622e8b3a7ea71
workflow-type: tm+mt
source-wordcount: '2137'
ht-degree: 0%

---


# Verbind recordtypen

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

U kunt recordtypen met elkaar verbinden of typen opnemen met objecttypen van andere toepassingen.

In dit artikel wordt beschreven hoe u twee recordtypen van Workfront Planning of een recordtype van Workfront Planning kunt verbinden met een object van een andere toepassing.

Nadat u de verbinding tussen verslagen of objecten types vestigt, kunt u individuele verslagen met elkaar verbinden, en vertoningsgebieden van het verbonden verslag of objecten types op een verslag van de Planning van Workfront tonen.

Voor algemene informatie over verbindingstypes, zie [ Verbonden overzicht van recordtypes ](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Voor informatie over het verbinden van verslagen of verslagen met voorwerpen van andere toepassingen, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

Voor een voorbeeld van het verbinden van verslagtypes en verslagen, zie [ Voorbeeld van het verbinden van verslagtypes en verslagen ](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

U moet het volgende hebben om tot de Planning van Workfront toegang te hebben:

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
<li>Eerste</li> 
<li>Ultieme</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td> 
   <td> 
<p>Alle </p> 
<p>Voor meer informatie over wat in elk Plan van de Planning van Workfront inbegrepen is, zie <a href="https://business.adobe.com/products/workfront/pricing.html"> Adobe Workfront tarifering en verpakking </a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td> <p>Standaard</p> 
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
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

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
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Verbind recordtypen

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klik de werkruimte waarvan verslagtypes u wilt verbinden,

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Klik het **+** pictogram in de hoger-juiste hoek van de lijstmening, dan klik de **Nieuwe verbinding** tabel.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Op het **type van Verslag** gebied, onderzoek naar een verslagtype, of selecteer één van het volgende:

   * Een ander recordtype uit de geselecteerde werkruimte

     ![](assets/new-connection-tab-fields-with-another-record-selected.png)

     >[!TIP]
     >
     > 
     >Als de geselecteerde werkruimte geen andere recordtypen bevat, wordt de sectie Werkruimte niet weergegeven.


   * Een recordtype van een andere werkruimte die werd gevormd om van andere werkruimten te verbinden. Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.

     ![](assets/connect-record-from-another-workspace-new-connection-tab.png)

     >[!TIP]
     >
     >Als er geen recordtypen zijn die zijn geconfigureerd om verbinding te maken met andere werkruimten, wordt de sectie Werkruimte niet weergegeven.


   * A **Project, Portfolio, Programma, Bedrijf**, of **Groep** van de **de Objecttypes van Workfront** sectie.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** van de **sectie van de Toepassingen van de Adobe**.

     ![](assets/aem-assets-connection-selection.png)

1. Werk de volgende gegevens bij:

   * **Naam**: De naam van verbonden gebied, aangezien het in de lijstmening of de verslagpagina van het originele verslagtype zal verschijnen. Hiermee maakt u de gekoppelde recordkolom in de tabelweergave van het oorspronkelijke recordtype of het gekoppelde recordveld voor de oorspronkelijke records. Standaard is de naam van het veld de naam van de record of het object waarmee u verbinding maakt.

   >[!TIP]
   >
   >U kunt meerdere verbindingen met hetzelfde record- of objecttype hebben. Als u de naam van het verbonden veld niet bewerkt, voegt Workfront een cijfer toe achter de naam van de verbonden record om het aantal verbonden recordtypen aan te geven met dezelfde naam.

   * **Beschrijving**: De extra informatie over het verbonden verslaggebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **staat veelvoudige verslagen** toe: Selecteer deze optie om erop te wijzen dat u toestaat dat de gebruikers veelvoudige verslagen kunnen toevoegen wanneer de verbonden verslagen van het verslagtype op de originele verslagen tonen. Dit is standaard geselecteerd.

     Deze optie is alleen beschikbaar wanneer u records verbindt vanuit twee verschillende werkruimten of een record en een Adobe Experience Manager-asset-object.

     ![](assets/new-connection-allow-multiple-records-box.png)

   * **het type van Verbinding**: Selecteer één van de volgende opties om erop te wijzen hoeveel verslagen zij met en van kunnen verbinden:

      * Veel tot veel
      * Eén naar vele
      * Vele tot één
      * Eén op één

     Deze optie is alleen beschikbaar wanneer u records verbindt vanuit dezelfde werkruimte of een record en een Workfront-objecttype.

     ![](assets/many-to-many-connection-picker.png)

     Voor meer informatie over verbindingstypes, zie [ Verbonden overzicht van verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Uitgezochte raadplegingsgebieden**: Selecteer deze optie om gebieden van het geselecteerde verslagtype toe te voegen. De opzoekvelden zijn velden die zijn gekoppeld aan het record- of objecttype waarnaar u een koppeling maakt. Als u deze koppelt, wordt informatie weergegeven uit de record of het object waarnaar u een koppeling maakt in de record waarvan u een koppeling wilt maken. Dit is standaard geselecteerd.

     >[!TIP]
     >
     > U kunt de volgende veldtypen niet toevoegen als opzoekvelden:
     >
     >    * Mensen
     >    * Gemaakt door
     >    * Laatst gewijzigd door
     >    * Workfront-typeahead-velden (inclusief velden zoals Projecteigenaar of Projectsponsor)

1. (Voorwaardelijk en facultatief) als u selecteerde om een voorwerp van Workfront te verbinden, selecteer de vorm van de a **Douane** van de **slechts voorwerpen van de Verbinding die deze criteria** sectie aanpassen. Alleen objecten waaraan de geselecteerde aangepaste formulieren zijn gekoppeld, kunnen worden gekoppeld aan het geselecteerde recordtype. U kunt meerdere formulieren selecteren.

   >[!NOTE]
   >
   > U moet in Workfront aangepaste formulieren maken voor de geselecteerde objecten voordat ze in deze lijst worden weergegeven.

1. (Voorwaardelijk) als u selecteerde om met Experience Manager Assets te verbinden, selecteer een bewaarplaats van de **opslagplaats van de Experience Manager** drop-down menu in de **activa van de Verbinding van de volgende bewaarplaats** sectie. Dit is een verplicht veld. Alleen repositories waartoe u toegang hebt in Experience Manager Assets-weergave in dit veld.

   >[!NOTE]
   >
   >Uw Workfront-beheerder kan Workfront-planningsvelden toewijzen aan Experience Manager Assets-velden via de metagegevenstoewijzing in Workfront. Voor meer informatie, zie [ activa meta-gegevensafbeelding tussen Adobe Workfront en Experience Manager Assets ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en) vormen.

1. (Voorwaardelijk) als u selecteerde om met Experience Manager Assets of met een het verslagtype van de Planning van Workfront te verbinden, schrap de **knevel van de Titel** in het **verschijning van het Verslag** gebied, als u niet de titel van verbonden verslagen of activa op het verbonden gebied wilt tonen. Als deze optie is uitgeschakeld, worden alleen de miniaturen van records weergegeven in de gekoppelde velden. Records zonder miniatuurafbeelding geven in plaats daarvan een afbeeldingspictogram weer. De schakeloptie is standaard geselecteerd. Een voorbeeld van hoe de verbonden verslagen in het **vormgeving van het Verslag** gebied zullen tonen.

   >[!TIP]
   >
   >    Wanneer u meerdere records toestaat om te worden gekoppeld, bespaart de weergave van alleen de miniatuur ruimte in kleinere gebieden, zoals in recordweergaven.
   >
   >De titel van een record is het primaire veld van de record. Voor meer informatie, zie [ Primair gebiedsoverzicht ](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Klik **creëren**.

1. (Voorwaardelijk) als u het **Uitgezochte raadplegingsgebied** plaatsen selecteerde, **voegt raadplegingsgebieden** doos open toe.

   Klik het **+** pictogram om gebieden van het **Niet geselecteerde gebied** toe te voegen.

   of

   Klik het **-** pictogram om gebieden uit het **Geselecteerde gebied van gebieden** te verwijderen

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   De waarden voor de verbonden velden worden automatisch ingevuld nadat u records of objecten hebt gekoppeld.

   >[!IMPORTANT]
   >
   >    Iedereen met Weergave of hogere machtigingen voor de werkruimte kan de informatie in de gekoppelde velden weergeven, ongeacht de machtigingen of het toegangsniveau in de toepassing van de gekoppelde objecttypen.


1. (Facultatief) klik **Overslaan** om het toevoegen van gebieden van het verbonden verslag of objecten type over te slaan. De **Naam** of de **Titel** van het verbonden verslag is het enige zichtbare gebied in de lijstmening van het verslagtype u van verbindt.

1. (Optioneel en voorwaardelijk) Als u een getal, valuta, percentage of datumveld wilt koppelen, selecteert u ook een aggregatorwaarde om meerdere waarden samen te vatten. De waarden voor de gekoppelde velden worden gescheiden door komma&#39;s of als een samengevatte waarde weergegeven volgens de door u gekozen aggregator, wanneer gebruikers meer dan één gekoppelde record selecteren in het veld voor gekoppelde records.

   Als het opzoekveld meerdere waarden bevat die niet worden samengevat, kunt u het volgende overwegen wanneer u het veld gebruikt bij het sorteren of groeperen in een weergave:

   * De eerste waarde sorteert

   * Records worden gegroepeerd per unieke combinatie van veldwaarden

   * De tijdlijnweergave is gebaseerd op de eerste datumwaarde.

   >[!IMPORTANT]
   >
   >    U moet een aggregatorwaarde selecteren wanneer u opzoekdatumvelden toevoegt, als u wilt dat de velden beschikbaar zijn om toe te voegen als start- en einddatum voor de tijdlijn- en kalenderweergave. U kunt bijvoorbeeld de MAX of de MIN-aggregator selecteren voor een veld voor de opzoekdatum.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Er zijn geen aggregators beschikbaar wanneer u recordtypen verbindt met Experience Manager Assets.

   Selecteer een van de volgende opties:

   * **niets**: Toont de waarden die uit veelvoudige verslagen komen die door komma&#39;s worden gescheiden. Dit is de standaardselectie.
   * **MAX**: Toont de hoogste waarde van alle waarden die uit veelvoudige verslagen komen die op het verbonden verslaggebied worden geselecteerd.
   * **MIN**: Toont de laagste waarde van alle waarden die uit veelvoudige verslagen komen die op het verbonden verslaggebied worden geselecteerd.
   * **SUM**: Toont het totaal van alle waarden die uit veelvoudige verslagen komen die op het verbonden verslaggebied worden geselecteerd.
   * **AVG**: Toont het gemiddelde van alle waarden die uit veelvoudige verslagen komen die op het verbonden verslaggebied worden geselecteerd.
   * **UNIQUE**: Verwijdert duplicaten uit de waarden van het raadplegingsgebied en toont slechts de unieke waarden. Dit is niet beschikbaar voor de volgende veldtypen:
      * Alinea
      * Selectievakje
      * Mensen

   >[!NOTE]
   >
   >U kunt bijvoorbeeld een koppeling maken naar de productrecord (gekoppelde record) in de campagnerecord (oorspronkelijke record) en deze de naam &quot;Productveld&quot; geven. U kunt er ook voor kiezen om het veld Begroting van de productrecord te koppelen aan de campagnerecord en deze &quot;Productbudget&quot; te noemen. Als u meerdere records in het veld &quot;Product&quot; mocht selecteren, kunt u Product 1 selecteren met een budget van € 100.000 en Product 2 met een budget van € 110.000 en Product 3 met een budget van € 100.000. U kunt de volgende begrotingsinformatie in het gekoppelde veld van de oorspronkelijke record weergeven, afhankelijk van de aggregator die u kiest:
   >
   >* **niets**: $100.000, $10.000, $100.000
   >* **MAX**: $110.000
   >* **MIN**: $100.000
   >* **SUM**: $310.000
   >* **AVG**: $103.000.33
   >* **UNIQUE**: $100.000
   >

1. (Facultatief) gebruik het **onderzoek** pictogram ![](assets/search-icon.png) om naar een gebied te zoeken.

1. Klik **voegt gebieden** toe om uw veranderingen te bewaren.

   De volgende items worden toegevoegd:

   * Een gekoppeld recordveld op het recordtype waarvan u een koppeling maakt. In het gekoppelde recordveld worden afzonderlijke records van het gekoppelde recordtype weergegeven nadat u ze handmatig hebt toegevoegd. Voor informatie over het toevoegen van verslagen, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md). De naam van het gekoppelde recordveld is de naam die u in stap 6 hebt geselecteerd. <!--accurate-->

   * Een gekoppeld (of opzoekveld) veld (of velden) waarin informatie over de gekoppelde record of objecttypen wordt weergegeven nadat u handmatig de records of objecten in het gekoppelde recordveld hebt toegevoegd. De gebieden van de opzoekopdracht worden gecreeerd slechts wanneer **Uitgezochte raadplegingsgebieden** het plaatsen wordt geselecteerd wanneer het creëren van de verbinding. Velden voor opzoeken krijgen automatisch een naam volgens dit patroon:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Bijvoorbeeld, als u een type van het verslagverslag van de Campagne met een type van het Verslag van het Programma koppelde en het Programma verbonden verslaggebied &quot;Informatie van het Programma&quot;noemt, dan uitgezocht om het gebied van de Begroting van het Programma in de de lijstmening van de Campagne ook te tonen, wordt het verbonden gebied automatisch genoemd `Budget (from Program information)` in de de lijstmening van de campagne.

   * Wanneer u recordtypen aan elkaar koppelt, wordt ook een gekoppeld recordveld toegevoegd aan het recordtype waarnaar u een koppeling maakt. De naam van het gekoppelde recordveld in het gekoppelde recordtype is de naam van het recordtype dat u koppelt.

     Als u bijvoorbeeld het recordtype &quot;Product&quot; koppelt aan het recordtype &quot;Campagne&quot; en u het verbonden veld van de campagne &quot;Gekoppeld product&quot; een naam geeft, wordt een veld &quot;Campagne&quot; met gekoppelde records gemaakt voor het recordtype product.

     >[!TIP]
     >
     > Er wordt geen gekoppeld recordveld gemaakt voor objecten van een andere toepassing naar het recordtype waarvan u een koppeling maakt in Workfront Planning.

1. (Optioneel en voorwaardelijk) Klik in de tabelweergave van het oorspronkelijke recordtype of het gekoppelde recordtype op de pijl omlaag in de koptekst van de gekoppelde recordvelden en klik vervolgens op een van de volgende opties:

   * **geef gebied** uit: U kunt de **Naam** en de **Beschrijving** informatie van het gebied bijwerken.
   * **geeft raadplegingsgebieden** uit: Voeg of verwijder om het even welke verbonden gebieden van het verslag toe.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Volg de aanwijzingen in bovenstaande stappen 16-17 om opzoekvelden toe te voegen of te verwijderen. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > U kunt geen opzoekvelden toevoegen die behoren tot recordtypen die u vanuit een andere toepassing koppelt aan objecttypen.
   >
   > U kunt bijvoorbeeld het opzoekveld Campagnestatus niet toevoegen aan een Workfront-project waarnaar u vanuit de campagnes een koppeling maakt.

1. (Optioneel) Klik op de pijl-omlaag in de koptekst van een gekoppeld recordveld of de koptekst van een opzoekveld van het recordtype dat u koppelt, en klik vervolgens op **Verwijderen** .

   Het recordveld of het opzoekveld wordt verwijderd. Als u een recordveld verwijdert, worden alle opzoekvelden die aan de gekoppelde record zijn gekoppeld, ook verwijderd.
