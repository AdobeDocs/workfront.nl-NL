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
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '6299'
ht-degree: 0%

---

# [!DNL Adobe Workfront] modules

U kunt de [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] -connector gebruiken om uw processen binnen [!DNL Workfront] te automatiseren. Als u een [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] -licentie hebt, kunt u deze ook gebruiken om verbinding te maken met apps en services van derden.

De aansluiting van [!DNL Workfront] telt niet mee voor het aantal actieve apps dat beschikbaar is voor uw organisatie. Alle scenario&#39;s, zelfs als ze alleen de [!DNL Workfront] -app gebruiken, tellen niet mee voor het totale aantal scenario&#39;s van uw organisatie.

Voor meer informatie over beschikbare apps en scenario&#39;s van uw organisatie, zie [ Organisaties ](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion]  organisaties en teams ](../../workfront-fusion/organizations/organizations-and-teams.md).

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren. Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het abonnement [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL Workfront] met [!DNL Workfront Fusion]

De [!DNL Workfront] -connector gebruikt OAuth 2.0 om verbinding te maken met [!DNL Workfront] .

U kunt rechtstreeks vanuit een [!DNL Workfront Fusion] -module verbinding maken met uw [!DNL Workfront] -account.

1. In om het even welke module van Adobe Workfront, voegt de klik **naast het gebied van de Verbinding toe.**
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
        <td>Voer uw [!DNL Workfront] client-id in. Dit is te vinden in het gebied van Toepassingen OAuth2 van het gebied van de Opstelling in Workfront. Open de specifieke toepassing waarmee u verbinding maakt om de client-id weer te geven.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Workfront] client-id in. Dit is te vinden in het gebied van Toepassingen OAuth2 van het gebied van de Opstelling in Workfront. Open de specifieke toepassing waarmee u verbinding maakt om de client-id weer te geven.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>Dit kan de standaardwaarde blijven of u kunt de URL van uw Workfront-instantie invoeren, gevolgd door <code>/integrations/oauth2</code> . <p>Voorbeeld: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Host prefix]</td>
        <td>In de meeste gevallen moet deze waarde <code>origin</code> zijn.
      </tr>
    </tbody>
    </table>

1. Klik op **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Als u geen SAML login knoop ziet, heeft uw organisatie geen Enige Sign-On (SSO) toegelaten. U kunt zich aanmelden met uw gebruikersnaam en wachtwoord.
>   
>   Voor meer informatie over SSO, zie [ Overzicht van enig teken-binnen  [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* OAuth 2.0-verbindingen met de [!DNL Workfront] API vertrouwen niet langer op API-sleutels.
>* Als u een verbinding met een Workfront Sandbox-omgeving wilt maken, moet u in die omgeving een OAuth2-toepassing maken en vervolgens de client-id en het clientgeheim gebruiken die door die toepassing zijn gegenereerd in uw verbinding.
>
>   Voor instructies bij het creëren van een toepassing OAuth2 in Workfront, zie [ tot een toepassing OAuth2 gebruikend gebruikersgeloofsbrieven (de stroom van de code van de Vergunning) ](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) in artikel leiden toepassingen OAuth2 voor de integratie van Workfront.

## [!DNL Workfront] modules en hun velden

Wanneer u [!DNL Workfront] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL Workfront] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).


