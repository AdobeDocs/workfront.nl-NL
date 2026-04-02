---
title: De lijstweergave beheren in de Adobe Workfront-planning
description: U kunt objecten en hun velden in een lijstweergave weergeven, wanneer u ze opent in de Verbonden recordpagina van een record, in Adobe Workfront Planning. In dit artikel wordt beschreven hoe u een lijstweergave kunt maken of bewerken op de pagina Verbonden records van een record.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '1857'
ht-degree: 0%

---


# De lijstweergave beheren in Adobe Workfront Planning

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt objecten in de lijstweergave bekijken in de volgende gebieden van Workfront Planning:

* Een verbonden registratiepagina voor projecten in het detailsgebied van een verslag

  ![ Projecten op verbonden verslagenpagina in lijstmening ](assets/projects-on-connected-records-page-list-view.png)

* Een lijst met aanvraagformulieren op recordtypeniveau

  ![ de vormen van het verzoek in lijstmening ](assets/request-forms-in-list-view.png)

In dit artikel wordt beschreven hoe u in Workfront Planning door een lijstweergave kunt navigeren, deze kunt maken of deze kunt bewerken.

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

## Overwegingen over lijstweergaven

* Neem het volgende in overweging voor de weergave van de lijst met verbonden records:

   * U kunt projecten in de lijstmening in de verbonden verslagenpagina van een verslag slechts bekijken. De lijstweergave is niet beschikbaar voor andere objecten of recordtypen in een verbonden recordpagina.

  Voor informatie over het creëren van een verbonden verslagenpagina, zie [ een Verbonden verslagenpagina aan een verslag ](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) toevoegen.
   * Voordat u een lijstweergave kunt weergeven in een verbonden recordpagina van een record, moet u Workfront-projecten verbinden met de recordtypen Planning. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
   * U kunt veelvoudige lijstmeningen voor projecten in de verbonden verslagenpagina van een verslag tot stand brengen.

* Bekijk het volgende voor de lijstweergave voor aanvraagformulieren:

   * U kunt geen extra lijstweergaven maken of bewerken voor het plannen van aanvraagformulieren. Workfront maakt één lijstweergave voor aanvraagformulieren. <!--this will change-->

     Voor informatie over verzoekvormen, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
* Afhankelijk van waar deze wordt weergegeven, bevat niet elke lijstweergave alle elementen die in dit artikel worden beschreven.

## Een lijstweergave beheren {#manage-a-list-view}

De de lijstmeningen van de Planning van Workfront zijn gelijkaardig aan Workfront verbeterde lijsten. De meeste elementen van verbeterde weergaven bestaan ook in lijstweergaven in Workfront Planning.

Voor meer informatie, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Ga naar een lijstweergave in een van de volgende gebieden:

   * Een verbonden registratiepagina voor projecten in het detailsgebied van een verslag
   * De pagina met aanvraagformulieren van een recordtype

1. (Voorwaardelijk) Voer, indien beschikbaar, een van de volgende handelingen uit om de lijstweergave te wijzigen:

   1. Vouw het menu van dropdown meningen in de upper-left hoek van de lijst uit om een andere mening te selecteren, of klik **Nieuwe mening** en creeer een andere.

      >[!TIP]
      >
      >Weergaven worden door het hele systeem gedeeld. Als u een mening van Projecten voor één verslagtype creeert, kunt u het op andere verslagtypes bekijken die verbonden projecten tonen.

   1. Beweeg over de naam van een bestaande mening en klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik één van het volgende:
      * **noem** anders, om de mening een nieuwe naam te geven
      * **Aandeel**, om de mening met anderen te delen
      * **Schrapping**, om de mening te schrappen.

      >[!NOTE]
      >
      >* U moet over beheerdersmachtigingen voor een weergave beschikken om de weergave te kunnen bewerken, delen of verwijderen.
      >
      >* U kunt de systeemweergaven niet wijzigen.
      >
      >* <span class="preview"> u kunt een mening terugstellen die met u werd gedeeld waaraan u slechts toestemmingen aan Mening hebt, nadat u het wijzigde om zijn originele voorkeur te herstellen, of u kunt het met uw veranderingen kopiëren en het exemplaar delen. Voor meer informatie, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

   1. Klik het **pictogram van de Filter** pictogram ![ van de Filter ](assets/filter-icon.png) om een filter aan de mening toe te voegen. De resultaten worden direct in de lijst gefilterd. U kunt filters niet opslaan en een naam geven. Filters worden onthouden wanneer u de pagina in de toekomst opent en maken deel uit van gedeelde weergaven.

      >[!TIP]
      >
      ><span class="preview"> om een gepersonaliseerd filter toe te passen, selecteer één van de volgende opties voor een gebiedswaarde:
      >
      ><div class="preview">
      >
      >* **me (het programma geopende gebruiker)** om naar het programma geopende gebruiker op gebieden te verwijzen die naar gebruikers verwijzen.
      >
      >* **Mijn teams** of **Mijn huisteam** om naar uw teams op gebieden te verwijzen die naar teams verwijzen.
      >
      >* **Mijn groepen** of **Mijn huisgroep** om naar uw groepen in gebieden te verwijzen die naar groepen verwijzen.
      >
      >* **Mijn bedrijf** om naar uw bedrijf op gebieden te verwijzen die naar bedrijven verwijzen.
      > 
      >* **Mijn rollen** of **Mijn primaire rol** om naar uw baanrollen op gebieden te verwijzen die naar rollen verwijzen.
      >
      ></div>

   1. Klik het **pictogram van Kolommen** pictogram van Kolommen ![ ](assets/columns-icon.png) om te selecteren welke kolommen aan vertoning of in de mening te verbergen.
   1. Houd de cursor boven de naam van een kolom en klik op de pijl omlaag links van de kolomnaam en klik op een van de volgende opties:
      * **noem** anders, om a **Eigen etiket** voor de kolom toe te voegen. De naam van het oorspronkelijke veld in Workfront verandert niet.
      * **Soort**, om de lijst door het geselecteerde gebied te sorteren. Aan de kolomkop wordt een sorteerpictogram toegevoegd dat de richting van het sorteren aangeeft.
   1. Klik het **+** pictogram in de hoger-juiste hoek van de lijst om kolommen aan de lijst toe te voegen of te verwijderen, dan klik **sparen**.

      De **manager van de Kolom** opent.

      U kunt alleen bestaande velden toevoegen aan de lijstweergave.
