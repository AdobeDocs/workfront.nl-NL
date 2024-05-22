---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Workfront-modules
description: Met de Adobe Workfront Fusion Adobe Workfront-connector kunt u uw processen in Workfront automatiseren. Als u een Workfront Fusion for Work Automation and Integration-licentie hebt, kunt u deze ook gebruiken om verbinding te maken met apps en services van derden.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 5803d21b0f606ad5beb138869a50d355d3273d4a
workflow-type: tm+mt
source-wordcount: '5784'
ht-degree: 0%

---

# [!DNL Adobe Workfront] modules

U kunt de [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] -aansluiting om uw processen te automatiseren binnen [!DNL Workfront]. Als u een [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] -licentie kunt u deze ook gebruiken om verbinding te maken met apps en services van derden.

De [!DNL Workfront] -connector telt niet mee voor het aantal actieve apps dat beschikbaar is voor uw organisatie. Alle scenario&#39;s, zelfs als zij slechts de [!DNL Workfront] , telt u niet mee voor het totale aantal scenario&#39;s van uw organisatie.

Ga voor meer informatie over de beschikbare apps en scenario&#39;s van uw organisatie naar [Organisaties](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organisaties en teams](../../workfront-fusion/organizations/organizations-and-teams.md).

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]

De [!DNL Workfront] -connector gebruikt OAuth 2.0 om verbinding te maken met [!DNL Workfront].

U kunt een verbinding maken met uw [!DNL Workfront] rechtstreeks vanuit een [!DNL Workfront Fusion] -module.

1. Klik in een willekeurige Adobe Workfront-module op **Toevoegen** naast het veld Verbinding.
1. Vul de volgende velden in:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Voer een naam in voor de nieuwe verbinding.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Selecteer of u verbinding maakt met een productieomgeving of niet.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Voer uw [!DNL Workfront] Client-id. Dit is te vinden in het gebied van Toepassingen OAuth2 van het gebied van de Opstelling in Workfront. Open de specifieke toepassing waarmee u verbinding maakt om de client-id weer te geven.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Workfront] Client-id. Dit is te vinden in het gebied van Toepassingen OAuth2 van het gebied van de Opstelling in Workfront. Open de specifieke toepassing waarmee u verbinding maakt om de client-id weer te geven.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>Dit kan de standaardwaarde blijven, of u kunt de URL van uw Workfront-instantie invoeren, gevolgd door <code>/integrations/oauth2</code>. <p>Voorbeeld: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Host prefix]</td>
        <td>In de meeste gevallen moet deze waarde <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Als u geen SAML login knoop ziet, heeft uw organisatie geen Enige Sign-On (SSO) toegelaten. U kunt zich aanmelden met uw gebruikersnaam en wachtwoord.
>   
>   Voor meer informatie over SSO, zie [Overzicht van Single Sign-On in [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* OAuth 2.0 verbindingen aan [!DNL Workfront] API is niet langer afhankelijk van API-sleutels.

## [!DNL Workfront] modules en hun velden

Wanneer u [!DNL Workfront] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Workfront] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>Als de meest actuele velden in een Workfront-module niet worden weergegeven, kan dit worden veroorzaakt door cacheproblemen. Wacht een uur en probeer het opnieuw.

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Triggers

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Watch Events]**

Deze triggermodule voert in real-time een scenario uit wanneer objecten van een specifiek type worden toegevoegd, bijgewerkt of verwijderd in Workfront

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

1. Klikken **[!UICONTROL Add]** aan de rechterzijde **Webhaak** doos.

