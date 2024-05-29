---
title: Verbind recordtypen
description: Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Adobe Workfront Planning-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 44073ea242803e28ca00c82811ae2865747d11c3
workflow-type: tm+mt
source-wordcount: '2253'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Verbind recordtypen

{{maestro-important-intro}}

Met Adobe Workfront Planning kunt u volledig aanpasbare werkruimten ontwerpen die recordtypen bevatten die in uw organisatie nodig zijn. Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Workfront Planning-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.

U kunt recordtypen met elkaar verbinden of typen opnemen met objecttypen van andere toepassingen.

Op deze manier kunt u velden van het gekoppelde record of objecttype weergeven in een Workfront-planningsrecord.

In dit artikel wordt beschreven hoe u twee recordtypen in Workfront Planning of een recordtype kunt verbinden met een object uit een andere toepassing.

Nadat u de verbinding tussen records of objecttypen tot stand hebt gebracht, kunt u afzonderlijke records met elkaar verbinden.

Voor informatie over het verbinden van een verslag van de Planning van Workfront met een voorwerp van een andere toepassing, zie [Connect-records](../records/connect-records.md).

Zie voor een voorbeeld van het verbinden van recordtypen [Voorbeeld van het verbinden van recordtypen en records](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

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
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Als u Adobe Workfront Planning-recordtypen wilt verbinden met Experience Manager Assets, hebt u een Adobe Experience Manager Assets-licentie nodig en moet het Workfront-exemplaar van uw organisatie zijn aangemeld bij de Adobe Unified Experience. Zie voor meer informatie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience voor Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het gesloten bètaprogramma voor Adobe Workfront Planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Overwegingen bij het verbinden van recordtypen

* U kunt de volgende entiteiten verbinden in de Planning van Adobe Workfront:

   * Twee recordtypen

     De recordtypen moeten tot dezelfde werkruimte behoren.
   * Een recordtype en een objecttype uit een andere toepassing.

* U kunt de volgende objecttypen verbinden vanuit de volgende toepassingen met Workfront Planning-recordtypen:

   * Adobe Workfront:

      * Projecten
      * Portfolio&#39;s
      * Programma&#39;s
      * Bedrijven
      * Groepen

   * Adobe Experience Manager Assets:

      * Afbeeldingen
      * Mappen

     >[!IMPORTANT]
     >
     >U moet een Adobe Experience Manager Assets-licentie hebben en het Workfront-exemplaar van uw organisatie moet zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console om Workfront Planning-records te verbinden met Adobe Experience Manager Assets.
     >
     >Als u vragen hebt over instaptoegang tot de Adobe Admin Console, raadpleegt u de [Veelgestelde vragen over Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nadat u afzonderlijke records voor een recordtype hebt gemaakt, kunt u de records waarmee u verbinding maakt, selecteren in het veld voor het gekoppelde recordtype. Zie voor meer informatie [Connect-records](../records/connect-records.md).

* Nadat u een recordtype met een ander verslagtype of met een objecten type van een andere toepassing verbindt, bestaan de volgende scenario&#39;s:

   * **Wanneer u twee recordtypen verbindt**: Een gekoppeld recordveld wordt gemaakt op het recordtype waarmee u verbinding maakt. Er wordt een vergelijkbaar gekoppeld recordveld gemaakt voor het recordtype waarmee u verbinding maakt.

     Als u bijvoorbeeld het recordtype ‘Campagne’ aansluit op het recordtype ‘Product’, wordt een gekoppeld recordveld met de naam ‘Gekoppeld product’ gemaakt op het recordtype ‘Campagne’ en wordt een gekoppeld recordtype met de naam ‘Campagne’ gemaakt op het recordtype ‘Product’.

   * **Wanneer u een recordtype verbindt met een objecttype van een andere toepassing**: Een gekoppeld recordveld wordt gemaakt op het recordtype waarmee u verbinding maakt. Er wordt automatisch geen gekoppeld recordveld gemaakt op het objecttype van de andere toepassing.

     Er wordt alleen een nieuw recordtype voor alleen-lezen-schrijven van Workfront-planning gemaakt voor het object van de andere toepassing wanneer de feitelijke objecten zijn verbonden met de planningsrecords van Workfront.

     Zie voor meer informatie [Connect-records](../records/connect-records.md).

   * **Wanneer u opzoekvelden toevoegt van de record of het object waarmee u verbinding maakt**: U kunt velden van het object van de andere toepassing verbinden met het recordtype Workfront Planning. Dit zijn gekoppelde of opzoekvelden. Gekoppelde velden geven automatisch informatie van verbonden records of objecten weer wanneer u de records of de objecten verbindt. De gekoppelde opzoekvelden zijn altijd alleen-lezen en worden automatisch gevuld met de waarden van de verbonden records of objecten.

     Als u bijvoorbeeld het recordtype ‘Campagne’ verbindt met een Workfront-project en u selecteert om het veld Geplande afsluitdatum van het project over te brengen naar de planningsrecord van Workfront, wordt automatisch een gekoppeld veld genaamd Geplande voltooiingsdatum (van project) gemaakt voor de campagne. U kunt dit gekoppelde veld niet handmatig bewerken. In het veld Geplande afsluitdatum (van project) wordt de geplande uitvoeringsdatum van de gekoppelde projecten weergegeven.

     >[!IMPORTANT]
     >
     >    Iedereen met Weergave of hogere machtigingen voor de werkruimte kan de informatie in de gekoppelde velden weergeven, ongeacht de machtigingen of het toegangsniveau in de toepassing van de gekoppelde objecttypen.

* Gekoppelde recordvelden worden voorafgegaan door een relatiepictogram ![](assets/relationship-field-icon.png).

  Gekoppelde velden worden voorafgegaan door een pictogram dat het veldtype aangeeft. Bijvoorbeeld pictogrammen die aangeven dat een veld een getal, alinea of datum is.

## Verbind recordtypen

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u recordtypen wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Klik op de knop **+** in de rechterbovenhoek van de tabelweergave klikt u op de knop **Nieuwe verbinding** tab.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. In de **Recordtype** veld, zoek naar een recordtype of selecteer een van de volgende opties:

   * Een ander recordtype uit het gedeelte van de werkruimte dat u hebt geselecteerd

     >[!TIP]
     >
     >Alleen recordtypen uit de geselecteerde werkruimte zijn beschikbaar voor verbinding.
     > 
     >Als de geselecteerde werkruimte geen andere recordtypen bevat, wordt de sectie Werkruimte niet weergegeven.

   * A **Project, Portfolio, Programma, Bedrijf**, of **Groep** van de **Workfront-objecttypen** sectie.
   * **Experience Manager Assets** van de **Adobe-toepassingen** sectie.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Werk de volgende gegevens bij:

   * **Naam**: De naam van het verbonden veld, zoals deze wordt weergegeven in de tabelweergave of de recordpagina van het oorspronkelijke recordtype. Hiermee maakt u de gekoppelde recordkolom in de tabelweergave van het oorspronkelijke recordtype of het gekoppelde recordveld voor de oorspronkelijke records.

   >[!TIP]
   >
   >We raden u aan de naam van de record waarnaar u een koppeling maakt, op te nemen in de naam van het verbonden recordveld om vast te leggen van welk recordtype het nieuwe veld afkomstig is. De naam van de gekoppelde record is niet zichtbaar in het nieuwe gekoppelde recordveld of de gekoppelde velden ervan.

   * **Beschrijving**: Aanvullende informatie over het verbonden recordveld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Meerdere records toestaan**: Selecteer deze optie om aan te geven dat gebruikers meerdere records mogen toevoegen wanneer het veld voor het gekoppelde recordtype wordt weergegeven op de oorspronkelijke records. Dit is standaard geselecteerd.
   * **Opzoekvelden selecteren**: Selecteer deze optie om velden van het geselecteerde recordtype toe te voegen. De opzoekvelden zijn velden die zijn gekoppeld aan het record- of objecttype waarnaar u een koppeling maakt. Als u deze koppelt, wordt informatie weergegeven uit de record of het object waarnaar u een koppeling maakt in de record waarvan u een koppeling wilt maken. Dit is standaard geselecteerd.

1. (Voorwaardelijk en optioneel) Als u een Workfront-object wilt verbinden, selecteert u een **Aangepast formulier** van de **Alleen objecten koppelen die aan deze criteria voldoen** sectie. Alleen objecten waaraan de geselecteerde aangepaste formulieren zijn gekoppeld, kunnen worden gekoppeld aan het geselecteerde recordtype. U kunt meerdere formulieren selecteren.

   ![](assets/workfront-project-connection-selection.png)

   >[!NOTE]
   >
   > U moet in Workfront aangepaste formulieren maken voor de geselecteerde objecten voordat ze in deze lijst worden weergegeven.

1. (Voorwaardelijk) Als u verbinding wilt maken met Experience Manager Assets, selecteert u een opslagplaats in het menu **Experience Manager-opslagplaats** vervolgkeuzemenu in het dialoogvenster **Elementen koppelen van de volgende gegevensopslagruimte** sectie. Dit is een verplicht veld. Alleen repositories waartoe u toegang hebt in Experience Manager Assets-weergave in dit veld.

   <!--replace the screen shot below when they fix the permissions info icon bug-->

   ![](assets/aem-assets-connection-selection.png)

1. Klikken **Maken**.

1. (Voorwaardelijk) Als u de optie **Opzoekveld selecteren** instellen, de **Opzoekvelden toevoegen** wordt geopend.

   Klik op de knop **+** pictogram om velden toe te voegen van de **Niet-geselecteerde velden** gebied.

   of

   Klik op de knop **-** pictogram om velden te verwijderen uit het dialoogvenster **Geselecteerde velden** gebied

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   De waarden voor de verbonden velden worden automatisch ingevuld nadat u records of objecten hebt gekoppeld.

   >[!IMPORTANT]
   >
   >    Iedereen met Weergave of hogere machtigingen voor de werkruimte kan de informatie in de gekoppelde velden weergeven, ongeacht de machtigingen of het toegangsniveau in de toepassing van de gekoppelde objecttypen.


1. (Optioneel) Klik op **Overslaan** en voeg geen velden toe uit de gekoppelde record of het gekoppelde object. De **Naam** van de gekoppelde record is het enige zichtbare veld in de tabelweergave van de oorspronkelijke record.

1. (Optioneel en voorwaardelijk) Als u een getal, valuta, percentage of datumveld wilt koppelen, selecteert u ook een aggregatorwaarde. De waarden voor de gekoppelde velden worden gescheiden door komma&#39;s of als een geaggregeerde waarde weergegeven volgens de aggregator die u kiest, wanneer gebruikers meer dan één gekoppelde record selecteren in het veld voor gekoppelde records.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Er zijn geen aggregators beschikbaar wanneer u recordtypen verbindt met Experience Manager Assets.

   Selecteer een van de volgende opties:

   * **Geen**: Geeft de waarden weer die afkomstig zijn van meerdere records gescheiden door komma&#39;s. Dit is de standaardselectie.
   * **MAX**: geeft de hoogste waarde weer van alle waarden die afkomstig zijn van meerdere records die in het gekoppelde recordveld zijn geselecteerd.
   * **MIN**: geeft de laagste waarde weer van alle waarden die afkomstig zijn van meerdere records die in het gekoppelde recordveld zijn geselecteerd.
   * **SUM**: geeft het totaal weer van alle waarden die afkomstig zijn van meerdere records die in het gekoppelde recordveld zijn geselecteerd.
   * **AVG**: geeft het gemiddelde weer van alle waarden die afkomstig zijn van meerdere records die in het gekoppelde recordveld zijn geselecteerd.
   * **UNIEK**: Hiermee verwijdert u duplicaten uit de waarden van het opzoekveld en geeft u alleen de unieke waarden weer. Dit is niet beschikbaar voor de volgende veldtypen:
      * Alinea
      * Selectievakje
      * Mensen

   >[!NOTE]
   >
   >U kunt bijvoorbeeld een koppeling maken naar de productrecord (gekoppelde record) in de campagnerecord (oorspronkelijke record) en deze de naam &quot;Productveld&quot; geven. U kunt er ook voor kiezen om het veld Begroting van de productrecord te koppelen aan de campagnerecord en deze &quot;Productbudget&quot; te noemen. Als u meerdere records in het veld &quot;Product&quot; mocht selecteren, kunt u Product 1 selecteren met een budget van € 100.000 en Product 2 met een budget van € 110.000 en Product 3 met een budget van € 100.000. U kunt de volgende begrotingsinformatie in het gekoppelde veld van de oorspronkelijke record weergeven, afhankelijk van de aggregator die u kiest:
   >
   >* **Geen**: $100.000, $110.000, $100.000
   >* **MAX**: $110.000
   >* **MIN**: $100.000
   >* **SUM**: $ 310.000
   >* **AVG**: $ 103.000,33
   >* **UNIEK**: $100.000
   >

1. (Optioneel) Gebruik de opdracht **zoeken** pictogram ![](assets/search-icon.png) om een veld te zoeken.

1. Klikken **Velden toevoegen** om uw wijzigingen op te slaan.

   De volgende items worden toegevoegd:

   * Een gekoppeld recordveld op het recordtype waarvan u een koppeling maakt. In het gekoppelde recordveld worden afzonderlijke records van het gekoppelde recordtype weergegeven nadat u ze handmatig hebt toegevoegd. Zie voor informatie over het toevoegen van records [Connect-records](/help/quicksilver/maestro/records/connect-records.md). De naam van het gekoppelde recordveld is de naam die u in stap 6 hebt geselecteerd. <!--accurate-->

   * Een gekoppeld veld (of gekoppelde velden) waarin informatie uit de velden van de gekoppelde record of objecttypen wordt weergegeven nadat u de records of objecten handmatig hebt toegevoegd in het gekoppelde recordveld. De gekoppelde velden worden alleen gemaakt wanneer de **Opzoekvelden selecteren** Deze instelling wordt geselecteerd bij het maken van de verbinding. De gekoppelde velden krijgen automatisch een naam op basis van dit patroon:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Bijvoorbeeld, als u een type van het verslagverslag van de Campagne met een verslagtype van het Programma koppelde en het Programma verbonden verslaggebied &quot;Informatie van het Programma&quot;noemt, dan uitgezocht om het gebied van de Begroting van het Programma in de de lijstmening van de Campagne ook te tonen, wordt het verbonden gebied automatisch genoemd `Budget (from Program information)` in de tabel van de campagne .

   * Wanneer u recordtypen aan elkaar koppelt, wordt ook een gekoppeld recordveld toegevoegd aan het recordtype waarnaar u een koppeling maakt. De naam van het gekoppelde recordveld in het gekoppelde recordtype is de naam van het recordtype dat u koppelt.

     Als u bijvoorbeeld het recordtype &quot;Product&quot; koppelt aan het recordtype &quot;Campagne&quot; en u het verbonden veld van de campagne &quot;Gekoppeld product&quot; een naam geeft, wordt een veld &quot;Campagne&quot; met gekoppelde records gemaakt voor het recordtype product.

     >[!TIP]
     >
     > Er wordt geen gekoppeld recordveld gemaakt voor objecten van een andere toepassing naar het recordtype waarvan u een koppeling maakt in Workfront Planning.

1. (Optioneel en voorwaardelijk) Klik in de tabelweergave van het oorspronkelijke recordtype of het gekoppelde recordtype op de pijl omlaag in de koptekst van de gekoppelde recordvelden en klik vervolgens op een van de volgende opties:

   * **Veld bewerken**: U kunt het dialoogvenster **Naam** en de **Beschrijving** informatie over het veld.
   * **Opzoekvelden bewerken**: Voeg de velden van een gekoppelde record toe of verwijder deze.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Volg de aanwijzingen in bovenstaande stappen 10-14 om opzoekvelden toe te voegen of te verwijderen. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > U kunt geen opzoekvelden toevoegen die behoren tot recordtypen die u vanuit een andere toepassing koppelt aan objecttypen.
   >
   > U kunt bijvoorbeeld het opzoekveld Campagnestatus niet toevoegen aan een Workfront-project waarnaar u vanuit de campagnes een koppeling maakt.

1. (Optioneel) Klik op de pijl omlaag in de koptekst van een gekoppeld recordveld of de koptekst van een opzoekveld in het recordtype waarvan u een koppeling maakt, en klik vervolgens op **Verwijderen**.

   Het recordveld of het opzoekveld wordt verwijderd. Als u een recordveld verwijdert, worden alle opzoekvelden die aan de gekoppelde record zijn gekoppeld, ook verwijderd.
