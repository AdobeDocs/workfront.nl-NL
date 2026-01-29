---
title: Recordtypen verbinden
description: Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Adobe Workfront Planning-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '2966'
ht-degree: 0%

---


<!--keep the 30 fields limit in yellow till Jan 2026; also the global record type cross-workspace capability information-->

<!--take production and preview references out at prod-->

# Verbind recordtypen

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

U kunt recordtypen met elkaar verbinden of u kunt recordtypen met objecttypen van andere toepassingen verbinden.

Het verbinden van recordtypen is handig wanneer u verschillende typen werkobjecten hebt die elkaar beïnvloeden. U kunt bijvoorbeeld met campagnes werken en elke campagne kan op meerdere merken betrekking hebben. Om deze relatie aan te geven, kunt u campagnes verbinden met merken. Hiermee maakt u een verbindingsveld voor merken in de campagnerecord.

Bovendien zou het werk voor elke campagne in veelvoudige projecten in Workfront kunnen worden gepland. Om dit aan te geven, kunt u de campagnes verbinden met de relevante projecten. Dit leidt tot een verbindingsgebied voor Projecten op het verslag van de Campagne.

Nadat de verbindingsvelden zijn gemaakt, kunt u afzonderlijke records verbinden tussen de twee record- of objecttypen.

>[!NOTE]
>
>U kunt tot 30 verbindingsgebieden voor één verslagtype hebben.

In dit artikel wordt beschreven hoe u twee recordtypen van Workfront Planning of een recordtype van Workfront Planning kunt verbinden met een object van een andere toepassing.

Nadat u de verbinding tussen verslagen of objecten types vestigt, wordt een verbindingsgebied toegevoegd aan een het verslagtype van de Planning. In het verbindingsgebied, kunt u individuele verslagen met elkaar verbinden, en vertoningsgebieden van het verbonden verslag of objecten types op een verslag van de Planning van Workfront.