1. Vorm webhaak in de **[!UICONTROL Add a hook]** weergegeven.

   Als u deze module configureert, worden de volgende velden weergegeven.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optioneel) Typ een nieuwe naam voor de webhaak</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Selecteer het type van [!DNL Workfront] neem op dat u de module wilt letten.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Selecteer of u naar het oude of het nieuwe frame wilt kijken.<ul><li><p><b>[!UICONTROL New state]</b></p><p>Een scenario activeren wanneer de record wordt gewijzigd <b>tot</b> een bepaalde waarde.</p><p>Als de status bijvoorbeeld is ingesteld op [!UICONTROL New State] en het filter is ingesteld op [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], activeert de webhaak een scenario als de [!UICONTROL Status] wijzigingen in [!UICONTROL In Progress], ongeacht wat de status daarvoor was. </p></li><li><p><b>[!UICONTROL Old state]</b></p><p>Een scenario activeren wanneer de record wordt gewijzigd <b>van</b> een bepaalde waarde.</p><p>Als de status bijvoorbeeld is ingesteld op [!UICONTROL Old State] en het filter is ingesteld op [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], activeert de webhaak een scenario wanneer een [!UICONTROL Status] dat momenteel [!UICONTROL In Progress] wijzigingen in een andere status. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>U kunt filters instellen om alleen te controleren op records die voldoen aan de criteria die u selecteert.</p> <p>Voer voor elk filter het veld in dat door het filter moet worden geëvalueerd, de operator en de waarde die door het filter moet worden toegestaan. U kunt meer dan één filter gebruiken door EN regels toe te voegen.</p> <p>Opmerking: u kunt filters niet bewerken in bestaande [!DNL Workfront] webhaken. Verschillende filters instellen voor [!DNL Workfront] -gebeurtenisabonnementen, verwijder de huidige webhaak en maak een nieuwe.</p> <p>Zie voor meer informatie over gebeurtenisfilters <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Abonnementsfilters voor gebeurtenissen in het dialoogvenster [!DNL Workfront] &gt; [!UICONTROL Watch Events] modules</a> in dit artikel.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclusief gebeurtenissen die in dit verband worden gemaakt</td> 
      <td>Schakel deze optie in om gebeurtenissen uit te sluiten die zijn gemaakt of bijgewerkt met dezelfde connector die deze triggermodule gebruikt. Dit kan situaties verhinderen waar een scenario zich zou teweegbrengen, veroorzakend het om in een eindeloze lijn te herhalen.<p><b>OPMERKING</b>Deze optie is niet opgenomen in het recordtype Toewijzing.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Kies of u op het scenario wilt letten <strong>[!UICONTROL New Records Only]</strong>, <strong>[!UICONTROL Updated Records Only]</strong>, <strong>[!UICONTROL New and Updated Records]</strong>, of <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Opmerking: als u <strong>[!UICONTROL New and Updated Records]</strong>Wanneer u de webhaak maakt, worden er twee gebeurtenisabonnementen gemaakt (voor hetzelfde webhadres).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Nadat WebHaak wordt gecreeerd, kunt u het adres van het eindpunt bekijken dat de gebeurtenissen worden verzonden naar.

Zie de sectie voor meer informatie [Voorbeelden van gebeurtenistaken](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) in de [!DNL Workfront] Help-artikel [API voor abonnementen voor gebeurtenissen](../../wf-api/general/event-subs-api.md).

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Watch Field]**

Deze triggermodule voert een scenario uit wanneer een veld dat u opgeeft, wordt bijgewerkt. De module retourneert zowel de oude als de nieuwe waarde van het veld dat u opgeeft. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] neem op dat u de module wilt letten.</p> <p>Selecteer bijvoorbeeld [!UICONTROL Task] als u wilt beginnen uitvoerend het scenario telkens als een verslaggebied in een taak wordt bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Selecteer het gebied dat u de module voor updates wilt letten. Deze velden geven de velden weer die uw [!DNL Workfront] de beheerder heeft opstelling voor het volgen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Watch Record]**

Deze triggermodule voert een scenario uit wanneer objecten van een specifiek type worden toegevoegd, bijgewerkt of beide. De module retourneert alle standaardvelden die zijn gekoppeld aan de record of records, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen. In de uitvoer geeft de module aan of elke record nieuw of bijgewerkt is.

Records die in de opgegeven periode zijn toegevoegd en bijgewerkt, worden geretourneerd als nieuwe records.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Kies of u op het scenario wilt letten <strong>[!UICONTROL New Records Only]</strong>, <strong>[!UICONTROL Updated Records Only]</strong>, of <strong>[!UICONTROL New and Updated Records]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(Wordt weergegeven nadat u een <strong>Filter</strong>.) Selecteer het type van [!DNL Workfront] neem op dat u de module wilt letten.</p> <p>Als u bijvoorbeeld elke keer dat een nieuw project wordt gemaakt het scenario wilt starten, selecteert u [!UICONTROL Project]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optional Filter]</td> 
   <td> <p>(Geavanceerd) Typ een API-codetekenreeks om aanvullende parameters of code te definiëren waarmee uw criteria worden verfijnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++


