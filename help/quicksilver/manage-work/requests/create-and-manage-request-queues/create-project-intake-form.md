---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Forms voor projectinname maken
description: Met formulieren voor het opnemen van projecten kunt u het maken van projecten in Workfront vereenvoudigen
author: Becky
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: 5ff71313c550d949079e7426b657a0a4e19a656c
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 0%

---

# Formulieren voor projectopname maken

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

De de innameformulieren van het project zijn een type van verzoekvorm die gebruikers toestaat om projecten aan te vragen. De projecten worden gecreeerd van de vorm, zonder het moeten een project van een voorgelegde kwestie tot stand brengen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Nieuwe licentie: standaard </p>
   of
   <p>Huidige licentie: abonnement </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn om formulieren voor het opnemen van projecten te maken. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere producten</td> 
   <td> <p>Uw organisatie moet de Planning van Workfront hebben gekocht om de eigenschappen van de Planning zoals automatisering te gebruiken.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mogelijkheden en beperkingen voor het opnemen van projecten in Forms

### Mogelijkheden

De innameformulieren voor projecten bevatten de volgende mogelijkheden:

#### Workfront-planningsautomatisering

Workfront-formulieren voor projectopname ondersteunen Workfront Planning Automations om de gemaakte projectspecifieke eigenschappen te configureren.

Voor meer informatie bij de automatisering van de Planning, zie [ de automatisering van de Planning van Adobe Workfront ](/help/quicksilver/planning/records/configure-automations-to-create-records.md) vormen.

### Goedkeuringsconfiguratie

De innameformulieren van het project omvatten de capaciteit om fiatteurs voor voorgelegde verzoeken te vormen.

### Beperkingen

#### Ondersteunde veldtypen

Forms voor het opnemen van projecten kan velden van elk aangepast formulier bevatten met het objecttype Project.

De volgende veldtypen worden momenteel niet ondersteund in Project Intake Forms:

* Sectie
* Formule
* Rollup
* Eén regel rollup
* Verbinding voor planning
* Native veldverwijzingen die worden verwezen naar native projectvelden, die alleen-lezen zijn (bijvoorbeeld `workRequiredExpression` )

#### Ervaring aanvragen

Formulieren voor het opnemen van projecten kunnen alleen worden gebruikt met de nieuwe ervaring die u opvraagt.

Voor informatie over de nieuwe het vragen ervaring, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

#### Delen

Formulieren voor het opnemen van projecten bieden geen ondersteuning voor openbare uitwisseling. Tot de opties voor delen behoren:

* **Iedereen**: Iedereen in het systeem kan de vorm gebruiken om een projectverzoek voor te leggen.
* **gespecificeerde gebruikers**: U kunt selecteren welke specifieke gebruikers toegang tot de vorm van het projectverzoek hebben.

## Een formulier voor projectopname maken

{{step1-to-requests}}

1. Laat de **Schakelaar aan een nieuwe ervaring** toe plaatsend, in de hoger-juiste hoek van het scherm.
1. Klik **vormen van het Verzoek** in de hoger-juiste hoek van het scherm.

   >[!NOTE]
   >
   >Omdat alleen Workfront-beheerders innameformulieren kunnen maken, is de knop Formulieren aanvragen alleen zichtbaar voor beheerders.

   Er wordt een lijst weergegeven met momenteel beschikbare aanvraagformulieren. Dit omvat aanvraagformulieren van Workfront Planning.

1. Klik **Nieuwe verzoekvorm** in de hoger-juiste hoek van het scherm.
1. Voer een naam in voor het aanvraagformulier. Door gebrek, is de naam van de vorm **Naamloze vorm**.
1. Selecteer het objecten type **Project** dichtbij de bovenkant van de dropdown lijst. Dit is momenteel het enige beschikbare Workfront-projecttype. Andere punten in de lijst behoren tot de Planning van Workfront.
1. (Facultatief) voeg a **Beschrijving** voor de verzoekvorm toe.
1. Klik **creëren**. Het aanvraagformulier voor het geselecteerde recordtype wordt geopend op het tabblad Formulier.

   De bouwer van de de projectinname vorm opent aan de Vorm tabel.

   Het inlaatformulier bevat standaard de volgende informatie:

   * **Standaard sectie**: Dit is de standaardsectieonderbreking die Workfront op de verzoekvorm van toepassing is. Alle verslaggebieden tonen op het **Standaard sectie** gebied.
   * **Onderwerp** gebied: Het gebied dat het verzoek in Workfront zal identificeren. De configuratie en de waarde van het onderwerpveld kunnen niet worden bewerkt.
   * Alle gebieden verbonden aan projecten.

     De velden in het aanvraagformulier zijn zichtbaar voor iedereen die een projectaanvraag indient.

1. Als u velden aan het formulier wilt toevoegen, klikt u op het veldtype in de linkernavigatie en selecteert u het veld.
1. (Facultatief) om een gebied te verwijderen, over het gebied op de vorm te bewegen die u wilt verwijderen, dan het **x** pictogram klikken om het te verwijderen.
1. (Facultatief) om de **Standaardsectie** uit de vorm te verwijderen, doe het volgende:

   1. Alle velden verwijderen uit de standaardsectie.
   1. Klik de **elementen van de Inhoud** tabel en voeg een nieuwe sectie toe, dan voeg een naam voor de sectie toe.
   1. Voeg velden toe aan de nieuwe sectie.
   1. Klik het **x** pictogram om de **Standaard sectie** te verwijderen.
