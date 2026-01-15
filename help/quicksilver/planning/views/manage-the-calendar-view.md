---
title: De kalenderweergave beheren
description: U kunt records en de bijbehorende velden weergeven in een kalenderweergave. In dit artikel wordt beschreven hoe u een kalenderweergave kunt maken en een bestaande weergave kunt bewerken of verwijderen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '1776'
ht-degree: 0%

---

# De kalenderweergave beheren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

U kunt records en de bijbehorende velden weergeven in een kalenderweergave, vanaf de pagina met recordtypen.

Voor informatie over de meningen van de Planning van Adobe Workfront en hoe te om hen te beheren, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

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
<p>Alle Workfront en alle planningspakketten</p>
<p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p> Standaard voor het maken en verwijderen van weergaven</p>
   <p>Medewerker of hoger om weergave-elementen bij te werken</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren voor een weergave</p>  
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen of te dupliceren</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
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
    <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
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
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table> -->

## Een kalenderweergave beheren {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Overweeg het volgende:

* U kunt alleen een kalenderweergave maken wanneer u ten minste twee datumvelden hebt die zijn gekoppeld aan een recordtype. Wanneer u een of geen datumvelden hebt gekoppeld aan een recordtype, wordt de optie voor de kalenderweergave grijs weergegeven.

  U kunt uit de gebieden van de verslagdatum, of raadplegingsdatumgebieden van verbonden verslag of objecten types selecteren.
* De volgende scenario&#39;s bestaan:

   * Wanneer zowel de begin- als einddatum geen waarden hebben, worden de records niet weergegeven in de kalender
   * Als de begin- of einddatum geen waarde hebben, wordt de record weergegeven als een eendaagse gebeurtenis
   * Wanneer de begindatum na de einddatum ligt, wordt de record niet weergegeven in de kalender.

Een kalenderweergave beheren:

