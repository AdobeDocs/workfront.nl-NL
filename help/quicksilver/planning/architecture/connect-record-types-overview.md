---
title: Overzicht van verbonden recordtypen
description: Een manier om aan te geven hoe individuele recordtypen op elkaar betrekking hebben, is ze met elkaar te verbinden. Bovendien kunt u Adobe Workfront Planning-recordtypen verbinden met objecttypen van andere toepassingen om de gebruikerservaring te verbeteren en de focus in één toepassing te houden.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 0%

---

# Overzicht van verbonden recordtypen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   -->

U kunt aangeven dat afzonderlijke recordtypen op elkaar betrekking hebben of op objecten van andere toepassingen door deze met elkaar te verbinden.

Dit artikel is een overzicht van recordtypeverbindingen en beschrijft de types van verbindingen u tussen verslag en objecten types kunt vestigen.

Voor informatie over u verbindt verslagtypes, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

## Overwegingen bij het verbinden van recordtypen

Er zijn twee stappen aan verbindingen in de Planning van Workfront:

1. Eerst moet u een verbinding tot stand brengen tussen twee recordtypen of een recordtype en een objecttype van een andere toepassing. Voor informatie over hoe u verslagtypes kunt verbinden, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Ten tweede kunt u afzonderlijke records van een bepaald type verbinden met records van een ander type nadat de twee recordtypen zijn verbonden. Voor informatie over het verbinden van verslagen, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

Overweeg het volgende over het verbinden van verslagtypes:

* U kunt de volgende entiteiten verbinden in de Planning van Adobe Workfront:

   * Twee recordtypen.

     Standaard kunt u twee recordtypen verbinden vanuit dezelfde werkruimte. U kunt ook recordtypen instellen om verbinding te maken met recordtypen van andere werkruimten. Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.
   * Een recordtype en een objecttype uit een andere toepassing.