### Handelingen

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Convert object]**

Deze actiemodule maakt een van de volgende omzettingen:

* Probleem converteren naar project
* Probleem converteren naar taak
* Taak omzetten in project

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Object type]</td> 
   <td> <p>Selecteer het type object dat u wilt omzetten. Dit is het type dat het object vóór de conversie heeft.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convert to]</td> 
   <td>Selecteer het object waarnaar u het wilt omzetten. Dit is het type dat het object na de conversie heeft.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL <Object> ID]</td> 
   <td> <p>Voer de id van het object in. </p> <p>Opmerking: wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Template ID]</td> 
   <td> <p>Als u in een project omzet, selecteer identiteitskaart van het Malplaatje die u voor het project wilt gebruiken.</p> <p>Opmerking: wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom forms]</td> 
   <td>Selecteer de aangepaste formulieren die u aan het nieuwe geconverteerde object wilt toevoegen en voer vervolgens waarden in voor de velden van het aangepaste formulier.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Options]</td> 
   <td> <p>Schakel de gewenste opties in wanneer u het object omzet. Welke opties beschikbaar zijn, is afhankelijk van het object waarnaar u converteert of van het object.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copy native fields]</td> 
   <td> <p>Schakel deze optie in om native velden van het oorspronkelijke object naar het nieuwe object te kopiëren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copy custom forms]</td> 
   <td> <p>Schakel deze optie in om native velden van het oorspronkelijke object naar het nieuwe object te kopiëren.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a record (attaching custom forms)]**

Deze actiemodule maakt een object, zoals een project, taak of uitgave in [!DNL Workfront]en kunt u een aangepast formulier toevoegen aan het nieuwe object. In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

U kunt deze module bijvoorbeeld gebruiken om een taak te maken in [!DNL Workfront] wanneer een client een nieuwe rij toevoegt aan een [!DNL Google Sheets] lijst van taken die moeten worden uitgevoerd.

Als u deze module configureert, worden de volgende velden weergegeven.

Zorg ervoor dat u het minimale aantal invoervelden opgeeft. Als u bijvoorbeeld een uitgave wilt maken, moet u een geldige bovenliggende project-id opgeven in het veld Project-id om aan te geven waar de uitgave in Workfront moet wonen. U kunt het toewijzingspaneel gebruiken om deze informatie van een andere module in uw scenario in kaart te brengen, of u kunt het manueel ingaan door in de naam te typen en dan het van de lijst te selecteren.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] record die u met de module wilt maken.</p> <p>Als u bijvoorbeeld een project wilt maken, selecteert u [!UICONTROL Project] van dropdown lijst en zorg dan ervoor dat u toegang tot gegevens (van vorige modules in het scenario) hebt die het project zullen bevolken.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Selecteer de velden die u beschikbaar wilt maken voor gegevensinvoer. Dit staat u toe om deze gebieden te gebruiken zonder het moeten door degenen scrollen u niet nodig hebt.</p> <p>Voor velden in aangepaste formulieren gebruikt u de opdracht <b>[!UICONTROL Attach Custom Form]</b> veld.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Attach Custom Form]</td> 
   <td>Selecteer de aangepaste formulieren die u aan het nieuwe object wilt toevoegen en voer vervolgens waarden voor die velden in.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.
>* Wanneer u de tekst voor een aangepast veld of een [!UICONTROL Note] object (opmerking of antwoord), kunt u HTML-tags gebruiken in het dialoogvenster [!UICONTROL Note Text] veld voor het maken van RTF-tekst, zoals vette of cursieve tekst.
>
>  Voor meer informatie over tekst met opmaak in updates raadpleegt u [Een update toevoegen aan een werkitem](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Create Record]**

Deze actiemodule maakt een object, zoals een project, taak of uitgave in Workfront. In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

