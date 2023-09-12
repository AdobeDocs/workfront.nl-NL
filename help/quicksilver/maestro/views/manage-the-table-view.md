---
title: De tabelweergave beheren
description: U kunt records en de bijbehorende velden in een tabelweergave weergeven wanneer u de pagina met recordtypen opent in Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: 4a3cf7211eef2b161a29b74e8e9b2b12c21eaf4d
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 0%

---


# De tabelweergave beheren

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt records en de bijbehorende velden in een tabelweergave weergeven wanneer u de pagina met recordtypen opent in Adobe Maestro.

Voor informatie over Maestro-weergaven en hoe deze te beheren, raadpleegt u [Recordweergaven beheren](../views/manage-record-views.md).

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

## Een tabelweergave beheren {#manage-a-table-view}

<!--insert screen shot of table view-->

Wanneer u een tabelweergave maakt, worden alle records van het geselecteerde type weergegeven in een tabel. Elke rij is een unieke record en elke kolom is een recordveld. Alle velden en alle records worden standaard weergegeven.

Een tabelweergave beheren:

1. Een tabelweergave maken, zoals wordt beschreven in het artikel [Recordweergaven beheren](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [Kolommen (of velden)](#add-columns-or-fields)
   * [Rijen (of records)](#add-rows-or-records)
   * [Filters](#add-filters)
   * [Groepering](#add-groupings)
   * [Sorteren](#sort-information)


### Kolommen (of velden) toevoegen {#add-columns}

De kolomkoppen van een Maestro- lijstmening tonen gebieden verbonden aan de verslagen in de mening. Dezelfde velden die in de tabelweergave worden weergegeven, worden ook weergegeven in de sectie Details van een Maestro-record. Zie voor meer informatie [Records bewerken](../records/edit-records.md).

<!-- this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. -->

Het toevoegen van kolommen aan een weergave is hetzelfde als het toevoegen van velden aan een recordtype.

U kunt maximaal 500 velden (of kolommen) toevoegen aan een tabelweergave.

1. Ga naar een recordtypepagina en selecteer een **Tabel** in het keuzemenu Weergave.
1. Beginnen met het toevoegen van velden (of kolommen), zoals beschreven in het artikel [Velden maken](../architecture-and-fields/create-fields.md).

   De kolommen die u toevoegt, zijn zichtbaar voor alle gebruikers die toegang hebben tot het recordtype en worden toegevoegd als nieuwe velden op de pagina Details van de records van het geselecteerde recordtype.

1. Voer een van de volgende handelingen uit om de kolommen in de tabel opnieuw te ordenen:

   * Pak de kolomkop en sleep deze naar de gewenste positie. De kolom die u kort hebt verplaatst, wordt weergegeven met een blauwe achtergrond totdat u andere aanpassingen in de tabel aanbrengt.

   * Klikken **Velden** in de werkbalk van de tabel, sleept u de velden in de gewenste volgorde en klikt u vervolgens buiten de **Velden, zichtbaarheid en volgorde** om het te sluiten.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)

   >[!TIP]
   >
   >* Het veld Naam is altijd het eerste veld in de tabelweergave.
   >
   >* U kunt het veld Naam niet naar een andere positie verplaatsen.
   >
   >* U kunt het veld Naam niet verbergen.
   >
   >* Het veld Naam is bevroren en maakt geen deel uit van de horizontale schuifbalk.

1. Als u de kolommen breder wilt maken, klikt u op de kolomscheidingslijnen en sleept u deze naar de gewenste plaats.

   >[!TIP]
   >
   >De wijzigingen die u aanbrengt in de kolombreedte en -volgorde zijn permanent en zichtbaar voor alle gebruikers die toegang hebben tot het recordtype.

1. Als u een kolom wilt verbergen, houdt u de muisaanwijzer boven de kolomkop en klikt u op de pijl omlaag en vervolgens op **Veld verbergen**

   of

   Klikken **Velden** in de tabelwerkbalk en schakelt u de schakeloptie uit die is gekoppeld aan de velden die u wilt verbergen.

   >[!TIP]
   >
   >Het aantal verborgen velden wordt links van het pictogram Velden op de werkbalk weergegeven.


1. Van de **Velden** Als u deze instelling instelt, schakelt u de schakeloptie in die is gekoppeld aan de velden die u wilt weergeven in de kolommen van de tabel. Alle velden worden standaard weergegeven.

### Rijen (of records) toevoegen {#add-rows}

De rijen van een Maestro- lijstmening tonen individuele verslagen van het geselecteerde verslagtype.

U kunt tot 10.000 verslagen (of rijen) voor een verslagtype in Maestro hebben.

Het toevoegen van rijen aan een Maestro- lijstmening is identiek aan het creëren van verslagen in een lijst.

Zie voor meer informatie [Records maken](../records/create-records.md).

<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### Filters toevoegen {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

Met filters vermindert u de hoeveelheid informatie die op het scherm wordt weergegeven.

Houd rekening met het volgende wanneer u werkt met filters in de tabelweergave:
<!-- this list is almost identical to the one for the table view - update both-->

* De filters die u voor de tabelweergave maakt, werken onafhankelijk van de filters in de tijdlijnweergave wanneer deze worden toegepast op hetzelfde recordtype.

* De filters zijn uniek voor de weergave die u selecteert. Op twee tabelweergaven van hetzelfde recordtype kunnen verschillende filters worden toegepast. Twee gebruikers die naar dezelfde tabelweergave kijken, zien hetzelfde filter dat op dat moment wordt toegepast.

* U kunt de filters die u maakt en toepast op een tabelweergave niet een naam geven.

* Als u filters verwijdert, worden deze verwijderd van iedereen die toegang heeft tot hetzelfde recordtype als u en wordt dezelfde weergave gebruikt als u gebruikt.

* Filters toevoegen aan de tabelweergave is hetzelfde als filters toevoegen aan de tijdlijnweergave.

Een filter toevoegen aan een tabelweergave:

1. Een tabelweergave maken voor een pagina met recordtypen, zoals wordt beschreven in het artikel [Recordweergaven beheren](../views/manage-record-views.md).
1. Selecteer een tabelweergave en klik op **Filters** rechtsboven in de tabel.
1. Klikken **Voorwaarde toevoegen** en voeg de volgende informatie toe:

   * Selecteer een veld waarop u wilt filteren <!-- the tip below might change-->

   * Selecteer een optie (of een filteroptie) om te bepalen aan welke voorwaarde het veld moet voldoen

     In de onderstaande tabel worden de beschikbare wijzigingstoetsen voor elk veldtype weergegeven.

     >[!TIP]
     >
     > U kunt geen gekoppelde velden selecteren. Zie voor meer informatie [Velden maken](../architecture-and-fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>Veldtype</b></th>
            <th><b>Modifiers</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Enkele regel, alinea </td>
            <td><p>Bevat</p>
            <p>Bevat niet</p>
            <p>Is</p>
            <p>Is niet</p>
            <p>Is leeg</p>
            <p>Is niet leeg</p></td>
        </tr>
        <tr><td>Enkel selecteren</td>
            <td><p>Is</p>
            <p>Is niet</p>
            <p>Is om het even welke</p>
            <p>Is geen van</p>
            <p>Is leeg</p>
            <p>Is niet leeg</p></td>
        </tr>
        <tr>
            <td>Meerdere selecties</td>
            <td><p>Heeft een van de</p>
            <p>Bevat alle</p>
            <p>Is exact</p>
            <p>Heeft geen van</p>
            <p>Is leeg</p>
            <p>Is niet leeg</p></td>
        </tr>
        <tr>
            <td>Numeriek, percentage, valuta</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Is leeg</p>
            <p>Is niet leeg</p></td>
        </tr>
        <tr>
            <td>Datum</td>
            <td><p>Is</p>
            <p>Is niet</p>
            <p>Is na</p>
            <p>Is voor</p>
            <p>Is tussen</p><p>Is niet tussen</p>
            <p>Is leeg</p><p>Is niet leeg</p></td>
        </tr>

     <tr>
            <td>Selectievakje</td>
            <td><p>Is</p>
        </tr>
        </tbody>
        </table>

   * Selecteer een waarde voor het geselecteerde veld.

   ![](assets/filter-ui-table-view.png)

   Er is geen limiet voor het aantal filtervoorwaarden dat u kunt toevoegen.

1. (Optioneel) Klik op **Voorwaarde toevoegen** om nog een filteroptie toe te voegen en de bovenstaande stappen te herhalen. Links van het pictogram Filters ziet u het aantal toegepaste filters.
1. Klik op de volgende operatoren om aan te geven hoe de filtervoorwaarden worden gekoppeld en moeten worden toegepast:

   * **en**: Aan alle opgegeven voorwaarden moet worden voldaan.
   * **of**: Aan alle opgegeven voorwaarden moet worden voldaan. Dit is de standaardoptie.

   De lijst met records wordt automatisch gefilterd.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Optioneel) Klik op **Filters** en klik vervolgens op de knop **x** pictogram om een filter te verwijderen. <!--right now you cannot "clear all" for filters, but this might come later-->

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. (***************check on this; this might be true for timeline, but not for table??? One dev said in a demo that there are unlimited groupings in a table - check *********************)
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. 
    
        >[!TIP]
        >
        > You cannot select linked fields. For information, see [Create fields](../architecture-and-fields/create-fields.md).  
    The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

-->

### Een sortering toevoegen {#sort-information}

Door een sortering toe te passen, kunt u informatie in een bepaalde orde organiseren.

U kunt de volgende gegevens sorteren:

* Alle records in een tabelweergave. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Houd rekening met het volgende wanneer u records in de tabelweergave sorteert:

<!-- if this is available for the timeline view, update both when you update one-->

* Sorteren is uniek voor de weergave die u selecteert. Twee tabelweergaven van hetzelfde recordtype kunnen verschillende sorteercriteria hebben. Twee gebruikers die naar dezelfde tabelweergave kijken, zien dezelfde sortering die momenteel wordt toegepast.

* U kunt de tekenreeksen die u maakt en toepast op een tabelweergave niet een naam geven.

* Het sorteren dat u maakt, blijft behouden wanneer u wegnavigeert.

* U kunt sorteren op zoveel velden als u ziet in de tabelweergave van een recordtype.

* Als u sorteercriteria verwijdert, worden deze verwijderd van iedereen die toegang heeft tot hetzelfde recordtype als u en wordt dezelfde weergave gebruikt als u.

Sorteren <!--ungrouped (add this when sorting for groupings will be available--> records, voert u de volgende handelingen uit:

1. Een tabelweergave maken, zoals wordt beschreven in het artikel [Recordweergaven beheren](../views/manage-record-views.md).
1. Klik op de knop **Sorteren** pictogram ![](assets/sort-icon.png) rechtsboven in de tabel

   of

   Houd de muis boven de naam van een kolom in de tabelweergave en klik op de pijl omlaag rechts van de kolomkopnaam en klik vervolgens op **Sorteren op dit veld**. Het veld wordt als een sorteerselectie toegevoegd in het pictogram Sorteren rechtsboven in de tabelweergave.
1. In de **Records sorteren op** klikt u op een van de voorgestelde velden of op **Een ander veld kiezen** en zoek naar een ander veld. Klik vervolgens op het veld wanneer het wordt weergegeven in de lijst.

   De sortering wordt automatisch toegepast op de tabelweergave en records worden gesorteerd op de geselecteerde criteria.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Optioneel) Herhaal bovenstaande stappen om te sorteren op extra velden.

   Het aantal velden dat u sorteert, wordt links van het pictogram Sorteren in de rechterbovenhoek van de werkbalk weergegeven. U kunt alleen velden kiezen die in de kolommen van de tabelweergave worden weergegeven.

   >[!TIP]
   >
   > U kunt geen gekoppelde velden selecteren. Zie voor meer informatie [Velden maken](../architecture-and-fields/create-fields.md).

1. (Optioneel) In het dialoogvenster **Records sorteren op** klikt u op **x** pictogram rechts van een sorteerveld om de sortering te verwijderen

   of

   Klikken **Alles wissen** om alle velden uit de sortering te verwijderen.

1. Klik buiten de **Records sorteren op** te sluiten.

   De gegevens in de tabel worden gesorteerd op basis van de geselecteerde criteria.

   In de velden die u voor de sortering selecteert, wordt een sorteerpictogram weergegeven, gevolgd door een getal dat de volgorde aangeeft waarin de sortering wordt toegepast.

   ![](assets/sorting-in-table-view.png)


<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->