![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>* Als de meest actuele velden in een Workfront-module niet worden weergegeven, kan dit worden veroorzaakt door cacheproblemen. Wacht een uur en probeer het opnieuw.
>* HTTP 429 statuscodes van Adobe Workfront moeten geen deactivaties veroorzaken, maar in plaats daarvan een korte uitvoeringspauze in het scenario teweegbrengen.

* [ Trekkers ](#triggers)
* [ Acties ](#actions)
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

1. Klik **[!UICONTROL Add]** aan het recht van de **doos Webhaak**.

1. Configureer de webhaak in het vak **[!UICONTROL Add a hook]** dat wordt weergegeven.

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
      <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Selecteer het type [!DNL Workfront] record dat u in de module wilt bekijken.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Selecteer of u naar het oude of het nieuwe frame wilt kijken.<ul><li><p><b>[!UICONTROL New state]</b></p><p>Trigger een scenario wanneer het verslag <b> in </b> een bepaalde waarde verandert.</p><p>Als de status bijvoorbeeld is ingesteld op [!UICONTROL New State] en het filter is ingesteld op [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] , activeert de webhaak een scenario wanneer de [!UICONTROL Status] verandert in [!UICONTROL In Progress] , ongeacht wat de status daarvoor was. </p></li><li><p><b>[!UICONTROL Old state]</b></p><p>Trigger een scenario wanneer het verslag <b> van </b> een bepaalde waarde verandert.</p><p>Als de status bijvoorbeeld is ingesteld op [!UICONTROL Old State] en het filter is ingesteld op [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] , activeert de webhaak een scenario wanneer een [!UICONTROL Status] die momenteel [!UICONTROL In Progress] is, verandert in een andere status. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>U kunt filters instellen om alleen te controleren op records die voldoen aan de criteria die u selecteert.</p> <p>Voer voor elk filter het veld in dat door het filter moet worden geëvalueerd, de operator en de waarde die door het filter moet worden toegestaan. U kunt meer dan één filter gebruiken door EN regels toe te voegen.</p> <p>Opmerking: u kunt filters in bestaande [!DNL Workfront] -webhaken niet bewerken. Als u verschillende filters wilt instellen voor [!DNL Workfront] -gebeurtenisabonnementen, verwijdert u de huidige webhaak en maakt u een nieuwe.</p> <p>Voor meer informatie over gebeurtenisfilters, zie <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref"> de abonnementfilters van de Gebeurtenis in [!DNL Workfront] &gt; [!UICONTROL Watch Events] modules </a> in dit artikel.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclusief gebeurtenissen die in dit verband worden gemaakt</td> 
      <td>Schakel deze optie in om gebeurtenissen uit te sluiten die zijn gemaakt of bijgewerkt met dezelfde connector die deze triggermodule gebruikt. Dit kan situaties verhinderen waar een scenario zich zou teweegbrengen, veroorzakend het om in een eindeloze lijn te herhalen.<p><b> NOTA </b> het type van het het verslag van de Toewijzing omvat deze optie niet.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Kies of u het scenario wilt bekijken <strong>[!UICONTROL New Records Only]</strong>, <strong>[!UICONTROL Updated Records Only]</strong>, <strong>[!UICONTROL New and Updated Records]</strong> of <strong>[!DNL Deleted Records Only]</strong> .</p> <p>Opmerking: als u <strong>[!UICONTROL New and Updated Records]</strong> kiest, maakt het maken van de webhaak twee gebeurtenisabonnementen (voor hetzelfde adres van de webhaak).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Nadat WebHaak wordt gecreeerd, kunt u het adres van het eindpunt bekijken dat de gebeurtenissen worden verzonden naar.

Voor meer informatie, zie de sectie [ Voorbeelden van de Payloads van de Gebeurtenis ](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) in het [!DNL Workfront] artikel van de Hulp [ Abonnement API van de Gebeurtenis ](../../wf-api/general/event-subs-api.md).

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record dat u in de module wilt bekijken.</p> <p>Selecteer bijvoorbeeld [!UICONTROL Task] als u wilt beginnen met het uitvoeren van het scenario telkens wanneer een recordveld in een taak wordt bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Selecteer het gebied dat u de module voor updates wilt letten. In deze velden staan de velden die de [!DNL Workfront] -beheerder heeft ingesteld voor bijhouden.</td> 
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

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Kies of u het scenario wilt bekijken <strong>[!UICONTROL New Records Only]</strong>, <strong>[!UICONTROL Updated Records Only]</strong> of <strong>[!UICONTROL New and Updated Records]</strong> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(Vertoningen nadat u a <strong> Filter </strong> kiest.) Selecteer het type van [!DNL Workfront] verslag dat u de module wilt letten op.</p> <p>Als u bijvoorbeeld elke keer dat een nieuw project wordt gemaakt het scenario wilt starten, selecteert u [!UICONTROL Project]</p> </td> 
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

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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

>[!NOTE]
>
>Vanaf juli 2024 kunnen aangepaste formulieren worden opgenomen bij de conversie van een object.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
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

In deze actiemodule wordt een object gemaakt, zoals een project, taak of uitgave in [!DNL Workfront] , en kunt u een aangepast formulier aan het nieuwe object toevoegen. In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

U kunt deze module bijvoorbeeld gebruiken om een taak te maken in [!DNL Workfront] wanneer een client een nieuwe rij toevoegt in een [!DNL Google Sheets] -lijst met taken die moeten worden uitgevoerd.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record dat u met de module wilt maken.</p> <p>Als u bijvoorbeeld een project wilt maken, selecteert u [!UICONTROL Project] in de vervolgkeuzelijst en controleert u of u toegang hebt tot gegevens (van vorige modules in het scenario) die het project vullen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Selecteer de velden die u beschikbaar wilt maken voor gegevensinvoer. Dit staat u toe om deze gebieden te gebruiken zonder het moeten door degenen scrollen u niet nodig hebt.</p> <p>Gebruik het veld <b>[!UICONTROL Attach Custom Form]</b> voor velden in aangepaste formulieren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Attach Custom Form]</td> 
   <td>Selecteer de aangepaste formulieren die u aan het nieuwe object wilt toevoegen en voer vervolgens waarden voor die velden in.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

>[!NOTE]
>
>* Wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.
>* Wanneer u de tekst voor een aangepast veld of een [!UICONTROL Note] -object (Opmerking of Antwoord) invoert, kunt u HTML-tags in het [!UICONTROL Note Text] -veld gebruiken om RTF-tekst, zoals vette of cursieve tekst, te maken.
>
>  Voor meer informatie over rijke tekst in updates, zie [ een update aan een het werkpunt ](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [ werk van de Update ](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md) toevoegen.
>

+++

+++ **[!UICONTROL Create Record]**

Deze actiemodule maakt een object, zoals een project, taak of uitgave in Workfront. In de module kunt u selecteren welke velden van het object beschikbaar zijn in de module.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

U kunt deze module bijvoorbeeld gebruiken om een taak te maken in [!DNL Workfront] wanneer een client een nieuwe rij toevoegt in een lijst met taken in Google Sheets die moeten worden uitgevoerd.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record dat u met de module wilt maken.</p> <p>Als u bijvoorbeeld een project wilt maken, selecteert u [!UICONTROL Project] in de vervolgkeuzelijst en controleert u of u toegang hebt tot gegevens (van vorige modules in het scenario) die het project vullen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td>Selecteer de velden die u beschikbaar wilt maken voor gegevensinvoer. Dit staat u toe om deze gebieden te gebruiken zonder het moeten door degenen scrollen u niet nodig hebt.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

>[!NOTE]
>
>* Wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.
>* Wanneer u de tekst voor een aangepast veld of een [!UICONTROL Note] -object (Opmerking of Antwoord) invoert, kunt u HTML-tags in het [!UICONTROL Note Text] -veld gebruiken om RTF-tekst, zoals vette of cursieve tekst, te maken.
>
>  Voor meer informatie over rijke tekst in updates, zie [ een update aan een het werkpunt ](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [ werk van de Update ](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md) toevoegen.
>

+++

+++ **[!UICONTROL Custom API Call]**

Met deze actiemodule kunt u een aangepaste, geverifieerde aanroep van de [!DNL Workfront] API maken. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de andere [!DNL Workfront] -modules kan worden uitgevoerd.

De module retourneert de volgende informatie:

* **[!UICONTROL Status Code]** (nummer): Dit geeft aan of uw HTTP-aanvraag is geslaagd of mislukt. Dit zijn standaardcodes die u kunt opzoeken op internet.
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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Ga een weg met betrekking tot <code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code> in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Selecteer de versie van de [!DNL Workfront] API die u wilt gebruiken in de module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object. Dit bepaalt het inhoudstype van het verzoek.</p> <p>Bijvoorbeeld:<code> {"Content-type":"application/json"}</code></p> <p>Opmerking: als u fouten krijgt en het moeilijk is om de oorsprong ervan te bepalen, kunt u overwegen koppen te wijzigen op basis van de documentatie van [!DNL Workfront] . Wanneer uw Aangepaste API-aanroep een HTTP-aanvraagfout van 422 retourneert, probeert u een header <code>"Content-Type":"text/plain"</code> te gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> <p>Tip: We raden u aan informatie via de JSON-hoofdtekst te verzenden in plaats van als queryparameters.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Force delete]</td> 
   <td>Schakel deze optie in om ervoor te zorgen dat de record wordt verwijderd, zelfs als de gebruikersinterface van [!DNL Workfront] bevestiging van de verwijdering zou vragen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Voer de unieke [!DNL Workfront] -id in van de record die u wilt verwijderen.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Workfront] in uw browser en kopieert u de tekst aan het einde van de URL na "ID=". Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i> 5e43010c03286a2a555e1d0a75d6a86e </i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Selecteer het type [!DNL Workfront] -record dat u wilt verwijderen door de module.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document ID]</td> 
   <td> <p>Wijs of voer handmatig de unieke [!DNL Workfront] id in van het document dat u wilt downloaden met de module.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Workfront] in uw browser en kopieert u de tekst aan het einde van de URL na "ID=". Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i> 5e43010c03286a2a555e1d0a75d6a86e </i></p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

