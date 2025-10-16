---
title: Een aanvraagformulier maken en beheren in Adobe Workfront-planning
description: Nadat u een recordtype hebt geselecteerd in het gedeelte Adobe Workfront Planning, kunt u een aanvraagformulier maken en dit koppelen aan dat recordtype. Vervolgens kunt u een koppeling naar de koppeling delen met andere interne of externe gebruikers. Gebruikers met een koppeling naar het formulier kunnen de veldwaarden erin invullen en door deze te verzenden, kunnen zij een nieuwe record toevoegen voor het bijbehorende recordtype.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '2686'
ht-degree: 0%

---

# Een aanvraagformulier maken en beheren in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


{{planning-important-intro}}

U kunt een aanvraagformulier maken en dit koppelen aan een recordtype in Adobe Workfront Planning. U kunt het formulier vervolgens met anderen delen en ze kunnen aanvragen indienen om records van dat type te maken.

In dit artikel wordt beschreven hoe een werkruimtebeheerder een aanvraagformulier kan maken dat is gekoppeld aan een recordtype.

Voor informatie over het voorleggen van een verzoek aan een verslagtype om een verslag tot stand te brengen, zie [&#x200B; de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakketten</p></td> 
   <td> 
<ul><li><p>Willekeurig Workfront-pakket</p></li>
en
<li><p>Willekeurig planningspakket</p></li></ul>
of
<ul><li><p>Willekeurig workflowpakket</p></li>
en
<li><p>Willekeurig planningspakket</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte of recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beperkingen op veld- en waardenweergave in aanvraagformulieren

Er zijn beperkingen in de manier waarop bepaalde velden worden weergegeven op het aanvraagformulier en hoe de waarden ervan later worden weergegeven op de records of op de pagina met aanvraagdetails nadat u een aanvraag hebt ingediend.

Voor informatie over het voorleggen van de verzoeken van de Planning van Workfront, zie [&#x200B; de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

* Hieronder volgt een aantal beperkingen voor de weergave van bepaalde velden in aanvraagformulieren, records die zijn gemaakt op een aanvraagformulier of op de pagina met aanvraagdetails:

   * U kunt geen velden van de volgende typen toevoegen aan een aanvraagformulier:

      * Gemaakt door, Laatst gewijzigd door, <span class="preview"> goedgekeurd door </span>
      * Gemaakt op datum, Laatste gewijzigde datum, <span class="preview"> Goedgekeurde datum </span>
      * Opzoekvelden van Workfront-objecten
      * Workfront Planning connected records lookup fields

* Hieronder ziet u verschillen tussen de manier waarop veldindelingen worden weergegeven in de aanvraagformulierbuilder en de manier waarop de waarden van de velden worden opgemaakt op de record of op de pagina met aanvraagdetails:

   * De velden Valuta, Nummer en Percentage worden weergegeven als een tekstveldtype voor één regel in de formulierbuilder.

     De veldindeling blijft echter wel behouden en de veldwaarden worden na het indienen van het verzoek weergegeven als valuta, cijfers en percentages, op het recordtype en op de pagina met aanvraagdetails.

* In het volgende voorbeeld wordt beschreven hoe bepaalde veldwaarden worden weergegeven op aanvraagformulieren en worden pagina&#39;s met informatie over de aanvraag weergegeven:

   * De speciale opmaak voor de velden Valuta, Aantal en Percentage blijft niet behouden. De decimale precisie blijft bijvoorbeeld niet behouden voor de waarden van deze velden in deze gebieden.
   * Veldwaarden voor personen worden weergegeven als id&#39;s.
   * Formule velden die niet naar andere velden of berekeningen verwijzen, geven geen waarden weer. Een veld met een formule `STRING` geeft bijvoorbeeld de waarde &quot;N/A&quot; weer.
   * Formule velden die naar valutavelden verwijzen, geven de waarden weer zonder rekening te houden met de wisselkoersen.
   * De waarden van de gebieden van de Paragraaf tonen een waarde &quot;N.v.t.&quot;op het verzoekformulier en zij tonen HTML markeringen in plaats van de geformatteerde tekst op de pagina van de verzoekdetails.

## Een aanvraagformulier maken

Als u een aanvraagformulier wilt maken, moet u beginnen met het maken van het formulier, de formulierdetails instellen en eindigen door het formulier te publiceren en te delen.

### Een aanvraagformulier maken

U kunt een verzoekvorm van het verslagtype tot stand brengen verbonden aan de vorm <!--span class="preview">, or from the Requests area of Workfront.</span>-->.

#### Een aanvraagformulier maken van een recordtype

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.

1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de naam van het verslagtype in de paginakop, dan klik **creeer verzoekvorm** of **beheer verzoekvormen**, als u reeds een vorm hebt en u extra degenen wilt creëren.
1. (Voorwaardelijk) als u een andere vorm wilt toevoegen, klik **Nieuwe verzoekvorm**.

   Het vak Aanvraagformulier maken wordt geopend.

1. Werk de naam van het aanvraagformulier bij in het vak Aanvraag maken. Door gebrek, is de naam van de vorm **Naamloze vorm**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Facultatief) voeg a **Beschrijving** voor de verzoekvorm toe.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klik **creëren**.

   Het aanvraagformulier voor het geselecteerde recordtype wordt geopend op het tabblad Formulier.
1. Ga aan [&#x200B; verder vormen de vorm &#x200B;](#configure-the-form).

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### Details instellen voor het aanvraagformulier

Formulierdetails worden verdeeld in tabbladen.

* Het **lusje van de Vorm** staat u toe om gebieden en inhoudselementen aan de vorm toe te voegen
* Het **lusje van de Configuratie** staat u toe om een goedkeuringsproces voor de vorm te plaatsen, en om de opties van de verzoekvoltooiing te plaatsen&lt;.
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### Formuliergegevens instellen

1. Beginnen creërend of het uitgeven van een verzoekvorm, zoals die in de sectie [&#x200B; wordt beschreven Begin creërend een verzoekvorm &#x200B;](#begin-creating-a-request-form).

   Het aanvraagformulier voor het geselecteerde recordtype wordt geopend op het tabblad Formulier.

   ![&#x200B; de verzoekvorm van campagnes geeft wijze uit &#x200B;](assets/campaigns-request-form-edit-mode.png)

   Het aanvraagformulier bevat standaard de volgende informatie:

   * De gebieden van het verslag beschikbaar in de lijstmening van het geselecteerde verslagtype. <!--they are working on removing the limitation below-->

   * **Standaard sectie**: Dit is de standaardsectieonderbreking die Workfront op de verzoekvorm van toepassing is. Alle verslaggebieden tonen op het **Standaard sectie** gebied.
   * **Onderwerp** gebied: Het gebied dat het verzoek in Workfront zal identificeren. De configuratie en de waarde van het onderwerpveld kunnen niet worden bewerkt.

     >[!NOTE]
     >
     >* Het **Onderwerp** gebied vereist een waarde wanneer het op de verzoekvorm zichtbaar is. Nochtans, kunt u het **Onderwerp** gebied verwijderen, indien nodig, en de verzoekers zullen het niet op de vorm zien wanneer zij het verzoek voorleggen.
     >* Wanneer het onderwerpveld ontbreekt op een aanvraagformulier, maar er een naamveld is voor de naam van de toekomstige record, wordt aan de naam van de aanvraag automatisch dezelfde naam toegewezen als aan de gemaakte record.
     >* Wanneer zowel het Onderwerp als de gebieden van de Naam op de verzoekvorm ontbreken, wordt het verzoek genoemd gebruikend het volgende patroon: `< Record name > request form < Entry date of the request >`; het verslag wordt genoemd **Naamloos**.

   * Alle velden die aan het recordtype zijn gekoppeld.

     De velden in het aanvraagformulier zijn zichtbaar voor iedereen die een aanvraag naar dit recordtype indient.

1. (Optioneel) Houd de muisaanwijzer boven alle velden in het formulier die u wilt verwijderen en klik vervolgens op het pictogram **x** om deze te verwijderen. Zij worden toegevoegd aan het **lusje van Gebieden** links van de vorm.

   Bijvoorbeeld, verwijder het **Onderwerp** gebied, aangezien dit niet in de Planning van Workfront zichtbaar is. <!--remove this example if this becomes visible in Planning?-->

1. (Facultatief) om de **Standaardsectie** uit de vorm te verwijderen, doe het volgende:

   1. Alle velden verwijderen uit de standaardsectie.
   1. Klik **de elementen van de Inhoud** en voeg een nieuwe sectie toe, dan voeg een naam voor de sectie toe.
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

   Voor meer informatie over de bouw van een douaneformulier, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. (Facultatief) klik **Voorproef** om te bekijken hoe de vorm voor andere gebruikers zal tonen wanneer zij het zullen gebruiken om een nieuw verslag voor te leggen.
1. Ga aan [&#x200B; de details van de Configuratie van de Opstelling &#x200B;](#set-up-configuration-details) verder als u meer details voor de vorm wilt vormen, of naar [&#x200B; Volledige creatie van de verzoekvorm &#x200B;](#complete-request-form-creation) gaan.

#### Configuratiegegevens instellen

Op het tabblad Configuratie kunt u het goedkeuringsproces instellen en configureren wanneer een aanvraag die op basis van dit formulier is gemaakt, wordt gemarkeerd als Voltooid.

1. Beginnen creërend of het uitgeven van een verzoekvorm, zoals die in de sectie [&#x200B; wordt beschreven Begin creërend een verzoekvorm &#x200B;](#begin-creating-a-request-form).

   Het aanvraagformulier voor het geselecteerde recordtype wordt geopend op het tabblad Formulier.
1. (Facultatief) opstelling om het even welke vormdetails, zoals die in [&#x200B; worden beschreven de details van de Vorm van de Opstelling &#x200B;](#set-up-form-details).

1. (Facultatief) klik het **lusje van de Configuratie**, dan voeg minstens één gebruiker of team aan het **Approvers** gebied toe om nieuwe verzoeken voor deze verslagvorm goed te keuren.

   ![&#x200B; het lusje van de Configuratie &#x200B;](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Wanneer u een aanvraagformulier aan fiatteurs koppelt, moet elk nieuw verzoek eerst worden goedgekeurd door alle fiatteurs voordat een nieuwe record wordt gegenereerd.
   * U kunt een of meer fiatteurs toevoegen aan een aanvraagformulier.
   * Als ten minste één fiatteur het verzoek afwijst, wordt het verzoek afgewezen en wordt de record niet gemaakt.
   * Elke fiatteur moet een beslissing nemen voordat een verzoek wordt goedgekeurd of afgewezen.
   * Als een team als fiatteur wordt geplaatst, wordt slechts één besluit vereist van het team.

     Voor meer informatie over het toevoegen van goedkeuringen aan aanvraagvormen, zie [&#x200B; goedkeuring aan een verzoekvorm &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md) toevoegen.

1. (Voorwaardelijk) als u het verslag wilt worden gecreeerd nadat om het even welke fiatteurs het heeft goedgekeurd, controleer **slechts één besluit wordt vereist** checkbox.

1. Selecteer of u een aanvraag die op basis van dit formulier is gemaakt, als volledig wilt markeren wanneer het aangevraagde object wordt gemaakt of wanneer het gevraagde object is voltooid.
1. (Voorwaardelijk) Als u ervoor hebt gekozen dat de aanvraag wordt gemarkeerd als voltooid wanneer het gewenste object is voltooid, selecteert u het veld en de waarde die aangeven wanneer het object is voltooid. U kunt bijvoorbeeld de status van het veld en de waarde Voltooien selecteren om de aanvraag te voltooien wanneer de status van het gemaakte object is ingesteld op Voltooien.
1. Ga aan <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[&#x200B; Volledige creatie van de verzoekvorm &#x200B;](#complete-request-form-creation) verder.

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### Volledig aanvraagformulier maken

1. Creeer en opstelling de vorm zoals die in [&#x200B; wordt beschreven Begin creërend een verzoekvorm &#x200B;](#begin-creating-a-request-form) en [&#x200B; opstellingsdetails voor de verzoekvorm &#x200B;](#set-up-details-for-the-request-form) wordt beschreven.
1. (Facultatief) klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de naam van de vorm in de kopbal, dan klik **uitgeven** om de naam van de vorm bij te werken.

1. Klik **publiceren** om de vorm te publiceren en een unieke verbinding voor het te verkrijgen.

   De volgende dingen doen zich voor:

   * De **Publish** knoop wordt verwijderd.
   * De **unpublish** knoop wordt toegevoegd aan de vorm. Als u erop klikt, is het formulier niet toegankelijk.
   * A **de knoop van het Aandeel** wordt toegevoegd aan de vorm.
   * Het formulier wordt beschikbaar in het gedeelte Aanvragen van het menu Main in Workfront.

1. Klik **Aandeel** om de vorm met anderen te delen.

   Voor informatie over het delen van een verzoekvorm, zie [&#x200B; een sectie van de verzoekvorm &#x200B;](#share-a-request-form) in dit artikel delen
1. Klik op de pijl die naar links wijst links van de naam van het formulier in de koptekst om het formulier te sluiten.

   De **vorm van het Verzoek** lijstmening opent en de vorm wordt toegevoegd aan het.

## Bestaande aanvraagformulieren beheren


1. Klik op de werkruimte waar u aanvraagformulieren wilt beheren.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.

1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) aan het recht van de naam van het verslagtype in de paginakop, dan klik **leidt verzoekvormen**.

   Alle aanvraagformulieren die aan het recordtype zijn gekoppeld, worden in een tabelweergave weergegeven.

1. (Facultatief) Beweeg over de naam van een verzoekvorm in de lijstmening, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de vormnaam, en klik één van het volgende:

   * **geef vorm** uit: Klik dit om informatie over de vorm verder uit te geven.
   * **unpublish**: Klik dit om de vorm ongedaan te maken die het uit het gebied van Verzoeken in Workfront verwijdert.
   * **Aandeel**: Klik dit om te wijzigen wie toegang tot de vorm heeft.
   * **verbinding van het Exemplaar**: Klik dit om snel de verbinding van de verzoekvorm te kopiëren zonder de vorm te openen.
   * **Schrapping**: Klik dit om de vorm te schrappen. Alle aanvragen en records die met het formulier zijn toegevoegd, worden niet verwijderd. Het formulier kan niet worden hersteld.

   ![&#x200B; Meer menu op verzoekvorm van de lijst van de verzoekvormen &#x200B;](assets/more-menu-on-request-form-from-request-forms-list.png)

1. Klik op de pijl die naar links wijst links van **Request-formulieren** in de header om de aanvraagformuliertabel te sluiten.

   De pagina met recordtypen wordt geopend.
1. (Facultatief en voorwaardelijk) klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) aan het recht van de naam van het verslagtype in de kopbal, dan doe één van het volgende:

   1. Klik **de verzoekvorm van de Update** om het even welke veranderingen in de verzoekvorm aan te brengen, dan klik een verzoekvorm om het te openen en uit te geven.
   1. Klik **verbinding van het Exemplaar om vorm** te verzoeken om de verbinding met de vorm met anderen te delen.

1. (Facultatief) ga naar het **gebied van Verzoeken** in Workfront en vind de gedeelde vorm om een verzoek voor te leggen. Voor informatie, zie [&#x200B; de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

## Een aanvraagformulier delen

1. Creeer een verzoekvorm zoals die in [&#x200B; wordt beschreven creeer een verzoekvorm voor een verslagtype &#x200B;](#create-a-request-form-for-a-record-type) sectie in dit artikel.
1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de naam van de verzoekvorm op de pagina van het verslagtype.
1. Klik **Aandeel** om de vorm met anderen te delen.

1. Om de vorm intern te delen, selecteer het **Interne delende** lusje, onderzoek naar de naam van een gebruiker, team, baanrol, groep, of bedrijf in de **toegang van de Verlening om dit vorm** gebied voor te leggen, dan het te selecteren wanneer het in de lijst verschijnt. De **voorlegt** toestemming wordt geselecteerd door gebrek voor elke entiteit.

   ![&#x200B; doos van het Aandeel voor aanvraagvorm &#x200B;](assets/share-box-for-request-form.png)

1. (Facultatief) klik het drop-down menu na de naam van een entiteit, dan klik **verwijderen** om hen uit de lijst te verwijderen en ophouden delend de vorm met hen.

   >[!NOTE]
   >
   >Naast teams, groepen, bedrijven, en baanrollen, kunt u slechts met gebruikers delen die aan Adobe Admin Console zijn toegevoegd. U kunt geen gebruikers met alleen Workfront toevoegen. Voor informatie, zie [&#x200B; gebruikers in Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.

1. In **die verzoeken door deze vorm** sectie kan voorleggen, selecteer van de volgende opties om erop te wijzen welke types van gebruikers tot deze vorm kunnen toegang hebben:

   * Alleen uitgenodigde personen hebben toegang
   * Iedereen met weergave of hogere toegang tot de werkruimte
   * Iedereen met een hogere of hogere toegang tot de werkruimte
1. (Facultatief) klik **verbinding van het Exemplaar** om de verbinding met de vorm met mensen te delen die toegang hebben om dit te doen. De koppeling wordt naar het klembord gekopieerd.
1. Om de vorm openbaar te delen, selecteer het **Openbare delen** lusje, dan laat **openbare verbinding** plaatsen toe creëren.

   ![&#x200B; Openbaar het delen voor verzoekvorm &#x200B;](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* Wanneer u **toelaat creeer openbare verbinding** plaatsen, kan iedereen tot de vorm toegang hebben en een nieuw verslag voorleggen, zelfs mensen buiten uw organisatie die geen rekening van Workfront hebben.
   >
   >* Een formulier dat de volgende veldtypen bevat, kan niet openbaar worden gedeeld:
   >
   >     * Workfront- of AEM Assets-verbindingen
   >     * Mensen
   >

1. Kies de vervaldatum van de a **Verbinding**.

   U kunt toekomstige datums selecteren binnen 180 dagen vanaf de huidige datum.

   >[!TIP]
   >
   >Nadat de datum voor delen is verlopen, is het aanvraagformulier niet meer beschikbaar in het gedeelte Aanvragen van Workfront en zijn de koppelingen die met andere gebruikers worden gedeeld, niet meer toegankelijk.

   Personen ontvangen een fout nadat de koppeling is verlopen en u moet de datum van de koppeling bijwerken en een nieuwe koppeling genereren om te delen voordat ze het formulier weer kunnen openen.


1. (Facultatief en voorwaardelijk) klik **sparen** om het delen details voor de vorm te bewaren.
1. (Voorwaardelijk) als de vorm eerder werd bewaard, klik **verbinding van het Exemplaar**.

   De opties voor het delen van formulieren worden opgeslagen en de koppeling wordt naar het klembord gekopieerd. U kunt deze nu delen met anderen.

   Voor informatie over het creëren van verslagen die een verbinding aan een verzoekvorm gebruiken, zie [&#x200B; verzoeken van de Planning van Adobe Workfront voorleggen &#x200B;](/help/quicksilver/planning/requests/submit-requests.md).

1. Klik **sparen** in de laag-juiste hoek van het **3&rbrace; lusje van de Vorm &lbrace;om de vorm te bewaren.**
