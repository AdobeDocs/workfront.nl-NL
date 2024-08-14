---
title: De tijdlijnweergave beheren
description: U kunt records weergeven in een tijdlijnweergave wanneer u de pagina met recordtypen opent in Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '1888'
ht-degree: 0%

---

# De tijdlijnweergave beheren

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

U kunt records weergeven in een tijdlijnweergave wanneer u de pagina met recordtypen opent in Adobe Workfront Planning.

Voor informatie over verslagmeningen, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <p> Adobe Workfront</p> </td>
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
   of
   <p>Huidig: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> Er zijn geen toegangscontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren voor een weergave</p>  
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> <p>Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Een tijdlijnweergave beheren {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Wanneer u een tijdlijnweergave maakt, worden alle records van het geselecteerde recordtype weergegeven in een chronologische tijdlijn.

Overweeg het volgende:

* U kunt alleen een tijdlijnweergave maken wanneer u ten minste twee datumvelden hebt gekoppeld aan een recordtype. Wanneer u een of geen datumvelden hebt gekoppeld aan een recordtype, wordt de optie voor de tijdlijnweergave grijs weergegeven.

  U kunt uit de gebieden van de verslagdatum, of raadplegingsdatumgebieden van verbonden verslag of objecten types selecteren.
* Afhankelijk van de datums die aan de records zijn gekoppeld, worden sommige records mogelijk niet in de tijdlijnweergave weergegeven in de volgende scenario&#39;s:

   * Wanneer de begin- en einddatum geen waarden hebben
   * Wanneer de begin- of einddatum geen waarde hebben
   * Wanneer de begindatum na de einddatum ligt

Een tijdlijnweergave beheren:

1. Ga naar de pagina met recordtypen waarvoor u de tijdlijn wilt weergeven.
1. Creeer een chronologiemening, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden standaard als balken in een tijdlijn weergegeven en gesorteerd in chronologische volgorde van hun begindatum.

   >[!TIP]
   >
   >    Het sorteren van de records in de tijdlijn is niet zichtbaar in de compacte weergave.


1. Voer een van de volgende handelingen uit om door de tijdlijn te navigeren:

   * Klik op de pictogrammen links en rechts of gebruik de horizontale schuifbalk om naar voren en naar achteren in de tijdlijn te gaan. Als u de pagina vernieuwt, blijft het geselecteerde tijdkader behouden.
   * Klik **vandaag** om de chronologie aan de datum van vandaag te centreren.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor het tijdframe om de tijdtoename bij te werken:

      * Jaar
      * Kwart
      * Maand
1. Klik **Schakelaar aan Standaard** mening om verslagen in afzonderlijke lijnen <!--check to see if they updated the name of the setting here--> te tonen

   of

   Klik **Schakelaar aan Compacte mening** om de verslagen te tonen waarvan data niet op de zelfde lijn snijden. <!--check to see if they updated the name of the setting here-->

   Records worden standaard weergegeven in de compacte weergave.

1. Ga als volgt te werk om snel records te zoeken die overeenkomen met een trefwoord:

   1. Klik het **pictogram van het 1} Onderzoek ![](assets/search-icon.png) en begin een sleutelwoord verbonden aan om het even welk gebied van een verslag te typen dat op het scherm toont.** Het aantal juiste overeenkomsten wordt weergegeven naast het zoekitem en de record met de juiste overeenkomst wordt gemarkeerd.

      ![](assets/search-box-and-results-timeline-view.png)

      U kunt elk woord of speciaal teken gebruiken dat op het scherm zichtbaar is.

      U kunt geen trefwoorden gebruiken die zijn gekoppeld aan velden die niet worden weergegeven in de tijdlijnweergave.

   1. Druk op Enter op het toetsenbord om naar het volgende gevonden veld te gaan.
   1. (Optioneel) Als er meer dan één overeenkomst is, klikt u op de pijl-omhoog of -omlaag rechts van het trefwoord Zoeken om alle overeenkomende items in de tabel te zoeken.
   1. Klik het **x** pictogram in het onderzoeksvakje om het onderzoekssleutelwoord te ontruimen.