+++

+++ **[!UICONTROL Misc Action]**

Met deze actiemodule kunt u handelingen uitvoeren met de API.

>[!NOTE]
>
>Vanaf juli 2024 bevat de handeling `convertToProject` het veld `copyCategories` . Als u deze instelt op `TRUE` , worden aangepaste formulieren opgenomen in het project waarnaar de uitgave wordt geconverteerd.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record waarmee u wilt communiceren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Selecteer de actie u de module wilt uitvoeren.</p> <p>Afhankelijk van de opties [!UICONTROL Record Type] en [!UICONTROL Action] die u kiest, moet u mogelijk extra velden invullen. Sommige combinaties van deze twee instellingen vereisen mogelijk alleen een record-id, terwijl andere (zoals Project voor de <strong>[!UICONTROL Record Type]</strong> en [!UICONTROL Attach Template] for the <strong>[!UICONTROL Action]</strong> ) aanvullende informatie vereisen (zoals een object-id en een sjabloon-id).</p><p>Voor opties beschikbaar aan sommige acties, zie <a href="#misc-action-options" class="MCXref xref"> Diverse actieopties </a> in dit artikel.</p> <p>Voor details over individuele gebieden, zie de <a href="http://developer.workfront.com/"> de ontwikkelaarsdocumentatie van Workfront </a>. <p><strong> Nota </strong>: De plaats van de ontwikkelaardocumentatie omvat informatie slechts door API versie 14, maar bevat nog waardevolle informatie voor API vraag. </p> 
    <ol> 
     <li value="1"> <p>Selecteer het recordtype in de linkernavigatie op de documentatiepagina voor ontwikkelaars van [!DNL Workfront] . De volgende typen hebben hun eigen pagina's:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projects]</p> </li> 
       <li> <p>[!UICONTROL Tasks]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Users]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>Selecteer <b>[!UICONTROL Other objects and endpoints]</b> voor alle andere recordtypen en zoek het recordtype op de alfabetische gesorteerde pagina's.</p> </li> 
     <li value="2"> <p>Zoek op de pagina van het juiste recordtype naar de handeling (Ctrl-F of Cmd-F).</p> </li> 
     <li value="3"> <p>Beschrijvingen weergeven voor beschikbare velden onder de geselecteerde handeling.</p> </li> 
    </ol> <p>Opmerking:  <p>Als u een proefdruk maakt via de module [!DNL Workfront] [!UICONTROL Misc Action] , kunt u het beste een proefdruk maken zonder geavanceerde opties en de proefdruk vervolgens bijwerken met de API voor SOAP [!DNL Workfront Proof] .</p> <p>Voor meer informatie bij het creëren van een proef met [!DNL Workfront] API (die deze module gebruikt), zie <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref"> Geavanceerde het proefdrukken opties wanneer het creëren van een proef door [!DNL Adobe Workfront] API </a> toevoegen</p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Voer de unieke [!DNL Workfront] -id in of wijs deze toe aan de record waarmee de module moet communiceren.<p>Als u de id wilt ophalen, opent u het object [!DNL Workfront] in uw browser en kopieert u de tekst aan het einde van de URL na "ID=". Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i> 5e43010c03286a2a555e1d0a75d6a86e </i></p></td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