U kunt deze module bijvoorbeeld gebruiken om een taak te maken in [!DNL Workfront] wanneer een client een nieuwe rij toevoegt in een lijst met Google-werkbladen die moet worden uitgevoerd.

Als u deze module configureert, worden de volgende velden weergegeven.

Zorg ervoor dat u het minimale aantal invoervelden opgeeft. Als u bijvoorbeeld een uitgave wilt maken, moet u een geldige bovenliggende project-id opgeven in het veld Project-id om aan te geven waar de uitgave in Workfront moet wonen. U kunt het toewijzingspaneel gebruiken om deze informatie van een andere module in uw scenario in kaart te brengen, of u kunt het manueel ingaan door in de naam te typen en dan het van de lijst te selecteren.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] record die u met de module wilt maken.</p> <p>Als u bijvoorbeeld een project wilt maken, selecteert u [!UICONTROL Project] van dropdown lijst en zorg dan ervoor dat u toegang tot gegevens (van vorige modules in het scenario) hebt die het project zullen bevolken.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td>Selecteer de velden die u beschikbaar wilt maken voor gegevensinvoer. Dit staat u toe om deze gebieden te gebruiken zonder het moeten door degenen scrollen u niet nodig hebt.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.
>* Wanneer u de tekst voor een aangepast veld of een [!UICONTROL Note] object (opmerking of antwoord), kunt u HTML-tags gebruiken in het dialoogvenster [!UICONTROL Note Text] veld voor het maken van RTF-tekst, zoals vette of cursieve tekst.
>
>  Voor meer informatie over tekst met opmaak in updates raadpleegt u [Een update toevoegen aan een werkitem](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Custom API Call]**

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Workfront] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Workfront] modules.

De module retourneert de volgende informatie:

* **[!UICONTROL Status Code]** (getal): Dit geeft aan of uw HTTP-aanvraag is geslaagd of mislukt. Dit zijn standaardcodes die u kunt opzoeken op internet.
* **[!UICONTROL Headers]** (object): een gedetailleerdere context voor de respons-/statuscode die geen betrekking heeft op de hoofdtekst van de uitvoer. Niet alle kopteksten in een antwoordkoptekst zijn reactiekoppen. Sommige koppen zijn daarom niet altijd even handig.

  De antwoordheaders zijn afhankelijk van de HTTP-aanvraag die u hebt gekozen bij het configureren van de module.

* **[!UICONTROL Body]** (object): afhankelijk van de HTTP-aanvraag die u hebt gekozen bij het configureren van de module, ontvangt u mogelijk gegevens terug. Deze gegevens, zoals de gegevens van een verzoek om GET, bevinden zich in dit object.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Een pad invoeren ten opzichte van<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Selecteer de versie van de [!DNL Workfront] API die u de module wilt gebruiken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object. Dit bepaalt het inhoudstype van het verzoek.</p> <p>Bijvoorbeeld:<code> {"Content-type":"application/json"}</code></p> <p>Nota: Als u fouten krijgt en het moeilijk is om hun oorsprong te bepalen, denk na wijzigend kopballen die op [!DNL Workfront] documentatie. Als uw Aangepaste API-oproep een HTTP-aanvraagfout van 422 retourneert, probeert u een <code>"Content-Type":"text/plain"</code> header.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> <p>Tip: We raden u aan informatie via de JSON-hoofdtekst te verzenden in plaats van als queryparameters.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Delete Record]**

Met deze actiemodule verwijdert u een object, zoals een project, taak of uitgave in Workfront.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Force delete]</td> 
   <td>Schakel deze optie in om ervoor te zorgen dat de record wordt verwijderd, zelfs als de [!DNL Workfront] De gebruikersinterface zou om bevestiging van de verwijdering verzoeken.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Voer de unieke [!DNL Workfront] Id van de record die u wilt verwijderen uit de module.</p> <p>Als u de id wilt ophalen, opent u de [!DNL Workfront] -object in uw browser en kopieer de tekst aan het einde van de URL na "ID=." Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Selecteer het type van [!DNL Workfront] record die u wilt verwijderen.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Wij adviseren de volgende scenario configuratie om de mogelijkheid te vermijden dat verslagen niet wegens asynchrone verrichtingen worden geschrapt.