* U kunt Workfront Planning-recordtypen verbinden met de volgende objecttypen vanuit de volgende toepassingen:

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
     >Als u vragen over het aan boord gaan aan Adobe Admin Console hebt, zie [ Adobe Verenigde Veelgestelde vragen van de Ervaring ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nadat u verslagen voor de verbonden verslagtypes creeert, kunt u hen met elkaar verbinden door het verbonden verslaggebied.  Voor informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

* Nadat u een recordtype met een ander verslagtype of met een objecten type van een andere toepassing verbindt, bestaan de volgende scenario&#39;s:

   * **wanneer u twee het verslagtypes van de Planning** verbindt: Een verbonden verslaggebied wordt gecreeerd op het verslagtype u van verbindt. Er wordt een vergelijkbaar gekoppeld recordveld gemaakt voor het recordtype waarmee u verbinding maakt.

     Als u bijvoorbeeld het recordtype ‘Campagne’ verbindt met het recordtype ‘Product’, wordt een gekoppeld recordveld (verbindingsveld) dat u &#39;Gekoppeld product&#39; noemt, gemaakt in het recordtype ‘Campagne’. Er wordt automatisch een gekoppeld recordtype met de naam &quot;Campagne&quot; gemaakt in het recordtype product.

   * **wanneer u een verslagtype met een objecten type van een andere toepassing** verbindt:

      * Er wordt een gekoppeld recordveld gemaakt op het recordtype waarmee u verbinding maakt. Er wordt automatisch geen gekoppeld recordveld gemaakt op het objecttype van de andere toepassing.
      * Planningsrecordvelden zijn niet toegankelijk vanuit Workfront-objecten.
      * Planningsrecords zijn zichtbaar vanaf het tabblad Planning van het Workfront-object. Voor informatie, zie [ recordverbindingen van de voorwerpen van Workfront beheren ](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * U kunt een aangepast veld voor de planningsverbinding maken en dit koppelen aan het aangepaste formulier van een Workfront-object. Voor informatie, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
      * De gebieden van het verslag van de planning zijn toegankelijk van de activa van Experience Manager wanneer uw beheerder van Workfront de meta-gegevensafbeelding door de integratie tussen Workfront en Adobe Experience Manager Assets vormt. Voor meer informatie, zie [ activa meta-gegevensafbeelding tussen Adobe Workfront en Experience Manager Assets ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) vormen.


   * **wanneer u raadplegingsgebieden van het verslag of het voorwerp toevoegt u met** verbindt: Naast het creëren van een verbonden verslaggebied, kunt u met gebieden van het verbonden verslag of objecttype ook verbinden dat raadplegingsgebieden wordt genoemd. Een gekoppeld veld (of opzoekveld) met informatie uit de record waarmee u verbinding maakt, wordt weergegeven in de record waaruit u verbinding maakt.

     U kunt velden van andere recordtypen of objecten van een andere toepassing verbinden met het recordtype Workfront Planning.

     Gekoppelde velden zijn alleen-lezen en geven automatisch informatie van verbonden records weer.

     U kunt verwijzen naar opzoekvelden van andere record- of objecttypen in formules, filters of groepen.

     Als u bijvoorbeeld het recordtype ‘Campagne’ verbindt met een Workfront-project en u selecteert om het veld Geplande afsluitdatum van het project over te brengen naar de planningsrecord van Workfront, wordt automatisch een gekoppeld veld genaamd Geplande voltooiingsdatum (van project) gemaakt voor de campagne. U kunt dit gekoppelde veld niet handmatig bewerken. In het veld Geplande afsluitdatum (van project) wordt de geplande uitvoeringsdatum van de gekoppelde projecten weergegeven.

     >[!IMPORTANT]
     >
     >Iedereen met de toestemmingen van de Mening of hoger aan de werkruimte kan de informatie in de raadplegingsgebieden, ongeacht hun toestemmingen of toegangsniveau in de toepassing van de verbonden objecten types of hun toestemmingen in andere werkruimten bekijken.

     De verbonden verslaggebieden worden voorafgegaan door het het gebiedspictogram van de verhouding ![ ](assets/relationship-field-icon.png).

     Gekoppelde velden worden voorafgegaan door een pictogram dat het veldtype aangeeft. Gekoppelde velden (of opzoekvelden) worden bijvoorbeeld voorafgegaan door pictogrammen die aangeven dat een veld een getal, alinea of datum is.

     >[!TIP]
     >
     >De gegevens van het datumveld van Workfront-objecten worden weergegeven in de 24-uursnotatie van Workfront, ongeacht hoe deze worden weergegeven in Workfront.
     >
     >Bijvoorbeeld, als de Geplande Datum van het Begin van een project als 3 :00 PM in Workfront toont, zal het als 15 :00 in de Planning van Workfront op een ingevoerd raadplegingsgebied tonen.


## Verbindingstypen

Nadat u een verbinding hebt gemaakt tussen twee recordtypen of tussen een record en een objecttype vanuit een andere toepassing, kunt u records toevoegen in de verbonden recordvelden.

Afhankelijk van het aantal records dat u aan een verbonden recordveld kunt toevoegen, zijn de volgende verbindingstypen waaruit u kunt kiezen bij het verbinden van recordtypen:

* [Veel tot veel](#many-to-many-connection-type)
* [Eén naar vele](#one-to-many-connection-type)
* [Vele tot één](#many-to-one-connection-type)
* [Eén op één](#many-to-one-connection-type)

>[!WARNING]
>
>Deze opties zijn niet beschikbaar wanneer u een verbinding tot stand brengt met:
>
>* Twee records uit verschillende werkruimten
>
>* Een recordtype en Experience Manager-elementen

### Vele-aan-vele verbindingstype

![ Velen aan vele verbindingsplukker ](assets/many-to-many-connection-picker.png)

Wanneer u een veel-op-veel verbinding tussen recordtypes creeert, kunt u veelvoudige verslagen op het verbindingsgebied van beide verslagtypes dan selecteren.

Bijvoorbeeld, als u een vele-aan-vele verbinding tussen campagnes en projecten creeert, kunt u veelvoudige projecten voor elke campagne, en veelvoudige campagnes voor elk project selecteren.

Een echt voorbeeld van een veel-op-veel relatietype is de relatie tussen films en acteurs. Elke film kan meerdere acteurs hebben, en elke actrice kan in veelvoudige films spelen.

Wanneer u dit verbindingstype selecteert, kunt u het verbindingstype niet wijzigen nadat u het hebt opgeslagen.

### Een-op-veel verbindingstype

![ Één aan vele verbindingsplukker ](assets/one-to-many-connection-picker.png)


Wanneer u een een-op-veel verbinding maakt tussen recordtypen, kunt u vervolgens meerdere records in het verbindingsveld in het huidige recordtype selecteren, maar met het bijbehorende verbindingsveld in het recordtype waarmee u verbinding maakt, kunt u slechts één record selecteren. Het verbonden verslaggebied dat automatisch op het tweede verslagtype wordt gecreeerd wordt automatisch geplaatst aan een vele-aan-één relatietype.

Als u bijvoorbeeld een een-op-een-verbinding maakt tussen campagnes en projecten, kunt u meerdere projecten selecteren voor elke campagne, maar elk project kan slechts met één campagne worden verbonden.

Een echt voorbeeld van een één-op-veel relatietype is de relatie tussen bibliotheken en boeken: een bibliotheek heeft veel boeken in zijn inventaris; maar één bepaald boek kan slechts in één bibliotheek op een bepaald tijdstip zijn.

Wanneer u dit verbindingstype selecteert, kunt u het later alleen wijzigen in een veel-op-veel-verbindingstype.

### Vele-aan-één verbindingstype

![ Velen aan één verbindingsplukker ](assets/many-to-one-connection-picker.png)


Wanneer u een veel-op-één verbinding tussen recordtypes creeert, kunt u elke verslag in het huidige verslagtype met slechts één verslag van het verbonden verslagtype verbinden. Het verbonden verslaggebied dat automatisch op het tweede verslagtype wordt gecreeerd wordt automatisch geplaatst aan een één-aan-vele relatietype.

Bijvoorbeeld, als u campagnes met projecten verbindt en u dit type van verbinding kiest, kunt u slechts één project aan een campagne toevoegen. Maar u kunt veelvoudige campagnes aan één project toevoegen.

Een echt voorbeeld van een vele-aan-één relatietype is de verhouding tussen vele films en één acteur: één actor kan in vele films zijn, maar elke film kan slechts één specifieke actor eenmaal in zijn gietvorm hebben.

Wanneer u dit verbindingstype selecteert, kunt u het later alleen wijzigen in een veel-op-veel-verbindingstype.

### Een-op-een verbindingstype

![ Één aan één verbindingsplukker ](assets/one-to-one-connection-picker.png)

Wanneer u een één-op-één verbinding tussen verslagtypes creeert, in beide verslagtypes kunt u elke verslag slechts met één verslag van het andere verslagtype verbinden.

Bijvoorbeeld, als u campagnes met projecten verbindt en u dit type van verbinding kiest, kunt u één campagne met één project verbinden. Eén project kan slechts op één campagne worden aangesloten.

Een echt voorbeeld van een één-op-één-relatie is de relatie die bestaat tussen een persoon en de unieke identificatiecode van zijn land (zoals een socialezekerheidsnummer, paspoort-ID, lokale identificatie-ID): elke persoon heeft slechts één unieke identificatiecode voor een land en elke unieke identificatiecode kan aan slechts één persoon worden gekoppeld.

Wanneer u dit verbindingstype selecteert, kunt u het later wijzigen in een ander verbindingstype.