#### Handelingsopties

##### Taak

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Handeling</th> 
   <th>Opties</th> 
  </tr> 
  <tr> 
   <td>Kopiëren</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignment</li>
   <li>clearConstraints</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Wist financiële gegevens</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Hiermee wist u herinneringsmeldingen</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Verplaatsen</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignment</li>
   <li>clearDocuments</li>
   <li>clearConstraints</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Wist financiële gegevens</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Hiermee wist u herinneringsmeldingen</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

##### Probleem

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Handeling</th> 
   <th>Opties</th> 
  </tr> 
  <tr> 
   <td>Kopiëren</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignment</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearPermissions</li>
   <li>clearProgress</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Omzetten in taak</td> 
   <td>
   <ul>
   <li>preserveIssue<p>Behoud het oorspronkelijke probleem en koppel zijn resolutie aan deze taak</p></li>
   <li>preservePrimaryContact<p>De primaire contactpersoon van de problemen toegang geven tot deze taak</p></li>
   <li>preserveCompletionDate<p>Behoud de geplande afsluitdatum van de uitgave</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Omzetten in project</td> 
   <td>
   <ul>
   <li>preserveIssue<p>Behoud het oorspronkelijke probleem en koppel zijn resolutie aan deze taak</p></li>
   <li>preservePrimaryContact<p>De primaire contactpersoon van de problemen toegang geven tot deze taak</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