>
>1. Verwijder de record synchroon.
>1. Voeg foutafhandeling toe aan de module Record verwijderen om de fout te negeren die wordt veroorzaakt door de 40 tweede time-out.


+++

+++ **[!UICONTROL Download Document]**

Deze actiemodule downloadt een document uit Workfront.

U geeft de id van de record op.

De module retourneert de inhoud, de bestandsnaam, de bestandsextensie en de bestandsgrootte van het document. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document ID]</td> 
   <td> <p>De kaart of gaat manueel het unieke in [!DNL Workfront] Id van het document dat u de module wilt downloaden.</p> <p>Als u de id wilt ophalen, opent u de [!DNL Workfront] -object in uw browser en kopieer de tekst aan het einde van de URL na "ID=." Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Misc Action]**

Met deze actiemodule kunt u handelingen uitvoeren met de API.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] record waarmee de module moet communiceren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Selecteer de actie u de module wilt uitvoeren.</p> <p>Afhankelijk van de [!UICONTROL Record Type] en [!UICONTROL Action] kiest u. Voor sommige combinaties van deze twee instellingen is mogelijk alleen een record-id vereist, terwijl voor andere (zoals Project voor de <strong>[!UICONTROL Record Type]</strong> en [!UICONTROL Attach Template] voor de <strong>[!UICONTROL Action]</strong>) aanvullende informatie vereist (zoals een object-id en een sjabloon-id).</p> <p>Zie voor meer informatie over afzonderlijke velden de <a href="http://developer.workfront.com/">Workfront-documentatie voor ontwikkelaars</a>. <p><strong>Opmerking</strong>: De site met ontwikkelaarsdocumentatie bevat alleen informatie via API-versie 14, maar bevat nog steeds waardevolle informatie voor API-aanroepen. </p> 
    <ol> 
     <li value="1"> <p>Selecteer het recordtype in de linkernavigatie op het tabblad [!DNL Workfront] pagina met ontwikkelaarsdocumentatie. De volgende typen hebben hun eigen pagina's:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projects]</p> </li> 
       <li> <p>[!UICONTROL Tasks]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Users]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>Voor alle andere recordtypen selecteert u <b>[!UICONTROL Other objects and endpoints]</b>en zoek het recordtype op de alfabetische gesorteerde pagina's.</p> </li> 
     <li value="2"> <p>Zoek op de pagina van het juiste recordtype naar de handeling (Ctrl-F of Cmd-F).</p> </li> 
     <li value="3"> <p>Beschrijvingen weergeven voor beschikbare velden onder de geselecteerde handeling.</p> </li> 
    </ol> <p>Opmerking:  <p>Als u een proefdruk maakt via het dialoogvenster [!DNL Workfront] [!UICONTROL Misc Action] kunt u het beste een proefdruk maken zonder geavanceerde opties en de proefdruk vervolgens bijwerken met de opdracht [!DNL Workfront Proof] SOAP API.</p> <p>Voor meer informatie over het maken van een proefdruk met de [!DNL Workfront] API (die door deze module wordt gebruikt), zie <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Geavanceerde opties voor proefdrukken toevoegen bij het maken van een proefdruk via het dialoogvenster [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL Workfront] Id van de record waarmee de module moet communiceren.<p>Als u de id wilt ophalen, opent u de [!DNL Workfront] -object in uw browser en kopieer de tekst aan het einde van de URL na "ID=." Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Read a Record]**

Deze actiemodule haalt gegevens op uit één record.

U geeft de id van de record op. U kunt ook opgeven welke verwante records u in de module wilt lezen.

Bijvoorbeeld, als het verslag dat de module leest een project is, kunt u specificeren dat u de taken van het project wilt lezen.

De module retourneert een array met gegevens uit de standaardvelden voor de uitvoer die u hebt opgegeven.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>

<td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>Kies de optie [!DNL Workfront] objecttype dat de module moet lezen.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>

<td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL References]</td>
   <td>Selecteer de verwijzingsvelden die u in de uitvoer wilt opnemen.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Collections]</td>
   <td>Selecteer de verwijzingsvelden die u in de uitvoer wilt opnemen.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Voer de unieke [!DNL Workfront] Id van de record die de module moet lezen.</p> <p>Als u de id wilt ophalen, opent u de [!DNL Workfront] -object in uw browser en kopieer de tekst aan het einde van de URL na "ID=." Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Update Record]**