1. Klik op een veld en gebruik vervolgens de besturingselementen in het rechterdeelvenster van het formulier om de grootte van het veld te definiëren, of een van de volgende gegevens:

   * **Etiket**: Dit is de naam van het gebied aangezien het op de verzoekvorm zal verschijnen. Hiermee wijzigt u de naam van het recordveld niet.
   * **Instructies**: Voeg meer informatie over het gebied toe.
   * **maak een vereist gebied**: Wanneer geselecteerd, moet het gebied een waarde hebben. Anders kan het formulier niet worden verzonden.
   * **voegt logica** toe: Bepaal welke voorwaarden moeten worden voldaan opdat het gebied tonen of verborgen zijn.

   >[!TIP]
   >
   >   Het veldtype van elk veld wordt boven in het rechtervenster weergegeven, nadat u het veld op het formulier hebt geselecteerd.
   >     

1. (Facultatief) klik de **elementen van de Inhoud** tabel op de linkerkant van de vorm, en voeg om het even welke volgende elementen toe:

   * **Beschrijvende tekst**
   * **de onderbreking van de Sectie**

   Voor meer informatie over de bouw van een douaneformulier, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Klik het **lusje van Automaties** op de linkerkant van de vorm, dan doe om het even welke volgend:

   * Een projectsjabloon selecteren
   * Aangepaste formulieren bijvoegen
   * Een eigenaar van een project instellen
   * Het project toevoegen aan een portfolio of programma

   Alle selecties die u hier aanbrengt, worden toegepast op projecten die op basis van dit inlaatformulier zijn gemaakt.

1. (Facultatief) klik **Voorproef** om te bekijken hoe de vorm voor andere gebruikers zal tonen wanneer zij het zullen gebruiken om een nieuw verslag voor te leggen.

1. (Facultatief) klik het **lusje van de Configuratie**, dan voeg minstens één gebruiker of team toe &lt; aan het **Approvers** gebied om nieuwe verzoeken voor deze inlaatvorm goed te keuren.

   * Wanneer u een inlaatformulier aan fiatteurs koppelt, moet elk nieuw verzoek eerst door alle fiatteurs worden goedgekeurd voordat het een project genereert.
   * U kunt een of meer fiatteurs toevoegen aan een inlaatformulier.
   * Als ten minste één fiatteur het verzoek afwijst, wordt het verzoek afgewezen en wordt het project niet gemaakt.
   * Alle fiatteurs moeten een besluit nemen voordat een project wordt goedgekeurd of afgewezen.
   * Als een team als fiatteur wordt geplaatst, wordt slechts één besluit vereist van het team.

     Voor meer informatie over het toevoegen van goedkeuringen aan aanvraagvormen, zie [ goedkeuring aan een verzoekvorm ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) toevoegen.

1. (Facultatief) klik het **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de naam van de vorm in de kopbal, dan klik **uitgeven** om de naam van de vorm bij te werken.

1. Klik **publiceren** om de vorm te publiceren en een unieke verbinding voor het te verkrijgen.

   De volgende dingen doen zich voor:

   * De **Publish** knoop wordt verwijderd.
   * De **unpublish** knoop wordt toegevoegd aan de vorm. Als u erop klikt, is het formulier niet toegankelijk.
   * A **de knoop van het Aandeel** wordt toegevoegd aan de vorm.
   * Het formulier wordt beschikbaar in het gedeelte Aanvragen van het menu Main in Workfront.

1. Klik **Aandeel** om de vorm met anderen te delen.
1. Klik op de pijl die naar links wijst links van de naam van het formulier in de koptekst om het formulier te sluiten.

   De **vorm van het Verzoek** lijstmening opent en de vorm wordt toegevoegd aan het.

1. (Facultatief) Beweeg over de naam van een verzoekvorm in de lijstmening, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de vormnaam, en klik één van het volgende:

   * **geef vorm** uit: Klik dit om informatie over de vorm verder uit te geven.
   * **unpublish**: Klik dit om de vorm ongedaan te maken die het uit het gebied van Verzoeken in Workfront verwijdert.
   * **Aandeel**: Klik dit om te wijzigen wie toegang tot de vorm heeft.
   * **verbinding van het Exemplaar**: Klik dit om snel de verbinding van de verzoekvorm te kopiëren zonder de vorm te openen.
   * **Schrapping**: Klik dit om de vorm te schrappen. Alle aanvragen en records die met het formulier zijn toegevoegd, worden niet verwijderd. Het formulier kan niet worden hersteld.

   >[!NOTE]
   >
   >U kunt innameformulieren voor projecten identificeren in de tabelweergave omdat deze &#39;Project&#39; weergeven in de kolom Type object.

1. Klik op de pijl die naar links wijst links van **Request-formulieren** in de header om de aanvraagformuliertabel te sluiten.