##### Project

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Handeling</th> 
   <th>Opties</th> 
  </tr> 
  <tr> 
   <td>Kopiëren</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignment</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Wist financiële gegevens</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Hiermee wist u herinneringsmeldingen</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Sjabloon bijvoegen / Opslaan als sjabloon</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignment</li>
   <li>clearBillingRates</li>
   <li>clearConstraints</li>
   <li>clearDeliverables<p>Duidelijke doelstellingen</p></li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Wist financiële gegevens</p></li>
   <li>clearHourTypes</li>
   <li>clearIssueSetup<p>Wist wachtrijeigenschappen en configuratie van problemen</p></li>
   <li>clearPredecessors</li>
   <li>clearRisks</li>
   <li>clearSharingOptions</li>
   <li>clearTimedNotifications<p>Hiermee wist u herinneringsmeldingen</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



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

<td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>Kies het objecttype [!DNL Workfront] dat u wilt lezen in de module.</td> 
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
   <td> <p>Voer de unieke [!DNL Workfront] id in van de record die u wilt lezen in de module.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Workfront] in uw browser en kopieert u de tekst aan het einde van de URL na "ID=". Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i> 5e43010c03286a2a555e1d0a75d6a86e </i></p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Voer de unieke [!DNL Workfront] id in van de record die u wilt bijwerken in de module.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Workfront] in uw browser en kopieert u de tekst aan het einde van de URL na "ID=". Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i> 5e43010c03286a2a555e1d0a75d6a86e </i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record dat u wilt bijwerken in de module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selecteer de velden die u beschikbaar wilt maken voor gegevensinvoer. Dit staat u toe om deze gebieden te gebruiken zonder het moeten door degenen scrollen u niet nodig hebt.</td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