Deze actiemodule werkt een voorwerp, zoals een project, een taak, of een kwestie bij. In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module.

U geeft de id van de record op.

De module retourneert de id van het object en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Voer de unieke [!DNL Workfront] Id van de record die de module moet bijwerken.</p> <p>Als u de id wilt ophalen, opent u de [!DNL Workfront] -object in uw browser en kopieer de tekst aan het einde van de URL na "ID=." Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] record dat de module moet worden bijgewerkt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selecteer de velden die u beschikbaar wilt maken voor gegevensinvoer. Dit staat u toe om deze gebieden te gebruiken zonder het moeten door degenen scrollen u niet nodig hebt.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.
>* Wanneer u de tekst voor een aangepast veld of een [!UICONTROL Note] object (opmerking of antwoord), kunt u HTML-tags gebruiken in het dialoogvenster [!UICONTROL Note Text] veld voor het maken van RTF-tekst, zoals vette of cursieve tekst.
>
>  Voor meer informatie over tekst met opmaak in updates raadpleegt u [Een update toevoegen aan een werkitem](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Upload Document]**

Deze actiemodule uploadt een document naar een [!DNL Workfront] object, zoals een project, taak of uitgave.

U geeft de locatie voor het document, het bestand dat u wilt uploaden en een optionele nieuwe naam voor het bestand op.

De module retourneert de id van het document en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Voer de unieke [!DNL Workfront] Id van de record waarnaar u het document wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Selecteer het type van [!DNL Workfront] registreer waar u de module het document wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

### Zoekopdrachten

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Read Related Records]**

Deze zoekmodule leest records die overeenkomen met de zoekquery die u opgeeft, in een bepaald bovenliggend object.

U geeft op welke velden u wilt opnemen in de uitvoer. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type bovenliggende record (Workfront-object) waarvan u de gekoppelde records wilt lezen.</p> <p>Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module</a> in dit artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>Voer de id in van de bovenliggende record waarvan u de gekoppelde records wilt lezen of wijs deze toe.</p> <p>Als u de id wilt ophalen, opent u de [!DNL Workfront] -object in uw browser en kopieer de tekst aan het einde van de URL na "ID=." Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Selecteer of wijs het type van kindverslag toe dat u de module wilt lezen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search]**

Deze zoekmodule zoekt naar records in een object in [!DNL Workfront] die overeenkomen met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] record waarnaar u wilt zoeken in de module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Selecteer een optie om op te geven of u wilt dat de module het eerste resultaat ophaalt dat overeenkomt met uw zoekcriteria of dat alle resultaten overeenkomen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria fields]</td> 
   <td> <p>Selecteer de velden die u voor de zoekcriteria wilt gebruiken. Deze velden zijn dan beschikbaar in het vervolgkeuzemenu Zoekcriteria.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Voer het veld in waarnaar u wilt zoeken, de operator die u in de query wilt gebruiken en de waarde waarnaar u in het veld zoekt.</p> <p>Opmerking: niet gebruiken <code>username </code>in uw zoekcriteria. Inclusief <code>username </code>in een API-query naar [!DNL Workfront] logt de gebruiker in Workfront, en het onderzoek zal niet succesvol zijn.</p> <p>Opmerking: <code>In</code> en <code>NotIn</code>werken met arrays. De invoer moet een arrayindeling hebben.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>Selecteer de verwijzingsvelden die u in de zoekopdracht wilt opnemen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Selecteer de verzamelingen die u aan de zoekopdracht wilt toevoegen.</td> 
  </tr> 
 </tbody> 
</table>
++

+++ **[!UICONTROL Search (Legacy)]**

