---
title: De tijdlijnweergave beheren
description: U kunt records weergeven in een tijdlijnweergave wanneer u de pagina met recordtypen opent in Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: a923d86f78e6dab4705289a8165c4b31ff68b5a2
workflow-type: tm+mt
source-wordcount: '1724'
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

Voor informatie over recordweergaven raadpleegt u [Recordweergaven beheren](/help/quicksilver/planning/views/manage-record-views.md).

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
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
   <p>Systeembeheerders hebben alleen toegang tot de weergaven die ze hebben gemaakt of die met hen worden gedeeld. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuratie op toegangsniveau</td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten voor de weergave beheren</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied van de Planning in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="/help/quicksilver/planning/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


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
1. Een tijdlijnweergave maken, zoals wordt beschreven in het artikel [Recordweergaven beheren](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden standaard als balken in een tijdlijn weergegeven en gesorteerd in chronologische volgorde van hun begindatum.

   >[!TIP]
   >
   >    Het sorteren van de records in de tijdlijn is niet zichtbaar in de compacte weergave.


1. Voer een van de volgende handelingen uit om door de tijdlijn te navigeren:

   * Klik op de pictogrammen links en rechts of gebruik de horizontale schuifbalk om naar voren en naar achteren in de tijdlijn te gaan.
   * Klikken **Vandaag** om de tijdlijn te centreren op de datum van vandaag.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor het tijdframe om de tijdtoename bij te werken:

      * Jaar
      * Kwart
      * Maand
1. Klikken **Overschakelen naar standaard** weergeven om records in afzonderlijke regels weer te geven <!--check to see if they updated the name of the setting here-->

   of

   Klikken **Overschakelen naar compacte weergave** om de records weer te geven waarvan de datums elkaar niet op dezelfde regel snijden. <!--check to see if they updated the name of the setting here-->

   Records worden standaard weergegeven in de compacte weergave.

1. Ga als volgt te werk om snel records te zoeken die overeenkomen met een trefwoord:

   1. Klik op de knop **Zoeken** pictogram ![](assets/search-icon.png) en begint een sleutelwoord te typen verbonden aan om het even welk gebied van een verslag dat op het scherm toont. Het aantal juiste overeenkomsten wordt weergegeven naast het zoekitem en de record met de juiste overeenkomst wordt gemarkeerd.

      ![](assets/search-box-and-results-timeline-view.png)

      U kunt elk woord of speciaal teken gebruiken dat op het scherm zichtbaar is.

      U kunt geen trefwoorden gebruiken die zijn gekoppeld aan velden die niet worden weergegeven in de tijdlijnweergave.

   1. Druk op Enter op het toetsenbord om naar het volgende gevonden veld te gaan.
   1. (Optioneel) Als er meer dan één overeenkomst is, klikt u op de pijl-omhoog of -omlaag rechts van het trefwoord Zoeken om alle overeenkomende items in de tabel te zoeken.
   1. Klik op de knop **x** in het zoekvak om het zoekwoord te wissen.

1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [Filters](#add-filters)
   * [Groepering](#add-grouping)
   * [Instellingen](#edit-the-timeline-view-settings)
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

  Zie de sectie Filters toevoegen in het artikel voor meer informatie [De tabelweergave beheren](/help/quicksilver/planning/views/manage-the-table-view.md).

* U kunt filteren door verbonden verslaggebieden of raadplegingsgebieden, maar niet voor die gebieden die het verbinden aan veelvoudige verslagen toestaan.

### Groepering toevoegen

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

U kunt records groeperen aan de hand van vergelijkbare informatie wanneer u een groepering toepast op een weergave.

Het toevoegen van groepen in de tijdlijnweergave lijkt op het toevoegen van groepen aan de tabelweergave.

Houd rekening met het volgende wanneer u werkt met groepen in de tijdlijnweergave:

* U kunt groepen toepassen in de tabel- en tijdlijnweergave. De groepen van de tabelweergave zijn onafhankelijk van de groepen in de tijdlijnweergave van hetzelfde recordtype.
* U kunt 3 niveaus van groepering in een mening toepassen. De records worden gegroepeerd in de volgorde van de groepen die u selecteert.
* U kunt tot 4 niveaus van groepering toepassen wanneer het gebruiken van API.
* De groepen zijn uniek voor de weergave die u selecteert. In twee tijdlijnweergaven van hetzelfde recordtype kunnen verschillende groeperingen worden toegepast. Twee gebruikers die naar dezelfde tijdlijnweergave kijken, zien dezelfde groepering die op dat moment wordt toegepast.
* U kunt de groepen die u maakt voor een tijdlijnweergave niet een naam geven.
* Als u groepen verwijdert, worden deze verwijderd van iedereen die toegang heeft tot hetzelfde recordtype als u en die dezelfde weergave weergeeft als u.
* U kunt groeperen door verbonden verslaggebieden of raadplegingsgebieden, maar niet voor die gebieden die het verbinden aan veelvoudige verslagen toestaan.

Een groep toevoegen in de tijdlijnweergave:

1. Een tijdlijnweergave maken voor een recordtype, zoals beschreven in het artikel [Recordweergaven beheren](/help/quicksilver/planning/views/manage-record-views.md).
1. Klikken **Groepering** in de rechterbovenhoek van de tijdlijnweergave.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klik op een van de voorgestelde velden of klik op **Een ander veld kiezen**, zoek naar een ander veld en klik op het veld wanneer het in de lijst wordt weergegeven.

   De groepering wordt automatisch toegepast op de tijdlijn en records worden weergegeven in het groepsvak.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Optioneel) Herhaal de bovenstaande stappen om maximaal drie groepen samen te voegen.

   Het aantal velden dat voor de groepering is geselecteerd, wordt weergegeven naast het pictogram Groeperen.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Optioneel) Binnen de **Records groeperen op** klikt u op **x** pictogram rechts van een veld dat is geselecteerd voor de groep om de groep te verwijderen

   of

   Klikken **Alles wissen** alle velden verwijderen.

1. Klik buiten de **Records groeperen op** te sluiten.
1. (Optioneel) Klik op **Instellingen** vervolgens **Kleur** aan kleurcodenegroepen. Zie de klasse [De weergave-instellingen voor de tijdlijn bewerken](#edit-the-timeline-view-settings) in dit artikel.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### De weergave-instellingen voor de tijdlijn bewerken {#edit-the-timeline-view-settings}

Werk de instellingen van de tijdlijnweergave bij om aan te geven wat en hoe informatie wordt weergegeven in het tijdlijngedeelte van de weergave.

1. Een tijdlijnweergave maken voor een recordtype, zoals beschreven in het artikel [Recordweergaven beheren](/help/quicksilver/planning/views/manage-record-views.md).
1. Klikken **Instellingen**.
1. Klikken **Datum en tijd** in het linkerdeelvenster selecteert u vervolgens een **Begindatum** en **Einddatum** om weer te geven op de tijdlijn. U kunt de standaardbegin- en einddatum kiezen of een datumveld kiezen dat beschikbaar is. De balken die de records weergeven, beginnen op de datum die u aangeeft voor de begindatum en eindigen op de datum die overeenkomt met de einddatum.

   >[!NOTE]
   >
   >Records die geen waarden hebben voor de begin- of einddatum of die later een begindatum hebben dan de einddatum, worden niet weergegeven in de tijdlijnweergave.

1. Klikken **Stijl van balk** in het linkerdeelvenster om aan te geven welke velden u op de recordbalken wilt weergeven.

   Het veld Naam is standaard geselecteerd. <!--adjust this when the primary field is released??-->

1. (Optioneel en voorwaardelijk) Als u miniaturen aan records hebt toegevoegd, selecteert u de optie Miniatuur om de afbeelding weer te geven die aan records is gekoppeld in de recordbalk.

   >[!NOTE]
   >
   >    U moet eerst miniaturen toevoegen in de tabelweergave voordat u ze kunt weergeven in de tijdlijnweergave. Zie voor meer informatie [Een miniatuur toevoegen aan een record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Klikken **Veld toevoegen** om maximaal vier velden aan de recordbalken toe te voegen.
1. Klik in het dialoogvenster **Zoeken in velden** en klik op het veld dat u wilt toevoegen.

   >[!TIP]
   >
   >   * U moet de velden maken voordat u deze aan de recordbalken kunt toevoegen.
   > 
   >   * Er moet ten minste één veld zijn geselecteerd. **Naam** is standaard geselecteerd.

   Aan de rechterkant wordt een voorvertoning weergegeven van hoe de balken eruit zullen zien op de tijdlijn.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klikken **Kleur** in het linkerdeelvenster om de kleuren van de records en groepen in de tijdlijn aan te passen.

   ![](assets/color-tab-timeline-view.png)

1. (Voorwaardelijk en optioneel) Als u een groepering aan de tijdlijnweergave hebt toegevoegd, kunt u een van de volgende opties selecteren om een kleur in te stellen voor de groepering in het dialoogvenster **Groeperingskleur instellen** sectie:

   * **Standaard (grijs)**: De kleur van de groepen is ingesteld op grijs. Dit is de standaardinstelling.
   * **Veldwaarden**: De kleur van de groepen komt overeen met de kleur van het veld waarop u groepeert.
U kunt de kleur van de groepen alleen aanpassen aan velden met opties voor kleurcodes.

   Multiselect- of single-select-velden kunnen bijvoorbeeld kleuropties hebben.

   Als u groepeert op velden zonder opties voor kleurcodering, blijft de kleur van de groep grijs.

   >[!TIP]
   >
   >Als u geen groepen hebt toegevoegd aan de tijdlijnweergave, wordt deze sectie niet weergegeven.

1. In de **Recordkleur instellen** selecteert u een van de volgende opties om een kleur in te stellen voor de records:

   * **Recordtype**: De kleur van de records komt overeen met de kleur van het geselecteerde recordtype. Dit is de standaardoptie.
   * **Veldwaarden**: De kleur van de records komt overeen met de kleur van een veld dat u opgeeft. Ga verder met stap 10. <!--ensure this stays accurate-->
   * **Groepering**: De kleur van de records komt overeen met de kleur die u voor de groepen hebt opgegeven. Deze optie is grijs als er geen groepen zijn toegepast op de tijdlijnweergave.
   * **Geen**: Records worden weergegeven in een witte balk.

1. (Voorwaardelijk) Als u **Veldwaarden** voor de recordkleuren selecteert u een veld in het dialoogvenster **De recordkleur afstemmen op** vervolgkeuzelijst.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Alleen velden met opties voor kleurcodes worden weergegeven in het keuzemenu.

   Multiselect- of single-select-velden kunnen bijvoorbeeld kleuropties hebben.

   Als u geen veld hebt met kleurgecodeerde opties voor het geselecteerde recordtype, wordt deze optie grijs weergegeven.

1. Klikken **Opslaan**.

   De records worden in de tijdlijnweergave weergegeven met de specificaties die u hebt geselecteerd.