U kunt het primaire veld niet verwijderen in de lijstweergave die in de eerste kolom wordt weergegeven.

   1. <span class="preview"> klik het **pictogram van de cellen van het Formaat** pictogram ![ de celpictogram van het Formaat ](assets/format-cells-icon.png). Het **vakje van het Formaat** opent.</span> <!--change the name of the box when they update it-->
      <span class="preview"> doe het volgende: </span>

      1. <span class="preview"> klik **toevoegen voorwaarde**.</span>
      1. <span class="preview"> op **als** lijn, selecteer een gebied en kies een gebiedswaarde en voeg een bepaling toe. De opties veranderen, afhankelijk van het gebiedstype u kiest. </span>

         >[!TIP]
         >
         ><span class="preview"> slechts zijn de gebieden zichtbaar in de lijstmening beschikbaar voor voorwaardelijk formatteren.</span>

      1. <span class="preview"> (Facultatief) in plaats van het toevoegen van een gebiedswaarde, klik **vergelijken met een ander gebied** pictogram ![ vergelijk met een ander gebied ](assets/compare-to-another-field-icon.png) en kies een gebied waarvan waarde u met de waarde van uw geselecteerd gebied wilt vergelijken. U kunt bijvoorbeeld de velden Projecteigenaar en Projectsponsor vergelijken. </span>

         >[!TIP]
         >
         ><span class="preview"> slechts zijn de gebieden zichtbaar in de lijstmening beschikbaar voor voorwaardelijke het formatteren. De velden die u vergelijkt, moeten van hetzelfde type zijn. </span>

      1. <span class="preview"> (Facultatief) klik **toevoegt voorwaarde** in **als** lijn om meer voorwaarden aan de zelfde regel toe te voegen.</span>

         >[!TIP]
         >
         ><span class="preview"> u kunt tot 10 voorwaarden in een conditioneringsregel toevoegen en u kunt tot 20 regels voor een gebied hebben.</span>

      1. <span class="preview"> klik de **of** schakelaar tussen voorwaarden om in **te veranderen en** en erop te wijzen dat de veelvoudige voorwaarden tezelfdertijd moeten worden vervuld. **Of** is de standaardschakelaar.</span>
      1. <span class="preview"> in de **2} lijn van het Formaat {, selecteer een gebied om erop te wijzen welke kolom zal worden geformatteerd.**</span> <!--edit this area, if it changes names??-->
      1. <span class="preview"> (Facultatief) klik het **pictogram van de kleurencirkel** pictogram ![ Kleurcirkel ](assets/color-circle.png) naast het gebied selecteerde, om het uit te breiden en een andere kleur in het **vult van de Cel** gebied te kiezen om de kleur van de achtergrond in een cel te veranderen of een kleur van het **de kleur van de Tekst** gebied te kiezen om de kleur van tekst in een cel te veranderen.</span>
      1. <span class="preview"> klik het **formaat van de Tekst** pictogram ![ het formaatpictogram van de Tekst ](assets/text-format-icon.png) en selecteer van de volgende opties om de tekst in een cel te formatteren:</span>
         * <span class="preview"> Vet </span>
         * <span class="preview"> Cursief </span>

      1. <span class="preview"> zet **toe is op rij** het plaatsen om het formatteren op de volledige rij van het gebied toe te passen dat aan de voorwaarden voldoet.</span>
      1. <span class="preview"> (Facultatief) klik **toevoegen voorwaarde** in het **vakje van het Formaat** om een andere regel voor een ander gebied toe te voegen en de herhaling hierboven de stappen.</span>
      1. <span class="preview"> (Facultatief) klik **Duidelijk alles** om al het formatteren te verwijderen.</span>
      1. <span class="preview"> klik buiten het **Formaat** vakje om het te sluiten.</span>

         <span class="preview"> dit keert u aan de lijstmening terug.</span>
         <span class="preview"> het formatteren wordt onmiddellijk toegepast op de lijstmening.</span>
         <span class="preview"> er is een blauw punt naast het **pictogram van de Cellen van het Formaat** om erop te wijzen dat de mening het speciale toegepaste formatteren heeft.</span>

   1. <span class="preview"> (Facultatief) klik het **Groeperen** pictogram ![ Groeperend pictogram ](assets/grouping-icon.png) &lt;!-Hebben ze dit bijgewerkt naar &quot;Groeperen&quot;?-> om items in de lijst te groeperen op basis van een gemeenschappelijk veld. Selecteer één van de opties, of gebruik de onderzoeksbar om een gebied te vinden.</span>

      <span class="preview"> het gebied moet een kolom in de lijst zijn alvorens u door het kunt groeperen. Niet kunnen alle gebiedstypes voor groeperingen worden gebruikt.</span>

   1. <span class="preview"> klik het **pictogram van de de hoogte van de Rij** ![ het hoogtepunt van de Rij ](assets/row-height-icon.png) om de verticale lengte van een rij bij te werken. Kies een van de volgende opties: </span>

      <div class="preview">

      * Kort
      * Standaard. Dit is de standaardoptie.
      * Medium
      * Lang

      </div>

   <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. (Optioneel) Voeg een trefwoord toe in het zoekvak rechtsboven in de lijst om naar een item te zoeken.

   Objecten die overeenkomen met de zoekterm worden gemarkeerd in de lijst.

1. (Optioneel en voorwaardelijk) Voer een van de volgende handelingen uit op de pagina met projectverbindingen van <!--change projects to items here when more items will display in the Glist--> om meer items aan de lijst toe te voegen en deze automatisch te verbinden met de geselecteerde record:

   * Klik **verbinden verslagen** in de hoger-juiste hoek van de lijst om bestaande punten toe te voegen.
   * Klik **Nieuwe rij** bij de bodem van de lijst om nieuwe punten toe te voegen.
1. Klik op de naam van een verbonden item in de lijst om het te openen op een ander browsertabblad.
1. Dubbelklik in een cel in de lijst om de gegevens van een veld te bewerken en druk vervolgens op Enter om de wijzigingen op te slaan.

   Sommige velden zijn alleen-lezen. Het percentage voltooide van een project is bijvoorbeeld een veld dat door het systeem wordt berekend en u kunt het niet handmatig bewerken.

1. Beweeg over de naam van een punt in de lijst en klik **Meer** menu [ Meer menu ](assets/more-menu.png) en klik **Mening** om het project in een ander lusje te openen

   of

   Selecteer een of meer items, bekijk de actiebalk onder aan de lijst en klik op een van de volgende items, indien beschikbaar. Afhankelijk van welk gebied u tot de lijstmening toegang hebt van, klik op één van de volgende opties:

   * **Schrapping** om het punt te schrappen. Als u een project verwijdert, wordt de verbinding met het project verbroken en verplaatst naar de prullenbak van Workfront. Workfront-beheerders kunnen verwijderde projecten herstellen tot 30 dagen nadat ze zijn verwijderd. Als u een formulier verwijdert, worden de aanvragen of records die bij het verzenden van het formulier zijn gemaakt, niet verwijderd.
   * **maak** los om het project van het verslag los te maken. Als u een project loskoppelt, verwijdert u het project en alle waarden van de opzoekvelden uit de huidige record.

     <!--update screen shot at preview release-->

     ![ bar van Acties in de Verbonden mening van de Lijst van de verslagenpagina ](assets/actions-bar-connected-records-page-list-view.png)

   * **geef vorm** uit: Opent een de verzoekvorm van de Planning en staat u toe om het uit te geven.
   * **unpublish**: maakt een verzoekvorm ongedaan. Hiermee verwijdert u het formulier uit het gebied Verzoeken en kunnen gebruikers geen aanvragen meer toevoegen aan dit recordtype.
   * **Aandeel**: Opent de het Delen doos voor een verzoekvorm waar u met anderen kunt delen.
   * **verbinding van het Exemplaar**: Kopieert een verbinding aan een het verzoekvorm van de Planning zodat kunt u het met andere gebruikers delen. Als het formulier algemeen wordt gedeeld, kunt u de koppeling delen met personen buiten Workfront Planning.

     ![ bar van Acties in de Planning van verzoekenlijst ](assets/actions-bar-in-inake-forms-list.png)