Deze zoekmodule zoekt naar records in een object in [!DNL Workfront] die overeenkomen met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Workfront] app voor [!DNL Workfront Fusion], zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Workfront] record waarnaar u wilt zoeken in de module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Selecteer een optie om op te geven of u wilt dat de module het eerste resultaat ophaalt dat overeenkomt met uw zoekcriteria of dat alle resultaten overeenkomen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Voer het veld in waarnaar u wilt zoeken, de operator die u in de query wilt gebruiken en de waarde waarnaar u in het veld zoekt.</p> <p>Opmerking: niet gebruiken <code>username </code>in uw zoekcriteria. Inclusief <code>username </code>in een API-query naar [!DNL Workfront] logt de gebruiker in Workfront, en het onderzoek zal niet succesvol zijn.</p> <p>Opmerking: <code>In</code> en <code>NotIn</code>werken met arrays. De invoer moet een arrayindeling hebben.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>Selecteer de verwijzingsvelden die u in de zoekopdracht wilt opnemen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Selecteer de verzamelingen die u aan de zoekopdracht wilt toevoegen.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst met de [!DNL Workfront] objecttypen waarvoor u deze module kunt gebruiken in [[!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] objecttypen beschikbaar voor elk [!DNL Workfront] module

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Objecttypen beschikbaar voor elk [!DNL Workfront] triggermodule**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Watch Record]</th> 
   <th>[!UICONTROL Watch Field]</th> 
   <th>[!UICONTROL Watch Events]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Goedkeuringsproces</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Toewijzing</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Basislijn</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Factureringsrecord </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Factureringsgraad</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bedrijf</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentmap</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documentaanvraag</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documentversie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Kosten</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Type uitgave</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groep</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uur</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Uurtype</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Probleem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteratie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Functie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dagboekinvoer</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mijlsteen</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mijlpad</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Opmerking</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Notititietag</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projectgebruiker</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Goedkeuring proefdrukken</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gereserveerde tijd* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapport</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risico</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type risico</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stap fiatteur</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taak</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sjabloon</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Sjabloontaak</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Bijwerken</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Objecttypen beschikbaar voor elk [!DNL Workfront] actiemodule**

>[!NOTE]
>
>De [!UICONTROL Download Document] module is niet in deze tabel opgenomen omdat [!DNL Workfront] objecttypen maken geen deel uit van de configuratie.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Create a record]</th> 
   <th>[!UICONTROL Update a record]</th> 
   <th>[!UICONTROL Delete a record]</th> 
   <th>[!UICONTROL Upload Document]</th> 
   <th>[!UICONTROL Read a record]</th> 
   <th>[!UICONTROL Custom API Call]</th> 
   <th>[!UICONTROL Misc Action]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Goedkeuringsproces</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Toewijzing</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Basislijn</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
   <tr> 
   <td>Factureringsrecord</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Factureringsgraad</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bedrijf</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentmap</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentversie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Wisselkoers</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Kosten</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Type uitgave</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Extern document</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Groep</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Uur</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uurtype</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Probleem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteratie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Functie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dagboekinvoer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Mijlsteen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mijlpad</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Opmerking</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Notititietag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projectgebruiker</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gereserveerde tijd* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risico</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type risico</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stap fiatteur</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taak</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sjabloon</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sjabloontaak</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tijdschema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Bijwerken</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Objecttypen beschikbaar voor elk [!DNL Workfront] zoekmodule**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Search]</th> 
   <th>[!UICONTROL Read Related Records]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Goedkeuringsproces</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Toewijzing</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Factureringsrecord</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Factureringsgraad</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bedrijf</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentmap</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentversie</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Kosten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type uitgave</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groep</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Uur</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uurtype</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Probleem</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteratie</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Functie</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dagboekinvoer</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mijlsteen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mijlpad</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Opmerking</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Notititietag</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projectgebruiker</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gereserveerde tijd* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risico</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type risico</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stap fiatteur</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taak</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sjabloon</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sjabloontaak</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gebruikersdelegatie</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Wij adviseren dat u tweemaal controleert om ervoor te zorgen dit werkt zoals u het zou verwachten.

+++

## Abonnementsfilters voor gebeurtenissen in het dialoogvenster [!DNL Workfront] > [!UICONTROL Watch Events] modules

>[!NOTE]
>
>We raden u aan om filters voor gebeurtenisabonnementen te gebruiken in uw [!UICONTROL Watch Events] modules.

