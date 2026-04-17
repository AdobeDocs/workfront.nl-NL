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
source-git-commit: a6c2bc4127a52fad209004995ea2262fa64c240d
workflow-type: tm+mt
source-wordcount: '1791'
ht-degree: 0%

---


# De lijstweergave beheren in Adobe Workfront Planning

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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
      >* U kunt een weergave herstellen die met u is gedeeld en waarvoor u alleen weergavemachtigingen hebt, nadat u de weergave hebt gewijzigd om de oorspronkelijke voorkeuren te herstellen, of u kunt de weergave met de wijzigingen kopiëren en de kopie delen. Voor meer informatie, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   1. Klik het **pictogram van de Filter** pictogram ![ van de Filter ](assets/filter-icon.png) om een filter aan de mening toe te voegen. De resultaten worden direct in de lijst gefilterd. U kunt filters niet opslaan en een naam geven. Filters worden onthouden wanneer u de pagina in de toekomst opent en maken deel uit van gedeelde weergaven.

      >[!TIP]
      >
      >Als u een gepersonaliseerd filter wilt toepassen, selecteert u een van de volgende opties voor een veldwaarde:
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

   1. Klik het **pictogram van Kolommen** pictogram van Kolommen ![ ](assets/columns-icon.png) om te selecteren welke kolommen aan vertoning of in de mening te verbergen.
   1. Houd de cursor boven de naam van een kolom en klik op de pijl omlaag links van de kolomnaam en klik op een van de volgende opties:
      * **noem** anders, om a **Eigen etiket** voor de kolom toe te voegen. De naam van het oorspronkelijke veld in Workfront verandert niet.
      * **Soort**, om de lijst door het geselecteerde gebied te sorteren. Aan de kolomkop wordt een sorteerpictogram toegevoegd dat de richting van het sorteren aangeeft.
   1. Klik het **+** pictogram in de hoger-juiste hoek van de lijst om kolommen aan de lijst toe te voegen of te verwijderen, dan klik **sparen**.

      De **manager van de Kolom** opent.

      U kunt alleen bestaande velden toevoegen aan de lijstweergave.
U kunt het primaire veld niet verwijderen in de lijstweergave die in de eerste kolom wordt weergegeven.

   1. Klik het **pictogram** de cellen van het Formaat {![ pictogram van de Cellen van het 0} Formaat. ](assets/format-cells-icon.png) Het **vakje van het Formaat** opent. <!--change the name of the box when they update it-->
Ga als volgt te werk:

      1. Klik **toevoegen voorwaarde**.
      1. In **als** lijn, selecteer een gebied en kies een gebiedswaarde en voeg een bepaling toe. De opties veranderen, afhankelijk van het gebiedstype u kiest.

         >[!TIP]
         >
         >Alleen velden die zichtbaar zijn in de lijstweergave zijn beschikbaar voor voorwaardelijke opmaak.

      1. (Facultatief) in plaats van het toevoegen van een gebiedswaarde, klik **vergelijken met een ander gebied** pictogram ![ vergelijk met een ander gebied ](assets/compare-to-another-field-icon.png) en kies een gebied de waarvan waarde u met de waarde van uw geselecteerd gebied wilt vergelijken. U kunt bijvoorbeeld de velden Projecteigenaar en Projectsponsor vergelijken.

         >[!TIP]
         >
         >Alleen velden die zichtbaar zijn in de lijstweergave zijn beschikbaar voor voorwaardelijke opmaak. De velden die u vergelijkt, moeten van hetzelfde type zijn.

      1. (Facultatief) klik **toevoegen voorwaarde** in **als** lijn om meer voorwaarden aan de zelfde regel toe te voegen.

         >[!TIP]
         >
         >U kunt maximaal 10 voorwaarden toevoegen aan een conditioneringsregel en u kunt maximaal 20 regels toepassen op een veld.

      1. Klik de **of** schakelaar tussen voorwaarden om in **en** te veranderen en erop te wijzen dat de veelvoudige voorwaarden tezelfdertijd moeten worden vervuld. **Of** is de standaardschakelaar.
      1. In de **lijn van het Formaat**, selecteer een gebied om erop te wijzen welke kolom zal worden geformatteerd. <!--edit this area, if it changes names??-->
      1. (Facultatief) klik het **pictogram van de kleurencirkel** Kleurcirkelpictogram ![ naast het geselecteerde gebied, om het uit te breiden en een andere kleur in het ](assets/color-circle.png) vult van de Cel **gebied te kiezen om de kleur van de achtergrond in een cel te veranderen of een kleur van het** kleur van de Tekst **gebied te kiezen om de kleur van tekst in een cel te veranderen.**
      1. Klik het **pictogram van het formaat van de Tekst 1} van de Tekst** ![ en selecteer van de volgende opties om de tekst in een cel te formatteren:](assets/text-format-icon.png)
         * Vet
         * Cursief

      1. Zet **toe is op rij** het plaatsen om het formatteren op de volledige rij van het gebied toe te passen dat aan de voorwaarden voldoet.
      1. (Facultatief) klik **toevoegen voorwaarde** in het **vakje van het Formaat** om een andere regel voor een ander gebied toe te voegen en de herhaling hierboven de stappen.
      1. (Optioneel) Klik op **Alles wissen** om alle opmaak te verwijderen.
      1. Klik buiten het **vakje van het Formaat** om het te sluiten.

         Hiermee keert u terug naar de lijstweergave.
De opmaak wordt direct toegepast op de lijstweergave.
Er is een blauw punt naast het **pictogram van de Cellen van het Formaat** om erop te wijzen dat de mening speciale toegepaste het formatteren heeft.

   1. (Facultatief) klik het **pictogram van de Groepering** pictogram van de Groepering ![ ](assets/grouping-icon.png) aan groepspunten in de lijst door een gemeenschappelijk gebied. <!--have they updated this to "Grouping"??--> Selecteer een van de opties of gebruik de zoekbalk om een veld te zoeken.

      Het veld moet een kolom in de lijst zijn voordat u het kunt groeperen. Niet alle veldtypen kunnen voor groepen worden gebruikt.

   1. Klik het **pictogram van de de hoogte van de Rij** ![ pictogram van de Rijhoogte om de verticale lengte van een rij bij te werken. ](assets/row-height-icon.png) Kies een van de volgende opties:

      * Kort
      * Standaard. Dit is de standaardoptie.
      * Medium
      * Lang

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