1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [Filters](#add-filters)
   * [Groepering](#add-grouping)
   * [ Montages ](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Filters toevoegen

U kunt de hoeveelheid informatie die op het scherm wordt weergegeven verminderen door filters te gebruiken.

Houd rekening met het volgende wanneer u werkt met filters in de tijdlijnweergave:

<!-- this list is almost identical to the one for the table view - update both-->

* De filters die u voor een tijdlijnweergave maakt, werken onafhankelijk van de filters in een andere weergave die op hetzelfde recordtype is toegepast.

* De filters zijn uniek voor de weergave die u selecteert. Op twee tijdlijnweergaven van hetzelfde recordtype kunnen verschillende filters worden toegepast.

* Twee gebruikers die naar dezelfde tijdlijnweergave kijken, zien hetzelfde filter dat op dat moment wordt toegepast.

* U kunt de filters die u maakt voor een tijdlijnweergave niet een naam geven.

* Als u filters verwijdert, worden deze verwijderd van iedereen die hetzelfde recordtype als u benadert en die dezelfde weergave als u weergeeft.

* Het toevoegen van filters in de tijdlijnweergave is hetzelfde als het toevoegen van filters in de tabelweergave.

  Voor meer informatie, zie &quot;filters&quot;sectie in artikel [ toevoegen de lijstmening ](/help/quicksilver/planning/views/manage-the-table-view.md) leidt.

* U kunt filteren op gekoppelde recordvelden of opzoekvelden.
* U kunt filteren door velden op te zoeken waarin meerdere waarden worden weergegeven.


### Groepering toevoegen

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

U kunt records groeperen aan de hand van vergelijkbare informatie wanneer u een groepering toepast op een weergave.

Het toevoegen van groepen in de tijdlijnweergave lijkt op het toevoegen van groepen aan de tabelweergave.

Houd rekening met het volgende wanneer u werkt met groepen in de tijdlijnweergave:

* U kunt groepen toepassen in de tabel- en tijdlijnweergave. De groepen van de tabelweergave zijn onafhankelijk van de groepen in de tijdlijnweergave van hetzelfde recordtype.
* U kunt 3 niveaus van groepering in een mening toepassen. De records worden gegroepeerd in de volgorde van de groepen die u selecteert.
&lt;!—* U kunt tot 4 niveaus van groepering toepassen wanneer het gebruiken van API. —deze nu controleren—>
* De groepen zijn uniek voor de weergave die u selecteert. Op twee tabelweergaven van hetzelfde recordtype kunnen verschillende groepen worden toegepast. Twee gebruikers die naar dezelfde tabelweergave kijken, zien dezelfde groepering die momenteel wordt toegepast.
* U kunt de groepen die u maakt voor een tabelweergave niet een naam geven.
* Als u groepen verwijdert, worden deze verwijderd van iedereen die toegang heeft tot hetzelfde recordtype als u en die dezelfde weergave weergeeft als u.
* U kunt records bewerken die in een groep worden vermeld.
* U kunt groeperen door verbonden verslaggebieden of raadplegingsgebieden.
* Wanneer u door raadplegingsgebieden met veelvoudige waarden groepeert (die niet door een aggregator zijn samengevat), worden de verslagen gegroepeerd door elke unieke combinatie gebiedswaarden.
* U kunt verwijzen naar een veld dat zich op maximaal 4 niveaus van het huidige recordtype bevindt. Bijvoorbeeld, als u een groepering voor een type van het verslag van de Activiteit creeert, en de Activiteit wordt verbonden met het type van het Verslag van het Product dat met het verslagtype van de Campagne wordt verbonden dat met een Project van Workfront wordt verbonden, kunt u de Status van het project in de groepering verwijzen u voor het verslagtype van de Activiteit creeert.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Een groep toevoegen in de tijdlijnweergave:

1. Creeer een chronologiemening voor een verslagtype, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).
1. Klik **Groepering** in de hoger-juiste hoek van de chronologiemening.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klik één van de voorgestelde gebieden, of klik **kies een verschillend gebied**, onderzoek naar een verschillend gebied, dan klik het wanneer het in de lijst toont.

   De groepering wordt automatisch toegepast op de tijdlijn en records worden weergegeven in het groepsvak.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Optioneel) Herhaal de bovenstaande stappen om maximaal drie groepen samen te voegen.

   Het aantal velden dat voor de groepering is geselecteerd, wordt weergegeven naast het pictogram Groeperen.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facultatief) binnen de **verslagen van de Groep door** doos, klik het **x** pictogram aan het recht van een gebied dat voor de groepering wordt geselecteerd om de groepering te verwijderen

   of

   Klik **ontruimen allen** om alle gebieden te verwijderen.