De [!DNL Workfront] [!UICONTROL Watch Events] module activeert scenario&#39;s op basis van een webhaak die een gebeurtenisabonnement maakt in het dialoogvenster [!DNL Workfront] API. Het gebeurtenisabonnement is een gegevensset die bepaalt welke gebeurtenissen naar de webhaak worden verzonden. Als u bijvoorbeeld een [!UICONTROL Watch Events] -module die op problemen let, verzendt het gebeurtenisabonnement alleen gebeurtenissen die met problemen te maken hebben.

Door gebeurtenisabonnementfilters te gebruiken, kunnen Fusion-gebruikers gebeurtenisabonnementen maken die beter geschikt zijn voor hun gebruik. U kunt bijvoorbeeld een gebeurtenisabonnement instellen in het dialoogvenster [!DNL Workfront] API om alleen problemen te verzenden die zich in een specifiek project bevinden, zodat de [!UICONTROL Watch Events] de module zal slechts voor kwesties in dat project teweegbrengen. De mogelijkheid om smallere triggers te maken verbetert het ontwerp van scenario&#39;s door het aantal irrelevante triggers te verminderen.

Dit is anders dan het instellen van een filter in het dialoogvenster [!DNL Workfront Fusion] scenario. Zonder een gebeurtenisabonnementfilter ontvangt uw webhaak alle gebeurtenissen die betrekking hebben op het objecttype dat u selecteert. De meeste van deze gebeurtenissen zijn niet relevant voor het scenario en moeten worden uitgefilterd voordat het scenario kan worden voortgezet.

De volgende operatoren zijn beschikbaar in het filter Workfront > Watch-gebeurtenissen:

* Gelijk
* Niet gelijk
* Groter dan
* Minder dan
* Groter dan of gelijk aan
* Kleiner dan of gelijk aan
* Bevat
* Exists
   * Deze operator heeft geen waarde nodig en het waardeveld ontbreekt.
* Is niet bestaand
   * Deze operator heeft geen waarde nodig en het waardeveld ontbreekt.
* Gewijzigd
   * Deze operator heeft geen waarde nodig en het waardeveld ontbreekt.
   * Deze operator negeert het veld Frame.
   * Wanneer u `Changed`, selecteert u **Alleen bijgewerkte gebeurtenissen** in de **Oorsprong record** veld.

>[!IMPORTANT]
>
>U kunt filters in bestaande [!DNL Workfront] webhaken. Verschillende filters instellen voor [!DNL Workfront] -gebeurtenisabonnementen, verwijder de huidige webhaak en maak een nieuwe.

>[!INFO]
>
>**Voorbeeld:** Overweeg een scenario dat nieuwe kwesties verwerkt die aan een specifieke gebruiker, Ana worden toegewezen.
>
>### Gebeurtenissen filteren met behulp van een gebeurtenisabonnementfilter (aanbevolen)
>
>Met het gebeurtenisfilter kunt u de webhaak zo instellen dat het scenario wordt geactiveerd wanneer een uitgave aan Ana wordt toegewezen wanneer de uitgave wordt gemaakt. Ana heeft de gebruikersnaam b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Als 100 kwesties in een dag worden gecreeerd, maar slechts twee van hen worden toegewezen aan Ana, zou het scenario tweemaal uitvoeren.
>
>### Gebeurtenissen filteren in het scenario (niet aanbevolen)
>
>Als u gebeurtenissen wilt filteren zodat alleen uitgaven die aan Ana zijn toegewezen, worden verwerkt, kunt u een filter maken na het dialoogvenster [!UICONTROL Watch Events] -module.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Als er in een dag 100 problemen worden gemaakt, maar slechts twee ervan worden toegewezen aan Ana, wordt het scenario 100 keer uitgevoerd. 98 van de uitvoeringen zouden bij de filter ophouden, maar de trekkermodule verbruikt nog steeds gegevens en voert bewerkingen uit in alle uitvoeringen.

Zie voor meer informatie over gebeurtenisabonnementen [Veelgestelde vragen - Abonnementen voor gebeurtenissen](../../wf-api/general/event-subs-faq.md).

Voor meer informatie over webhooks raadpleegt u [Instant triggers (webhaken) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Zie voor meer informatie over filters in scenario&#39;s [Een filter toevoegen aan een scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