Voor algemene informatie over verbindingstypes, zie [&#x200B; Verbonden overzicht van recordtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Voor informatie over het verbinden van verslagen of verslagen met voorwerpen van andere toepassingen, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

Voor een voorbeeld van het verbinden van verslagtypes en verslagen, zie [&#x200B; Voorbeeld van het verbinden van verslagtypes en verslagen &#x200B;](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->


## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Recordtypen verbinden vanuit dezelfde werkruimte: </p>
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
<li><p>Willekeurige workflow en planningspakket</li></ul>

<p>Recordtypen verbinden vanuit verschillende werkruimten:</p>

<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
<li><p>Willekeurige workflow en planningpakket voor Prime of Ultimate</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
<tr> 
<td> 
   <p> Aanvullende producten</p> </td> 
   <td> 
   <p> Als u recordtypen wilt verbinden met objecten uit de volgende toepassingen, moet u niet alleen over Adobe Workfront beschikken, maar ook over het volgende:</p>
   <ul><li><p>Een Adobe Experience Manager Assets-licentie en integratie tussen AEM Assets en Workfront om AEM-middelen te verbinden met planningsrecordtypen.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md"> Adobe Workfront voor Experience Manager Assets en de Hoofdzaak van Activa: artikelindex </a>. </p></li>
   <li><p> Een Adobe GenStudio for Performance Marketing-licentie om recordtypen te verbinden met GenStudio Brands</p>
   <p>Voor informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/get-started"> begonnen worden met Adobe GenStudio for Performance Marketing </a>.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren in een werkruimte</p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li>
   <li><p> Adobe Experience Manager Assets, if you want to connect AEM assets with Planning record types<p>
   <p>You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p>
   </li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p></td> 
  </tr> 
 
</tbody> 
</table> -->

## Verbind recordtypen

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klik de werkruimte waarvan verslagtypes u wilt verbinden,

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Klik het **+** pictogram in de hoger-juiste hoek van de lijstmening, dan klik de **Nieuwe verbinding** tabel.

   ![&#x200B; Nieuw verbindingslusje met de opties van Workfront AEM &#x200B;](assets/new-connection-tab-with-workfront-aem-options-no-buttons.png)

1. Zoek naar een recordtype, of selecteer één van het volgende:

   * Een recordtype uit de huidige werkruimte

     ![&#x200B; multi-uitgezochte verbindingskiezer voor zelfde-werkruimte verslagtype &#x200B;](assets/multi-select-connection-picker-record-type.png)

     >[!TIP]
     >
     > 
     >Als de geselecteerde werkruimte geen andere recordtypen bevat, wordt de sectie Werkruimte niet weergegeven.

   * Een recordtype van een andere werkruimte die werd gevormd om van andere werkruimten te verbinden.

     >[!TIP]
     >
     >**toestaat verbindend met dit verslagtype in andere werkruimten** het plaatsen moet voor een verslagtype in **worden toegelaten dwars-werkruimtemontages** lusje van **geef verslagtype** doos uit, voor een verslagtype om van andere werkruimten toegankelijk te zijn. Als er geen recordtypen zijn die zijn geconfigureerd om verbinding te maken met andere werkruimten, wordt de sectie Werkruimte niet weergegeven.
     >
     >Voor informatie, zie [&#x200B; mogelijkheden van de dwars-werkruimte voor verslagtypes &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen. <!--update screen shot at production-->
     >
     >![&#x200B; geef verslagtype doos dwars-werkruimte montages tabel uit &#x200B;](assets/edit-record-type-box-advanced-settings-tab.png)

     <!--Old:
        [!TIP]
        The **Allow connecting to this record type in other workspaces** setting must be enabled for a record type in the **Advanced settings** tab of the **Edit record type** box, for a record type to be accessible from other workspaces. If there are no record types that are configured to connect from other workspaces, the workspace section does not display.
        ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
        -->

   Voor informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.

   * A **Project, Portfolio, Programma, Bedrijf**, of **Groep** van de **de Objecttypes van Workfront** sectie.

     ![&#x200B; de selectie van de het projectverbinding van Workfront &#x200B;](assets/multi-select-connection-picker-project.png)

   <div class="preview">

   * Een **Origineel verzoek** objecten type van de **3&rbrace; sectie van de Types van Objecten van Workfront.**

     Het oorspronkelijke gemaakte aanvraagverbindingsveld geeft de naam weer van het verzonden planningsverzoek waarmee het object is gemaakt. De naam van het verzoek is ook zichtbaar op het **Onderwerp** gebied van het verzoek.

     >[!NOTE]
     >
     >U moet aanvraagformulieren maken en publiceren om planningsaanvragen in te dienen voor het maken van records in Workfront Planning.
     >
     >Raadpleeg de volgende artikelen voor meer informatie:
     >* [&#x200B; creeer en beheer een verzoekvorm in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/requests/create-request-form.md)
     >* [&#x200B; legt de Verzoeken van de Planning van Adobe Workfront voor om verslagen &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

     ![&#x200B; Oorspronkelijke selectie van de verzoekverbinding &#x200B;](assets/original-request-connection-selection.png)

   </div>


   * **Experience Manager Assets** van de **Toepassingen van Adobe** sectie.

     ![&#x200B; de verbindingsselectie van AEM Assets &#x200B;](assets/aem-assets-connection-selection.png)

     Er wordt een tabblad Nieuwe verbinding geopend voor de geselecteerde record of het geselecteerde objecttype.

   * A **Merk** van Adobe GenStudio for Performance Marketing van de **Adobe GenStudio** sectie

     ![&#x200B; de verbindingsselectie van het Merk van GenStudio &#x200B;](assets/brand-genstudio-connection-selection.png)

1. Werk het **gebied van de Naam** met de naam van het nieuwe verbonden gebied bij, aangezien het in de lijstmening of de verslagpagina van het originele verslagtype zal verschijnen. Hiermee maakt u de verbonden recordkolom (of het gekoppelde veld) in de tabelweergave van het oorspronkelijke recordtype. Standaard is de naam van het veld de naam van de record of het object waarmee u verbinding maakt.

   >[!TIP]
   >
   >U kunt meerdere verbindingen met hetzelfde record- of objecttype hebben. Als u de naam van het verbonden veld niet bewerkt, voegt Workfront een cijfer toe achter de naam van de verbonden record om het aantal verbonden recordtypen aan te geven met dezelfde naam.

1. Werk het **gebied van de Beschrijving** bij door informatie over het verbonden verslaggebied toe te voegen. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. (Voorwaardelijk) wanneer u verslagtypes van twee verschillende werkruimten, een verslagtype en een de activavoorwerp van Adobe Experience Manager, of een verslagtype en een Merk van GenStudio verbindt, selecteer **toestaan veelvoudige verslagen**. Als u deze optie selecteert, geeft u aan dat gebruikers meerdere records mogen toevoegen wanneer het veld voor het verbonden recordtype wordt weergegeven op de oorspronkelijke records. Dit is standaard geselecteerd.

   ![&#x200B; Nieuwe verbinding aan verslagtype van een andere werkruimte &#x200B;](assets/new-connection-allow-multiple-records-box.png)

1. (Voorwaardelijk) Wanneer u recordtypes van de zelfde werkruimte, of een het verslagtype van de Planning met een objecten van Workfront type verbindt, selecteer één van het volgende:

   * **multi-uitgezochte**: Selecteer dit om één verslag van het huidige verslagtype toe te staan om met veelvoudige verslagen van het type van verbindingsverslag te verbinden.
   * **enig-uitgezochte**: Selecteer dit om één verslag van het huidige verslagtype toe te staan om met één verslag van het type van verbindingsverslag te verbinden.

1. Selecteer **creeer corresponderend gebied op verbonden verslagtype**. Als deze optie is geselecteerd, wordt een verbindingsveld gemaakt op het recordtype waarmee u bent verbonden, naast het verbindingsveld dat aan het huidige recordtype is toegevoegd. Dit is standaard uitgeschakeld.

   >[!TIP]
   >
   >* Naast de limiet van 30 verbindingsvelden voor één recordtype, geldt een limiet van 500 velden voor één recordtype. We raden u aan deze instelling uit te schakelen, vooral voor taxonomische recordtypen, om te voorkomen dat deze limiet wordt bereikt.
   >
   >* Het selecteren van **creeert corresponderend gebied op verbonden verslagtype** is een eerste vereiste voor het creëren van hiërarchieën.

1. (Voorwaardelijk) als u **toeliet creeer het corresponderende gebied op verbonden verslagtype**, kies van de volgende opties om erop te wijzen hoeveel verslagengebruikers met en van kunnen verbinden:

   * Veel tot veel
   * Eén naar vele
   * Vele tot één
   * Eén op één

   Voor meer informatie over verbindingstypes, zie [&#x200B; Verbonden overzicht van verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   >[!NOTE]
   >
   >Als u een-op-een of een-op-een selecteert voor het verbindingstype en u later een record of een object wilt verbinden dat al ergens anders is verbonden, ontvangt u een waarschuwing dat het opnieuw verbinden van de record de oorspronkelijke verbinding zal verwijderen. U kunt het verwijderen toestaan of een andere record selecteren.

1. (Voorwaardelijk en facultatief) wanneer u selecteert om een voorwerp van Workfront te verbinden, kies de vorm van de a **Douane** van de **slechts voorwerpen van de Verbinding die deze criteria** sectie aanpassen. Alleen objecten waaraan de geselecteerde aangepaste formulieren zijn gekoppeld, kunnen worden gekoppeld aan het geselecteerde recordtype. U kunt meerdere formulieren selecteren.

   >[!NOTE]
   >
   > U moet in Workfront aangepaste formulieren maken voor de geselecteerde objecten voordat ze in deze lijst worden weergegeven.

1. (Voorwaardelijk) wanneer u om met Experience Manager Assets selecteert te verbinden, kies een bewaarplaats van de **bewaarplaats van Experience Manager** drop-down menu in de **activa van de Verbinding van de volgende bewaarplaats** sectie. Dit is een verplicht veld. Alleen repositories waartoe u toegang hebt in Experience Manager Assets-weergave in dit veld.

   >[!NOTE]
   >
   >Uw Workfront-beheerder kan Workfront-planningsvelden toewijzen aan Experience Manager Assets-velden via de metagegevenstoewijzing in Workfront. Voor meer informatie, zie [&#x200B; activa meta-gegevensafbeelding tussen Adobe Workfront en Experience Manager Assets &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) vormen.


1. (Voorwaardelijk) wanneer u om met Experience Manager Assets, aan een het verslagtype van de Planning van Workfront, of aan een Merk van GenStudio selecteert te verbinden, één van de volgende opties op het **vormgeving van het Verslag** gebied kiezen:

   * **Naam en beeld**: Zowel zullen de naam als de duimnagel of het pictogram van de verbonden verslagen op het verbonden verslaggebied tonen. Dit is de standaardoptie.
   * **Naam**: Slechts zal de naam van de verbonden verslagen op het verbonden verslaggebied tonen.
   * **Beeld**: Slechts zullen de duimnagel of het pictogram van de verbonden verslagen op het verbonden verslaggebied tonen.

   Records zonder miniatuurafbeelding geven in plaats daarvan het pictogram voor het recordtype weer. Een voorbeeld van hoe de verbonden verslagen in het **vormgeving van het Verslag** gebied zullen tonen.

   >[!NOTE]
   >
   >* Wanneer u meerdere records toestaat om te worden gekoppeld, bespaart de weergave van alleen de miniatuur ruimte in kleinere gebieden, zoals in recordweergaven.
   >
   >* De naam van een record is het primaire veld in de record. Voor meer informatie, zie [&#x200B; Primair gebiedsoverzicht &#x200B;](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >* Een recordweergave selecteren is niet beschikbaar wanneer u Workfront-objecttypen selecteert.
   >
   >* Wat u in het vormgevingsgebied Opnemen selecteert, bepaalt hoe de records overal in het systeem worden weergegeven in verbindingen, inclusief alle weergaven en detailpagina&#39;s.

1. Selecteer de **Uitgezochte raadplegingsgebieden** om gebieden van het verslagtype toe te voegen u met verbindt. De opzoekvelden zijn velden die zijn gekoppeld aan het record- of objecttype waarnaar u een koppeling maakt. Als u deze koppelt, wordt informatie weergegeven uit de record of het object waarnaar u een koppeling maakt in de record waarvan u een koppeling maakt. Dit is standaard geselecteerd.

   >[!TIP]
   >
   >* U kunt geen Workfront-tekstkopvelden (zoals velden zoals Projecteigenaar of Projectsponsor) toevoegen als opzoekvelden.
   >
   >* De gegevens van het datumveld van Workfront-objecten worden weergegeven in de 24-uursnotatie van Workfront, ongeacht hoe deze worden weergegeven in Workfront.
   >
   >   Bijvoorbeeld, als de Geplande Datum van het Begin van een project als 3 :00 PM in Workfront toont, zal het als 15 :00 in de Planning van Workfront op een ingevoerd raadplegingsgebied tonen.
   >* In de productieomgeving kunt u geen velden Personen toevoegen als opzoekvelden. <span class="preview"> u kunt de gebieden van Mensen als raadplegingsgebieden in het milieu van de Voorproef toevoegen.</span>
   >

1. Klik **creëren**.

1. (Voorwaardelijk) als u het **Uitgezochte raadplegingsgebied** plaatsen selecteerde, **voegt raadplegingsgebieden** doos open toe.

   Klik het **+** pictogram om gebieden van het **Niet geselecteerde gebied** toe te voegen.

   of

   Klik het **-** pictogram om gebieden uit het **Geselecteerde gebied van gebieden** te verwijderen

   ![&#x200B; voegt raadplegingsgebieden voor een ander verslagtype doos &#x200B;](assets/add-lookup-fields-for-another-maestro-record-type-box.png) toe

   De waarden voor de verbonden velden worden automatisch ingevuld nadat u records of objecten hebt gekoppeld.

   >[!IMPORTANT]
   >
   >    Iedereen met Weergave of hogere machtigingen voor de werkruimte kan de informatie in de gekoppelde velden weergeven, ongeacht de machtigingen of het toegangsniveau in de toepassing van de gekoppelde objecttypen.

1. (Facultatief) klik **Overslaan** om het toevoegen van gebieden van het verbonden verslag of objecten type over te slaan. De naam of het primaire veld van de gekoppelde record is het enige zichtbare veld in de tabelweergave van het recordtype waarmee u verbinding maakt.

1. Kies een aggregator voor de opzoekvelden die u toevoegt.

   >[!NOTE]
   >
   >U kunt geen aggregators toevoegen voor de volgende gebiedstypes:
   >
   >    * Alinea
   >    * Selectievakje

   De waarden voor de gekoppelde velden worden gescheiden door komma&#39;s of als een samengevatte waarde weergegeven volgens de door u gekozen aggregator, wanneer gebruikers meer dan één gekoppelde record selecteren in het veld voor gekoppelde records.

   Als het opzoekveld meerdere waarden bevat die niet worden samengevat, kunt u het volgende overwegen wanneer u het veld gebruikt bij het sorteren of groeperen in een weergave:

   * De eerste waarde sorteert

   * Records worden gegroepeerd per unieke combinatie van veldwaarden

   * De tijdlijnweergave wordt gebaseerd op de eerste datumwaarde van het verbonden recordtype, wanneer deze wordt weergegeven in de weergave

   >[!IMPORTANT]
   >
   > U moet een aggregatorwaarde selecteren wanneer u opzoekdatumvelden toevoegt, als u wilt dat de velden beschikbaar zijn om toe te voegen als start- en einddatum voor de tijdlijn- en kalenderweergave. U kunt bijvoorbeeld de MAX of de MIN-aggregator selecteren voor een veld voor de opzoekdatum.

   ![&#x200B; daling van de Samenvoeger neer voor verbonden aantalgebied &#x200B;](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Er zijn geen aggregators beschikbaar wanneer u recordtypen verbindt met het volgende:
   >* Experience Manager Assets
   >* GenStudio-merken.
   >

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
   >U kunt bijvoorbeeld de productrecord (gekoppelde record) van de campagnerecord (oorspronkelijke record) koppelen en deze de naam &quot;Productveld&quot; geven. U kunt er ook voor kiezen om het veld Begroting van de productrecord te koppelen aan de campagnerecord en deze &quot;Productbudget&quot; te noemen. Als u meerdere records in het veld &quot;Product&quot; mocht selecteren, kunt u Product 1 selecteren met een budget van € 100.000 en Product 2 met een budget van € 110.000 en Product 3 met een budget van € 100.000. U kunt de volgende begrotingsinformatie in het gekoppelde veld van de oorspronkelijke record weergeven, afhankelijk van de aggregator die u kiest:
   >
   >* **niets**: $100.000, $10.000, $100.000
   >* **MAX**: $110.000
   >* **MIN**: $100.000
   >* **SUM**: $310.000
   >* **AVG**: $103.000.33
   >* **UNIQUE**: $100.000
   >

1. (Facultatief) gebruik het **pictogram van het onderzoek** Onderzoek ![&#x200B; aan onderzoek naar een gebied.](assets/search-icon.png)

1. Klik **voegt gebieden** toe om uw veranderingen te bewaren.

   De volgende items worden toegevoegd:

   * Een gekoppeld recordveld op het recordtype waarvan u een koppeling maakt. In het gekoppelde recordveld worden afzonderlijke records van het gekoppelde recordtype weergegeven nadat u ze handmatig hebt toegevoegd. Voor informatie over het toevoegen van verslagen, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md). De naam van het gekoppelde recordveld is de naam die u in stap 6 hebt geselecteerd. <!--accurate-->

   * Een gekoppeld (of opzoekveld) veld (of velden) waarin informatie over de gekoppelde record of objecttypen wordt weergegeven nadat u handmatig de records of objecten in het gekoppelde recordveld hebt toegevoegd. De gebieden van de opzoekopdracht worden gecreeerd slechts wanneer **Uitgezochte raadplegingsgebieden** het plaatsen wordt geselecteerd wanneer het creëren van de verbinding. Velden voor opzoeken krijgen automatisch een naam volgens dit patroon:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Bijvoorbeeld, als u een type van het verslagverslag van de Campagne met een type van het Verslag van het Programma koppelde en het Programma verbonden verslaggebied &quot;Informatie van het Programma,&quot;toen selecteerde om het gebied van de Begroting van het Programma in de de lijstmening van de Campagne ook te tonen, wordt het verbonden gebied automatisch genoemd `Budget (from Program information)` in de de lijstmening van de campagne.

   * Wanneer u recordtypes met elkaar verbindt, wordt een verbonden verslaggebied ook toegevoegd op het verslagtype u met verbindt, slechts wanneer u **creeert het overeenkomstige gebied op verbonden verslagtype** plaatsen toelaat. De naam van het gekoppelde recordveld in het gekoppelde recordtype is de naam van het recordtype dat u koppelt.

     Als u bijvoorbeeld het recordtype &quot;Product&quot; koppelt aan het recordtype &quot;Campagne&quot; en u het gekoppelde veld van de campagne &quot;Gekoppeld product&quot; een naam hebt gegeven, wordt een veld &quot;Campagne&quot; met gekoppelde records gemaakt voor het recordtype product.

     >[!TIP]
     >
     > Een gekoppeld recordveld wordt niet gemaakt voor objecten uit een andere toepassing in hun respectievelijke toepassingen.
     > We raden u aan geen koppelingen te maken naar taxonomische recordtypen, aangezien er een limiet van 500 velden geldt, naast de limiet van 30 verbonden velden voor elk recordtype.


1. (Optioneel en voorwaardelijk) Klik in de tabelweergave van het oorspronkelijke recordtype of het gekoppelde recordtype op de pijl omlaag in de koptekst van de gekoppelde recordvelden en klik vervolgens op een van de volgende opties:

   * **geef gebied** uit: Werk de **Naam** en de **Beschrijving** informatie van het gebied bij.
   * **geeft raadplegingsgebieden** uit: Voeg of verwijder om het even welke verbonden gebieden van het verslag toe.

   ![&#x200B; geef gebied en raadplegingsgebieden drop-down menu in lijstkolom uit &#x200B;](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Volg de aanwijzingen in bovenstaande stappen 16-17 om opzoekvelden toe te voegen of te verwijderen. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > U kunt geen opzoekvelden toevoegen die behoren tot recordtypen die u vanuit een andere toepassing koppelt aan objecttypen.
   >
   > U kunt bijvoorbeeld het opzoekveld Campagnestatus niet toevoegen aan een Workfront-project waarnaar u vanuit de campagnes een koppeling maakt.

1. (Optioneel) Klik op de pijl-omlaag in de koptekst van een gekoppeld recordveld of de koptekst van een opzoekveld van het recordtype dat u koppelt, en klik vervolgens op **Verwijderen** .

   Het recordveld of het opzoekveld wordt verwijderd. Als u een recordveld verwijdert, worden alle opzoekvelden die aan de gekoppelde record zijn gekoppeld, ook verwijderd.
