---
product-area: resource-management
navigation-topic: resource-planning
title: Informatie filteren in de bronnenplanner
description: Gebruikend filters, kunt u wijzigen welke informatie in de Planner van het Middel van alle informatie toont die in het systeem wordt opgeslagen.
author: Lisa
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '2390'
ht-degree: 0%

---

# Gegevens filteren in de bronnenplanner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

Gebruikend filters, kunt u wijzigen welke informatie in de Planner van het Middel van alle informatie toont die in het systeem wordt opgeslagen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td><p>Nieuw: alle</p>
       <p>of</p>
       <p>Huidig: Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Licht of hoger</p>
       <p>of</p>
       <p>Huidig: Controleren of hoger</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>De toegang van de mening of hoger tot Projecten, Gebruikers, en het Beheer van het Middel</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemmingen of hoger van de mening voor projecten</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van de filters Bronnen

Om de hoeveelheid informatie te minimaliseren die in de Planner van het Middel wordt getoond, verstrekt Adobe Workfront een StandaardFilter met vooraf geconfigureerde criteria. Voor informatie over de StandaardFilter, zie het sectie [ Overzicht van de StandaardFilter in de Planner van het Middel ](#overview-of-the-default-filter-in-the-resource-planner) in dit artikel.

U kunt ook aangepaste filters maken. Voor informatie van het aanpassen van filters in de Planner van het Middel, zie de sectie [ de filters van de Planner van het Middel ](#create-resource-planner-filters) in dit artikel creëren.

Overweeg het volgende wanneer het gebruiken van filters in de Planner van het Middel:

* De filters die u maakt, zijn alleen voor u zichtbaar. U kunt filters delen om deze beschikbaar te maken voor andere gebruikers.
* Als Workfront-beheerder kunt u alleen filters zien die u maakt of die met u worden gedeeld.
* De gefilterde resultaten veranderen niet wanneer u een verschillende mening voor de Planner van het Middel selecteert.\
  Voor meer informatie over het veranderen van de mening in de Planner van het Middel, zie de de selectiesectie van de &quot;van het Project/van de Rol/van de Gebruiker&quot;in [ navigatie van de Planner van het Middel ](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* Het toepassen van een filter verandert niet de toewijzing en beschikbaarheidsgegevens in de Planner van het Middel voor projecten, rollen, of gebruikers. Een filter wijzigt alleen het aantal objecten dat u in de functie Bronnen ziet.
* Filteren is van toepassing op alle voorwerpen die tezelfdertijd in de Planner van het Middel tonen. Als u bijvoorbeeld voor een specifieke gebruiker filtert, geeft de functie Bronnen alleen de volgende resultaten weer:

   * Projecten waarbij die gebruiker deel uitmaakt van de bronnenpool (voor de projectweergave en de weergave Rol) of een toewijzing heeft voor het project (voor de weergave Gebruiker)
   * Rollen verbonden aan de gebruiker op die projecten\
     Andere rollen of gebruikers op de projecten waaraan de gebruiker wordt geassocieerd tonen niet.

## Overzicht van het standaardfilter in de bronnenplanner {#overview-of-the-default-filter-in-the-resource-planner}

Als u de functie Bronnen voor het eerst opent, past Workfront het filter Standaard toe. U kunt het filter Standaard bewerken en alleen filteren op de items die u wilt weergeven. Voor informatie bij het wijzigen van een filters, zie de sectie [ een filter in de Planner van het Middel ](#edit-a-filter-in-the-resource-planner) in dit artikel uitgeven.

Houd rekening met het volgende wanneer u het filter Standaard gebruikt:

* De standaardfilter wint informatie slechts van projecten met het volgende terug:

   * Een geplande afsluitdatum die valt na de eerste datum van de huidige maand
   * Een geplande begindatum die valt vóór de laatste dag van de vierde maand vanaf de huidige datum
   * Status van huidige of geplande

  >[!IMPORTANT]
  >
  >Het standaardfilter wint informatie van de projecten terug die altijd binnen vier maanden beginnen met de eerste dag van de huidige maand, ongeacht het tijdkader u aan de vertoning in de Planner van het Middel selecteert.

* In de Mening van de Gebruiker, tonen alle gebruikers in de systeemvertoning maar slechts de gebruikers verbonden aan de gefiltreerde projecten uurinformatie.
* U kunt de informatie in het standaardfilter bewerken zonder het filter op te slaan.
* U kunt een kopie van het filter Standaard dupliceren en bewerken, de gewenste criteria erin wijzigen en deze vervolgens opslaan als een nieuw filter.
* U kunt het standaardfilter niet verwijderen of delen.

  ![ RP_new_default_fitler_criteria__1_.PNG ](assets/rp-new-default-fitler-criteria--1--301x547.png)

## Bronplannerfilters maken {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

Het maken van een filter in de Planner van het Middel is identiek voor alle meningen.

Zorg ervoor dat de eerste vereisten voor het weergeven van de juiste informatie in de functie Bronnen aanwezig zijn voordat u een filter maakt.\
Voor informatie over het ontmoeten van de noodzakelijke eerste vereisten om met de Planner van het Middel te werken, zie de &quot;Eerste vereisten voor het werken in de sectie van de Planner van het Middel&quot;in het ](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artikel van de Planner van 0} het overzicht van het Middel.[

Houd rekening met het volgende wanneer u een filter maakt:

* Er is geen limiet voor het aantal objecten waarvoor u in één keer kunt filteren.
* De beschikbare velden die u aan een filterwijziging kunt toevoegen, zijn afhankelijk van het object van de weergave die u op de functie Bronnen toepast. U kunt bijvoorbeeld alleen in de weergave Gebruiker filteren op de velden Uitgave of Taak, omdat deze objecten alleen in de weergave Gebruiker worden weergegeven. Als u een filter voor Kwesties of Taken in de mening van de Gebruiker bouwt en dan het op de mening van het Project of van de Rol toepast, wordt het genegeerd omdat de gebieden niet in de mening van het Project of van de Rol bestaan. In dit geval lijkt het filter niet beschikbaar.

Een filter maken in de bronnenplanner:

{{step1-to-resourcing}}

De **vertoningen van de Planner** door gebrek.

Door gebrek, de eerste keer u tot de Planner van het Middel toegang hebt, wordt de <strong> StandaardFilter </strong> toegepast.<br> voor meer informatie over de Standaardfilter, zie het <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref"> Overzicht van de StandaardFilter in de 2} sectie van de Planner van het Middel {in dit artikel.</a>

1. In de upper-left hoek van, klik het **pictogram van de Filter**.
   ![ filter_icon.png ](assets/filter-icon.png)
of
Vouw het **drop-down menu van de Filter** uit en klik **voeg Nieuwe Filter** toe.
   ![ dropdown van de Filter ](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. Als u een filter wilt maken aan de hand van de ingebouwde criteria, geeft u een van de volgende velden op:

   * **Portfolio**: Begin typend de naam van de portefeuille die de informatie bevat u in de Planner van het Middel wilt omvatten, dan klik de naam wanneer het in de lijst verschijnt.\
     Herhaal dit proces om informatie uit meerdere portfolio&#39;s op te nemen.

   * **Status van het Project**: Breid het drop-down menu van de Status van het Project uit en selecteer één of veelvoudige projectstatussen beschikbaar in de lijst.
   * **Team**: Begin typend de naam van één of veelvoudige teams verbonden aan de gebruikers die aan taken in de projecten worden toegewezen u wilt bekijken.
   * **Rol van de Baan**: Begin typend de naam van één of veelvoudige baanrollen verbonden aan de gebruikers die aan taken in de projecten worden toegewezen u wilt bekijken.
   * **Pools**: Begin typend de naam van één of veelvoudige Groepen van het Middel die met de projecten (voor de Mening van het Project), de gebruikers (voor de Mening van de Gebruiker), of verbonden met zowel de projecten als de gebruikers (voor de Mening van de Rol) worden geassocieerd die u wilt bekijken.
   * **Groep**: Begin typend de naam van één of veelvoudige groepen verbonden aan de gebruikers (in de mening van de Gebruiker) of projecten (in de meningen van het Project en van de Rol) die u wilt bekijken.

1. Klik **toevoegen de Regel van de Filter**, dan begin het typen van de gebiedsnaam die u door in het **Type aan filterpunten** doos wilt filteren. Als het veld beschikbaar is, wordt het gevuld voor elk object waaraan het kan worden gekoppeld.

   >[!IMPORTANT]
   >
   >Wanneer u naar aangepaste velden verwijst, moet u de veldnaam en niet het veldlabel typen. Het veldlabel wordt weergegeven op een aangepast formulier dat is gekoppeld aan een object. Voor informatie over het verschil tussen het etiket en de naam van een douanegebied, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Klik op de naam van het veld om het aan het filter toe te voegen wanneer het in de lijst wordt weergegeven.\
   Voor meer informatie over de gebieden u in de lijst ziet, zie [ Verklarende woordenlijst van de terminologie van Adobe Workfront ](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (Optioneel) Selecteer de filter- en voorwaardomstandigheden voor het filter. De beschikbare bepalingen worden beschreven in [ Filter en voorwaardenbepalingen ](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   U kunt op gebruiker-gebaseerde of op datum-gebaseerde vervangingen gebruiken om voor informatie te filtreren verbonden aan het het programma geopende gebruiker.\
   Voor informatie over gesteunde vervangingen in filters, zie [ overzicht van de de filtervariabelen van de Vervanging ](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klik **sparen** om de filterregel te bewaren.
1. (Facultatief) klik **toevoegen de Regel van de Filter** om een nieuwe regel voor een ander voorwerp of gebied toe te voegen.
1. Klik **toepassen** om de filter toe te passen zonder het op te slaan.

   of

   Klik **sparen Filter** om de filter te bewaren.\
   ![ RP_Apply_or_Save_buttons_on_filters.png ](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (Voorwaardelijk) nadat u **** klikt sparen, specificeer een naam voor de filter in het **vakje van de Naam van de Filter** binnen **sparen de dialoogdoos van de Filter**. Dit is een verplicht veld.\
   ![ RP_new_save_filter_box__with_Save_button__without_apply.png ](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >Als uw filternaam speciale tekens bevat, gebruikt u alleen de volgende tekens:
   >
   >* Komma
   >* Snede
   >* Afbreekstreepje
   >* Onderstrepingsteken

1. Klik **sparen**.

   De resultaten in de Planner van het Middel worden nu gefiltreerd door de informatie u in de filterregels omvatte.

## Een bestaand filter toepassen

Wanneer u of iemand met toegang tot de Planner van het Middel een filter opslaat, wordt het beschikbaar aan iedereen die de Planner van het Middel gebruikt.

Een bestaand filter toepassen:

1. Ga naar de bronnenplanner.
1. In de upper-left hoek, breid het **drop-down menu van de Filter** uit.

   In dit menu ziet u filters die u hebt gemaakt of andere filters die met u zijn gemaakt en gedeeld.\
   ![ RP_filter_drop_down.png ](assets/rp-filter-drop-down-350x152.png)

1. Selecteer een filter in het vervolgkeuzemenu. U kunt filters zien die u of andere gebruikers in dit menu hebben gemaakt.\
   Wanneer u een filter selecteert, vermindert het automatisch de hoeveelheid informatie die in de Planner van het Middel toont.

## Een filter bewerken in de functie Bronnen {#edit-a-filter-in-the-resource-planner}

U kunt een filter in de Planner van het Middel uitgeven door één van het volgende te doen:

* [ noem een filter ](#rename-a-filter) anders
* [ geef de informatie in een filter ](#edit-the-information-in-a-filter) uit
* [Een filter dupliceren](#duplicate-a-filter)

Wanneer u een filter bewerkt, wordt het bijgewerkt voor alle gebruikers in het systeem die toegang hebben tot de functie voor het toewijzen van bronnen.

### De naam van een filter wijzigen {#rename-a-filter}

U kunt de naam van een filter wijzigen zonder de criteria te wijzigen. We raden u aan andere gebruikers in het systeem op de hoogte te stellen van deze wijziging, aangezien filters zichtbaar zijn voor andere gebruikers. Deze wijziging is van invloed op de lijsten met filters voor iedereen die de functie Bronnen kan zien.

1. Ga naar de Planner van het Middel en breid **drop-down menu van de Filter** uit om een bewaarde filter te selecteren.
1. Vouw het **drop-down menu van de Filter** uit. Zoek het filter waarvan u de naam wilt wijzigen en houd het boven de naam.
1. Selecteer **anders noemen filter** pictogram naast de naam van de filter.

   ![ geef filteropties uit ](assets/rp-filter-options-edit-350x154.png)

1. Specificeer een nieuwe naam voor de filter in de **Naam van de Filter** doos.
1. Klik **sparen**.\
   De informatie in het filter is gelijk en de naam wordt bijgewerkt.

### De informatie in een filter bewerken {#edit-the-information-in-a-filter}

U kunt de gegevens die u in een filter opneemt, wijzigen zonder de naam ervan te wijzigen. We raden u aan andere gebruikers in het systeem op de hoogte te stellen van deze wijziging, aangezien filters voor hen zichtbaar zijn. Deze wijziging is van invloed op de lijsten met filters voor iedereen die de functie Bronnen kan zien.

1. Ga naar de Planner van het Middel en breid **drop-down menu van de Filter** in de upper-left hoek uit.
1. Selecteer een bestaand filter dat u wilt bewerken.
1. Klik het **pictogram van de Filter**.\
   ![ filter_icon.png ](assets/filter-icon.png)

1. Voeg nieuwe velden toe aan het filter.\
   Voor informatie over de bouw van filters, zie [ de filters van de Planner van het Middel ](#create-resource-planner-filters) creëren.

1. Beweeg over de bestaande gebieden die voor de filter worden geselecteerd, en klik **uitgeven** pictogram om een ander gebied te selecteren, of **schrap** pictogram om het gebied te schrappen.\
   ![ RP_custom_filter_delete_and_edit_icons.png ](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (Facultatief) klik **toevoegen de Regel van de Filter** om nieuwe gebieden aan de filter toe te voegen.\
   Voor meer informatie over het bepalen van filtercriteria, zie [ de filters van de Planner van het Middel ](#create-resource-planner-filters) creëren.

1. Klik **toepassen** om de filter toe te passen zonder het op te slaan.

   of

   Klik **sparen** om de filter te bewaren.\
   Het filter wordt met dezelfde naam maar met nieuwe filtercriteria opgeslagen.

### Een filter dupliceren {#duplicate-a-filter}

U kunt een bestaand filter dupliceren. De oorspronkelijke filtercriteria blijven hetzelfde in het gedupliceerde filter en u kunt het nieuwe filter onder een andere naam opslaan.

1. Ga naar de Planner van het Middel en breid **drop-down menu van de Filter** in de upper-left hoek uit.
1. Houd de muis boven de naam van een opgeslagen filter dat u wilt dupliceren.
1. Klik het **Dubbele** pictogram.

   ![ Dupliceer filter ](assets/rp-filter-options---duplicate-350x154.png)\
   Het vak Filter dupliceren wordt weergegeven.

1. Op het **gebied van de Naam van de Filter**, specificeer een nieuwe naam voor de gedupliceerde filter.\
   De standaardnaam voor de nieuwe filter is *`<Original Filter Name>`(exemplaar)*.

1. Klik **sparen**. Er wordt een nieuw filter gemaakt met dezelfde criteria als het oorspronkelijke filter en met een nieuwe naam.

   >[!NOTE]
   >
   >Hoewel u 2 filters door de zelfde naam en met identieke criteria kunt hebben, adviseren wij dat u filters met unieke het filtreren criteria en namen in uw Planner van het Middel bewaart om verwarring te vermijden.

## Een filter verwijderen

U kunt een filter verwijderen wanneer het niet meer nodig is. U kunt het standaardfilter niet verwijderen.

Voor informatie over de StandaardFilter, zie het [ Overzicht van de StandaardFilter in de sectie van de Planner van het Middel ](#overview-of-the-default-filter-in-the-resource-planner) in dit artikel.

Wanneer u een filter verwijdert, wordt het filter verwijderd voor alle Workfront-gebruikers die toegang hebben tot de Resource Planner. Voordat u het filter verwijdert, moet u ervoor zorgen dat het filter dat u wilt verwijderen niet meer wordt gebruikt door iemand anders die in de Resource Planner werkt. Een verwijderd filter kan niet worden hersteld.

Een filter verwijderen:

1. Ga naar de bronnenplanner.
1. Vouw het **drop-down menu van de Filter** uit.
1. Zoek het filter dat u wilt verwijderen en houd de muisaanwijzer boven de naam van het filter.
1. Selecteer het **filter van de Schrapping** pictogram naast de naam van de filter.

   ![ filter van de Schrapping ](assets/rp-filter-options---delete-350x154.png)

1. Klik **Schrapping** in het **de dialoogvakje van de Filter van de Schrapping**.

1. Het filter wordt verwijderd uit de bronnenplanner.

## Een filter delen

U kunt een filter delen dat u hebt gemaakt of dat u toegang hebt om met andere gebruikers te delen. U kunt het standaardfilter niet delen, maar u kunt het wel dupliceren en de kopie delen.

>[!NOTE]
>
>Alle gebruikers, inclusief Workfront-beheerders, hebben alleen toegang tot filters die ze hebben gemaakt of die met hen zijn gedeeld. U kunt een filter met specifieke gebruikers delen om een filter ter beschikking te stellen van alle gebruikers van de Planner van het Middel.

Voor informatie over de StandaardFilter, zie het [ Overzicht van de StandaardFilter in de sectie van de Planner van het Middel ](#overview-of-the-default-filter-in-the-resource-planner) in dit artikel.

Voor informatie over het dupliceren van filters, zie [ een filter ](#duplicate-a-filter) sectie in dit artikel dupliceren.

1. Ga naar de bronnenplanner.
1. Vouw het **drop-down menu van de Filter** uit.
1. Zoek het filter dat u wilt delen en houd de muisaanwijzer boven de naam van het filter.
1. Selecteer het **filter van het Aandeel** pictogram naast de naam van de filter.

   ![ filter van het Aandeel ](assets/rp-filter-options---share-350x154.png)

   Het dialoogvenster Filtertoegang wordt weergegeven.

1. (Facultatief) om de filter ter beschikking te stellen van alle gebruikers van de Planner van het Middel, klik het **pictogram van Montages**, dan uitgezocht **maak dit zichtbare systeem-breed**.

   ![ maak zichtbaar systeem-breed ](assets/make-this-visible-system-wide-350x119.png)

1. In **geef de filtertoegang van de middelplanner tot:** doos, begin de namen van gebruikers, teams, rollen, groepen, of bedrijven te typen die u de filter met wilt delen.
1. Selecteer een van de volgende machtigingsniveaus:

   * Weergave
   * Beheren

     Voor informatie over toestemmingen in Workfront, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (Facultatief) klik **Geavanceerde Plaatsende** s om toestemmingen voor elk niveau toe te voegen door hen te selecteren of toestemmingen voor elk niveau te verwijderen door hen te deselecteren.

   ![ filter van het Aandeel ](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. Klik **sparen**.

   Het filter wordt gedeeld met de entiteiten die u selecteerde en het verschijnt in het **Gedeeld met me** gebied.

   ![ Gedeeld met me ](assets/rp-shared-with-me-area.png)
