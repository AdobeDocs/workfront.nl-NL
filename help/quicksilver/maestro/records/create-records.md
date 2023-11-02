---
title: Records maken
description: In Adobe Maestro is een record een instantie van een recordtype. U moet recordtypen maken voordat u afzonderlijke records kunt maken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 0699740f8ef0932316843d9aec0008ccdeb319f5
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Records maken

>[!IMPORTANT]
>
>De informatie in dit artikel heeft betrekking op Adobe Maestro, een nieuw aanbod van Adobe.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

In Adobe Maestro is een record een instantie van een recordtype.

U kunt de volgende typen records hebben:

* **Operationele gegevens**: Deze vertegenwoordigen werkgerelateerde objecten. Voor een operationeel record met de naam &#39;Campagne&#39; kunt u bijvoorbeeld records met een naam als &#39;Maandelijkse nieuwsbrief&#39; of &#39;Zomerverkoop&#39; hebben genoemd.
* **Taxonomische gegevens**: Ze vertegenwoordigen kenmerken die aan operationele records kunnen worden gekoppeld. Voor een taxonomie-recordtype met de naam &#39;Kanaal&#39; kunt u bijvoorbeeld taxonomieën als &#39;E-mail&#39;, &#39;Sociale media&#39; of &#39;Advertising&#39; een naam geven.

Het creëren van operationele verslagen is identiek aan het creëren van taxonomieverslagen, of taxonomieën.

U kunt records maken in Maestro door een van de volgende handelingen uit te voeren:

* Deze handmatig maken voor Maestro-recordtypen
* Verbind hen met verslagen Maestro van derdetoepassingen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p>  
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

## Records maken door deze handmatig toe te voegen aan een recordtype <!--in a record type table (I don't think you can create them elsewhere right now)-->

U kunt records maken in de tabelweergave van een pagina met recordtypen.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->en klik vervolgens op **Maestro** ![](assets/maestro-icon.png).
De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
1. Klik op een opnametype. Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture-and-fields/create-record-types.md).

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.
Alle records van het geselecteerde type worden weergegeven in de tabelweergave.

1. (Voorwaardelijk) Als de pagina met recordtypen niet wordt geopend in de tabelweergave, klikt u op de knop **Weergave** en selecteert u een bestaande **Tabelweergave** ![](assets/table-view-icon.png) of klik op **Weergave maken > Tabel** een tabelweergave maken.

1. Klik op **Nieuw &lt; Naam recordtype >** in de laatste rij van de tabel

   of

   Klikken **Shift + Enter** op uw toetsenbord vanuit een willekeurige kolom of rij van de tabel. Hiermee voegt u een lege rij toe.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Typ informatie in de nieuwe rij over de nieuwe record.

   >[!NOTE]
   >
   >  * Het veld Naam is geen verplicht veld. Wij raden u echter aan een naam voor de record toe te voegen, omdat het nuttig is om records te identificeren wanneer u records aan elkaar koppelt.
   >
   >  * Velden die naar andere recordtypen of berekende velden verwijzen, zijn alleen-lezen velden.

1. Ga door met het toevoegen van informatie over elke rij en klik vervolgens op **Enter** op uw toetsenbord om uw wijzigingen op te slaan.

## Records maken door deze vanuit een andere toepassing te verbinden

U kunt records uit andere toepassingen importeren door deze te koppelen aan Maestro-gekoppelde records.

1. Maak een Maestro-recordtype, zoals beschreven in het dialoogvenster [Recordtypen maken](../architecture-and-fields/create-record-types.md).

1. Maak Maestro-records voor het recordtype dat u in de vorige stap hebt gemaakt. Zie de sectie [Records maken door deze handmatig toe te voegen aan een recordtype](#create-records-by-manually-adding-them-to-a-record-type) in dit artikel.

1. Maak een verbinding met een objecttype vanuit een externe toepassing voor het recordtype Maestro dat u hebt gemaakt. Zie voor meer informatie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

1. Voeg records uit de toepassing van een andere fabrikant toe aan de Maestro-records die u hierboven hebt gemaakt met behulp van het gekoppelde recordveld dat u in de vorige stap hebt gemaakt. Zie voor meer informatie [Connect-records](../records/connect-records.md).

   De volgende items worden gemaakt in Maestro:

   * Een alleen-lezen maestro-recordtype dat verwijst naar het recordtype van derden waarnaar u in het verbonden recordveld hebt gekoppeld.

     Als u bijvoorbeeld een Maestro-recordtype verbindt met Workfront-projecten, wordt in dezelfde werkruimte een alleen-lezen recordtype gemaakt met de naam &quot;Workfront-projecten&quot;.
   * Alleen-lezen records in de pagina met recordtypen van derden. De records die u hebt geïmporteerd uit de toepassing van derden, blijven alleen-lezen en kunnen alleen in de oorspronkelijke toepassing worden bijgewerkt.


## Records maken door gegevens uit een externe lijst te kopiëren en te plakken

1. Start in Maestro records in de tabelweergave, zoals wordt beschreven in de sectie [Records maken door deze handmatig toe te voegen aan een recordtype](#create-records-by-manually-adding-them-to-a-record-type) in dit artikel.

   Zorg ervoor dat de tabel Maestro de kolommen (of de velden) bevat die u wilt vullen met de nieuwe recordgegevens.

1. Klikken **Nieuw &lt; Naam recordtype >** in de laatste rij van de tabel om zoveel nieuwe rijen aan de tabel toe te voegen als u wilt dat de nieuwe records worden gemaakt.

   Voeg bijvoorbeeld 10 rijen toe aan de tabelweergave als u de gegevens voor 10 nieuwe records uit een andere toepassing wilt plakken.

1. Maak in een andere toepassing een lijst met records die u wilt importeren in Maestro.

   U kunt bijvoorbeeld een Excel-werkblad gebruiken om uw lijst te maken.

   De lijst moet informatie in tabelvorm bevatten.

   >[!TIP]
   >
   > De kolommen in de lijst moeten informatie bevatten voor de bestaande velden die u in Maestro hebt.
   >
   > Zorg ervoor dat u de gewenste velden hebt die al in Maestro zijn gemaakt en dat de gegevens op uw blad in de juiste indeling worden weergegeven die overeenkomt met die van elk veld in Maestro.

1. Selecteer in de toepassing van derden meerdere rijen en kolommen en plak de informatie in de tabelweergave met recordtype, te beginnen met de eerste nieuwe record.

   De volgende informatie wordt geïmporteerd in Maestro:

   * De rijen bevatten de nieuwe records
   * De kolommen vullen informatie voor de gebieden van de verslagen.
