---
title: Verbind recordtypen
description: Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Maestro-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '2116'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
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

Met Adobe Maestro kunt u volledig aanpasbare werkruimten ontwerpen die recordtypen bevatten die in uw organisatie nodig zijn. Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Maestro-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.

U kunt het volgende verbinden:

* Operationele registratietypen van Maestro
* Maestro-taxonomieën
* Operationele registratietypen en taxonomieën van Maestro
* Operationele recordtypen en taxonomieën van Maestro met objecttypen van andere toepassingen.

Op deze manier kunt u velden van het gekoppelde record of objecttype weergeven op een andere Maestro-record.

In dit artikel wordt beschreven hoe u twee Maestro-recordtypen of een Maestro-recordtype kunt verbinden met een object uit een andere toepassing.

Nadat de verbinding tussen record- of objecttypen tot stand is gebracht, kunt u afzonderlijke records met elkaar verbinden.

Zie voor meer informatie over het verbinden van een Maestro-record met een object vanuit een andere toepassing [Connect-records](../records/connect-records.md).

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
   <p> Adobe Workfront</p> <p>Als u Maestro-recordtypen wilt verbinden met Experience Manager Assets, hebt u een Adobe Experience Manager Assets-licentie nodig en moet het Workfront-exemplaar van uw organisatie zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Overwegingen bij het verbinden van recordtypen

Overweeg het volgende:

* U kunt de volgende entiteiten verbinden in Maestro:

   * Twee typen operationeel record
   * Twee taxonomieën
   * Een operationeel recordtype en een taxonomie
   * Een operationeel recordtype of een taxonomie en een objecttype van een andere toepassing.

  Alle typen bedrijfsrecords en taxonomieën moeten tot dezelfde werkruimte behoren.