>[!NOTE]
>
>* Wanneer u de id van een object opgeeft, kunt u de naam van het object beginnen te typen en het vervolgens in de lijst selecteren. De module gaat dan aangewezen identiteitskaart in het gebied in.
>* Wanneer u de tekst voor een aangepast veld of een [!UICONTROL Note] -object (Opmerking of Antwoord) invoert, kunt u HTML-tags in het [!UICONTROL Note Text] -veld gebruiken om RTF-tekst, zoals vette of cursieve tekst, te maken.
>
>  Voor meer informatie over rijke tekst in updates, zie [ een update aan een het werkpunt ](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [ werk van de Update ](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md) toevoegen.
>

+++

+++ **[!UICONTROL Upload Document]**

Deze actiemodule uploadt een document naar een [!DNL Workfront] -object, zoals een project, taak of uitgave. Deze module uploadt het document in delen, waardoor het uploadproces voor Workfront soepeler verloopt.

U geeft de locatie voor het document, het bestand dat u wilt uploaden en een optionele nieuwe naam voor het bestand op.

De module retourneert de id van het document en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Voer de unieke [!DNL Workfront] -id in van de record waarnaar u het document wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Selecteer het type [!DNL Workfront] -record waarin u het document wilt uploaden door de module.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td>Afhankelijk van het type verwante record moet u mogelijk een map-id invoeren of toewijzen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

+++

+++ **[!UICONTROL Upload Document (Legacy)]**

Deze actiemodule uploadt een document naar een [!DNL Workfront] -object, zoals een project, taak of uitgave. Het gehele document tegelijk uploadt.

U geeft de locatie voor het document, het bestand dat u wilt uploaden en een optionele nieuwe naam voor het bestand op.

De module retourneert de id van het document en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Voer de unieke [!DNL Workfront] -id in van de record waarnaar u het document wilt uploaden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Selecteer het type [!DNL Workfront] -record waarin u het document wilt uploaden door de module.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td>Afhankelijk van het type verwante record moet u mogelijk een map-id invoeren of toewijzen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

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
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type bovenliggende record (Workfront-object) waarvan u de gekoppelde records wilt lezen.</p> <p>Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] objecten types beschikbaar voor elke [!DNL Workfront] module </a> in dit artikel kunt gebruiken.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>Voer de id in van de bovenliggende record waarvan u de gekoppelde records wilt lezen of wijs deze toe.</p> <p>Als u de id wilt ophalen, opent u het object [!DNL Workfront] in uw browser en kopieert u de tekst aan het einde van de URL na "ID=". Bijvoorbeeld: https://my.workfront.com/project/view?ID=<i> 5e43010c03286a2a555e1d0a75d6a86e </i></p> </td> 
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

Deze zoekmodule zoekt naar records in een object in [!DNL Workfront] dat overeenkomt met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record waarnaar u wilt zoeken in de module.</p> </td> 
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
   <td> <p>Voer het veld in waarnaar u wilt zoeken, de operator die u in de query wilt gebruiken en de waarde waarnaar u in het veld zoekt.</p> <p>Opmerking: gebruik <code>username </code> niet in de zoekcriteria. Als u <code>username </code> opneemt in een API-query voor [!DNL Workfront] , wordt de gebruiker aangemeld bij Workfront. De zoekopdracht is dan niet geslaagd.</p> <p>Opmerking: <code>In</code> en <code>NotIn</code> werken met arrays. De invoer moet een arrayindeling hebben.</p></td> 
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

+++

+++ **[!UICONTROL Search (Legacy)]**

Deze zoekmodule zoekt naar records in een object in [!DNL Workfront] dat overeenkomt met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type [!DNL Workfront] record waarnaar u wilt zoeken in de module.</p> </td> 
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
   <td> <p>Voer het veld in waarnaar u wilt zoeken, de operator die u in de query wilt gebruiken en de waarde waarnaar u in het veld zoekt.</p> <p>Opmerking: gebruik <code>username </code> niet in de zoekcriteria. Als u <code>username </code> opneemt in een API-query voor [!DNL Workfront] , wordt de gebruiker aangemeld bij Workfront. De zoekopdracht is dan niet geslaagd.</p> <p>Opmerking: <code>In</code> en <code>NotIn</code> werken met arrays. De invoer moet een arrayindeling hebben.</p></td> 
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