1. Ga naar de recordtypepagina waarvoor u de kalender wilt bekijken.
1. Creeer een kalendermening, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).

   ![ de meningsvoorbeeld van de Kalender ](assets/calendar-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden in een kalender weergegeven als balken. De kleur van de balken komt standaard overeen met de kleur van het recordpictogram.

1. Voer een van de volgende handelingen uit om door de kalender te navigeren:

   * Klik op de linker- en rechterpictogrammen in de linkerbovenhoek van de kalender of gebruik de horizontale schuifregelaar om in de kalender voor- en achteruit te gaan.
   * Klik **vandaag** in de hoger-juiste hoek om de kalender aan de datum van vandaag te centreren.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor de tijd om de tijdstappen bij te werken:

      * **Maand**: De vertoningen van verslagen in een maandelijkse kalender.

      * **Week**: De vertoning van verslagen op de volgende gebieden:

         * Records die zich uitstrekken over meerdere dagen worden boven aan de kalender weergegeven.
         * Records die een dag of minder duren, worden weergegeven in de onderste helft van de kalenderweergave. Als u hebt opgegeven dat u het uur van de begin- en einddatum wilt weergeven, wordt de record op het juiste tijdstip weergegeven binnen de dag dat deze plaatsvindt.

1. (Facultatief) klik het **Volledige het schermpictogram** pictogram ![ open volledig het schermpictogram ](assets/open-full-screen-icon.png) om de mening in volledig scherm te openen, dan de **Uitgang volledig scherm** pictogram ![ van de Uitgang het volledige het schermpictogram ](assets/exit-full-screen-icon.png) of Escape op uw toetsenbord om het volledige scherm weg te gaan.

1. Voer een van de volgende handelingen uit om records te maken in de kalenderweergave of de datums ervan te bewerken:

   * Dubbelklik op een willekeurige plaats in de kalender om een record te maken.

     Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.

   * Klik op de linker- of rechtermarge van een recordbalk en sleep deze naar een nieuwe positie. Als u de grootte van de balken van de records wijzigt, worden de begin- of einddatums onmiddellijk bijgewerkt.

   * Sleep de recordbalken om hun positie en datums bij te werken. Als u de balken van de records verplaatst, worden de begin- en einddatum onmiddellijk bijgewerkt.

     Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [Filters](#add-filters)
   * [Rijhoogte](#modify-row-height)
   * [Instellingen](#edit-the-calendar-view-settings)

   <!--* [Grouping](#add-grouping)-->
   <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Filters toevoegen

U kunt de hoeveelheid informatie die op het scherm wordt weergegeven verminderen door filters te gebruiken.

Houd rekening met het volgende wanneer u werkt met filters in de kalenderweergave:

<!-- this list is almost identical to the one for the table view - update both-->

* De filters die u voor een kalenderweergave maakt, werken onafhankelijk van de filters in een andere weergave die op hetzelfde recordtype is toegepast.

* De filters zijn uniek voor de weergave die u selecteert. Op twee kalenderweergaven van hetzelfde recordtype kunnen verschillende filters worden toegepast.

* Twee gebruikers die naar dezelfde kalenderweergave kijken, zien hetzelfde filter dat op dat moment wordt toegepast.

* U kunt de filters die u maakt voor een kalenderweergave niet een naam geven.

* Als u filters verwijdert, worden deze verwijderd van iedereen die hetzelfde recordtype als u benadert en die dezelfde weergave als u weergeeft.

* U kunt filteren op gekoppelde recordvelden of opzoekvelden.

* U kunt filteren door velden op te zoeken waarin meerdere waarden worden weergegeven.

Een filter toevoegen aan een kalenderweergave:

1. Creeer een kalendermening voor een verslagtype pagina, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).
1. Selecteer een kalendermening, dan klik **Filters** in de toolbar van de kalender.
1. Klik **toevoegen voorwaarde** en voeg de volgende informatie toe:

   * **selecteer een gebied** om naar een gebied te zoeken en het van de lijst te selecteren

   * **selecteer een optie** (of een filterbepaling) om te bepalen welk soort voorwaarde het gebied moet ontmoeten

     In de onderstaande tabel worden de beschikbare wijzigingstoetsen voor elk veldtype weergegeven.

     <table>
        <thead>
        <tr>
            <th><b>Veldtype</b></th>
            <th><b>Modifiers</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Enkele regel, alinea, formule </td>
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
            <td>Meerdere selecties, personen</td>
            <td><p>Heeft een van de</p>
            <p>Bevat alle</p>
            <p>Is exact</p>
            <p>Heeft geen van</p>
            <p>Is leeg</p>
            <p>Is niet leeg</p></td>
        </tr>
        <tr>
            <td>Getal, percentage, valuta</td>
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

   ![ de lijstmening van de Filter UI ](assets/filter-ui-table-view.png)

   Er is geen limiet voor het aantal filtervoorwaarden dat u kunt toevoegen.

1. (Facultatief) klik **toevoegen voorwaarde** om een andere het filtreren optie toe te voegen en de bovengenoemde stappen te herhalen. Links van het pictogram Filters ziet u het aantal toegepaste filters.
1. Klik op de volgende operatoren om aan te geven hoe de filtervoorwaarden worden gekoppeld en moeten worden toegepast:

   * **EN**: Alle gespecificeerde voorwaarden moeten worden voldaan aan.
   * **OF**: Om het even welke gespecificeerde voorwaarden moeten worden voldaan aan. Dit is de standaardoptie.

   1. (Facultatief) voeg extra **EN** of **OF** exploitanten tussen veelvoudige voorwaardengroeperingen toe.

      ![ Multi-tiered filters in meningen ](assets/multi-tiered-filters-in-views.png)

   De lijst met records wordt automatisch gefilterd.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Facultatief) klik het **x** pictogram om een filtervoorwaarde te verwijderen.
1. (Facultatief) klik **Filters** om de filterdoos te sluiten. <!--right now you cannot "clear all" for filters, but this might come later-->


### Rijhoogte wijzigen

U kunt de rijhoogte van een kalendercel wijzigen om het aantal recordbalken dat u in elke cel weergeeft, te verhogen of te verlagen.

Het aantal records dat in de kalender wordt weergegeven, is afhankelijk van het aantal velden dat u op de recordbalken weergeeft.

>[!TIP]
>
>Deze instelling is alleen beschikbaar wanneer u de kalender per maand weergeeft.


1. Creeer een kalendermening voor een verslagtype pagina, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).
1. (Voorwaardelijk) toon de kalendermening door maand, dan klik **de hoogte van de Rij** in de toolbar van de kalender.
1. Kies een van de volgende opties:

   <table>
    <thead>
    <tr>
        <th><b>Rijhoogte, optie</b></th>
        <th><b>Standaardmaximum aantal records</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>Kort</td>
        <td><p>Bevat:</p>

   <ul><li>2 records met 1 veld</li>
    <li>1 record met meer dan 1 veld</li></ul>
        </td>
    </tr>
    <tr><td>Standard</td>
        <td><p>Bevat:</p>

   <ul><li>4 records met 1 veld</li>
    <li>2 record met meer dan 1 veld</li></ul>
        </td>
    </tr>
    <tr>
        <td>Medium</td>
        <td><p>Bevat:</p>

   <ul><li>8 records met 1 veld</li>
    <li>4 records met meer dan 1 veld</li></ul>
        </td>
    </tr>
    <tr>
        <td>Lang</td>
        <td><p>Bevat:</p>

   <ul><li>12 records met 1 veld</li>
    <li>6 records met meer dan 1 veld</li></ul>
        </td>
    </tr>
    <tr>
        <td>Aanpassen aan inhoud</td>
        <td><p>Alle records zijn zichtbaar, tot 500 records</p></td>
    </tr>
    </tbody>
    </table>

1. (Facultatief) klik **meer** als er verslagen zijn die niet zichtbaar in de kalender zijn.

</span>

### De instellingen van de kalenderweergave bewerken

Werk de instellingen van de kalenderweergave bij om aan te geven wat en hoe informatie in de weergave wordt weergegeven.

1. Creeer een kalendermening voor een verslagtype, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).
1. Klik **Montages**.
1. Klik **Datum en tijd** in het linkerpaneel, dan de datum van het a **Begin** en een **einddatum** om op de kalender te tonen. U kunt de standaardbegin- en einddatum kiezen of een datumveld kiezen dat beschikbaar is.

   De balken die de records weergeven, beginnen op de datum die u aangeeft voor de begindatum en eindigen op de datum die overeenkomt met de einddatum.

   >[!NOTE]
   >
   >* Records die geen waarden hebben voor de begin- of einddatum of die later een begindatum hebben dan de einddatum, worden niet weergegeven in de kalenderweergave.
   >
   >* Als u aanvullende records weergeeft met de optie Indeling, zijn de begin- en einddatums die van de hoofdrecord. U kunt geen begin- en einddatums kiezen voor de verbonden records in dit gebied.

1. Klik **stijl van de Bar** in het linkerpaneel, om te wijzen op welke informatie u op de verslagbars wilt tonen.

   Het primaire veld (of de titel) van de record, zoals gedefinieerd in de tabelweergave van de record, wordt standaard geselecteerd.
   <!--adjust this when the primary field is released??-->

1. (Facultatief en voorwaardelijk) als u duimnagels aan verslagen toevoegde, selecteer de **optie van de Duimnagel** om het beeld te tonen verbonden aan verslagen in hun verslagbar.

   >[!NOTE]
   >
   >    U moet eerst miniaturen toevoegen in de tabelweergave voordat u ze kunt weergeven in de kalenderweergave. Voor meer informatie, zie [ een duimnagel aan een verslag ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toevoegen.

1. Klik **toevoegen gebied**, dan klik binnen het **vakje van het Onderzoek gebieden**, en klik het gebied u wilt toevoegen.

   >[!TIP]
   >
   >   * U moet de velden maken voordat u deze aan de recordbalken kunt toevoegen.
   > 
   >   * Er moet ten minste één veld zijn geselecteerd. **Naam** wordt geselecteerd door gebrek.
   >
   >   * U kunt maximaal vijf velden toevoegen.

   Aan de rechterkant wordt een voorbeeld weergegeven van hoe de balken eruit zullen zien op de kalender.

   ![ de stijlsectie van de Bar in de montages van de kalendermening ](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. Klik **Kleur** in het linkerpaneel, om de kleuren van de verslagen op de kalender aan te passen.

   ![ paneel van de Kleur op de montages van de kalendermening ](assets/color-panel-on-calendar-view-settings.png)

1. In de **Vastgestelde verslagkleur aan** sectie, selecteer van de volgende opties om een kleur voor de verslagen te plaatsen:

   * **type van Verslag**: De kleur van de verslagbars in de kalender past de kleur van het verslagtype aan u selecteerde. Dit is de standaardoptie.
   * **waarden van het Gebied**: De kleur van de verslagen past de kleur van een gebied aan dat u specificeert.
   * **niets**: De vertoningen van verslagen in een witte bar.

1. (Voorwaardelijk) als u **waarden van het Gebied** voor de verslagkleuren selecteerde, selecteer een gebied van **gelijke de verslagkleur aan** drop-down menu.

   ![ de selecteur van het Gebied drop-down menu voor kalendermening ](assets/field-selector-drop-down-menu-calendar-view.png)

   Alleen velden met opties voor kleurcodes worden weergegeven in het keuzemenu.

   Multiselect- of single-select-velden kunnen bijvoorbeeld kleuropties hebben.

   Als u geen veld hebt met kleurgecodeerde opties voor het geselecteerde recordtype, wordt deze optie grijs weergegeven.


1. Klik **sparen**.

   De records worden in de kalenderweergave weergegeven met de specificaties die u hebt geselecteerd.