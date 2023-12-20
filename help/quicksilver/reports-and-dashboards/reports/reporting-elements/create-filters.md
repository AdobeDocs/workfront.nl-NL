---
product-area: reporting
navigation-topic: reporting-elements
title: Filters maken of bewerken in Adobe Workfront
description: U kunt de hoeveelheid informatie beperken die u op het scherm weergeeft in een lijst met items met een filter. U kunt bepaalde criteria definiëren op basis van bepaalde gegevens over een object en alleen de objecten weergeven die aan deze criteria voldoen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '2462'
ht-degree: 0%

---

# Filters maken of bewerken in Adobe Workfront

U kunt de hoeveelheid informatie beperken die u op het scherm weergeeft in een lijst met items met een filter. U kunt bepaalde criteria definiëren op basis van bepaalde gegevens over een object en alleen de objecten weergeven die aan deze criteria voldoen.

U kunt de volgende typen filters toepassen in Adobe Workfront:

* Snelle filters in een lijst met objecten om een item te zoeken met een trefwoord. Dit zijn tijdelijke filters die u niet kunt opslaan voor toekomstig gebruik.

  Zie voor informatie over snelle filters [Het snelle filter toepassen op een lijst](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

* Permanente filters die u kunt opslaan en gebruiken in meerdere lijsten en rapporten. In dit artikel wordt beschreven hoe u een permanent filter kunt maken of een bestaand filter in een lijst of rapport kunt bewerken.

* Filters in andere gebieden van Workfront, buiten lijsten en rapporten.

  Voor een lijst met alle filters in Workfront en de gebieden waarop u deze kunt toepassen, raadpleegt u [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Nieuw: Medewerker of hoger</p>

of

<p>Huidig: Verzoek of hoger</p>

<p><b>OPMERKING:</b></p>

Als u een filter in een rapport wilt bewerken, hebt u de volgende licentie nodig:

<p>Nieuw: Plan</p>

of

<p>Huidig: Standaard</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <ul><li><p>Toegang tot filters, weergaven en groepen bewerken</p></li></ul>
    <p><b>OPMERKING:</b></p>
   Om een filter in een rapport uit te geven, moet u de volgende configuratie van het toegangsniveau hebben, naast Edit toegang tot Filters, Weergaven, en Groepen:

<ul><li><p>Toegang tot rapporten, dashboards en kalenders bewerken</p></li></ul>

<p><b>OPMERKING:</b></p> <p> Als u geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten voor een filter beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Typen filteropbouwinterfaces

U kunt filters tot stand brengen gebruikend de types van filterbouwers die in de hieronder lijst worden beschreven:

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Het type Builder</strong></td>
<td><strong>Object Filter</strong></td>
<td><strong>Indien beschikbaar</strong></td>
</tr>
<tr>
<td>Standard builder</td>
<td>
<ul>
<li> <p>Projecten</p> </li>
<li> <p>Taken </p> </li>
<li> <p>Problemen</p> </li>
<li> <p>Portfolio's</p> </li>
<li> <p>Programma's</p> </li>
<li> <p>Gebruikers</p> </li>
<li> <p>Sjablonen</p> </li>
<li> <p>Groepen</p> </li>
</ul>
</td>
<td>
<ul>
<li> <p>Lijsten </p> </li>
</ul>
<ul>
<li> <p>De lijst van Projecten in de Planner van het Scenario</p> <p>Voor de Scenario Planner is een aanvullende licentie vereist. Voor informatie over de Workfront Scenario Planner raadpleegt u <a href="../../../scenario-planner/scenario-planner-overview.md">Overzicht van de functie Scenario Planner</a>. </p> </li>
</ul>
<p><b>OPMERKING:</b></p> <p>Standaardbuilders voor filters zijn niet beschikbaar in rapporten.
</td>
</tr>
<tr>
<td>Verouderde bouwer</td>
<td>Alle objecten </td>
<td>Lijsten en rapporten</td>
</tr>
</tbody>
</table>

Zie voor informatie over Workfront-objecten [Objecten in Adobe Workfront begrijpen](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Houd rekening met het volgende wanneer u filters maakt met behulp van de verschillende interfaces:

* U kunt de standaardbuilder vinden op dezelfde plaatsen als waar u de oudere filterinterface vindt voor de gebieden die in de bovenstaande tabel worden vermeld.
* De standaard builder is de standaardeigenschap voor alle gebieden waar het beschikbaar is. Als u wilt overschakelen naar de verouderde filterontwikkelaar, klikt u op de knop **Meer** menu naast [!UICONTROL **Filters**] en selecteert u [!UICONTROL **Terug naar Oudere filters**].

  ![Terug naar Oudere filters](assets/use-legacy-filters.png)

* Opgeslagen filters zijn beschikbaar in beide builders, ongeacht welke ervaring u gebruikte om ze oorspronkelijk te bouwen. Als u bijvoorbeeld een filter hebt gemaakt met de verouderde builder, kunt u dit ook vinden en wijzigen in de standaardbuilderinterface.

  >[!TIP]
  >
  >Een filter &quot;Alle&quot; wordt niet opgenomen in de standaardbuilder, omdat alle lijstitems worden weergegeven wanneer er geen filters worden toegepast. Klikken [!UICONTROL **Alles wissen**] rechtsboven in de builder actieve filters verwijderen en alle items weergeven. Indien [!UICONTROL **Alles wissen**] worden grijs weergegeven, worden er geen filters toegepast.

* De standaard en erfenisbouwers hebben een lichtjes verschillende syntaxis wanneer het bouwen van veelvoudige-instructiefilters die EN en OF exploitanten combineren. Hierdoor kunnen deze filters anders worden weergegeven wanneer u overschakelt van de ene naar de andere builder.

  >[!INFO]
  >
  >Het volgende scenario bestaat:
  >
  >1. Met de standaardbuilder kunt u een filter maken met de volgende syntaxis:
  >
  >   `(A OR B) AND C`
  >
  >1. Ga naar de verouderde builder en bewerk het filter met de syntaxis van de verouderde builder, zoals beschreven in de [Een filter maken of bewerken in de verouderde builder](#create-filter-in-legacy-builder) in dit artikel. In de syntaxis voor de verouderde builder worden de filterinstructies als volgt weergegeven:
  >
  >   `A AND C`
  >   `OR`
  >   `B AND C`
  >
  >1. Wijzig het filter in de oudere interface.
  >1. Ga terug naar de standaardbuilder. De filterinstructie wordt weergegeven volgens de logica die wordt ondersteund in de verouderde builder, zoals hierboven beschreven.
  >
  >   Het filter wordt als volgt weergegeven in de standaardbuilderinterface:
  >  
  >   `A AND C`
  >   `OR`
  >   `B AND C`
  > 
  >   Dit gebeurt omdat het filter is gewijzigd in de oudere interface.

## Een filter maken of bewerken in de standaardbuilder

U kunt op de volgende manieren filters maken met de standaardbuilderinterface:

* Van kras
* Een bestaand filter bewerken
* Een bestaand filter dupliceren
* Een bestaand filter dupliceren, bewerken en opslaan als een nieuw filter

Maak een filter met de standaardbuilderinterface:

1. Ga naar een lijst waar u een filter wilt tot stand brengen of die het filter bevat u wilt aanpassen.
1. Klik op de knop **Filter** pictogram ![Filterpictogram](assets/filter-nwepng.png) om de builderinterface te openen.

   ![Standaardfilterconstructor](assets/new-filters-all-filter-types.png)

1. Bekijk de volgende lijsten met filters:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favoriet</strong></td>
   <td>Filters die u als favorieten hebt gemarkeerd. Wanneer u een filter favoriete, wordt de originele plaats getoond onder de filternaam, en het wordt verborgen van de originele lijst tenzij u het als favoriet verwijdert.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Opgeslagen</strong></td>
   <td>Filters die u zelf hebt gemaakt en opgeslagen. In deze lijst worden standaard opgeslagen filters weergegeven in de volgorde van de laatst opgeslagen filters, maar u kunt de filternamen slepen om de lijst handmatig opnieuw te rangschikken.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Standaardwaarden systeem</strong></td>
   <td>De standaardfilters van het systeem van Workfront, evenals filters die de beheerder van Workfront aan uw lijst van filters, of op het systeemniveau of in uw lay-outmalplaatje toevoegde.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Gedeeld met mij</strong></td>
   <td>Filters die anderen met u hebben gemaakt en gedeeld of die op het hele systeem worden gedeeld.</td>
   </tr>
   </tbody>
   </table>

1. Voer een van de volgende handelingen uit:

   * Klikken **Nieuw filter** een geheel nieuw filter maken.
   * Houd de muis boven een bestaand filter dat u kunt beheren en klik op de knop **Bewerken** pictogram ![Pictogram Bewerken](assets/edit-icon.png) om het te bewerken.

     of

     Houd de muisaanwijzer boven een bestaand filter dat u kunt weergeven, en klik op de knop **Meer** menu ![Het menu Meer](assets/more-icon-spectrum.png)en klik op **Dupliceren** om het bestaande filter te kopiëren en een kopie te bewerken.

   ![Meer menuopties](assets/new-filters-more-menu-options-with-delete.png)

1. (Voorwaardelijk) Afhankelijk van het feit of u objecten wilt zoeken die overeenkomen met alle instructies in een filtergroep of een van de instructies in een filtergroep, kunt u een van de volgende opties selecteren:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Opnemen als alles waar is</strong></td>
   <td>De objecten die door het filter worden gevonden, moeten overeenkomen met alle filtercriteria in een filtergroep. In dit geval, worden de filterverklaringen verbonden door de exploitant AND. Dit is de standaardselectie.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Opnemen indien van toepassing</strong></td>
   <td>De objecten die door het filter worden gevonden, moeten overeenkomen met alle filtercriteria in een filtergroep. In dit geval worden de filterinstructies verbonden door de operator OR.</td>
   </tr>
   </tbody>
   </table>

   ![Opnemen als alle of een echt vervolgkeuzemenu](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   Zie voor meer informatie over filteroperatoren [Overzicht van filters in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klik op het vervolgkeuzemenu met velden om een lijst weer te geven met onlangs gebruikte velden en stel velden voor waarop u wilt filteren. De voorgestelde velden worden momenteel weergegeven in de lijst waarop u filtert.

   U kunt ook **Bladeren door velden** om een lijst weer te geven van alle velden waarop u kunt filteren. De velden in de geavanceerde zoekopdracht worden gegroepeerd op objectcategorie.

   ![Een veld zoeken waarop u wilt filteren](assets/new-filter-search-for-field.png)

1. Klik op de vervolgkeuzelijst met opties om een optie te selecteren. De standaardbepaling is &quot;evenaart.&quot;

   Zie voor meer informatie [Filter- en voorwaardenmodificatoren](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!TIP]
   >
   >Terwijl u het filter maakt, worden de resultaten direct in de lijst weergegeven. Als het filterdeelvenster de lijst bedekt, kunt u deze sluiten om de weergave te zien. De informatie die u hebt ingevoerd, blijft in de builder staan wanneer u het deelvenster opnieuw opent.

1. Typ de waarde van een veld waarop u wilt filteren. Typ bijvoorbeeld de naam van een uitgave als u wilt filteren op `Issue:Name`. Selecteer de waarde wanneer deze in de lijst wordt weergegeven.

   >[!TIP]
   >
   >Afhankelijk van de optie die u hebt geselecteerd, kunt u meerdere waarden selecteren.

1. Klikken **Filter toevoegen** om een ander veld te selecteren en nieuwe filtercriteria toe te voegen aan de filterinstructie.
1. (Optioneel) Klik op de knop **Verwijderen** pictogram ![Pictogram Verwijderen](assets/delete.png) om bestaande filterinstructies te verwijderen.

   of

   Klikken **Alles wissen** alle filtercriteria te wissen.

1. (Optioneel) Klik op **Filtergroep toevoegen** om een andere reeks filtercriteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

   >[!TIP]
   >
   >Wellicht wilt u een andere filtergroep gebruiken wanneer u de groepen via een andere operator wilt laten verbinden dan de operator in een filterinstructie.

   >[!INFO]
   >
   >Wanneer u filtert voor projecten die &quot;marketing&quot;in de naam bevatten die of niet volledig zijn en niet op Greep zijn, kunt u de volgende veelvoudige filtergroepen gebruiken:
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >In dit geval, wordt elke filterverklaring verbonden door EN, en de filtergroepen worden verbonden door OF.

1. (Optioneel) Klik op **Tekstmodus** om het filter verder te bouwen gebruikend tekstwijze.

   ![Tekstmodus selecteren](assets/new-filter-select-text-mode.png)

   De interface van de tekstmodus wordt geopend.

   ![Interface van de tekstmodus](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >We raden u aan zoveel mogelijk van het filter te maken met de standaardbuilderinterface en alleen tekstmodus te gebruiken wanneer u wijzigingen moet aanbrengen in het filter die alleen worden ondersteund in de tekstmodus.

   Zie voor meer informatie over het maken van een filter met de interface van de tekstmodus [Een filter bewerken in de tekstmodus](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Klikken **Tekstmodus afsluiten** om aan de standaardbouwerinterface terug te keren.

   >[!WARNING]
   >
   >Sommige instructies in de tekstmodus worden niet ondersteund in de standaardbuilder of de oudere interface. Als u de tekstmodus afsluit wanneer u deze typen instructies hebt gemaakt, wordt mogelijk een waarschuwingsbericht gegenereerd.

1. (Optioneel) Klik op **Toepassen** om het filter op de lijst toe te passen en de resultaten te zien.

   Als het filter geen resultaten oplevert, is de lijst leeg.

1. Klikken **Opslaan als nieuw** om het filter op te slaan voor toekomstig gebruik.

   ![Geef het filter een naam en sla het op](assets/save-as-untitled-filter-ui-nwe.png)

1. Selecteren **Naamloos filter** en typ in plaats daarvan de naam van het nieuwe filter.

   >[!TIP]
   >
   >Geef het filter een naam, zodat u het later kunt vinden. Als u het filter geen naam geeft, wordt het filter Naamloos filter in het systeem genoemd.

1. Selecteer een pictogram voor het nieuwe filter in het menu **Pictogram** vervolgkeuzelijst.

   ![Een pictogram voor het filter selecteren](assets/new-filter-select-icon.png)

1. (Optioneel) Voeg een beschrijving van het filter toe om aan te geven wat er uniek aan is. De beschrijving wordt onder de filternaam in de lijst met filters weergegeven.

   >[!TIP]
   >
   >Klikken **Annuleren** neemt u altijd terug naar het filtergebied.

1. Klikken **Opslaan**. Het filter wordt opgeslagen in de lijst Opgeslagen en wordt toegepast op de lijst met items.
1. (Optioneel) Als u een filter naar de lijst Favorieten wilt verplaatsen, beweegt u de muisaanwijzer over een willekeurig filter in de filterlade en klikt u op het pictogram Favoriet ![Pictogram Favoriet](assets/favorites-icon-small.png).

   of

   Houd de muisaanwijzer boven een filter in de filterlade en klik op het menu Meer ![Het menu Meer](assets/more-icon-spectrum.png)en klik op **Favoriet**.

1. (Optioneel) Klik op de knop **Stapelfilters** om gestapelde filters te activeren. Met deze optie kunt u meerdere opgeslagen filters toepassen. De filterregels worden toegepast in de volgorde waarin u ze selecteert.

   >[!TIP]
   >
   >Er is geen limiet voor het aantal filters dat u kunt selecteren.
   >
   >Wanneer u meerdere filters selecteert, moet tegelijkertijd aan alle bijbehorende voorwaarden worden voldaan om overeenkomende resultaten weer te geven.

   ![Stapelfilters](assets/new-filter-stack-filters.png)

   Het aantal filters dat u hebt geselecteerd, wordt weergegeven naast het filterpictogram boven aan de lijst met items.

   ![Aantal geselecteerde filters](assets/number-of-filters-selected.png)

1. (Optioneel) Voer een van de volgende handelingen uit:

   * Deel het filter met anderen of maak het systeembreed beschikbaar. Zie voor meer informatie [Een filter, weergave of groep delen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

   * Verwijder het filter als het niet meer geldig is of als het niet meer gedupliceerd is. U kunt alleen filters verwijderen die u bezit. U kunt filters verwijderen die met u zijn gedeeld. Zie voor meer informatie [Filters, weergaven en groepen verwijderen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

## Een filter maken of bewerken in de verouderde builder {#create-filter-in-legacy-builder}

U kunt oudere filters op de volgende manieren maken in lijsten en rapporten:

* Van kras
* Een bestaand filter bewerken en opslaan als een nieuw filter

Ongeacht de methode die u gebruikt om filters te maken, lijkt het alsof u een geheel nieuw filter maakt of een bestaand filter gebruikt.

1. Ga naar een lijst of een rapport die het filter bevat dat u wilt aanpassen.
1. Klik op de knop **Filter** pictogram ![Filterpictogram](assets/filter-nwepng.png).

   >[!TIP]
   >
   >De rapportmaker moet ervoor zorgen dat filters worden bewerkt om de vervolgkeuzelijst Filter in een rapport te kunnen bekijken. Het filter Standaard rapporteren wordt standaard toegepast op een rapport. Het filter Standaard rapporteren kan alleen worden aangepast wanneer u het rapport bewerkt.

   ![Vervolgkeuzelijst Filter](assets/filter-drop-down-expanded-nwe.png)

1. Klikken **Nieuw filter** boven aan de lijst met filters.

   of

   Houd de muisaanwijzer boven het filter dat u wilt wijzigen en klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png).

   De builder voor het aanpassen van de filterlanceringen.

1. Voer een van de volgende handelingen uit:

   * Wijzig bestaande filterregels door op de bestaande regel te klikken en een nieuwe optie te selecteren.
   * Filterregel toevoegen door te klikken **Een andere filterregel toevoegen** typt u eerst de naam van de optie waaraan u een regel wilt toevoegen in het dialoogvenster **Typ de veldnaam** en klikt u erop wanneer het wordt weergegeven in de vervolgkeuzelijst.

     Velden die zijn gekoppeld aan het object van het filter worden weergegeven in het dialoogvenster **Typ de veldnaam** doos.

   * Klikken **EN** of **OF** wanneer u een nieuwe filterregel toevoegt.\
     Wanneer het toevoegen van filterregels, gebruik de filterbepalingen om de voorwaarde van uw filter te vestigen. Zie voor meer informatie over filtermodifiers [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

     >[!NOTE]
     >
     >Wanneer u een groep EN verklaringen door veelvoudige OF verklaringen verbindt, moet u de gebieden herhalen die niet tussen OF verklaringen voor elke groep verklaringen veranderen.
     >
     >![Aangesloten filterinstructies](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-2022.png)
     >
     >Wanneer u een filter voor taken bouwt die het woord &quot;marketing&quot;bevatten en in projecten met een status van Huidige of Planning zijn, moet u de volgende filterregels hebben:
     >
     >`Task: Name Contains Marketing`
     >`AND`
     >`Project: Status Equals Current`
     >`OR`
     >`Task: Name Contains Marketing`
     >`AND`
     >`Project: Status Equals Planning`
     >
     >Hoewel de Taak: Naam bevat &quot;marketing&quot;verandert niet tussen de twee EN filtergroepen, moet het in de tweede groep worden herhaald.

   * Verwijder een bestaande filterregel door op het pictogram X te klikken.

1. (Optioneel) Klik op **Overschakelen naar tekstmodus** om een filter toe te voegen met de interface Tekstmodus.

   Zie voor meer informatie over het maken van een filter met de interface van de tekstmodus [Een filter bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Klikken **Filter opslaan** om een nieuw filter te maken of het geselecteerde filter te vervangen door uw wijzigingen.

   of

   Klikken **Opslaan als nieuw filter** om een nieuw filter te maken van het geselecteerde filter.

   Het nieuwe filter wordt weergegeven in de lijst met filters en wordt automatisch toegepast op de lijst of het rapport dat u hebt geselecteerd.

1. (Optioneel) Voer een van de volgende handelingen uit:

   * U kunt filters delen die u met andere gebruikers maakt, of deze in het hele systeem beschikbaar maken. Zie voor meer informatie [Een filter, weergave of groep delen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
   * Verwijder de filters die u niet meer in de lijst wilt weergeven. Zie voor meer informatie [Filters, weergaven en groepen verwijderen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).