Zie een lijst van de [!DNL Workfront] objecten types waarvoor u deze module in [[!DNL Workfront]  objecten types beschikbaar voor elke  [!DNL Workfront]  module ](#workfront-object-types-available-for-each-workfront-module) kunt gebruiken.

+++

## [!DNL Workfront] objecttypen beschikbaar voor elke [!DNL Workfront] -module

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**types van Objecten beschikbaar voor elke [!DNL Workfront] trekkermodule**

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

+++**types van Objecten beschikbaar voor elke [!DNL Workfront] actiemodule**

>[!NOTE]
>
>De module [!UICONTROL Download Document] is niet in deze tabel opgenomen omdat objecttypen van [!DNL Workfront] geen deel uitmaken van de configuratie ervan.

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
   <td> </td> 
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

+++**types van Objecten beschikbaar voor elke [!DNL Workfront] onderzoeksmodule**

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

## Filters voor gebeurtenisabonnementen in de modules [!DNL Workfront] > [!UICONTROL Watch Events]

>[!NOTE]
>
>We raden u ten zeerste aan filters voor gebeurtenisabonnementen in uw [!UICONTROL Watch Events] -modules te gebruiken.

De module [!DNL Workfront] [!UICONTROL Watch Events] activeert scenario&#39;s op basis van een webhaak die een gebeurtenisabonnement maakt in de API [!DNL Workfront] . Het gebeurtenisabonnement is een gegevensset die bepaalt welke gebeurtenissen naar de webhaak worden verzonden. Als u bijvoorbeeld een module [!UICONTROL Watch Events] instelt die op problemen let, verzendt het gebeurtenisabonnement alleen gebeurtenissen die met problemen te maken hebben.

Door gebeurtenisabonnementfilters te gebruiken, kunnen Fusion-gebruikers gebeurtenisabonnementen maken die beter geschikt zijn voor hun gebruik. U kunt bijvoorbeeld een gebeurtenisabonnement instellen in de [!DNL Workfront] API om alleen problemen te verzenden die zich in een specifiek project bevinden naar de webhaak. Zo zorgt u ervoor dat de module [!UICONTROL Watch Events] alleen wordt geactiveerd voor problemen in dat project. De mogelijkheid om smallere triggers te maken verbetert het ontwerp van scenario&#39;s door het aantal irrelevante triggers te verminderen.

Dit is anders dan het instellen van een filter in het [!DNL Workfront Fusion] -scenario. Zonder een gebeurtenisabonnementfilter ontvangt uw webhaak alle gebeurtenissen die betrekking hebben op het objecttype dat u selecteert. De meeste van deze gebeurtenissen zijn niet relevant voor het scenario en moeten worden uitgefilterd voordat het scenario kan worden voortgezet.

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
   * Wanneer het gebruiken van `Changed`, selecteer **Bijgewerkte Gebeurtenissen slechts** op het **gebied van de Oorsprong van het Verslag**.

>[!IMPORTANT]
>
>U kunt filters in bestaande [!DNL Workfront] -webhaken niet bewerken. Als u verschillende filters wilt instellen voor [!DNL Workfront] -gebeurtenisabonnementen, verwijdert u de huidige webhaak en maakt u een nieuwe.

>[!INFO]
>
>**Voorbeeld:** overweeg een scenario dat nieuwe kwesties verwerkt die aan een specifieke gebruiker, Ana worden toegewezen.
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
>Als u gebeurtenissen wilt filteren zodat alleen uitgaven worden verwerkt die aan Ana zijn toegewezen, kunt u een filter maken na de module [!UICONTROL Watch Events] .
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Als er in een dag 100 problemen worden gemaakt, maar slechts twee ervan worden toegewezen aan Ana, wordt het scenario 100 keer uitgevoerd. 98 van de uitvoeringen zouden bij de filter ophouden, maar de trekkermodule verbruikt nog steeds gegevens en voert bewerkingen uit in alle uitvoeringen.

Voor meer informatie over gebeurtenisabonnementen, zie [ FAQs - de Abonnementen van de Gebeurtenis ](../../wf-api/general/event-subs-faq.md).

Voor meer informatie over webhooks, zie [ Onmiddellijke trekkers (webhooks) in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Voor meer informatie over filters in scenario&#39;s, zie [ een filter aan een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md) toevoegen.

