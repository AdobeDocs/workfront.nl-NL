---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die de Dynamica 365 van Microsoft gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Microsoft Dynamics 365]en deze verbinding maken met meerdere toepassingen en services van derden.

>[!NOTE]
>
>De [!DNL Microsoft Dynamics 365] connector wordt niet ondersteund [!DNL Dynamics Finance and Operations].

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr>
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!DNL Microsoft Dynamics] 365, hebt u een [!DNL Microsoft Dynamics 365] account.

## Connect Microsoft Dynamics 365 to Workfront Fusion

U kunt een verbinding maken met uw [!DNL Microsoft Dynamics 365] rechtstreeks vanuit een [!DNL Microsoft Dynamics 365] module.

1. In alle [!DNL Microsoft Dynamics 365] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Voer een naam in voor de verbinding.
1. In de **[!UICONTROL Resource]** veld, voert u het adres in van uw [!DNL Dynamics 365] account, zonder `https://`.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

>[!NOTE]
>
>Bij registratie [!DNL Workfront Fusion] in uw [!DNL Microsoft Azure] portaal, gebruik volgende omleiding URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`



## [!DNL Microsoft Dynamics 365] modules en hun velden

Wanneer u [!DNL Microsoft Dynamics 365] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Microsoft Dynamics 365] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Watch Records (Scheduled)]](#watch-records-scheduled)
* [[!UICONTROL Watch Records (Real Time)]](#watch-records-real-time)
* [[!UICONTROL Create Record]](#create-record)
* [[!UICONTROL Make an API Call]](#make-an-api-call)
* [[!UICONTROL Delete Record]](#delete-record)
* [[!UICONTROL Read Records]](#read-records)
* [[!UICONTROL Update Record]](#update-record)
* [[!UICONTROL Search Records]](#search-records)

### [!UICONTROL Watch Records (Scheduled)]

Deze geplande triggermodule voert een scenario uit wanneer een record in het opgegeven object wordt gemaakt of bijgewerkt na de laatste geplande uitvoering [!DNL Dynamics 365].

De output van de module wijst erop of het verslag dat het vond nieuw of bijgewerkt is (als het zowel in de tijdspanne werd toegevoegd en bijgewerkt, is het duidelijk als nieuw). U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Dit gebeurt op een regelmatig gepland interval dat u specificeert.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Selecteer of u de module wilt controleren <strong>[!UICONTROL Only new records]</strong>, <strong>[!UICONTROL Updated records only]</strong>, of <strong>[!UICONTROL New records and all changes]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Kies de optie [!UICONTROL Microsoft Dynamics 365] recordtype waarop u het scenario wilt letten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Watch Records (Real Time)]

Deze instant trigger-module voert een scenario uit wanneer een record (object) die u opgeeft, wordt gemaakt of bijgewerkt in [!DNL Dynamics 365].

In deze module is een webhaak vereist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecteer de webhaak die u voor deze module wilt gebruiken. </p> <p>Een nieuwe webhaak toevoegen:</p> 
    <ol> 
     <li value="1"> <p>Klikken <strong>[!UICONTROL Add]</strong> rechts van het veld Webhaak</p> </li> 
     <li value="2"> <p>In de <strong>[!UICONTROL Webhook]</strong> Typ een beschrijvende naam voor de webhaak.</p> </li> 
     <li value="3"> <p>In de <strong>[!UICONTROL Connection]</strong> veld, selecteert u de gewenste verbinding</p> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </li> 
     <li value="4"> <p>Klikken <strong>[!UICONTROL Save]</strong> om uw webhaak op te slaan en terug te keren naar de module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create Record]

Deze actiemodule leidt tot een entiteit, zoals een benoeming of een taak,.

U geeft informatie op over de entiteit die u wilt maken.

De module retourneert de id van de nieuwe entiteit en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type entiteit dat de module moet maken.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>Voer in deze velden de waarde in die het werkitem voor een bepaalde eigenschap moet hebben. Beschikbare velden zijn afhankelijk van het type entiteit.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make an API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Microsoft Dynamics 365] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Microsoft Dynamics 365] modules.

De module keert informatie over de statuscode, kopballen, en lichaam terug. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Zie voor meer informatie de [!DNL Microsoft] documentatie over het gebruik van de [!DNL Dynamics 365 Customer Engagement Web API].

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Een pad invoeren ten opzichte van <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Voor meer in</p> </td> 
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

### [!UICONTROL Delete Record]

Met deze actiemodule verwijdert u een entiteit.

U geeft de id van de entiteit op.

De module retourneert de id van de entiteit en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Selecteer het type entiteit dat u wilt verwijderen uit de module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>De unieke sleutel invoeren of toewijzen [!DNL Microsoft Dynamics 365] Id van de record die u wilt verwijderen uit de module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Read Records]

Deze actiemodule leest gegevens van één entiteit in [!DNL Microsoft Dynamics 365].

U geeft de id van de entiteit op.

De module retourneert de id van de entiteit en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type entiteit dat de module moet lezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL Microsoft Dynamics 365] Id van de record die de module moet lezen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update Record]

Deze actiemodule werkt een entiteit bij.

U geeft de id van de entiteit op.

De module retourneert de id van de bijgewerkte record en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type entiteit dat de module moet bijwerken.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>Voer in deze velden de waarde in die het werkitem voor een bepaalde eigenschap moet hebben. Beschikbare velden zijn afhankelijk van het type entiteit.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>De unieke sleutel invoeren of toewijzen [!DNL Microsoft Dynamics] 365 ID van de record die u wilt bijwerken in de module.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search Records]

Deze zoekmodule zoekt naar records in een object in [!DNL Microsoft Dynamics 365] die overeenkomen met de zoekquery die u opgeeft. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Voor instructies over het aansluiten van uw [!DNL Microsoft Dynamics 365] account aan [!DNL Workfront Fusion], zie <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in dit artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selecteer het type entiteit dat de module moet bijwerken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>Selecteer het filter dat u voor deze zoekopdracht wilt gebruiken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standard Filters]</strong> </p> <p>Stel het filter in door een veld en een operator te selecteren en de waarde die u wilt zoeken in te voeren of toe te wijzen. U kunt EN of OF regels aan uw filter gebruiken.</p> </li> 
     <li> <p><strong>[!UICONTROL Query Functions]</strong> </p> <p>Voer de [!DNL Dynamics 365] web-API queryfunctie die u wilt gebruiken om te zoeken. </p> <p>Voor meer informatie over vraagfuncties, zie <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API Query Function Reference</a> in de [!DNL Microsoft] documentatie.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>Geef de volgorde op waarin de items worden geretourneerd. U kunt meerdere soorten toevoegen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Geef het veld op waarin u de resultaten wilt sorteren.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Geef de richting van de sortering op (oplopend of aflopend).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen.</p> </td> 
  </tr> 
 </tbody> 
</table>