* U kunt de volgende objecten vanuit de volgende toepassingen verbinden met Maestro-recordtypen:

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
     >U moet een Adobe Experience Manager Assets-licentie hebben en het Workfront-exemplaar van uw organisatie moet zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console om Maestro-records te kunnen verbinden met Adobe Experience Manager Assets.
     >
     >Als u vragen hebt over instaptoegang tot de Adobe Admin Console, raadpleegt u de [Veelgestelde vragen over Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nadat u een recordtype met een ander verslagtype of met een objecten type van een andere toepassing verbindt, bestaan de volgende scenario&#39;s:

   * **Wanneer u twee recordtypen verbindt**: Een gekoppeld recordveld wordt gemaakt op het recordtype waarmee u verbinding maakt. Er wordt een vergelijkbaar gekoppeld recordveld gemaakt voor het recordtype waarmee u verbinding maakt.

     Als u bijvoorbeeld het recordtype ‘Campagne’ aansluit op het recordtype ‘Product’, wordt een gekoppeld recordveld met de naam ‘Gekoppeld product’ gemaakt op het recordtype ‘Campagne’ en wordt een gekoppeld recordtype met de naam ‘Campagne’ gemaakt op het recordtype ‘Product’.

   * **Wanneer u een recordtype verbindt met een objecttype van een andere toepassing**: Een gekoppeld recordveld wordt gemaakt op het recordtype waarmee u verbinding maakt. Er wordt automatisch geen gekoppeld recordveld gemaakt voor het toepassingsobject van een derde.

     Een nieuw recordtype met het kenmerk Alleen-lezen van Maestro wordt alleen voor het toepassingsobject van derden gemaakt wanneer de feitelijke objecten met de Maestro-records zijn verbonden.

     Zie voor meer informatie [Connect-records](../records/connect-records.md).

   * **Wanneer u opzoekvelden toevoegt van de record of het object waarmee u verbinding maakt**: Gekoppelde velden worden toegevoegd aan de record waarvan u verbinding maakt en geven informatie weer uit de opzoekvelden die u hebt geselecteerd voor de records waarvan u een koppeling maakt. De recordvelden zijn altijd alleen-lezen en worden automatisch gevuld met de waarden van het externe object.

     Als u bijvoorbeeld het recordtype &#39;Campaign&#39; (Maestro) verbindt met een Workfront-project en u het veld Geplande voltooiingsdatum van het project wilt overbrengen naar de Maestro-record, wordt automatisch een gekoppeld veld genaamd Geplande voltooiingsdatum (van project) gemaakt voor de record waarvan u een koppeling maakt.

     >[!IMPORTANT]
     >
     >    Iedereen met Weergave of hogere machtigingen voor de werkruimte kan de informatie in de gekoppelde velden weergeven, ongeacht de machtigingen of het toegangsniveau in de toepassing van de gekoppelde objecttypen door derden.

* Gekoppelde recordvelden worden voorafgegaan door een relatiepictogram ![](assets/relationship-field-icon.png).

  Gekoppelde velden worden voorafgegaan door een pictogram dat het veldtype aangeeft. Bijvoorbeeld pictogrammen die aangeven dat een veld een getal, alinea of datum is.

* Nadat u afzonderlijke records voor een recordtype hebt gemaakt, kunt u de records waarmee u verbinding maakt, selecteren in het veld voor het gekoppelde recordtype. Zie voor meer informatie [Connect-records](../records/connect-records.md).

## Verbind recordtypen

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u recordtypen wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Klik op de knop **+** in de rechterbovenhoek van de tabelweergave klikt u op de knop **Nieuwe verbinding** tab.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. In de **Recordtype** veld, zoek naar een recordtype of selecteer een van de volgende opties: <!--is the field name spelled right? lowercase "t"?-->

   * Een ander type bedrijfsrecord of een taxonomie in de werkruimte die u hebt geselecteerd

     >[!TIP]
     >
     >Alleen recordtypen en taxonomieën in de werkruimte die u hebt geselecteerd, zijn beschikbaar voor verbinding.
     > 
     >Als de geselecteerde werkruimte geen andere recordtypen bevat, wordt de naam van de werkruimte niet weergegeven.

   * A **Project, Portfolio, Programma, Bedrijf**, of **Groep** van de **Workfront-objecttypen** sectie.
   * **Experience Manager Assets** van de **Adobe-toepassingen** sectie.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Werk de volgende gegevens bij:

   * **Naam**: De naam van het verbonden veld, zoals deze wordt weergegeven in de tabelweergave of op de pagina Details van het oorspronkelijke recordtype. Hiermee maakt u de gekoppelde recordkolom in de tabelweergave van het oorspronkelijke recordtype of het gekoppelde recordveld voor de oorspronkelijke records. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >We raden u aan de naam van de record waarnaar u een koppeling maakt, op te nemen in de naam van het verbonden recordveld om vast te leggen van welk recordtype het nieuwe veld afkomstig is. De naam van de gekoppelde record is niet zichtbaar in het nieuwe gekoppelde recordveld of de gekoppelde velden ervan.

   * **Beschrijving**: Aanvullende informatie over het verbonden recordveld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Meerdere records toestaan**: Selecteer deze optie om aan te geven dat gebruikers meerdere records mogen toevoegen wanneer het veld voor het gekoppelde recordtype wordt weergegeven op de oorspronkelijke records. Dit is standaard geselecteerd.
   * **Opzoekvelden selecteren**: Selecteer deze optie om velden van het geselecteerde recordtype toe te voegen. De opzoekvelden zijn gekoppeld aan het record- of objecttype waarnaar u een koppeling maakt.  Dit is standaard geselecteerd.

1. (Voorwaardelijk en optioneel) Als u een Workfront-object wilt verbinden, selecteert u een **Aangepast formulier** van de **Alleen projecten koppelen die aan deze criteria voldoen** sectie. <!--this needs to be updated for each object when they fix this UI.--> Alleen objecten waaraan de geselecteerde aangepaste formulieren zijn gekoppeld, kunnen worden gekoppeld aan het geselecteerde Maestro-recordtype. U kunt meerdere formulieren selecteren.

   ![](assets/workfront-project-connection-selection.png)

1. (Voorwaardelijk) Als u verbinding wilt maken met Experience Manager Assets, selecteert u een opslagplaats in het menu **Experience Manager-opslagplaats** vervolgkeuzemenu in het dialoogvenster **Elementen koppelen van de volgende gegevensopslagruimte** sectie. Dit is een verplicht veld. Alleen repositories waartoe u toegang hebt in Experience Manager Assets-weergave in dit veld.

   ![](assets/aem-assets-connection-selection.png)

1. Klikken **Maken**.

1. (Voorwaardelijk) Als u de optie **Opzoekveld selecteren** instellen, de **Opzoekvelden toevoegen** wordt geopend.

   Klik op de knop **+** pictogram om velden toe te voegen van de **Niet-geselecteerde velden** gebied.

   of

   Klik op de knop **-** pictogram om velden te verwijderen uit het dialoogvenster **Geselecteerde velden** gebied

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   >[!IMPORTANT]
   >
   >    Iedereen met Weergave of hogere machtigingen voor de werkruimte kan de informatie in de gekoppelde velden weergeven, ongeacht de machtigingen of het toegangsniveau in de toepassing van de gekoppelde objecttypen door derden.


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

   >[!NOTE]
   >
   >U kunt bijvoorbeeld een koppeling maken naar de productrecord (gekoppelde record) in de campagnerecord (oorspronkelijke record) en deze de naam &quot;Productveld&quot; geven. U kunt er ook voor kiezen om het veld Begroting van de productrecord te koppelen aan de campagnerecord en deze &quot;Productbudget&quot; te noemen. Als u meerdere records in het veld &quot;Product&quot; mocht selecteren, kunt u Product 1 selecteren met een budget van € 120.000 en Product 2 met een budget van € 100.000. U kunt de volgende begrotingsinformatie in het gekoppelde veld van de oorspronkelijke record weergeven, afhankelijk van de aggregator die u kiest:
   >
   >* **Geen**: $120.000, $100.000
   >* **MAX**: $120.000
   >* **MIN**: $100.000
   >* **SUM**: $ 220.000
   >* **AVG**: $110.000
   >

1. (Optioneel) Gebruik de opdracht **zoeken** pictogram ![](assets/search-icon.png) om een veld te zoeken.

1. Klikken **Velden toevoegen** om uw wijzigingen op te slaan.

   De volgende items worden toegevoegd:

   * Een gekoppeld recordveld op het recordtype waarvan u een koppeling maakt. In het gekoppelde recordveld worden afzonderlijke records van het gekoppelde recordtype weergegeven nadat u ze handmatig hebt toegevoegd. Zie voor informatie over het toevoegen van records [Connect-records](/help/quicksilver/maestro/records/connect-records.md). De naam van het gekoppelde recordveld is de naam die u in stap 6 hebt geselecteerd. <!--accurate-->

   * Een gekoppeld veld (of velden) waarin informatie uit de velden van het gekoppelde recordtype wordt weergegeven nadat u de records handmatig hebt toegevoegd in het gekoppelde recordveld. De gekoppelde velden worden alleen gemaakt wanneer de **Opzoekvelden selecteren** Deze instelling wordt geselecteerd bij het maken van de verbinding. De gekoppelde velden krijgen een naam volgens dit patroon:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Wanneer u Maestro-recordtypen aan elkaar koppelt, wordt ook een gekoppeld recordveld toegevoegd aan het recordtype waarnaar u een koppeling maakt. De naam van het gekoppelde recordveld in het gekoppelde recordtype is de naam van het recordtype dat u koppelt.

     Als u bijvoorbeeld het recordtype &quot;Product&quot; koppelt aan het recordtype &quot;Campagne&quot; en u het verbonden veld van de campagne &quot;Gekoppeld product&quot; een naam geeft, wordt een veld &quot;Campagne&quot; met gekoppelde records gemaakt voor het recordtype product.

     >[!TIP]
     >
     > Een gekoppeld recordveld naar het recordtype waarvan u een koppeling maakt, wordt niet gemaakt voor objecten van een externe toepassing.

1. (Optioneel) Klik in het oorspronkelijke recordtype of in de tabelweergave van het gekoppelde recordtype op de pijl omlaag in de koptekst van de gekoppelde recordvelden en klik vervolgens op een van de volgende opties:

   * **Veld bewerken**: U kunt het dialoogvenster **Naam** en de **Beschrijving** informatie over het veld.
   * **Opzoekvelden bewerken**: Voeg de velden van een gekoppelde record toe of verwijder deze.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Volg de aanwijzingen in bovenstaande stappen 10-14 om opzoekvelden toe te voegen of te verwijderen. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > U kunt de opzoekvelden niet toevoegen van de record die u koppelt aan het gekoppelde recordtype dat een object aangeeft in een toepassing van een derde.
   >
   > U kunt bijvoorbeeld het opzoekveld van een Maestro-object ‘Campagne’ niet toevoegen vanuit het veld ‘Campagne’ voor gekoppelde records dat wordt weergegeven in het recordtype Maestro-project wanneer u een koppeling naar Workfront-projecten tot stand brengt.

1. (Optioneel) Klik op de pijl omlaag in de koptekst van het gekoppelde recordveld in het recordtype waarvan u een koppeling maakt, en klik vervolgens op **Verwijderen**.

   Het recordveld en eventuele aanvullende gekoppelde opzoekvelden worden verwijderd en de velden en hun gegevens kunnen niet worden hersteld.

   >[!TIP]
   >
   >    Het gekoppelde recordveld in het recordtype waarnaar u koppelt, wordt niet verwijderd. <!-- is this still accurate?! -->
