---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Allocadia
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Allocadia gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---

# [!DNL Allocadia] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Allocadia]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!DNL Allocadia] modules, moet u een [!DNL Allocadia] account.

## Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]

U kunt een verbinding maken met uw [!DNL Allocadia] rechtstreeks vanuit een [!DNL Allocadia] module.

1. In alle [!DNL Allocadia] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Selecteer of u de server van Noord-Amerika of de server van Europa wilt gebruiken.
1. Voer uw gebruikersnaam en wachtwoord in.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Allocadia] modules en hun velden

Wanneer u [!DNL Allocadia] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Allocadia] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Triggers

#### [!UICONTROL Watch Record]

Deze triggermodule voert een scenario uit wanneer objecten van een specifiek type worden toegevoegd, bijgewerkt of beide. De module retourneert alle standaardvelden die zijn gekoppeld aan de record of records, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het verbinden van uw Allocadia-account met [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] naar Workfront Fusion</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Selecteer of u het scenario op Alleen Nieuwe records wilt letten, [!UICONTROL Updated Records Only]of Nieuwe en bijgewerkte records.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type entiteit</td> 
   <td>Selecteer het allocadia-recordtype waarop u de module wilt letten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uitvoer</td> 
   <td> <p>Selecteer de velden die u in de uitvoer van de module wilt opnemen. Beschikbare velden zijn afhankelijk van het type entiteit dat u hebt geselecteerd.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limiet</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt letten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [Aangepaste API-aanroep](#custom-api-call)
* [Record lezen](#read-record)
* [Record maken](#create-record)
* [Record verwijderen](#delete-record)
* [Record bijwerken](#update-record)

#### [!UICONTROL Custom API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Allocadia] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Allocadia] modules.

De handeling is gebaseerd op het door u opgegeven eenheidstype (allocadia-objecttype).

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Allocadia] account aan [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Een pad invoeren ten opzichte van <code>https://api-na.allocadia.com/{version}</code> of <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Read Record]

Deze actiemodule leest gegevens uit één record in [!DNL Allocadia].

U geeft de id van de record op.

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Allocadia] account aan [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type van [!DNL Allocadia] record dat de module moet lezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer van de module wilt opnemen. Beschikbare velden zijn afhankelijk van de [!UICONTROL Entity Type] geselecteerd.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL Allocadia] Id van de record die de module moet lezen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Record]

Deze actiemodule maakt een record.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Allocadia] account aan [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer of u een nieuwe record wilt maken op basis van de regel- of kolomkeuze.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Selecteer het budget waar u een record wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Selecteer de kolom die u wilt gebruiken om een nieuwe record te maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Een label voor de nieuwe record invoeren of toewijzen</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Record]

Deze actiemodule verwijdert een bepaalde record.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Allocadia] account aan [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Selecteer het type entiteit dat u wilt verwijderen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Line item]</strong> </p> <p>Geef de id van het lijstitem op</p> </li> 
     <li> <p><strong>[!UICONTROL Column Choice]</strong> </p> <p>Selecteer het budget waaruit u een record wilt verwijderen en voer vervolgens de kolom-id en de keuze-id in.</p> </li> 
     <li> <p><strong>[!UICONTROL Forecast Tags]</strong> </p> <p>Selecteer het budget waaruit u een record wilt verwijderen en voer vervolgens de tag-id in.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update Record]

Deze actiemodule werkt een record bij, zoals een regelitem, een gebruiker of een kolomkeuze.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!UICONTROL Allocadia] account aan [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type van [!DNL Allocadia] record dat de module moet worden bijgewerkt. Andere velden worden weergegeven op basis van het eenheidstype dat u selecteert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Selecteer het budget waar u een record wilt bijwerken. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

#### [!UICONTROL Search Record]

Deze zoekmodule zoekt naar records in een object in [!DNL Allocadia] die overeenkomen met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

U geeft het gewenste type records op.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Allocadia] account aan [!DNL Workfront Fusion], zie <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type van [!DNL Allocadia] record waarnaar u wilt zoeken in de module. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Selecteer het budget dat u wilt zoeken. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Selecteer of u de module Alle Overeenkomende Verslagen, of het Eerste Overeenkomende slechts Verslag wilt terugkeren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Selecteer het veld waarnaar u wilt zoeken, selecteer de bewerking en voer de waarde in of wijs de waarde toe waarnaar u wilt zoeken. U kunt [!DNL AND] of [!DNL OR] regels om uw zoekopdracht verder te filteren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer van de module wilt opnemen. Beschikbare velden zijn afhankelijk van het type entiteit dat u hebt geselecteerd.</p> </td> 
  </tr> 
 </tbody> 
</table>