1. Klik buiten de **verslagen van de Groep door** doos om het te sluiten.
1. (Facultatief) klik **Montages**, toen **Kleur** aan kleur-code groeperingen. Voor meer informatie, zie [ uitgeven de sectie van de chronologiemening montages ](#edit-the-timeline-view-settings) in dit artikel.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### De weergave-instellingen voor de tijdlijn bewerken {#edit-the-timeline-view-settings}

Werk de instellingen van de tijdlijnweergave bij om aan te geven wat en hoe informatie wordt weergegeven in het tijdlijngedeelte van de weergave.

1. Creeer een chronologiemening voor een verslagtype, zoals die in artikel [ wordt beschreven beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md).
1. Klik **Montages**.
1. Klik **Datum en tijd** in het linkerpaneel, dan de datum van het a **Begin** en een **einddatum** om op de chronologie te tonen. U kunt de standaardbegin- en einddatum kiezen of een datumveld kiezen dat beschikbaar is. De balken die de records weergeven, beginnen op de datum die u aangeeft voor de begindatum en eindigen op de datum die overeenkomt met de einddatum.

   >[!NOTE]
   >
   >Records die geen waarden hebben voor de begin- of einddatum of die later een begindatum hebben dan de einddatum, worden niet weergegeven in de tijdlijnweergave.

1. Klik **stijl van de Bar** in het linkerpaneel, om te wijzen op welke gebieden u op de verslagbars wilt tonen.

   Het primaire veld (of de titel) van de record, zoals gedefinieerd in de tabelweergave van de record, wordt standaard geselecteerd. <!--adjust this when the primary field is released??-->

1. (Optioneel en voorwaardelijk) Als u miniaturen aan records hebt toegevoegd, selecteert u de optie Miniatuur om de afbeelding weer te geven die aan records is gekoppeld in de recordbalk.

   >[!NOTE]
   >
   >    U moet eerst miniaturen toevoegen in de tabelweergave voordat u ze kunt weergeven in de tijdlijnweergave. Voor meer informatie, zie [ een duimnagel aan een verslag ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toevoegen.

1. Klik **voeg gebied** toe om tot 4 gebieden aan de verslagbars toe te voegen.
1. Klik binnen de **gebieden van het Onderzoek** doos, en klik het gebied u wilt toevoegen.

   >[!TIP]
   >
   >   * U moet de velden maken voordat u deze aan de recordbalken kunt toevoegen.
   > 
   >   * Er moet ten minste één veld zijn geselecteerd. **Naam** wordt geselecteerd door gebrek.

   Aan de rechterkant wordt een voorvertoning weergegeven van hoe de balken eruit zullen zien op de tijdlijn.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klik **Kleur** in het linkerpaneel, om de kleuren van de verslagen en de groeperingen in de chronologie aan te passen.

   ![](assets/color-tab-timeline-view.png)

1. (Voorwaardelijk en facultatief) als u een groepering aan de chronologiemening toevoegde, selecteer van de volgende opties om een kleur voor de groepering in de **Vastgestelde groeperingskleur** sectie te plaatsen:

   * **Gebrek (grijs)**: De kleur van de groeperingen wordt geplaatst aan grijs. Dit is de standaardinstelling.
   * **waarden van het Gebied**: De kleur van de groeperingen past de kleur van het gebied aan u groepert door.

     >[!NOTE]
     >
     >    * U kunt de kleur alleen aanpassen aan velden met opties voor kleurcodes. U kunt bijvoorbeeld de kleur aanpassen aan statusvelden of aan velden met opties die zijn gekoppeld aan kleuren.
     >    
     >    * U kunt de kleur niet aanpassen aan opzoekvelden van gekoppelde record- of objecttypen.


   Multiselect- of single-select-velden kunnen bijvoorbeeld kleuropties hebben.

   Als u groepeert op velden zonder opties voor kleurcodering, blijft de kleur van de groep grijs.

   >[!TIP]
   >
   >Als u geen groepen hebt toegevoegd aan de tijdlijnweergave, wordt deze sectie niet weergegeven.

1. In de **plaats verslagkleur** sectie, selecteer van de volgende opties om een kleur voor de verslagen te plaatsen:

   * **type van Verslag**: De kleur van de verslagen past de kleur van het verslagtype aan u selecteerde. Dit is de standaardoptie.
   * **waarden van het Gebied**: De kleur van de verslagen past de kleur van een gebied aan dat u specificeert. Ga verder met stap 10. <!--ensure this stays accurate-->
   * **Groepering**: De kleur van de verslagen past de kleur aan die u voor de groeperingen verwees. Deze optie is grijs als er geen groepen zijn toegepast op de tijdlijnweergave.
   * **niets**: De vertoningen van verslagen in een witte bar.

1. (Voorwaardelijk) als u **waarden van het Gebied** voor de verslagkleuren selecteerde, selecteer een gebied van **gelijke de verslagkleur aan** drop-down menu.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Alleen velden met opties voor kleurcodes worden weergegeven in het keuzemenu.

   Multiselect- of single-select-velden kunnen bijvoorbeeld kleuropties hebben.

   Als u geen veld hebt met kleurgecodeerde opties voor het geselecteerde recordtype, wordt deze optie grijs weergegeven.

1. Klik **sparen**.

   De records worden in de tijdlijnweergave weergegeven met de specificaties die u hebt geselecteerd.
