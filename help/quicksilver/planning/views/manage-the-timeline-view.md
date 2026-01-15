---
title: De tijdlijnweergave beheren
description: Open en bewerk records in een tijdlijnweergave op de pagina met recordtypen voor Adobe Workfront Planning. In dit artikel wordt beschreven hoe u een tijdlijnweergave kunt maken en een bestaande weergave kunt bewerken of verwijderen. Pas de tijdlijn aan met filters, groepen en instellingen. Gebruik de functie Onderverdeling om verbonden records weer te geven.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '3912'
ht-degree: 0%

---

# De tijdlijnweergave beheren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

U kunt records weergeven in een tijdlijnweergave wanneer u de pagina met recordtypen opent in Adobe Workfront Planning.

Voor informatie over verslagmeningen, zie [&#x200B; verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md) leiden.

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

## Een tijdlijnweergave beheren {#manage-a-timeline-view}

Wanneer u een tijdlijnweergave maakt, worden alle records van het geselecteerde recordtype weergegeven in een chronologische tijdlijn.

Overweeg het volgende:

* U kunt alleen een tijdlijnweergave maken wanneer u ten minste twee datumvelden hebt gekoppeld aan een recordtype. Wanneer u een of geen datumvelden hebt gekoppeld aan een recordtype, wordt de optie voor de tijdlijnweergave grijs weergegeven.

  Bij het maken van een tijdlijnweergave kunt u uit de volgende datumvelden een keuze maken:

   * Recorddatums
   * Door het systeem gegenereerde velden opnemen: Aanmaakdatum, Datum van laatste wijziging
   * Datums opzoeken van verbonden record- of objecttypen (alleen wanneer u er een aggregator voor hebt toegevoegd wanneer u de record- of objecttypen hebt verbonden)
* Afhankelijk van de datums die aan de records zijn gekoppeld, worden sommige records mogelijk niet in de tijdlijnweergave weergegeven in de volgende scenario&#39;s:

   * Wanneer de begin- en einddatum geen waarden hebben
   * Wanneer de begin- of einddatum geen waarde hebben
   * Wanneer de begindatum na de einddatum ligt

Een tijdlijnweergave beheren:

1. Ga naar de pagina met recordtypen waarvoor u de tijdlijn wilt weergeven.
1. Creeer een chronologiemening, zoals die in artikel [&#x200B; wordt beschreven beheer verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md).

   ![&#x200B; de meningsvoorbeeld van de Chronologie &#x200B;](assets/timeline-view-example.png)

   De records die zijn gekoppeld aan het geselecteerde recordtype, worden standaard als balken in een tijdlijn weergegeven en gesorteerd in chronologische volgorde van hun begindatum.

   >[!TIP]
   >
   >    Het sorteren van de records in de tijdlijn is niet zichtbaar in de compacte weergave.

1. (Voorwaardelijk) Als uw beheerder aangepaste kwarten heeft toegelaten, en Workfront problemen met de manier ontdekt de douanekwarten worden gevormd, zou u een waarschuwing kunnen ontvangen wanneer het openen van de chronologiemening.

   De volgende scenario&#39;s bestaan:

   * Als er tussenruimten of overlappingen zijn gevonden tussen de datums van de kwartalen, ontvangt u mogelijk een melding dat aangepaste kwartalen nu kunnen worden ingesteld en wellicht moeten worden bewerkt.

     ![&#x200B; het bericht van het kwartier van de Douane mist of hiaten tussen kwartalen &#x200B;](assets/custom-quarter-notification-missing-or-gaps.png)

     >[!TIP]
     >
     >Dit bericht moet alleen direct worden weergegeven nadat uw organisatie Planningen en aangepaste kwartalen al waren ingeschakeld voor de aankoop. Overlappingen en tussenruimten zijn niet toegestaan nadat u Workfront Planning voor uw organisatie hebt ingeschakeld.

   * Als kwarten gedeeltelijk zijn opgezet, en sommige maanden binnen hetzelfde jaar missen, zou u een bericht kunnen ontvangen wanneer u scrolt om de ontbrekende kwarten te tonen dat de rest van het jaar met de ontbrekende kwarten moet worden opgesteld.

   ![&#x200B; Ontbrekend origineel bericht van douanekwartalen op chronologiemening &#x200B;](assets/missing-custom-quarters-original-message-on-timeline-view.png)

   De waarschuwingsberichten over de aangepaste kwartalen worden één keer per gebruiker weergegeven.

   >[!NOTE]
   >
   >Als het aangepaste kwart niet goed is opgeslagen, worden de klassieke kwartalen weergegeven in de tijdlijnweergave.
   >Nadat u aangepaste kwartalen hebt ingesteld in het gedeelte Instellen, worden in de tijdlijnweergave de aangepaste kwartalen weergegeven in plaats van de klassieke kwartalen.
   >Voor informatie, zie [&#x200B; douanekwarten &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md) toelaten.

1. (Voorwaardelijk) als u een beheerder van Workfront bent, klik **ga naar Opstelling** aan opstelling uw kwarten. Als niet, klik **O.K.** en vraag uw beheerder van Workfront aan opstelling de douanekwartalen.

   >[!TIP]
   >
   >De knop Ga naar setup wordt alleen weergegeven voor de Workfront-beheerder.

1. (Optioneel en voorwaardelijk) Wanneer de naam van de record wordt afgekapt, houdt u de muisaanwijzer boven een recordbalk om de volledige naam van de record en aanvullende informatie weer te geven. Voor informatie over vestiging bar truncation in de chronologie, zie de sectie [&#x200B; de montages van de chronologiemening &#x200B;](#edit-the-timeline-view-settings) in dit artikel uitgeven.

1. Voer een van de volgende handelingen uit om door de tijdlijn te navigeren:

   * Klik op de pictogrammen links en rechts in de linkerbovenhoek of gebruik de horizontale schuifbalk om naar voren en naar achteren in de tijdlijn te gaan. Als u de pagina vernieuwt, blijft het geselecteerde tijdkader behouden.
   * Klik **vandaag** in de hoger-juiste hoek om de chronologie aan de datum van vandaag te centreren.
   * Selecteer een van de volgende opties in het vervolgkeuzemenu voor het tijdframe om de tijdtoename bij te werken en de weergave bij te werken:

      * **Jaar**: De kwartalen en de maanden van vertoningen met jaaraanwijzing.
      * **Kwartaal**: De maanden en de weken van vertoningen met kwartaanwijzing.
      * **Maand**: De weken en dagen van vertoningen.
1. (Facultatief) klik **Schakelaar aan Compacte mening** om de verslagen te tonen waarvan data niet op de zelfde lijn snijden. <!--check to see if they updated the name of the setting here-->
1. (Voorwaardelijk) als u uw wijze in **Compact** veranderde, klik **Schakelaar aan Standaard** mening om verslagen in afzonderlijke lijnen te tonen. De **Standaard** optie is het gebrek.  <!--check to see if they updated the name of the setting here-->

1. Ga als volgt te werk om snel records te zoeken die overeenkomen met een trefwoord:

   1. Klik het **pictogram van het Onderzoek** pictogram van het 1&rbrace; Onderzoek ![&#x200B; en begin een sleutelwoord verbonden aan om het even welk gebied van een verslag te typen dat op het scherm toont. &#x200B;](assets/search-icon.png) Het aantal juiste overeenkomsten wordt weergegeven naast het zoekitem en de record met de juiste overeenkomst wordt gemarkeerd.

      ![&#x200B; vakje van het Onderzoek en de mening van de resultaatchronologie &#x200B;](assets/search-box-and-results-timeline-view.png)

      U kunt elk woord of speciaal teken gebruiken dat op het scherm zichtbaar is.

      U kunt geen trefwoorden gebruiken die zijn gekoppeld aan velden die niet worden weergegeven in de tijdlijnweergave.

   1. Druk op Enter op het toetsenbord om naar het volgende gevonden veld te gaan.
   1. (Optioneel) Als er meer dan één overeenkomst is, klikt u op de pijl-omhoog of -omlaag rechts van het trefwoord Zoeken om alle overeenkomende items in de tabel te zoeken.
   1. Klik het **x** pictogram in het onderzoeksvakje om het onderzoekssleutelwoord te ontruimen.

   1. (Facultatief) klik het **Volledige het schermpictogram** pictogram ![&#x200B; open volledig het schermpictogram &#x200B;](assets/open-full-screen-icon.png) om de mening in volledig scherm te openen, dan de **Uitgang volledig scherm** pictogram ![&#x200B; van de Uitgang het volledige het schermpictogram &#x200B;](assets/exit-full-screen-icon.png) of Escape op uw toetsenbord om het volledige scherm weg te gaan.

1. (Facultatief) klik **Uitsplitsing** om verbonden verslagen op de chronologie te tonen.

   Voor informatie, zie het sectie [&#x200B; Gebruik de eigenschap van de Onderverdeling aan vertoning verbonden verslagen in de chronologiemening &#x200B;](#break-down-connected-records-in-the-timeline-view) in dit artikel.
1. Voer een van de volgende handelingen uit om records te maken in de tijdlijnweergave of de datums ervan te bewerken:

   * Dubbelklik ergens op de tijdlijn om een record te maken.

     Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.

   >[!TIP]
   >
   >Dubbelklikken om records in de tijdlijn te maken is niet mogelijk binnen een groep.

   * Klik op de linker- of rechtermarge van een recordbalk en sleep deze naar een nieuwe positie. Als u de grootte van de balken van de records wijzigt, worden de begin- of einddatums onmiddellijk bijgewerkt.

   * Sleep records om de positie en datums in de tijdlijn bij te werken. Als u de balken van de records verplaatst, worden de begin- en einddatum onmiddellijk bijgewerkt.

     Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

   >[!TIP]
   >
   >Vergroten/verkleinen en slepen van records is niet mogelijk in de tijdlijn voor Workfront- en AEM Assets-objecttypen die in afsplitsingen worden weergegeven.

1. Werk de volgende weergave-elementen bij zoals in de onderstaande subsecties wordt beschreven:
   * [Filters](#add-filters)
   * [Groepering](#add-grouping)
   * [&#x200B; Montages &#x200B;](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

### Filters toevoegen

U kunt de hoeveelheid informatie die op het scherm wordt weergegeven verminderen door filters te gebruiken.

Houd rekening met het volgende wanneer u werkt met filters in de tijdlijnweergave:

<!-- this list is almost identical to the one for the table view - update both-->

* De filters die u voor een tijdlijnweergave maakt, werken onafhankelijk van de filters in een andere weergave die op hetzelfde recordtype is toegepast.

* De filters zijn uniek voor de weergave die u selecteert. Op twee tijdlijnweergaven van hetzelfde recordtype kunnen verschillende filters worden toegepast.

* Twee gebruikers die naar dezelfde tijdlijnweergave kijken, zien hetzelfde filter dat op dat moment wordt toegepast.

* U kunt de filters die u maakt voor een tijdlijnweergave niet een naam geven.

* Als u filters verwijdert, worden deze verwijderd van iedereen die hetzelfde recordtype als u benadert en die dezelfde weergave als u weergeeft.

* U kunt filteren op gekoppelde recordvelden of opzoekvelden.
* U kunt filteren door velden op te zoeken waarin meerdere waarden worden weergegeven.

Een filter toevoegen aan een tijdlijnweergave:

1. Creeer een chronologiemening voor een verslagtype pagina, zoals die in artikel [&#x200B; wordt beschreven beheer verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md).
1. Selecteer een chronologiemening, dan klik **Filters** in de hoger-juiste hoek van de lijst.
1. Klik **toevoegen voorwaarde** en voeg de volgende informatie toe:

   * **selecteer een gebied** aan Onderzoek naar een gebied of en selecteer het van de lijst.

   * **selecteer een optie** (of een filterbepaling) om te bepalen welk soort voorwaarde het gebied moet ontmoeten.

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

   ![&#x200B; de lijstmening van de Filter UI &#x200B;](assets/filter-ui-table-view.png)

   Er is geen limiet voor het aantal filtervoorwaarden dat u kunt toevoegen.

1. (Facultatief) klik **toevoegen voorwaarde** om een andere het filtreren optie toe te voegen en de bovengenoemde stappen te herhalen. Het aantal toegepaste filters toont links van het **pictogram van Filters**.
1. Klik op de volgende operatoren links om aan te geven hoe de filtervoorwaarden worden gekoppeld en moeten worden toegepast:

   * **EN**: Alle gespecificeerde voorwaarden moeten worden voldaan aan.
   * **OF**: Om het even welke gespecificeerde voorwaarden moeten worden voldaan aan.
Dit is de standaardoptie.

   1. (Facultatief) voeg extra filtergroeperingen toe en sluit zich bij hen aan door **EN** of **OF** exploitanten.

      ![&#x200B; Multi-tiered filters in meningen &#x200B;](assets/multi-tiered-filters-in-views.png)

   De lijst met records wordt automatisch gefilterd op basis van de filtercriteria.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Facultatief) klik het **x** pictogram om een filtervoorwaarde te verwijderen.
1. (Facultatief) klik **Filters** of overal anders op de pagina om de filtersdoos te sluiten. <!--right now you cannot "clear all" for filters, but this might come later-->


### Groepering toevoegen

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

U kunt records groeperen aan de hand van vergelijkbare informatie wanneer u een groepering toepast op een weergave.

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
* Groepen worden in alfabetische volgorde van hun waarden weergegeven.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Een groep toevoegen in de tijdlijnweergave:

1. Creeer een chronologiemening voor een verslagtype, zoals die in artikel [&#x200B; wordt beschreven beheer verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md).
1. Klik **Groepering** in de hoger-juiste hoek van de chronologiemening.

   ![&#x200B; het groeperen van UI chronologiemening met verbonden gebieden &#x200B;](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klik één van de voorgestelde gebieden, of klik **kies een verschillend gebied**, en onderzoek naar een verschillend gebied, dan klik het wanneer het in de lijst toont.

   De groepering wordt automatisch toegepast op de tijdlijn en records worden weergegeven in het groepsvak.

1. (Optioneel) Herhaal de bovenstaande stappen om maximaal drie groepen samen te voegen.

   Het aantal velden dat voor de groepering is geselecteerd, wordt weergegeven naast het pictogram Groeperen.

   ![&#x200B; groepering die in chronologiemening wordt toegepast &#x200B;](assets/grouping-applied-in-timeline-view.png)

1. In de **verslagen van de Groep door** doos, belemmering en laat vallen de groeperingen in de correcte orde.

1. (Facultatief) binnen de **verslagen van de Groep door** doos, klik het **x** pictogram aan het recht van een gebied dat voor de groepering wordt geselecteerd om de groepering te verwijderen

   of

   Klik **ontruimen allen** om alle gebieden te verwijderen.

1. Klik buiten de **verslagen van de Groep door** doos om het te sluiten.
1. (Facultatief) klik **Montages**, toen **Kleur** aan kleur-code groeperingen. Voor meer informatie, zie [&#x200B; uitgeven de sectie van de chronologiemening montages &#x200B;](#edit-the-timeline-view-settings) in dit artikel.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### De weergave-instellingen voor de tijdlijn bewerken {#edit-the-timeline-view-settings}

Werk de instellingen van de tijdlijnweergave bij om aan te geven wat en hoe informatie wordt weergegeven in het tijdlijngedeelte van de weergave.

1. Creeer een chronologiemening voor een verslagtype, zoals die in artikel [&#x200B; wordt beschreven beheer verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md).
1. Klik **Montages**.
1. Klik **Datum en tijd** in het linkerpaneel, dan de datum van het a **Begin** en een **einddatum** om op de chronologie te tonen. U kunt de standaardbegin- en einddatum kiezen of een datumveld kiezen dat beschikbaar is.

   De balken die de records weergeven, beginnen op de datum die u aangeeft voor de begindatum en eindigen op de datum die overeenkomt met de einddatum.

   >[!NOTE]
   >
   >* Records die geen waarden hebben voor de begin- of einddatum of die later een begindatum hebben dan de einddatum, worden niet weergegeven in de tijdlijnweergave.
   >
   >* Als u aanvullende records weergeeft met de optie Indeling, zijn de begin- en einddatums die van de hoofdrecord. U kunt geen begin- en einddatums kiezen voor de verbonden records in dit gebied.

1. (Voorwaardelijk en facultatief) als uw een beheerder van Workfront bent, klik **gaan naar Opstelling** in de **doos van de Douane van het Gebruik** om naar het gebied van de Opstelling en opstellings douanekwarten te gaan. Nadat u aangepaste kwarten hebt ingesteld, kunt u deze weergeven in de tijdlijnweergave in plaats van in de klassieke kwartalen. Als u geen beheerder van Workfront bent, kunt u verzoeken dat de douanekwarten voor uw organisatie van een beheerder worden toegelaten.

   Voor informatie, zie [&#x200B; douanekwarten &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md) toelaten.

   ![&#x200B; de douane van het kwartalen van het Gebruik waarschuwing binnen de montages van de chronologiemening &#x200B;](assets/use-custom-quarters-warning-inside-timelive-view-settings.png)

   >[!TIP]
   >
   >De knop Ga naar setup wordt alleen weergegeven voor de Workfront-beheerder.

1. Klik **stijl van de Bar** in het linkerpaneel, om te wijzen op welke informatie u op de verslagbars wilt tonen.

   U kunt de staafstijl van de hoofdrecord en van de verbonden records definiëren wanneer u de optie Onderverdeling in de standaardweergave gebruikt.

   Het primaire veld (of de titel) van de record, zoals gedefinieerd in de tabelweergave van de record, wordt standaard geselecteerd.
   <!--adjust this when the primary field is released??-->

1. (Facultatief en voorwaardelijk) als u duimnagels aan verslagen toevoegde, selecteer de **optie van de Duimnagel** om het beeld te tonen verbonden aan verslagen in hun verslagbar.

   >[!NOTE]
   >
   >    U moet eerst miniaturen toevoegen in de tabelweergave voordat u ze kunt weergeven in de tijdlijnweergave. Voor meer informatie, zie [&#x200B; een duimnagel aan een verslag &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) toevoegen.

1. Klik **toevoegen gebied**, dan klik binnen het **vakje van het Onderzoek gebieden**, en klik het gebied u wilt toevoegen.

   >[!TIP]
   >
   >   * U moet de velden maken voordat u deze aan de recordbalken kunt toevoegen.
   > 
   >   * Er moet ten minste één veld zijn geselecteerd. **Naam** wordt geselecteerd door gebrek.
   >
   >   * U kunt maximaal vijf velden toevoegen.

   Aan de rechterkant wordt een voorvertoning weergegeven van hoe de balken eruit zullen zien op de tijdlijn.

   ![&#x200B; de chronologiemontages van het paneel van de Details van het Verslag met voorproef &#x200B;](assets/record-details-panel-timeline-settings-with-preview.png)

1. (Facultatief en voorwaardelijk) als u de chronologie op de Standaardwijze toont, selecteer **de details van de bar van de Kortting** plaatsen. Als deze optie is geselecteerd, wordt de informatie op de recordbalken ingekort en wordt deze alleen volledig weergegeven wanneer u de muisaanwijzer op de balken plaatst. Deze instelling is standaard uitgeschakeld en de recordgegevens worden volledig op de balken weergegeven.

   ![&#x200B; Truncate die op benadrukte doos van chronologiemontages wordt toegelaten &#x200B;](assets/truncate-setting-enabled-on-timeline-settings-highlighted.png)

   >[!TIP]
   >
   >De instelling voor de details van de afloopbalk is niet beschikbaar bij het weergeven van de tijdlijnweergave in de compacte modus.
   >

1. Klik **Kleur** in het linkerpaneel, om de kleuren van de verslagen en de groeperingen in de chronologie aan te passen.

   ![&#x200B; het lusje van de Kleur chronologiemening &#x200B;](assets/color-tab-timeline-view.png)

   U kunt de kleur definiëren van de hoofdrecord en van de verbonden records wanneer u de optie Onderverdeling in de standaardweergave gebruikt.

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

   ![&#x200B; de selecteur van het Gebied drop-down menu in chronologiemening &#x200B;](assets/field-selector-drop-down-menu-timeline-view.png)

   Alleen velden met opties voor kleurcodes worden weergegeven in het keuzemenu.

   Multiselect- of single-select-velden kunnen bijvoorbeeld kleuropties hebben.

   Als u geen veld hebt met kleurgecodeerde opties voor het geselecteerde recordtype, wordt deze optie grijs weergegeven.

1. (Facultatief) als u de **Opsplitsing** optie gebruikt, herhaal de stappen die met stap 4 voor elk verbonden verslag beginnen in de chronologie wordt getoond.

1. Klik **sparen**.

   De records worden in de tijdlijnweergave weergegeven met de specificaties die u hebt geselecteerd.

### Verbonden records in de tijdlijnweergave opsplitsen

U kunt verbonden verslagen in de chronologiemening van een verslag tonen door de eigenschap van de Onderverdeling te gebruiken. Door records op te delen op basis van hun verbindingen kunt u de tijdlijnen van andere verbonden records weergeven en begrijpen hoe deze de prestaties en deadlines van uw records kunnen beïnvloeden.

#### Overwegingen bij het gebruik van de functie Onderverdeling

Houd rekening met het volgende wanneer u de tijdlijn van de records splitst op basis van de gekoppelde recordtypen:

* U kunt verbonden records of objecten weergeven onder de records van het geselecteerde recordtype in de tijdlijnweergave.
* U kunt verbonden verslagen in de chronologiemening slechts tonen wanneer het bekijken van de verslagen op Standaardwijze. U kunt de optie Onderverdeling niet gebruiken in de compacte modus van de tijdlijnweergave.
* U kunt het volgende weergeven in de tijdlijnweergave met de functie Onderverdeling:
   * Workfront Planning records die zijn verbonden met het geselecteerde recordtype.
   * Workfront-objecttypen of Experience Manager-elementen die zijn verbonden met het geselecteerde recordtype.
   * Workfront Planning-records of -objecten uit andere toepassingen die zijn verbonden met records die zijn verbonden met het geselecteerde recordtype.

     U kunt bijvoorbeeld campagnes verbinden met portfolio&#39;s. Bovendien zou u een ander verslagtype, producten, met projecten, evenals met campagnes kunnen verbinden. Wanneer u de tijdlijnweergave van de campagne maakt, kunt u de campagnes opsplitsen op portfolio&#39;s, producten en projecten.

* U kunt geen objecttypen weergeven die alleen zijn verbonden met Workfront-objecten in Workfront, maar die niet zijn verbonden met een recordtype voor Workfront Planning. U kunt alleen objecten of recordtypen weergeven die zijn verbonden in Workfront Planning.

  Taken zijn bijvoorbeeld verbonden met projecten in Workfront. Gebruikend de eigenschap van de Onderverdeling, kunt u projecten tonen die met campagnes in Planning, maar geen taken verbonden aan projecten in Workfront worden verbonden.

  Als u zowel portefeuilles als projecten in de chronologiemening van een het verslagtype van de Planning van Workfront wilt tonen, zowel moeten de portefeuilles als de projecten met het verslag van de Planning of met een verslag worden verbonden dat met het verslag van de Planning wordt verbonden waarvan chronologiemening u beheert.
* U kunt geen Adobe GenStudio-merken weergeven die zijn verbonden met planningsrecordtypen.
Voor informatie, zie [&#x200B; verbind verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
* U kunt alleen recordtypen weergeven die zijn gekoppeld aan ten minste twee datumvelden.
* De datumvelden voor de recordtypen die u in de tijdlijnweergave wilt weergeven, moeten zichtbaar zijn in de tabelweergave van het geselecteerde recordtype, als opzoekvelden.
* De begin- en einddatums van de recordtypen die u in de tijdlijnweergave wilt weergeven, moeten in chronologische volgorde worden weergegeven. Als een record bijvoorbeeld een startdatum van 31 januari en een einddatum van 1 januari heeft, wordt deze niet weergegeven in de tijdlijnweergave. Voor meer informatie, zie de sectie [&#x200B; een chronologiemening &#x200B;](#manage-a-timeline-view) in dit artikel beheren.
* Er geldt een limiet van 5 recordtypen die u kunt opnemen in de indeling van een record.

#### Verbonden records opsplitsen

1. Creeer een chronologiemening voor een verslagtype, zoals die in artikel [&#x200B; wordt beschreven beheer verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md).
1. Van de **Standaard** of **Compacte** wijzen, klik **Onderbreking** in de hoger-juiste hoek van de chronologiemening.
1. Vouw **Uitgezocht een verbonden verslagtype** doos uit en selecteer een verbonden verslagtype. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![&#x200B; de plukker en knoop van de Onderbreking op chronologiemening &#x200B;](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Als u geen verbonden verslagen hebt, of als de verbonden verslagen minstens twee datumgebieden hebben, **Uitgezocht een verbonden verslagtype** doos is niet beschikbaar.

1. Kies de datum van het a **Begin** en een **de datumgebied van het Eind**.

   >[!TIP]
   >
   >    De begin- en einddatum moeten opeenvolgend zijn. Als de einddatum valt vóór de begindatum, worden er geen records weergegeven in de tijdlijn.

   Er wordt een pijl naar rechts weergegeven op de geselecteerde balk van de record in de tijdlijn als deze zijn verbonden met andere records.
1. Klik op de pijl naar rechts om een recordtype uit te vouwen en de bijbehorende verbindingen weer te geven. <!--update screen shot at production-->

   ![&#x200B; Campagnes die door programma&#39;s in de chronologiemening worden verdeeld &#x200B;](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

   >[!IMPORTANT]
   >
   >    Wanneer u veelvoudige verbonden verslagen in de mislukking toont, zijn zij niet in hiërarchische orde.
   >
   >Bijvoorbeeld, als u de chronologie van de campagnes bekijkt en u Producten en toen Programma&#39;s aan de uitsplitsing toevoegt, worden de Programma&#39;s niet noodzakelijk verbonden met de Producten eerst.
   >
   >Zowel Producten als Programma&#39;s moeten met de campagnes worden verbonden om als keuzen voor de verdelingsoptie te tonen, en u kunt hen aan de onderbreking in om het even welke orde toevoegen.

1. (Voorwaardelijk) als u de chronologie op de Compacte wijze bekijkt, klik **mening van de Schakelaar**. De uitsplitsing is niet zichtbaar op **Compacte** wijze.

   >[!TIP]
   >
   >Selecteer **tonen dit niet opnieuw** in de **Schakelaar aan de Standaardmening?** gebruiken voordat u van weergave verandert.
   >
   >Deze voorkeur wordt slechts herinnerd voor huidige browser. Als u browsers of computers wijzigt, moet u deze voorkeur opnieuw selecteren.
   >
   >U kunt niet terugkeren naar de compacte modus nadat u de weergave hebt ingesteld op Standaard en verbonden records hebt weergegeven in de weergave.
1. (Optioneel) Herhaal bovenstaande stappen om meer verbonden records toe te voegen.



